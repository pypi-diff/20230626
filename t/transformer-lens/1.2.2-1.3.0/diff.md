# Comparing `tmp/transformer_lens-1.2.2.tar.gz` & `tmp/transformer_lens-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformer_lens-1.2.2.tar", max compression
+gzip compressed data, was "transformer_lens-1.3.0.tar", max compression
```

## Comparing `transformer_lens-1.2.2.tar` & `transformer_lens-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-04-24 07:40:25.148681 transformer_lens-1.2.2/LICENSE
--rw-r--r--   0        0        0     8084 2023-04-24 07:40:25.148681 transformer_lens-1.2.2/README.md
--rw-r--r--   0        0        0     1902 2023-04-24 07:41:40.743673 transformer_lens-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    36290 2023-04-24 07:40:25.240679 transformer_lens-1.2.2/transformer_lens/ActivationCache.py
--rw-r--r--   0        0        0     7776 2023-04-24 07:40:25.240679 transformer_lens-1.2.2/transformer_lens/FactoredMatrix.py
--rw-r--r--   0        0        0    81131 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/HookedTransformer.py
--rw-r--r--   0        0        0    12588 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/HookedTransformerConfig.py
--rw-r--r--   0        0        0      867 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/__init__.py
--rw-r--r--   0        0        0    36777 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/components.py
--rw-r--r--   0        0        0    12267 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/evals.py
--rw-r--r--   0        0        0     8525 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/head_detector.py
--rw-r--r--   0        0        0    19943 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/hook_points.py
--rw-r--r--   0        0        0    50594 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/loading_from_pretrained.py
--rw-r--r--   0        0        0     2092 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/make_docs.py
--rw-r--r--   0        0        0    11177 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/model_properties_table.md
--rw-r--r--   0        0        0     2865 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/past_key_value_caching.py
--rw-r--r--   0        0        0    24180 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/patching.py
--rw-r--r--   0        0        0     5511 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/train.py
--rw-r--r--   0        0        0        0 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/utilities/__init__.py
--rw-r--r--   0        0        0     1257 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/utilities/devices.py
--rw-r--r--   0        0        0    28437 2023-04-24 07:40:25.244679 transformer_lens-1.2.2/transformer_lens/utils.py
--rw-r--r--   0        0        0     9911 1970-01-01 00:00:00.000000 transformer_lens-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-26 11:14:25.623748 transformer_lens-1.3.0/LICENSE
+-rw-r--r--   0        0        0     8356 2023-06-26 11:14:25.623748 transformer_lens-1.3.0/README.md
+-rw-r--r--   0        0        0     2110 2023-06-26 11:15:21.616249 transformer_lens-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    36946 2023-06-26 11:14:25.727757 transformer_lens-1.3.0/transformer_lens/ActivationCache.py
+-rw-r--r--   0        0        0     8710 2023-06-26 11:14:25.727757 transformer_lens-1.3.0/transformer_lens/FactoredMatrix.py
+-rw-r--r--   0        0        0    15731 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/HookedEncoder.py
+-rw-r--r--   0        0        0    83370 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/HookedTransformer.py
+-rw-r--r--   0        0        0    12604 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/HookedTransformerConfig.py
+-rw-r--r--   0        0        0     5577 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/SVDInterpreter.py
+-rw-r--r--   0        0        0      951 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/__init__.py
+-rw-r--r--   0        0        0    44079 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/components.py
+-rw-r--r--   0        0        0    12215 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/evals.py
+-rw-r--r--   0        0        0    12379 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/head_detector.py
+-rw-r--r--   0        0        0    21888 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/hook_points.py
+-rw-r--r--   0        0        0    61578 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/loading_from_pretrained.py
+-rw-r--r--   0        0        0     2161 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/make_docs.py
+-rw-r--r--   0        0        0    11177 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/model_properties_table.md
+-rw-r--r--   0        0        0     2867 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/past_key_value_caching.py
+-rw-r--r--   0        0        0    30494 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/patching.py
+-rw-r--r--   0        0        0     5399 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/train.py
+-rw-r--r--   0        0        0        0 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/utilities/__init__.py
+-rw-r--r--   0        0        0     2510 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/utilities/devices.py
+-rw-r--r--   0        0        0    31584 2023-06-26 11:14:25.731757 transformer_lens-1.3.0/transformer_lens/utils.py
+-rw-r--r--   0        0        0    10177 1970-01-01 00:00:00.000000 transformer_lens-1.3.0/PKG-INFO
```

### Comparing `transformer_lens-1.2.2/LICENSE` & `transformer_lens-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.2.2/README.md` & `transformer_lens-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # TransformerLens
 
+![TransformerLens](assets/rm_transformer_lens_logo.png)
+
 [![Pypi](https://img.shields.io/pypi/v/transformer-lens)](https://pypi.org/project/transformer-lens/)
 
 (Formerly known as EasyTransformer)
 
 ## [Read the Docs Here](https://neelnanda-io.github.io/TransformerLens/)
 
 ## [Main Tutorial Here](https://neelnanda.io/transformer-lens-demo)
@@ -74,14 +76,21 @@
 
 #### Running the tests
 
 - All tests via `make test`
 - Unit tests only via `make unit-test`
 - Acceptance tests only via `make acceptance-test`
 
+### Formatting
+
+This project uses `pycln`, `isort` and `black` for formatting, pull requests are checked in github actions.
+
+- Format all files via `make format`
+- Only check the formatting via `make check-format`
+
 ### Demos
 
 If adding a feature, please add it to the demo notebook in the `demos` folder, and check that it works in the demo format. This can be tested by replacing `pip install git+https://github.com/JayBaileyCS/TransformerLens.git` with `pip install git+https://github.com/<YOUR_USERNAME_HERE>/TransformerLens.git` in the demo notebook, and running it in a fresh environment.
 
 ## Citation
 
 Please cite this library as:
```

### Comparing `transformer_lens-1.2.2/pyproject.toml` & `transformer_lens-1.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "transformer-lens"
-version = "v1.2.2" # This is automatically set by the CD pipeline on release
+version = "v1.3.0" # This is automatically set by the CD pipeline on release
 description = "An implementation of transformers tailored for mechanistic interpretability."
 authors = ["Neel Nanda <77788841+neelnanda-io@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "transformer_lens"}]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
+python = ">=3.7.4,<4.0"
 einops = ">=0.6.0"
 numpy = [{ version = ">=1.21", python = "<3.10" },
          { version = ">=1.23", python = ">=3.10" }]
 torch = ">=1.10"
 datasets = ">=2.7.1"
 transformers = ">=4.25.1"
 tqdm = ">=4.64.1"
@@ -23,32 +23,41 @@
 jaxtyping = ">=0.2.11"
 sphinx = {version = "5.2.3", optional = true, python = ">=3.8,<3.10"}
 sphinxcontrib-napoleon = {version = ">=0.7", optional = true, python = ">=3.8,<3.10"}
 sphinx-autobuild = {version = ">=2021.3.14", optional = true, python = ">=3.8,<3.10"}
 furo = {version = ">=2022.12.7", optional = true, python = ">=3.8,<3.10"}
 myst-parser = {version = ">=0.18.1", optional = true, python = ">=3.8,<3.10"}
 tabulate= {version = ">=0.9.0", optional = true, python = ">=3.8,<3.10"}
+typeguard = "^3.0.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.2.0"
 pytest-cov = ">=4.0.0"
 mypy = ">=0.991"
 jupyter = ">=1.0.0"
 circuitsvis = ">=1.38.1"
 plotly = ">=5.12.0"
+isort = "5.8.0"
+black = "^23.3.0"
+pycln = "^2.1.3"
 
 [tool.poetry.group.jupyter.dependencies]
 jupyterlab = ">=3.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinx-autobuild", "sphinxcontrib-napoleon", "furo", "myst_parser","tabulate"]
 
 [tool.pytest.ini_options]
 filterwarnings = [
+    "ignore:pkg_resources is deprecated as an API:DeprecationWarning",
     # Ignore numpy.distutils deprecation warning caused by pandas
     # More info: https://numpy.org/doc/stable/reference/distutils.html#module-numpy.distutils
     "ignore:distutils Version classes are deprecated:DeprecationWarning"
-]
+]
+
+[tool.isort]
+profile = "black"
+extend_skip = ["__init__.py"]
```

### Comparing `transformer_lens-1.2.2/transformer_lens/ActivationCache.py` & `transformer_lens-1.3.0/transformer_lens/ActivationCache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # %%
 from __future__ import annotations
-import transformer_lens.utils as utils
-from transformer_lens.utils import Slice, SliceInput
-from jaxtyping import Float
-import torch
+
+import logging
+from typing import Dict, List, Optional, Tuple, Union
+
 import einops
+import numpy as np
+import torch
 from fancy_einsum import einsum
-from typing import Optional, Union, Dict
+from jaxtyping import Float, Int
 from typing_extensions import Literal
-import re
-import numpy as np
-import logging
+
+import transformer_lens.utils as utils
+from transformer_lens.utils import Slice, SliceInput
+
 
 class ActivationCache:
     """
     A wrapper around a dictionary of cached activations from a model run, with a variety of helper functions. In general, any utility which is specifically about editing/processing activations should be a method here, while any utility which is more general should be a function in utils.py, and any utility which is specifically about model weights should be in HookedTransformer.py or components.py.
 
     NOTE: This is designed to be used with the HookedTransformer class, and will not work with other models. It's also designed to be used with all activations of HookedTransformer being cached, and some internal methods will break without that.
 
@@ -185,37 +188,53 @@
             )
         if return_labels:
             return components, labels
         else:
             return components
 
     def logit_attrs(
-            self,
-            residual_stack: TT[T.num_components, T.batch_and_pos_dims:..., T.d_model],
-            tokens: Union[str, int, TT[()], TT[T.batch], TT[T.batch, T.position]],
-            incorrect_tokens: Union[str, int, TT[()], TT[T.batch], TT[T.batch, T.position]] = None,
-            pos_slice: Union[Slice, SliceInput] = None,
-            batch_slice: Union[Slice, SliceInput] = None,
-            has_batch_dim: bool = True
-        ) -> TT[T.num_components, T.batch_and_pos_dims:...]:
+        self,
+        residual_stack: Float[
+            torch.Tensor, "num_components *batch_and_pos_dims d_model"
+        ],
+        tokens: Union[
+            str,
+            int,
+            Int[torch.Tensor, ""],
+            Int[torch.Tensor, "batch"],
+            Int[torch.Tensor, "batch position"],
+        ],
+        incorrect_tokens: Optional[
+            Union[
+                str,
+                int,
+                Int[torch.Tensor, ""],
+                Int[torch.Tensor, "batch"],
+                Int[torch.Tensor, "batch position"],
+            ]
+        ] = None,
+        pos_slice: Union[Slice, SliceInput] = None,
+        batch_slice: Union[Slice, SliceInput] = None,
+        has_batch_dim: bool = True,
+    ) -> Float[torch.Tensor, "num_components *batch_and_pos_dims"]:
         """Returns the logit attributions for the residual stack on an input of tokens, or the logit difference attributions for the residual stack if incorrect_tokens is provided.
 
         Args:
-            residual_stack (TT["num_components", "batch_and_pos_dims":..., "d_model"]): stack of components of residual stream to get logit attributions for.
-            tokens (Union[str, int, TT[()], TT["batch"], TT["batch", "position"]]): tokens to compute logit attributions on.
-            incorrect_tokens (Union[str, int, TT[()], TT["batch"], TT["batch", "position"]], optional): if provided, compute attributions on logit difference between tokens and incorrect_tokens.
+            residual_stack (Float[torch.Tensor, "num_components *batch_and_pos_dims d_model"]): stack of components of residual stream to get logit attributions for.
+            tokens (Union[str, int, Int[torch.Tensor, ""], Int[torch.Tensor, "batch"], Int[torch.Tensor, "batch position"]]): tokens to compute logit attributions on.
+            incorrect_tokens (Union[str, int, Int[torch.Tensor, ""], Int[torch.Tensor, "batch"], Int[torch.Tensor, "batch position"]], optional): if provided, compute attributions on logit difference between tokens and incorrect_tokens.
                 Must have the same shape as tokens.
             pos_slice (Slice, optional): The slice to apply layer norm scaling on.
                 Defaults to None, do nothing.
             batch_slice (Slice, optional): The slice to take on the batch dimension during layer norm scaling.
                 Defaults to None, do nothing.
             has_batch_dim (bool, optional): Whether residual_stack has a batch dimension.
                 Defaults to True.
         Returns:
-            Components: A [num_components, batch_and_pos_dims:...] tensor of the logit attributions or logit difference attributions if incorrect_tokens was provided.
+            Components: A [num_components, *batch_and_pos_dims] tensor of the logit attributions or logit difference attributions if incorrect_tokens was provided.
         """
         if not isinstance(pos_slice, Slice):
             pos_slice = Slice(pos_slice)
 
         if not isinstance(batch_slice, Slice):
             batch_slice = Slice(batch_slice)
 
@@ -225,32 +244,46 @@
         elif isinstance(tokens, int):
             tokens = torch.as_tensor(tokens)
 
         logit_directions = self.model.tokens_to_residual_directions(tokens)
 
         if incorrect_tokens is not None:
             if isinstance(incorrect_tokens, str):
-                incorrect_tokens = torch.as_tensor(self.model.to_single_token(incorrect_tokens))
+                incorrect_tokens = torch.as_tensor(
+                    self.model.to_single_token(incorrect_tokens)
+                )
 
             elif isinstance(incorrect_tokens, int):
                 incorrect_tokens = torch.as_tensor(incorrect_tokens)
 
             if tokens.shape != incorrect_tokens.shape:
-                raise ValueError(f"tokens and incorrect_tokens must have the same shape! (tokens.shape={tokens.shape}, incorrect_tokens.shape={incorrect_tokens.shape})")
-        
-            # If incorrect_tokens was provided, take the logit difference
-            logit_directions = logit_directions - self.model.tokens_to_residual_directions(incorrect_tokens)
+                raise ValueError(
+                    f"tokens and incorrect_tokens must have the same shape! (tokens.shape={tokens.shape}, incorrect_tokens.shape={incorrect_tokens.shape})"
+                )
 
+            # If incorrect_tokens was provided, take the logit difference
+            logit_directions = (
+                logit_directions
+                - self.model.tokens_to_residual_directions(incorrect_tokens)
+            )
 
-        scaled_residual_stack = self.apply_ln_to_stack(residual_stack, layer=-1, pos_slice=pos_slice, batch_slice=batch_slice, has_batch_dim=has_batch_dim)
+        scaled_residual_stack = self.apply_ln_to_stack(
+            residual_stack,
+            layer=-1,
+            pos_slice=pos_slice,
+            batch_slice=batch_slice,
+            has_batch_dim=has_batch_dim,
+        )
 
-        logit_attrs = einsum("... d_model, ... d_model -> ...", scaled_residual_stack, logit_directions)
+        logit_attrs = einsum(
+            "... d_model, ... d_model -> ...", scaled_residual_stack, logit_directions
+        )
 
         return logit_attrs
-        
+
     def decompose_resid(
         self,
         layer: Optional[int] = None,
         mlp_input: bool = False,
         mode: Literal["all", "mlp", "attn"] = "all",
         apply_ln: bool = False,
         pos_slice: Union[Slice, SliceInput] = None,
@@ -392,46 +425,44 @@
             components = torch.zeros(
                 0,
                 *pos_slice.apply(self["hook_embed"], dim=-2).shape,
                 device=self.model.cfg.device,
             )
 
         if apply_ln:
-            components = self.apply_ln_to_stack(
-                components, layer, pos_slice=pos_slice
-            )
-            
+            components = self.apply_ln_to_stack(components, layer, pos_slice=pos_slice)
+
         if return_labels:
             return components, labels
         else:
             return components
-    
+
     def stack_activation(
         self,
         activation_name: str,
         layer: int = -1,
         sublayer_type: Optional[str] = None,
     ) -> Float[torch.Tensor, "layers_covered ..."]:
         """Returns a stack of all head results (ie residual stream contribution) up to layer L. A good way to decompose the outputs of attention layers into attribution by specific heads. The output shape is exactly the same shape as the activations, just with a leading layers dimension.
 
         Args:
             activation_name (str): The name of the activation to be stacked
             layer (int): Layer index - heads at all layers strictly before this are included. layer must be in [1, n_layers-1], or any of (n_layers, -1, None), which all mean the final layer
             sublayer_type (str, *optional*): The sub layer type of the activation, passed to utils.get_act_name. Can normally be inferred
             incl_remainder (bool, optional): Whether to return a final term which is "the rest of the residual stream". Defaults to False.
         """
-        
+
         if layer is None or layer == -1:
             # Default to the residual stream immediately pre unembed
             layer = self.model.cfg.n_layers
-        
+
         components = []
         for l in range(layer):
             components.append(self[(activation_name, l, sublayer_type)])
-        
+
         return torch.stack(components, dim=0)
 
     def get_neuron_results(
         self,
         layer: int,
         neuron_slice: Union[Slice, SliceInput] = None,
         pos_slice: Union[Slice, SliceInput] = None,
@@ -467,15 +498,20 @@
         self,
         layer: int,
         pos_slice: Union[Slice, SliceInput] = None,
         neuron_slice: Union[Slice, SliceInput] = None,
         return_labels: bool = False,
         incl_remainder: bool = False,
         apply_ln: bool = False,
-    ) -> Float[torch.Tensor, "num_components *batch_and_pos_dims d_model"]:
+    ) -> Union[
+        Float[torch.Tensor, "num_components *batch_and_pos_dims d_model"],
+        Tuple[
+            Float[torch.Tensor, "num_components *batch_and_pos_dims d_model"], List[str]
+        ],
+    ]:
         """Returns a stack of all neuron results (ie residual stream contribution) up to layer L - ie the amount each individual neuron contributes to the residual stream. Also returns a list of labels of the form "L0N0" for the neurons. A good way to decompose the outputs of MLP layers into attribution by specific neurons.
 
         Note that doing this for all neurons is SUPER expensive on GPU memory and only works for small models or short inputs.
 
         Args:
             layer (int): Layer index - heads at all layers strictly before this are included. layer must be in [1, n_layers]
             pos_slice (Slice, optional): Slice of the positions. Defaults to None. See utils.Slice for details.
@@ -493,15 +529,15 @@
         labels = []
 
         if not isinstance(neuron_slice, Slice):
             neuron_slice = Slice(neuron_slice)
         if not isinstance(pos_slice, Slice):
             pos_slice = Slice(pos_slice)
 
-        neuron_labels = neuron_slice.apply(np.arange(self.model.cfg.d_mlp), dim=0)
+        neuron_labels = neuron_slice.apply(torch.arange(self.model.cfg.d_mlp), dim=0)
         if type(neuron_labels) == int:
             neuron_labels = np.array([neuron_labels])
         for l in range(layer):
             # Note that this has shape batch x pos x head_index x d_model
             components.append(
                 self.get_neuron_results(
                     l, pos_slice=pos_slice, neuron_slice=neuron_slice
@@ -526,31 +562,31 @@
             components = torch.zeros(
                 0,
                 *pos_slice.apply(self["hook_embed"], dim=-2).shape,
                 device=self.model.cfg.device,
             )
 
         if apply_ln:
-            components = self.apply_ln_to_stack(
-                components, layer, pos_slice=pos_slice
-            )
+            components = self.apply_ln_to_stack(components, layer, pos_slice=pos_slice)
 
         if return_labels:
             return components, labels
         else:
             return components
 
     def apply_ln_to_stack(
         self,
-        residual_stack: Float[torch.Tensor, "num_components *batch_and_pos_dims d_model"],
+        residual_stack: Float[
+            torch.Tensor, "num_components *batch_and_pos_dims d_model"
+        ],
         layer: Optional[int] = None,
         mlp_input: bool = False,
         pos_slice: Union[Slice, SliceInput] = None,
         batch_slice: Union[Slice, SliceInput] = None,
-        has_batch_dim: bool = True
+        has_batch_dim: bool = True,
     ) -> Float[torch.Tensor, "num_components *batch_and_pos_dims d_model"]:
         """Takes a stack of components of the residual stream (eg outputs of decompose_resid or accumulated_resid), treats them as the input to a specific layer, and applies the layer norm scaling of that layer to them, using the cached scale factors - simulating what that component of the residual stream contributes to that layer's input.
 
         The layernorm scale is global across the entire residual stream for each layer, batch element and position, which is why we need to use the cached scale factors rather than just applying a new LayerNorm.
 
         If the model does not use LayerNorm, it returns the residual stack unchanged.
```

### Comparing `transformer_lens-1.2.2/transformer_lens/FactoredMatrix.py` & `transformer_lens-1.3.0/transformer_lens/FactoredMatrix.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from __future__ import annotations
 
 from functools import lru_cache
-from typing import Union, Tuple
+from typing import List, Tuple, Union
 
 import torch
 from jaxtyping import Float
+from typeguard import typeguard_ignore
 
 import transformer_lens.utils as utils
 
+
 class FactoredMatrix:
     """
     Class to represent low rank factored matrices, where the matrix is represented as a product of two matrices. Has utilities for efficient calculation of eigenvalues, norm and SVD.
     """
 
-    def __init__(self, A: Float[torch.Tensor, "... ldim mdim"], B: Float[torch.Tensor, "... mdim rdim"]):
+    def __init__(
+        self,
+        A: Float[torch.Tensor, "... ldim mdim"],
+        B: Float[torch.Tensor, "... mdim rdim"],
+    ):
         self.A = A
         self.B = B
         assert self.A.size(-1) == self.B.size(
             -2
         ), f"Factored matrix must match on inner dimension, shapes were a: {self.A.shape}, b:{self.B.shape}"
         self.ldim = self.A.size(-2)
         self.rdim = self.B.size(-1)
@@ -27,15 +33,20 @@
             self.ldim,
             self.rdim,
         )
         self.A = self.A.broadcast_to(self.shape[:-2] + (self.ldim, self.mdim))
         self.B = self.B.broadcast_to(self.shape[:-2] + (self.mdim, self.rdim))
 
     def __matmul__(
-        self, other: Union[Float[torch.Tensor, "... rdim new_rdim"], Float[torch.Tensor, "rdim"], FactoredMatrix]
+        self,
+        other: Union[
+            Float[torch.Tensor, "... rdim new_rdim"],
+            Float[torch.Tensor, "rdim"],
+            FactoredMatrix,
+        ],
     ) -> Union[FactoredMatrix, Float[torch.Tensor, "... ldim"]]:
         if isinstance(other, torch.Tensor):
             if other.ndim < 2:
                 # It's a vector, so we collapse the factorisation and just return a vector
                 # Squeezing/Unsqueezing is to preserve broadcasting working nicely
                 return (self.A @ (self.B @ other.unsqueeze(-1))).squeeze(-1)
             else:
@@ -46,15 +57,20 @@
                     return FactoredMatrix(self.A, self.B @ other)
                 else:
                     return FactoredMatrix(self.AB, other)
         elif isinstance(other, FactoredMatrix):
             return (self @ other.A) @ other.B
 
     def __rmatmul__(
-        self, other: Union[Float[torch.Tensor, "... new_rdim ldim"], Float[torch.Tensor, "ldim"], FactoredMatrix]
+        self,
+        other: Union[
+            Float[torch.Tensor, "... new_rdim ldim"],
+            Float[torch.Tensor, "ldim"],
+            FactoredMatrix,
+        ],
     ) -> Union[FactoredMatrix, Float[torch.Tensor, "... rdim"]]:
         if isinstance(other, torch.Tensor):
             assert (
                 other.size(-1) == self.ldim
             ), f"Left matrix must match on inner dimension, shapes were self: {self.shape}, other:{other.shape}"
             if other.ndim < 2:
                 # It's a vector, so we collapse the factorisation and just return a vector
@@ -63,27 +79,30 @@
                 return FactoredMatrix(other @ self.A, self.B)
             else:
                 return FactoredMatrix(other, self.AB)
         elif isinstance(other, FactoredMatrix):
             return other.A @ (other.B @ self)
 
     @property
+    @typeguard_ignore
     def AB(self) -> Float[torch.Tensor, "*leading_dims ldim rdim"]:
         """The product matrix - expensive to compute, and can consume a lot of GPU memory"""
         return self.A @ self.B
 
     @property
+    @typeguard_ignore
     def BA(self) -> Float[torch.Tensor, "*leading_dims rdim ldim"]:
         """The reverse product. Only makes sense when ldim==rdim"""
         assert (
             self.rdim == self.ldim
         ), f"Can only take ba if ldim==rdim, shapes were self: {self.shape}"
         return self.B @ self.A
 
     @property
+    @typeguard_ignore
     def T(self) -> FactoredMatrix:
         return FactoredMatrix(self.B.transpose(-2, -1), self.A.transpose(-2, -1))
 
     @lru_cache(maxsize=None)
     def svd(
         self,
     ) -> Tuple[
@@ -102,40 +121,58 @@
         Um, Sm, Vhm = torch.svd(middle)
         U = Ua @ Um
         Vh = Vhb @ Vhm
         S = Sm
         return U, S, Vh
 
     @property
+    @typeguard_ignore
     def U(self) -> Float[torch.Tensor, "*leading_dims ldim mdim"]:
         return self.svd()[0]
 
     @property
+    @typeguard_ignore
     def S(self) -> Float[torch.Tensor, "*leading_dims mdim"]:
         return self.svd()[1]
 
     @property
+    @typeguard_ignore
     def Vh(self) -> Float[torch.Tensor, "*leading_dims rdim mdim"]:
         return self.svd()[2]
 
     @property
+    @typeguard_ignore
     def eigenvalues(self) -> Float[torch.Tensor, "*leading_dims mdim"]:
         """Eigenvalues of AB are the same as for BA (apart from trailing zeros), because if BAv=kv ABAv = A(BAv)=kAv, so Av is an eigenvector of AB with eigenvalue k."""
         return torch.linalg.eig(self.BA).eigenvalues
 
+    def _convert_to_slice(self, sequence: Union[Tuple, List], idx: int) -> Tuple:
+        """
+        e.g. if sequence = (1, 2, 3) and idx = 1, return (1, slice(2, 3), 3)
+        """
+        if isinstance(idx, int):
+            sequence = list(sequence)
+            sequence[idx] = slice(sequence[idx], sequence[idx] + 1)
+            sequence = tuple(sequence)
+
+        return sequence
+
     def __getitem__(self, idx: Union[int, Tuple]) -> FactoredMatrix:
         """Indexing - assumed to only apply to the leading dimensions."""
         if not isinstance(idx, tuple):
             idx = (idx,)
         length = len([i for i in idx if i is not None])
         if length <= len(self.shape) - 2:
             return FactoredMatrix(self.A[idx], self.B[idx])
         elif length == len(self.shape) - 1:
+            idx = self._convert_to_slice(idx, -1)
             return FactoredMatrix(self.A[idx], self.B[idx[:-1]])
         elif length == len(self.shape):
+            idx = self._convert_to_slice(idx, -1)
+            idx = self._convert_to_slice(idx, -2)
             return FactoredMatrix(
                 self.A[idx[:-1]], self.B[idx[:-2] + (slice(None), idx[-1])]
             )
         else:
             raise ValueError(
                 f"{idx} is too long an index for a FactoredMatrix with shape {self.shape}"
             )
@@ -158,14 +195,15 @@
             self.S.sqrt()[..., :, None] * utils.transpose(self.Vh),
         )
 
     def get_corner(self, k=3):
         return utils.get_corner(self.A[..., :k, :] @ self.B[..., :, :k], k)
 
     @property
+    @typeguard_ignore
     def ndim(self) -> int:
         return len(self.shape)
 
     def collapse_l(self) -> Float[torch.Tensor, "*leading_dims mdim rdim"]:
         """
         Collapses the left side of the factorization by removing the orthogonal factor (given by self.U). Returns a (..., mdim, rdim) tensor
         """
@@ -177,13 +215,15 @@
         """
         return self.U * self.S[..., None, :]
 
     def unsqueeze(self, k: int) -> FactoredMatrix:
         return FactoredMatrix(self.A.unsqueeze(k), self.B.unsqueeze(k))
 
     @property
+    @typeguard_ignore
     def pair(
         self,
     ) -> Tuple[
-        Float[torch.Tensor, "*leading_dims ldim mdim"], Float[torch.Tensor, "*leading_dims mdim rdim"]
+        Float[torch.Tensor, "*leading_dims ldim mdim"],
+        Float[torch.Tensor, "*leading_dims mdim rdim"],
     ]:
-        return (self.A, self.B)
+        return (self.A, self.B)
```

### Comparing `transformer_lens-1.2.2/transformer_lens/HookedTransformer.py` & `transformer_lens-1.3.0/transformer_lens/HookedTransformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,73 @@
-from typing import Callable, Union, List, Tuple, Dict, Optional, NamedTuple, overload
-from typing_extensions import Literal
+import logging
+from functools import lru_cache
+from typing import Dict, List, NamedTuple, Optional, Tuple, Union, overload
+
+import einops
+import numpy as np
 import torch
 import torch.nn as nn
-import torch.nn.functional as F
-import numpy as np
-import einops
-import logging
 import tqdm.auto as tqdm
-import re
-from huggingface_hub import HfApi
-from functools import partial, lru_cache
-from collections import namedtuple
+from fancy_einsum import einsum
 from jaxtyping import Float, Int
+from transformers import AutoTokenizer, PreTrainedTokenizerBase
+from typeguard import typeguard_ignore
+from typing_extensions import Literal
 
-from transformers import (
-    AutoTokenizer,
-    PreTrainedTokenizer,
-)
-from datasets.load import load_dataset
-
-from transformer_lens.hook_points import HookedRootModule, HookPoint
+import transformer_lens.loading_from_pretrained as loading
+import transformer_lens.utils as utils
 from transformer_lens import HookedTransformerConfig
 from transformer_lens.ActivationCache import ActivationCache
-from transformer_lens.FactoredMatrix import FactoredMatrix
-# Note - activation cache is used with run_with_cache, past_key_value_caching is used for generation.
-from transformer_lens.past_key_value_caching import (
-    HookedTransformerKeyValueCache,
+from transformer_lens.components import (
+    Embed,
+    LayerNorm,
+    LayerNormPre,
+    PosEmbed,
+    RMSNorm,
+    RMSNormPre,
+    TransformerBlock,
+    Unembed,
 )
+from transformer_lens.FactoredMatrix import FactoredMatrix
+from transformer_lens.hook_points import HookedRootModule, HookPoint
 
-from transformer_lens.components import *
-import transformer_lens.loading_from_pretrained as loading
-import transformer_lens.utils as utils
+# Note - activation cache is used with run_with_cache, past_key_value_caching is used for generation.
+from transformer_lens.past_key_value_caching import HookedTransformerKeyValueCache
 from transformer_lens.utilities import devices
 
-SingleLoss = Float[torch.Tensor, ""] # Type alias for a single element tensor
+SingleLoss = Float[torch.Tensor, ""]  # Type alias for a single element tensor
 LossPerToken = Float[torch.Tensor, "batch pos-1"]
 Loss = Union[SingleLoss, LossPerToken]
 
+
 # Named tuple object for if we want to output both logits and loss
 class Output(NamedTuple):
     logits: Float[torch.Tensor, "batch pos d_vocab"]
     loss: Loss
 
 
 class HookedTransformer(HookedRootModule):
     """
     This class implements a full Transformer using the components in ./components.py, with
     HookPoints on every interesting activation. It inherits from HookedRootModule.
 
-    It can have a pretrained Transformer's weights automatically loaded in via the HookedTransformer.from_pretrained class method. It can also be instantiated with randomly initialized weights via __init__ and being passed a dict or HookedTransformerConfig object.
+    It can have a pretrained Transformer's weights automatically loaded in via the HookedTransformer.from_pretrained
+    class method. It can also be instantiated with randomly initialized weights via __init__ and being passed a dict or
+    HookedTransformerConfig object.
     """
 
     def __init__(
         self,
         cfg,
         tokenizer=None,
         move_to_device=True,
     ):
         """
-        Model initialization. Note that if you want to load the model from pretrained weights, you should use the HookedTransformer.from_pretrained() class method instead of this one.
+        Model initialization. Note that if you want to load the model from pretrained weights, you should use the
+        HookedTransformer.from_pretrained() class method instead of this one.
 
         cfg Union[HookedTransformerConfig, Dict]: The config to use for the
             model.
         tokenizer (*optional): The tokenizer to use for the model. If not
             provided, it is inferred from cfg.tokenizer_name or initialized to None.
             If None, then the model cannot be passed strings, and d_vocab must be explicitly set.
         move_to_device (bool): Whether to move the model to the device specified in cfg.
@@ -70,68 +75,60 @@
             will be split across multiple devices.
         """
         super().__init__()
         if isinstance(cfg, Dict):
             cfg = HookedTransformerConfig(**cfg)
         elif isinstance(cfg, str):
             raise ValueError(
-                "Please pass in a config dictionary or HookedTransformerConfig object. If you want to load a pretrained model, use HookedTransformer.from_pretrained() instead."
+                "Please pass in a config dictionary or HookedTransformerConfig object. If you want to load a "
+                "pretrained model, use HookedTransformer.from_pretrained() instead."
             )
         self.cfg = cfg
 
         assert (
             self.cfg.n_devices == 1 or move_to_device
         ), "If n_devices > 1, must move_to_device"
 
         if tokenizer is not None:
-            self.tokenizer = tokenizer
+            self.set_tokenizer(tokenizer)
         elif self.cfg.tokenizer_name is not None:
             # If we have a tokenizer name, we can load it from HuggingFace
-            if 'llama' in self.cfg.tokenizer_name: 
+            if "llama" in self.cfg.tokenizer_name:
                 # llama tokenizer requires special handling
                 print("Warning: LLaMA tokenizer not loaded. Please load manually.")
-            else: 
-                self.tokenizer = AutoTokenizer.from_pretrained(self.cfg.tokenizer_name)
-                if self.tokenizer.eos_token is None:
-                    self.tokenizer.eos_token = "<|endoftext|>"
-                if self.tokenizer.pad_token is None:
-                    self.tokenizer.pad_token = self.tokenizer.eos_token
-                if self.tokenizer.bos_token is None:
-                    self.tokenizer.bos_token = self.tokenizer.eos_token
+            else:
+                self.set_tokenizer(
+                    AutoTokenizer.from_pretrained(self.cfg.tokenizer_name)
+                )
         else:
-            # If no tokenizer name is provided, we assume we're training on an algorithmic task and will pass in tokens directly. In this case, we don't need a tokenizer.
-            self.tokenizer = None
-
-        if self.cfg.d_vocab == -1:
-            # If we have a tokenizer, vocab size can be inferred from it.
+            # If no tokenizer name is provided, we assume we're training on an algorithmic task and will pass in tokens
+            # directly. In this case, we don't need a tokenizer.
             assert (
-                self.tokenizer is not None
+                self.cfg.d_vocab != -1
             ), "Must provide a tokenizer if d_vocab is not provided"
-            self.cfg.d_vocab = max(self.tokenizer.vocab.values()) + 1
-        if self.cfg.d_vocab_out == -1:
-            self.cfg.d_vocab_out = self.cfg.d_vocab
+            self.tokenizer = None
 
         self.embed = Embed(self.cfg)
         self.hook_embed = HookPoint()  # [batch, pos, d_model]
 
         if self.cfg.positional_embedding_type != "rotary":
             self.pos_embed = PosEmbed(self.cfg)
             self.hook_pos_embed = HookPoint()  # [batch, pos, d__dictmodel]
 
         if self.cfg.use_hook_tokens:
-            self.hook_tokens = HookPoint() # [batch, pos]
+            self.hook_tokens = HookPoint()  # [batch, pos]
 
         self.blocks = nn.ModuleList(
             [
                 TransformerBlock(self.cfg, block_index)
                 for block_index in range(self.cfg.n_layers)
             ]
         )
 
-        if self.cfg.normalization_type == "RMS": 
+        if self.cfg.normalization_type == "RMS":
             self.ln_final = RMSNorm(self.cfg)
         elif self.cfg.normalization_type == "RMSPre":
             self.ln_final = RMSNormPre(self.cfg)
         elif self.cfg.normalization_type == "LN":
             if self.cfg.final_rms:
                 self.ln_final = RMSNorm(self.cfg)
             else:
@@ -151,99 +148,131 @@
             )
         self.unembed = Unembed(self.cfg)
 
         if self.cfg.init_weights:
             self.init_weights()
 
         if move_to_device:
-            # We load the devices in a pipeline manner - the first device gets the embed and pos_embed layers and the first n_layers // n_devices blocks,
-            # the second gets the next n_layers // n_devices blocks ... the last gets the last n_layers // n_devices blocks, the final
+            # We load the devices in a pipeline manner - the first device gets the embed and pos_embed layers and the
+            # first n_layers // n_devices blocks,
+            # the second gets the next n_layers // n_devices blocks ... the last gets the last n_layers // n_devices
+            # blocks, the final
             # normalization layer (if it exists) and the unembed layer
             HookedTransformer.move_model_modules_to_device(self)
 
-        # Helper variable to store a small (10K-20K) dataset of training data. Empty by default, can be loaded with load_sample_training_dataset
+        # Helper variable to store a small (10K-20K) dataset of training data. Empty by default, can be loaded with
+        # load_sample_training_dataset
         self.dataset = None
 
         # Gives each module a parameter with its name (relative to this root module)
         # Needed for HookPoints to work
         self.setup()
 
-    def check_hooks_to_add(self, hook_point, hook_point_name, hook, dir="fwd", is_permanent=False) -> None:
+    def check_hooks_to_add(
+        self,
+        hook_point,
+        hook_point_name,
+        hook,
+        dir="fwd",
+        is_permanent=False,
+        prepend=False,
+    ) -> None:
         if hook_point_name.endswith("attn.hook_result"):
-            assert self.cfg.use_attn_result, f"Cannot add hook {hook_point_name} if use_attn_result_hook is False"
+            assert (
+                self.cfg.use_attn_result
+            ), f"Cannot add hook {hook_point_name} if use_attn_result_hook is False"
         if hook_point_name.endswith(("hook_q_input", "hook_k_input", "hook_v_input")):
-            assert self.cfg.use_split_qkv_input, f"Cannot add hook {hook_point_name} if use_split_qkv_input is False"
+            assert (
+                self.cfg.use_split_qkv_input
+            ), f"Cannot add hook {hook_point_name} if use_split_qkv_input is False"
 
     @overload
     def forward(
-        self, 
-        input, 
-        return_type: Literal["logits"], 
+        self,
+        input,
+        return_type: Literal["logits"],
         loss_per_token: bool = False,
         prepend_bos: bool = True,
-        stop_at_layer: Optional[int] = None, 
-        past_kv_cache: Optional[HookedTransformerKeyValueCache] = None) -> Loss:
+        stop_at_layer: Optional[int] = None,
+        past_kv_cache: Optional[HookedTransformerKeyValueCache] = None,
+    ) -> Loss:
         ...
 
     @overload
     def forward(
-        self, 
-        input, 
-        return_type: Literal["loss"], 
+        self,
+        input,
+        return_type: Literal["loss"],
         loss_per_token: bool = False,
         prepend_bos: bool = True,
-        stop_at_layer: Optional[int] = None, 
-        past_kv_cache: Optional[HookedTransformerKeyValueCache] = None) -> Loss:
+        stop_at_layer: Optional[int] = None,
+        past_kv_cache: Optional[HookedTransformerKeyValueCache] = None,
+    ) -> Loss:
         ...
-    
+
     @overload
     def forward(
-        self, 
-        input, 
-        return_type: Literal["both"], 
+        self,
+        input,
+        return_type: Literal["both"],
         loss_per_token: bool = False,
         prepend_bos: bool = True,
-        stop_at_layer: Optional[int] = None, 
-        past_kv_cache: Optional[HookedTransformerKeyValueCache] = None) -> Tuple[Float[torch.Tensor, "batch pos d_vocab"], Loss]:
+        stop_at_layer: Optional[int] = None,
+        past_kv_cache: Optional[HookedTransformerKeyValueCache] = None,
+    ) -> Tuple[Float[torch.Tensor, "batch pos d_vocab"], Loss]:
         ...
 
     @overload
     def forward(
-        self, 
-        input, 
-        return_type: Literal[None], 
+        self,
+        input,
+        return_type: Literal[None],
         loss_per_token: bool = False,
         prepend_bos: bool = True,
-        stop_at_layer: Optional[int] = None, 
-        past_kv_cache: Optional[HookedTransformerKeyValueCache] = None) -> None:
+        stop_at_layer: Optional[int] = None,
+        past_kv_cache: Optional[HookedTransformerKeyValueCache] = None,
+    ) -> None:
         ...
 
     # TODO make sure type assertions are provided
     def forward(
         self,
         input: Union[str, List[str], Int[torch.Tensor, "batch pos"]],
         return_type: Optional[str] = "logits",
         loss_per_token: bool = False,
         prepend_bos: bool = True,
-        stop_at_layer: Optional[int] = None, 
+        stop_at_layer: Optional[int] = None,
         past_kv_cache: Optional[HookedTransformerKeyValueCache] = None,
     ) -> Union[
         None,
         Float[torch.Tensor, "batch pos d_vocab"],
         Loss,
         Tuple[Float[torch.Tensor, "batch pos d_vocab"], Loss],
     ]:
-        """Input is either a batch of tokens ([batch, pos]) or a text string, a string is automatically tokenized to a batch of a single element. The prepend_bos flag only applies when inputting a text string.
+        """Input is either a batch of tokens ([batch, pos]) or a text string, a string is automatically tokenized to a
+        batch of a single element. The prepend_bos flag only applies when inputting a text string.
 
-        return_type Optional[str]: The type of output to return. Can be one of: None (return nothing, don't calculate logits), 'logits' (return logits), 'loss' (return cross-entropy loss), 'both' (return logits and loss)
-        loss_per_token bool: Whether to return the (next token prediction) loss per token (True) or average (False). Average loss is a scalar (averaged over position *and* batch), per-token loss is a tensor ([batch, position-1]) - position-1 because we're predicting the next token, and there's no specified next token for the final token. Defaults to False.
-        prepend_bos bool: Whether to prepend the BOS token to the input. Only applies when input is a string. Defaults to True (unlike to_tokens) - even for models not explicitly trained with this, heads often use the first position as a resting position and accordingly lose information from the first token, so this empirically seems to give better results.
-        stop_at_layer Optional[int]: If not None, stop the forward pass at the specified layer. Exclusive - ie, stop_at_layer = 0 will only run the embedding layer, stop_at_layer = 1 will run the embedding layer and the first transformer block, etc. Supports negative indexing. Useful for analysis of intermediate layers, eg finding neuron activations in layer 3 of a 24 layer model. Defaults to None (run the full model).
-
-        Note that loss is the standard "predict the next token" cross-entropy loss for GPT-2 style language models - if you want a custom loss function, the recommended behaviour is returning the logits and then applying your custom loss function.
+        return_type Optional[str]: The type of output to return. Can be one of: None (return nothing, don't calculate
+            logits), 'logits' (return logits), 'loss' (return cross-entropy loss), 'both' (return logits and loss)
+        loss_per_token bool: Whether to return the (next token prediction) loss per token (True) or average (False).
+            Average loss is a scalar (averaged over position *and* batch), per-token loss is a tensor ([batch, position-1])
+            - position-1 because we're predicting the next token, and there's no specified next token for the final
+            token. Defaults to False.
+        prepend_bos bool: Whether to prepend the BOS token to the input. Only applies when input is a string. Defaults
+            to True (unlike to_tokens) - even for models not explicitly trained with this, heads often use the first
+            position as a resting position and accordingly lose information from the first token, so this empirically
+            seems to give better results.
+        stop_at_layer Optional[int]: If not None, stop the forward pass at the specified layer. Exclusive - ie,
+        stop_at_layer = 0 will only run the embedding layer, stop_at_layer = 1 will run the embedding layer and the
+        first transformer block, etc. Supports negative indexing. Useful for analysis of intermediate layers, eg finding
+        neuron activations in layer 3 of a 24 layer model. Defaults to None (run the full model).
+
+        Note that loss is the standard "predict the next token" cross-entropy loss for GPT-2 style language models -
+        if you want a custom loss function, the recommended behaviour is returning the logits and then applying your
+        custom loss function.
         """
         if type(input) == str or type(input) == list:
             # If text, convert to tokens (batch_size=1)
             assert (
                 self.tokenizer is not None
             ), "Must provide a tokenizer if passing a string to the model"
             # This is only intended to support passing in a single string
@@ -286,37 +315,41 @@
         if self.cfg.positional_embedding_type == "standard":
             pos_embed = self.hook_pos_embed(
                 self.pos_embed(tokens, pos_offset)
             )  # [batch, pos, d_model]
             residual = embed + pos_embed  # [batch, pos, d_model]
             shortformer_pos_embed = None
         elif self.cfg.positional_embedding_type == "shortformer":
-            # If we're using shortformer style attention, we don't add the positional embedding to the residual stream. See HookedTransformerConfig for details
+            # If we're using shortformer style attention, we don't add the positional embedding to the residual stream.
+            # See HookedTransformerConfig for details
             pos_embed = self.hook_pos_embed(
                 self.pos_embed(tokens, pos_offset)
             )  # [batch, pos, d_model]
             residual = embed
             shortformer_pos_embed = pos_embed
         elif self.cfg.positional_embedding_type == "rotary":
-            # Rotary doesn't use positional embeddings, instead they're applied when dot producting keys and queries. See HookedTransformerConfig for details
+            # Rotary doesn't use positional embeddings, instead they're applied when dot producting keys and queries.
+            # See HookedTransformerConfig for details
             residual = embed
             shortformer_pos_embed = None
         else:
             raise ValueError(
                 f"Invalid positional_embedding_type passed in {self.cfg.positional_embedding_type}"
             )
-        
+
         if stop_at_layer is None:
             # We iterate through every block by default
             transformer_block_list = self.blocks
         else:
-            # If we explicitly want to stop at a layer, we only iterate through the blocks up to that layer. Note that this is exclusive, eg stop_at_layer==0 means to only run the embed, stop_at_layer==-1 means to run every layer *apart* from the final one, etc.
-            transformer_block_list = self.blocks[:stop_at_layer] # type: ignore
- 
-        for i, block in enumerate(transformer_block_list): # type: ignore
+            # If we explicitly want to stop at a layer, we only iterate through the blocks up to that layer. Note that
+            # this is exclusive, eg stop_at_layer==0 means to only run the embed, stop_at_layer==-1 means to run every
+            # layer *apart* from the final one, etc.
+            transformer_block_list = self.blocks[:stop_at_layer]  # type: ignore
+
+        for i, block in enumerate(transformer_block_list):  # type: ignore
             # Note that each block includes skip connections, so we don't need
             # residual + block(residual)
             # If we're using multiple GPUs, we need to send the residual and shortformer_pos_embed to the correct GPU
             residual = residual.to(devices.get_device_for_block_index(i, self.cfg))
             if shortformer_pos_embed is not None:
                 shortformer_pos_embed = shortformer_pos_embed.to(
                     devices.get_device_for_block_index(i, self.cfg)
@@ -325,15 +358,15 @@
             residual = block(
                 residual,
                 past_kv_cache_entry=past_kv_cache[i]
                 if past_kv_cache is not None
                 else None,  # Cache contains a list of HookedTransformerKeyValueCache objects, one for each block
                 shortformer_pos_embed=shortformer_pos_embed,
             )  # [batch, pos, d_model]
-        
+
         if stop_at_layer is not None:
             # When we stop at an early layer, we end here rather than doing further computation
             return None
 
         if self.cfg.normalization_type is not None:
             residual = self.ln_final(residual)  # [batch, pos, d_model]
         if return_type is None:
@@ -385,15 +418,17 @@
             Float[torch.Tensor, "batch pos d_vocab"],
             Loss,
             Tuple[Float[torch.Tensor, "batch pos d_vocab"], Loss],
         ],
         Union[ActivationCache, Dict[str, torch.Tensor]],
     ]:
         """
-        Wrapper around run_with_cache in HookedRootModule. If return_cache_object is True, this will return an ActivationCache object, with a bunch of useful HookedTransformer specific methods, otherwise it will return a dictionary of activations as in HookedRootModule.
+        Wrapper around run_with_cache in HookedRootModule. If return_cache_object is True, this will return an
+        ActivationCache object, with a bunch of useful HookedTransformer specific methods, otherwise it will return a
+        dictionary of activations as in HookedRootModule.
         """
         out, cache_dict = super().run_with_cache(
             *model_args, remove_batch_dim=remove_batch_dim, **kwargs
         )
         if return_cache_object:
             cache = ActivationCache(
                 cache_dict, self, has_batch_dim=not remove_batch_dim
@@ -403,59 +438,88 @@
             return out, cache_dict
 
     def set_tokenizer(self, tokenizer):
         """
         Sets the tokenizer to use for this model.
         tokenizer (PreTrainedTokenizer): a pretrained HuggingFace tokenizer
         """
-        assert isinstance(tokenizer, PreTrainedTokenizer)
+        assert isinstance(
+            tokenizer, PreTrainedTokenizerBase
+        ), f"{type(tokenizer)} is not a supported tokenizer, please use PreTrainedTokenizer or PreTrainedTokenizerFast"
         self.tokenizer = tokenizer
-        self.tokenizer.pad_token = self.tokenizer.eos_token
+
+        if self.tokenizer.eos_token is None:
+            self.tokenizer.eos_token = "<|endoftext|>"
+        if self.tokenizer.pad_token is None:
+            self.tokenizer.pad_token = self.tokenizer.eos_token
+        if self.tokenizer.bos_token is None:
+            self.tokenizer.bos_token = self.tokenizer.eos_token
+
+        # Infer vocab size from tokenizer
+        if self.cfg.d_vocab == -1:
+            self.cfg.d_vocab = max(self.tokenizer.vocab.values()) + 1
+        if self.cfg.d_vocab_out == -1:
+            self.cfg.d_vocab_out = self.cfg.d_vocab
 
     def to_tokens(
         self,
         input: Union[str, List[str]],
         prepend_bos: bool = True,
         move_to_device: bool = True,
-        truncate: bool = True
+        truncate: bool = True,
     ) -> Int[torch.Tensor, "batch pos"]:
         """
-        Converts a string to a tensor of tokens. If prepend_bos is True, prepends the BOS token to the input - this is recommended when creating a sequence of tokens to be input to a model. 
+        Converts a string to a tensor of tokens. If prepend_bos is True, prepends the BOS token to the input - this is
+        recommended when creating a sequence of tokens to be input to a model.
 
         Args:
             input (Union[str, List[str]]). The input to tokenize
             prepend_bos (bool): Whether to prepend a beginning of sequence token. Defaults to True
-            move_to_device (bool): Whether to move the output tensor of tokens to the device the model lives on. Defaults to True
-            truncate (bool): If the output tokens are too long, whether to truncate the output tokens to the model's max context window. Does nothing for shorter inputs. Defaults to True.
-
-        Gotcha: prepend_bos prepends a beginning of string token. This is a recommended default when inputting a prompt to the model as the first token is often treated weirdly, but should only be done at the START of the prompt. Make sure to turn it off if you're looking at the tokenization of part of the prompt!
+            move_to_device (bool): Whether to move the output tensor of tokens to the device the model lives on.
+            Defaults to True
+            truncate (bool): If the output tokens are too long, whether to truncate the output tokens to the model's
+            max context window. Does nothing for shorter inputs. Defaults to True.
+
+        Gotcha: prepend_bos prepends a beginning of string token. This is a recommended default when inputting a prompt
+        to the model as the first token is often treated weirdly, but should only be done at the START of the prompt.
+        Make sure to turn it off if you're looking at the tokenization of part of the prompt!
         (Note: some models eg GPT-2 were not trained with a BOS token, others (OPT and my models) were)
 
-        Gotcha2: Tokenization of a string depends on whether there is a preceding space and whether the first letter is capitalized. It's easy to shoot yourself in the foot here if you're not careful!
+        Gotcha2: Tokenization of a string depends on whether there is a preceding space and whether the first letter is
+        capitalized. It's easy to shoot yourself in the foot here if you're not careful!
         """
         assert self.tokenizer is not None, "Cannot use to_tokens without a tokenizer"
         if prepend_bos:
             if isinstance(input, str):
                 input = self.tokenizer.bos_token + input
             else:
                 input = [self.tokenizer.bos_token + string for string in input]
         tokens = self.tokenizer(
-            input, 
-            return_tensors = "pt", 
-            padding = True,
-            truncation = truncate,
-            max_length = self.cfg.n_ctx if truncate else None,
-            add_special_tokens = False if self.tokenizer.name_or_path.startswith('facebook/opt') else True  # As we manually add the BOS token
-            )["input_ids"]
+            input,
+            return_tensors="pt",
+            padding=True,
+            truncation=truncate,
+            max_length=self.cfg.n_ctx if truncate else None,
+            add_special_tokens=False
+            if self.tokenizer.name_or_path.startswith("facebook/opt")
+            else True,  # As we manually add the BOS token
+        )["input_ids"]
         if move_to_device:
             tokens = tokens.to(self.cfg.device)
         return tokens
 
     def to_string(
-        self, tokens: Union[Int[torch.Tensor, "batch pos"], Int[torch.Tensor, "pos"], np.ndarray, List[Float[torch.Tensor, "pos"]]]
+        self,
+        tokens: Union[
+            Int[torch.Tensor, ""],
+            Int[torch.Tensor, "batch pos"],
+            Int[torch.Tensor, "pos"],
+            np.ndarray,
+            List[Int[torch.Tensor, "pos"]],
+        ],
     ) -> Union[str, List[str]]:
         """
         Converts a tensor of tokens to a string (if rank 1) or a list of strings (if rank 2).
 
         Accepts lists of tokens and numpy arrays as inputs too (and converts to tensors internally)
         """
         assert self.tokenizer is not None, "Cannot use to_string without a tokenizer"
@@ -474,34 +538,41 @@
         elif len(tokens.shape) <= 1:
             return self.tokenizer.decode(tokens, clean_up_tokenization_spaces=False)
         else:
             raise ValueError(f"Invalid shape passed in: {tokens.shape}")
 
     def to_str_tokens(
         self,
-        input: Union[str,
-                     Int[torch.Tensor, "pos"],
-                     Int[torch.Tensor, "1 pos"],
-                     Int[np.ndarray, "pos"],
-                     Int[np.ndarray, "1 pos"],
-                     list],
+        input: Union[
+            str,
+            Int[torch.Tensor, "pos"],
+            Int[torch.Tensor, "1 pos"],
+            Int[np.ndarray, "pos"],
+            Int[np.ndarray, "1 pos"],
+            list,
+        ],
         prepend_bos: bool = True,
     ) -> List[str]:
         """Method to map text, a list of text or tokens to a list of tokens as strings
 
-        Gotcha: prepend_bos prepends a beginning of string token. This is a recommended default when inputting a prompt to the model as the first token is often treated weirdly, but should only be done at the START of the prompt. Make sure to turn it off if you're looking at the tokenization of part of the prompt!
+        Gotcha: prepend_bos prepends a beginning of string token. This is a recommended default when inputting a prompt
+        to the model as the first token is often treated weirdly, but should only be done at the START of the prompt.
+        Make sure to turn it off if you're looking at the tokenization of part of the prompt!
         (Note: some models eg GPT-2 were not trained with a BOS token, others (OPT and my models) were)
 
-        Gotcha2: Tokenization of a string depends on whether there is a preceding space and whether the first letter is capitalized. It's easy to shoot yourself in the foot here if you're not careful!
+        Gotcha2: Tokenization of a string depends on whether there is a preceding space and whether the first letter is
+        capitalized. It's easy to shoot yourself in the foot here if you're not careful!
 
         Gotcha3: If passing a string that exceeds the model's context length (model.cfg.n_ctx), it will be truncated.
 
         Args:
-            input (Union[str, list, torch.Tensor]): The input - either a string or a tensor of tokens. If tokens, should be a tensor of shape [pos] or [1, pos]
-            prepend_bos (bool, optional): Whether to prepend a BOS token. Only applies if input is a string. Defaults to True.
+            input (Union[str, list, torch.Tensor]): The input - either a string or a tensor of tokens. If tokens, should
+            be a tensor of shape [pos] or [1, pos]
+            prepend_bos (bool, optional): Whether to prepend a BOS token. Only applies if input is a string. Defaults to
+            True.
 
         Returns:
             str_tokens: List of individual tokens as strings
         """
         if isinstance(input, list):
             return list(
                 map(lambda tokens: self.to_str_tokens(tokens, prepend_bos), input)
@@ -530,15 +601,16 @@
             raise ValueError(f"Invalid input type to to_str_tokens: {type(input)}")
         str_tokens = self.tokenizer.batch_decode(
             tokens, clean_up_tokenization_spaces=False
         )
         return str_tokens
 
     def to_single_token(self, string):
-        """Maps a string that makes up a single token to the id for that token. Raises an error for strings that are not a single token! If uncertain use to_tokens"""
+        """Maps a string that makes up a single token to the id for that token. Raises an error for strings that are
+        not a single token! If uncertain use to_tokens"""
 
         # We use the to_tokens method, do not append a BOS token
         token = self.to_tokens(string, prepend_bos=False).squeeze()
         # If token shape is non-empty, raise error
         assert not token.shape, f"Input string: {string} is not a single token!"
         return token.item()
 
@@ -548,114 +620,129 @@
         token = self.to_str_tokens(torch.tensor([int_token]))
         assert len(token) == 1
         return token[0]
 
     def get_token_position(
         self,
         single_token: Union[str, int],
-        input: Union[str, Union[Float[torch.Tensor, "pos"], Float[torch.Tensor, "1 pos"]]],
+        input: Union[
+            str, Union[Float[torch.Tensor, "pos"], Float[torch.Tensor, "1 pos"]]
+        ],
         mode="first",
         prepend_bos=True,
     ):
         """
-        Get the position of a single_token in a string or sequence of tokens. Raises an error if the token is not present.
+        Get the position of a single_token in a string or sequence of tokens. Raises an error if the token is not
+        present.
 
-        Gotcha: If you're inputting a string, it'll automatically be tokenized. Be careful about prepend_bos is true or false! When a string is input to the model, a BOS (beginning of sequence) token is prepended by default when the string is tokenized. But this should only be done at the START of the input, not when inputting part of the prompt. If you're getting weird off-by-one errors, check carefully for what the setting should be!
+        Gotcha: If you're inputting a string, it'll automatically be tokenized. Be careful about prepend_bos is true or
+        false! When a string is input to the model, a BOS (beginning of sequence) token is prepended by default when the
+        string is tokenized. But this should only be done at the START of the input, not when inputting part of the
+        prompt. If you're getting weird off-by-one errors, check carefully for what the setting should be!
 
         Args:
             single_token (Union[str, int]): The token to search for. Can
                 be a token index, or a string (but the string must correspond to a
                 single token)
             input (Union[str, torch.Tensor]): The sequence to
-                search in. Can be a string or a rank 1 tensor of tokens or a rank 2 tensor of tokens with a dummy batch dimension.
-            mode (str, optional): If there are multiple matches, which match to return. Supports "first" or "last". Defaults to "first".
-            prepend_bos (bool): Prepends a BOS (beginning of sequence) token when tokenizing a string. Only matters when inputting a string to 
-                the function, otherwise ignored. 
+                search in. Can be a string or a rank 1 tensor of tokens or a rank 2 tensor of tokens with a dummy batch
+                dimension.
+            mode (str, optional): If there are multiple matches, which match to return. Supports "first" or "last".
+                Defaults to "first".
+            prepend_bos (bool): Prepends a BOS (beginning of sequence) token when tokenizing a string. Only matters when
+                inputting a string to the function, otherwise ignored.
         """
         if isinstance(input, str):
             # If the input is a string, convert to tensor
             tokens = self.to_tokens(input, prepend_bos=prepend_bos)
         else:
             tokens = input
-        
 
         if len(tokens.shape) == 2:
             # If the tokens have shape [1, seq_len], flatten to [seq_len]
             assert (
                 tokens.shape[0] == 1
             ), f"If tokens are rank two, they must have shape [1, seq_len], not {tokens.shape}"
             tokens = tokens[0]
 
         if isinstance(single_token, str):
             # If the single token is a string, convert to an integer
             single_token = self.to_single_token(single_token)
         elif isinstance(single_token, torch.Tensor):
             single_token = single_token.item()
 
-        indices = torch.arange(len(tokens))[tokens == single_token]
-        assert len(indices)>0, f"The token does not occur in the prompt"
+        indices = torch.arange(len(tokens), device=tokens.device)[
+            tokens == single_token
+        ]
+        assert len(indices) > 0, f"The token does not occur in the prompt"
         if mode == "first":
             return indices[0].item()
         elif mode == "last":
             return indices[-1].item()
         else:
             raise ValueError(f"mode must be 'first' or 'last', not {mode}")
 
-    def tokens_to_residual_directions(self, tokens: Union[str, int, Int[torch.Tensor, ""], Int[torch.Tensor, "pos"], Int[torch.Tensor, "batch pos"]]) -> Union[Float[torch.Tensor, "d_model"], Float[torch.Tensor, "pos d_model"], Float[torch.Tensor, "batch pos d_model"]]:
-        """Maps tokens to a tensor with the unembedding vector for those tokens, ie the vector in the residual stream that we dot with to the get the logit for that token.
+    def tokens_to_residual_directions(
+        self,
+        tokens: Union[
+            str,
+            int,
+            Int[torch.Tensor, ""],
+            Int[torch.Tensor, "pos"],
+            Int[torch.Tensor, "batch pos"],
+        ],
+    ) -> Union[
+        Float[torch.Tensor, "d_model"],
+        Float[torch.Tensor, "pos d_model"],
+        Float[torch.Tensor, "batch pos d_model"],
+    ]:
+        """Maps tokens to a tensor with the unembedding vector for those tokens, ie the vector in the residual stream
+        that we dot with to the get the logit for that token.
 
-        WARNING: If you use this without folding in LayerNorm, the results will be misleading and may be incorrect, as the LN weights change the unembed map. This is done automatically with the fold_ln flag on from_pretrained
-        
-        WARNING 2: LayerNorm scaling will scale up or down the effective direction in the residual stream for each output token on any given input token position. ActivationCache.apply_ln_to_stack will apply the appropriate scaling to these directions.
+        WARNING: If you use this without folding in LayerNorm, the results will be misleading and may be incorrect, as
+        the LN weights change the unembed map. This is done automatically with the fold_ln flag on from_pretrained
+
+        WARNING 2: LayerNorm scaling will scale up or down the effective direction in the residual stream for each
+        output token on any given input token position. ActivationCache.apply_ln_to_stack will apply the appropriate
+        scaling to these directions.
 
         Args:
-            tokens (Union[str, int, torch.Tensor]): The token(s). If a single token, can be a single element tensor, an integer, or string. If string, will be mapped to a single token using to_single_token, and an error raised if it's multiple tokens.
-            The method also works for a batch of input tokens
+            tokens (Union[str, int, torch.Tensor]): The token(s). If a single token, can be a single element tensor, an
+                integer, or string. If string, will be mapped to a single token using to_single_token, and an error
+                raised if it's multiple tokens. The method also works for a batch of input tokens
 
         Returns:
             residual_direction torch.Tensor: The unembedding vector for the token(s), a stack of [d_model] tensor.
         """
-        if isinstance(tokens, torch.Tensor) and tokens.numel()>1:
+        if isinstance(tokens, torch.Tensor) and tokens.numel() > 1:
             # If the tokens are a tensor, and have more than one element, assume they are a batch of tokens
             residual_directions = self.W_U[:, tokens]
-            residual_directions = einops.rearrange(residual_directions, "d_model ... -> ... d_model")
+            residual_directions = einops.rearrange(
+                residual_directions, "d_model ... -> ... d_model"
+            )
             return residual_directions
         else:
             # Otherwise there is a single token
             if isinstance(tokens, str):
                 token = self.to_single_token(tokens)
             elif isinstance(tokens, int):
                 token = tokens
-            elif isinstance(tokens, torch.Tensor) and tokens.numel()==1:
+            elif isinstance(tokens, torch.Tensor) and tokens.numel() == 1:
                 token = tokens.item()
             else:
                 raise ValueError(f"Invalid token type: {type(tokens)}")
             residual_direction = self.W_U[:, token]
             return residual_direction
 
-
-    def to(self, device_or_dtype, print_details=True):
-        """
-        Wrapper around to that also changes self.cfg.device if it's a torch.device or string. If torch.dtype, just passes through
-        """
-        if isinstance(device_or_dtype, torch.device):
-            self.cfg.device = device_or_dtype.type
-            if print_details: 
-                print("Moving model to device: ", self.cfg.device)
-        elif isinstance(device_or_dtype, str):
-            self.cfg.device = device_or_dtype
-            if print_details: 
-                print("Moving model to device: ", self.cfg.device)
-        elif isinstance(device_or_dtype, torch.dtype):
-            if print_details: 
-                print("Changing model dtype to", device_or_dtype)
-            # change state_dict dtypes
-            for k, v in self.state_dict().items():
-                self.state_dict()[k] = v.to(device_or_dtype)
-        return nn.Module.to(self, device_or_dtype)
+    def to(
+        self,
+        device_or_dtype: Union[torch.device, str, torch.dtype],
+        print_details: bool = True,
+    ):
+        return devices.move_to_and_update_config(self, device_or_dtype, print_details)
 
     def cuda(self):
         # Wrapper around cuda that also changes self.cfg.device
         return self.to("cuda")
 
     def cpu(self):
         # Wrapper around cuda that also changes self.cfg.device
@@ -688,21 +775,30 @@
         refactor_factored_attn_matrices=False,
         checkpoint_index=None,
         checkpoint_value=None,
         hf_model=None,
         device=None,
         n_devices=1,
         move_state_dict_to_device=True,
-        **model_kwargs,
-    ):
-        """Class method to load in a pretrained model weights to the HookedTransformer format and optionally to do some processing to make the model easier to interpret. Currently supports loading from most autoregressive HuggingFace models (GPT2, GPTNeo, GPTJ, OPT) and from a range of toy models and SoLU models trained by me (Neel Nanda).
-
-        Also supports loading from a checkpoint for checkpointed models (currently, models trained by me (NeelNanda) and the stanford-crfm models). These can either be determined by the checkpoint index (the index of the checkpoint in the checkpoint list) or by the checkpoint value (the value of the checkpoint, eg 1000 for a checkpoint taken at step 1000 or after 1000 tokens. Each model has checkpoints labelled with exactly one of labels and steps). If neither is specified the final model is loaded. If both are specified, the checkpoint index is used.
+        tokenizer=None,
+        move_to_device=True,
+        **from_pretrained_kwargs,
+    ) -> "HookedTransformer":
+        """Class method to load in a pretrained model weights to the HookedTransformer format and optionally to do some
+        processing to make the model easier to interpret. Currently supports loading from most autoregressive
+        HuggingFace models (GPT2, GPTNeo, GPTJ, OPT) and from a range of toy models and SoLU models trained by me (Neel Nanda).
+
+        Also supports loading from a checkpoint for checkpointed models (currently, models trained by me (NeelNanda) and
+        the stanford-crfm models). These can either be determined by the checkpoint index (the index of the checkpoint
+        in the checkpoint list) or by the checkpoint value (the value of the checkpoint, eg 1000 for a checkpoint taken
+        at step 1000 or after 1000 tokens. Each model has checkpoints labelled with exactly one of labels and steps).
+        If neither is specified the final model is loaded. If both are specified, the checkpoint index is used.
 
-        See load_and_process_state_dict for details on the processing (folding layer norm, centering the unembedding and centering the writing weights)
+        See load_and_process_state_dict for details on the processing (folding layer norm, centering the unembedding and
+        centering the writing weights)
 
         Args:
             model_name (str): The model name - must be an element of OFFICIAL_MODEL_NAMES or an alias of one.
             fold_ln (bool, optional): Whether to fold in the LayerNorm weights to the
                 subsequent linear layer. This does not change the computation.
                 Defaults to True.
             center_writing_weights (bool, optional): Whether to center weights
@@ -727,39 +823,74 @@
             device (str, optional): The device to load the model onto. By
                 default will load to CUDA if available, else CPU.
             n_devices (int, optional): The number of devices to split the model
                 across. Defaults to 1. If greater than 1, `device` must be cuda.
             move_state_dict_to_device (bool): Whether to move the state dict to the
                 relevant device before processing and loading in the weights.
                 Defaults to True.
-            model_kwargs (dict, optional): Any additional kwargs to pass to the
-                HookedTransformer initialization.
+            tokenizer (*optional): The tokenizer to use for the model. If not
+                provided, it is inferred from cfg.tokenizer_name or initialized to None.
+                If None, then the model cannot be passed strings, and d_vocab must be explicitly set.
+            move_to_device (bool, optional): Whether to move the model to the device specified in cfg.
+                device. Must be true if `n_devices` in the config is greater than 1, since the model's layers
+                will be split across multiple devices.
+            from_pretrained_kwargs (dict, optional): Any other optional argument passed to HuggingFace's
+                from_pretrained (e.g. "cache_dir" or "torch_dtype"). Also passed to other HuggingFace
+                functions when compatible. For some models or arguments it doesn't work, especially for
+                models that are not internally loaded with HuggingFace's from_pretrained (e.g. SoLU models).
         """
+
         # Get the model name used in HuggingFace, rather than the alias.
         official_model_name = loading.get_official_model_name(model_name)
 
         # Load the config into an HookedTransformerConfig object. If loading from a
         # checkpoint, the config object will contain the information about the
         # checkpoint
         cfg = loading.get_pretrained_model_config(
             official_model_name,
             checkpoint_index=checkpoint_index,
             checkpoint_value=checkpoint_value,
             fold_ln=fold_ln,
             device=device,
             n_devices=n_devices,
+            **from_pretrained_kwargs,
         )
 
-        # Get the state dict of the model (ie a mapping of parameter names to tensors), processed to match the HookedTransformer parameter names.
+        if cfg.positional_embedding_type == "shortformer":
+            if fold_ln:
+                logging.warning(
+                    "You tried to specify fold_ln=True for a shortformer model, but this can't be done! Setting fold_"
+                    "ln=False instead."
+                )
+                fold_ln = False
+            if center_unembed:
+                logging.warning(
+                    "You tried to specify center_unembed=True for a shortformer model, but this can't be done! "
+                    "Setting center_unembed=False instead."
+                )
+                center_unembed = False
+            if center_writing_weights:
+                logging.warning(
+                    "You tried to specify center_writing_weights=True for a shortformer model, but this can't be done! "
+                    "Setting center_writing_weights=False instead."
+                )
+                center_writing_weights = False
+
+        # Get the state dict of the model (ie a mapping of parameter names to tensors), processed to match the
+        # HookedTransformer parameter names.
         state_dict = loading.get_pretrained_state_dict(
-            official_model_name, cfg, hf_model
+            official_model_name, cfg, hf_model, **from_pretrained_kwargs
         )
 
         # Create the HookedTransformer object
-        model = cls(cfg, **model_kwargs)
+        model = cls(cfg, tokenizer, move_to_device)
+
+        dtype = from_pretrained_kwargs.get("torch_dtype", None)
+        if dtype is not None:
+            model = model.to(dtype)
 
         model.load_and_process_state_dict(
             state_dict,
             fold_ln=fold_ln,
             center_writing_weights=center_writing_weights,
             center_unembed=center_unembed,
             refactor_factored_attn_matrices=refactor_factored_attn_matrices,
@@ -776,40 +907,47 @@
         model_name: str,
         fold_ln=False,
         center_writing_weights=False,
         center_unembed=False,
         refactor_factored_attn_matrices=False,
         **from_pretrained_kwargs,
     ):
-        """Wrapper for from_pretrained with all boolean flags related to simplifying the model set to False. Refer to from_pretrained for details."""
+        """Wrapper for from_pretrained with all boolean flags related to simplifying the model set to False. Refer to
+        from_pretrained for details."""
         return cls.from_pretrained(
             model_name,
             fold_ln=fold_ln,
             center_writing_weights=center_writing_weights,
             center_unembed=center_unembed,
             refactor_factored_attn_matrices=refactor_factored_attn_matrices,
             **from_pretrained_kwargs,
         )
 
     def init_weights(self):
         """
-        Initialize weights matrices with a normal of std=initializer_range (default=0.02). This roughly follows the GPT-2 paper's scheme (but with truncation, and not halving the std for W_pos).
+        Initialize weights matrices with a normal of std=initializer_range (default=0.02). This roughly follows the
+        GPT-2 paper's scheme (but with truncation, and not halving the std for W_pos).
 
-        LayerNorm weights are already initialized to 1.0, and all biases are initialized to 0.0 (including LayerNorm), so this just initializes weight matrices.
+        LayerNorm weights are already initialized to 1.0, and all biases are initialized to 0.0 (including LayerNorm),
+        so this just initializes weight matrices.
 
-        Weight matrices are set to empty by default (to save space + compute, since they're the bulk of the parameters), so it is important to call this if you are not loading in pretrained weights! Note that this function assumes that weight names being with W_
+        Weight matrices are set to empty by default (to save space + compute, since they're the bulk of the parameters),
+        so it is important to call this if you are not loading in pretrained weights! Note that this function assumes that weight names being with W_
 
         Set seed here to ensure determinism.
 
-        This does NOT follow the PyTorch scheme, which as far as I can tell is super out of date but no one has gotten round to updating it?
+        This does NOT follow the PyTorch scheme, which as far as I can tell is super out of date but no one has gotten
+        round to updating it?
         https://github.com/pytorch/pytorch/issues/18182
 
-        PyTorch Transformers are especially bad - TransformerEncoder initializes all layers to the exact same weights?! https://github.com/pytorch/pytorch/issues/72253
+        PyTorch Transformers are especially bad - TransformerEncoder initializes all layers to the exact same weights?!
+        https://github.com/pytorch/pytorch/issues/72253
 
-        The best paper I've found on transformer initialization is the muP paper, but haven't integrated those ideas yet: https://arxiv.org/abs/2203.03466
+        The best paper I've found on transformer initialization is the muP paper, but haven't integrated those ideas yet:
+        https://arxiv.org/abs/2203.03466
         """
 
         if self.cfg.seed is not None:
             torch.manual_seed(self.cfg.seed)
 
         for name, param in self.named_parameters():
             if "W_" in name:
@@ -821,43 +959,45 @@
         fold_ln: bool = True,
         center_writing_weights: bool = True,
         center_unembed: bool = True,
         fold_value_biases: bool = True,
         refactor_factored_attn_matrices: bool = False,
         move_state_dict_to_device: bool = True,
     ):
-        """Method to load a state dict into the model, and to apply processing to simplify it. The state dict is assumed to be in the HookedTransformer format.
+        """Method to load a state dict into the model, and to apply processing to simplify it. The state dict is assumed
+        to be in the HookedTransformer format.
 
         See the relevant method (same name as the flag) for more details on the folding, centering and processing flags.
 
         Args:
             state_dict (dict): The state dict of the model, in HookedTransformer format
             fold_ln (bool, optional): Whether to fold in the LayerNorm weights to the
                 subsequent linear layer. This does not change the computation. Defaults to True.
             center_writing_weights (bool, optional): Whether to center weights writing to the
-                residual stream (ie set mean to be zero). Due to LayerNorm this doesn't change the computation. Defaults to True.
+                residual stream (ie set mean to be zero). Due to LayerNorm this doesn't change the computation.
+                Defaults to True.
             center_unembed (bool, optional): Whether to center W_U (ie set mean to be zero).
-                Softmax is translation invariant so this doesn't affect log probs or loss, but does change logits. Defaults to True.
-            fold_value_biases (bool, optional): Whether to fold the value biases into the output bias. Because attention patterns add up to 1, the value biases always have a constant effect on a layer's output, and it doesn't matter which head a bias is associated with. We can factor this all into a single output bias to the layer, and make it easier to interpret the head's output.
+                Softmax is translation invariant so this doesn't affect log probs or loss, but does change logits.
+                Defaults to True.
+            fold_value_biases (bool, optional): Whether to fold the value biases into the output bias.
+                Because attention patterns add up to 1, the value biases always have a constant effect on a layer's
+                output, and it doesn't matter which head a bias is associated with. We can factor this all into a single
+                output bias to the layer, and make it easier to interpret the head's output.
             refactor_factored_attn_matrices (bool, optional): Whether to convert the factored
                 matrices (W_Q & W_K, and W_O & W_V) to be "even". Defaults to False
-            move_state_dict_to_device (bool, optional): Whether to move the state dict to the device of the model. Defaults to True.
-            model_name (str, optional): checks the model name for special cases of state dict loading. Only used for Redwood 2L model currently
+            move_state_dict_to_device (bool, optional): Whether to move the state dict to the device of the model.
+                Defaults to True.
+            model_name (str, optional): checks the model name for special cases of state dict loading. Only used for
+                Redwood 2L model currently
         """
 
         assert (
             self.cfg.n_devices == 1 or move_state_dict_to_device
         ), "If n_devices > 1, move_state_dict_to_device must be True"
 
-        
-        if self.cfg.positional_embedding_type == "shortformer":
-            if fold_ln:
-                logging.warning("You tried to specify fold_ln=True for a shortformer model, but this can't be done! Setting fold_ln=False instead.")
-                fold_ln = False
-
         if move_state_dict_to_device:
             for k, v in state_dict.items():
                 if k.startswith("embed") or k.startswith("pos_embed"):
                     state_dict[k] = v.to(
                         devices.get_device_for_block_index(0, self.cfg)
                     )
                 elif k.startswith("ln_final") or k.startswith("unembed"):
@@ -880,15 +1020,16 @@
         state_dict = self.fill_missing_keys(state_dict)
         if fold_ln:
             if self.cfg.normalization_type not in ["LN", "LNPre"]:
                 logging.warning(
                     "You are not using LayerNorm, so the layer norm weights can't be folded! Skipping"
                 )
             else:
-                # Note - you can run fold_layer_norm while normalization_type is LN, but this is not advised! It mostly goes wrong when you're training the model.
+                # Note - you can run fold_layer_norm while normalization_type is LN, but this is not advised! It mostly
+                # goes wrong when you're training the model.
                 state_dict = self.fold_layer_norm(state_dict)
         if center_writing_weights:
             if self.cfg.normalization_type not in ["LN", "LNPre"]:
                 logging.warning(
                     "You are not using LayerNorm, so the writing weights can't be centered! Skipping"
                 )
             elif self.cfg.final_rms:
@@ -902,53 +1043,30 @@
         if fold_value_biases:
             state_dict = self.fold_value_biases(state_dict)
         if refactor_factored_attn_matrices:
             state_dict = self.refactor_factored_attn_matrices(state_dict)
         self.load_state_dict(state_dict)
 
     def fill_missing_keys(self, state_dict):
-        """Takes in a state dict from a pretrained model, and fills in any missing keys with the default initialization.
-
-        This function is assumed to be run before weights are initialized.
-
-        Args:
-            state_dict (dict): State dict from a pretrained model
-
-        Returns:
-            dict: State dict with missing keys filled in
-        """
-        # Get the default state dict
-        default_state_dict = self.state_dict()
-        # Get the keys that are missing from the pretrained model
-        missing_keys = set(default_state_dict.keys()) - set(state_dict.keys())
-        # Fill in the missing keys with the default initialization
-        for key in missing_keys:
-            if "hf_model" in key:
-                # Skip keys that are from the HuggingFace model, if loading from HF.
-                continue
-            if "W_" in key:
-                logging.warning(
-                    "Missing key for a weight matrix in pretrained, filled in with an empty tensor: {}".format(
-                        key
-                    )
-                )
-            state_dict[key] = default_state_dict[key]
-        return state_dict
+        return loading.fill_missing_keys(self, state_dict)
 
     def fold_layer_norm(self, state_dict: Dict[str, torch.Tensor]):
-        """Takes in a state dict from a pretrained model, formatted to be consistent with HookedTransformer but with LayerNorm weights and biases. Folds these into the neighbouring weights. See further_comments.md for more details
+        """Takes in a state dict from a pretrained model, formatted to be consistent with HookedTransformer but with
+        LayerNorm weights and biases. Folds these into the neighbouring weights. See further_comments.md for more details
 
         Args:
             state_dict (Dict[str, torch.Tensor]): State dict of pretrained model
         """
         for l in range(self.cfg.n_layers):
             # Fold ln1 into attention - it's important to fold biases first,
             # since biases depend on weights but not vice versa
-            # The various indexing is just to broadcast ln.b and ln.w along every axis other than d_model. Each weight matrix right multiplies.
-            # To fold in the bias, we use the W_ matrix to map it to the hidden space of the layer, so we need to sum along axis -2, which is the residual stream space axis.
+            # The various indexing is just to broadcast ln.b and ln.w along every axis other than d_model.
+            # Each weight matrix right multiplies.
+            # To fold in the bias, we use the W_ matrix to map it to the hidden space of the layer,
+            # so we need to sum along axis -2, which is the residual stream space axis.
             state_dict[f"blocks.{l}.attn.b_Q"] = state_dict[f"blocks.{l}.attn.b_Q"] + (
                 state_dict[f"blocks.{l}.attn.W_Q"]
                 * state_dict[f"blocks.{l}.ln1.b"][None, :, None]
             ).sum(-2)
             state_dict[f"blocks.{l}.attn.b_K"] = state_dict[f"blocks.{l}.attn.b_K"] + (
                 state_dict[f"blocks.{l}.attn.W_K"]
                 * state_dict[f"blocks.{l}.ln1.b"][None, :, None]
@@ -967,32 +1085,35 @@
                 * state_dict[f"blocks.{l}.ln1.w"][None, :, None]
             )
             state_dict[f"blocks.{l}.attn.W_V"] = (
                 state_dict[f"blocks.{l}.attn.W_V"]
                 * state_dict[f"blocks.{l}.ln1.w"][None, :, None]
             )
 
-            # Finally, we center the weights reading from the residual stream. The output of the first 
-            # part of the LayerNorm is mean 0 and standard deviation 1, so the mean of any input vector 
+            # Finally, we center the weights reading from the residual stream. The output of the first
+            # part of the LayerNorm is mean 0 and standard deviation 1, so the mean of any input vector
             # of the matrix doesn't matter and can be set to zero.
-            # Equivalently, the output of LayerNormPre is orthogonal to the vector of all 1s (because 
+            # Equivalently, the output of LayerNormPre is orthogonal to the vector of all 1s (because
             # dotting with that gets the sum), so we can remove the component of the matrix parallel to this.
             state_dict[f"blocks.{l}.attn.W_Q"] -= einops.reduce(
-                state_dict[f"blocks.{l}.attn.W_Q"], 
-                "head_index d_model d_head -> head_index 1 d_head", 
-                "mean")
+                state_dict[f"blocks.{l}.attn.W_Q"],
+                "head_index d_model d_head -> head_index 1 d_head",
+                "mean",
+            )
             state_dict[f"blocks.{l}.attn.W_K"] -= einops.reduce(
-                state_dict[f"blocks.{l}.attn.W_K"], 
-                "head_index d_model d_head -> head_index 1 d_head", 
-                "mean")
+                state_dict[f"blocks.{l}.attn.W_K"],
+                "head_index d_model d_head -> head_index 1 d_head",
+                "mean",
+            )
             state_dict[f"blocks.{l}.attn.W_V"] -= einops.reduce(
-                state_dict[f"blocks.{l}.attn.W_V"], 
-                "head_index d_model d_head -> head_index 1 d_head", 
-                "mean")
-            
+                state_dict[f"blocks.{l}.attn.W_V"],
+                "head_index d_model d_head -> head_index 1 d_head",
+                "mean",
+            )
+
             del (
                 state_dict[f"blocks.{l}.ln1.w"],
                 state_dict[f"blocks.{l}.ln1.b"],
             )
 
             # Fold ln2 into MLP
             if not self.cfg.attn_only:
@@ -1007,21 +1128,21 @@
                 state_dict[f"blocks.{l}.mlp.W_in"] = (
                     state_dict[f"blocks.{l}.mlp.W_in"]
                     * state_dict[f"blocks.{l}.ln2.w"][:, None]
                 )
 
                 # Center the weights that read in from the LayerNormPre
                 state_dict[f"blocks.{l}.mlp.W_in"] -= einops.reduce(
-                    state_dict[f"blocks.{l}.mlp.W_in"], 
-                    "d_model d_mlp -> 1 d_mlp", 
-                    "mean")
+                    state_dict[f"blocks.{l}.mlp.W_in"],
+                    "d_model d_mlp -> 1 d_mlp",
+                    "mean",
+                )
 
                 del state_dict[f"blocks.{l}.ln2.w"], state_dict[f"blocks.{l}.ln2.b"]
 
-
                 if self.cfg.act_fn.startswith("solu"):
                     # Fold ln3 into activation
                     state_dict[f"blocks.{l}.mlp.b_out"] = state_dict[
                         f"blocks.{l}.mlp.b_out"
                     ] + (
                         state_dict[f"blocks.{l}.mlp.W_out"]
                         * state_dict[f"blocks.{l}.mlp.ln.b"][:, None]
@@ -1031,17 +1152,18 @@
                     state_dict[f"blocks.{l}.mlp.W_out"] = (
                         state_dict[f"blocks.{l}.mlp.W_out"]
                         * state_dict[f"blocks.{l}.mlp.ln.w"][:, None]
                     )
 
                     # Center the weights that read in from the LayerNormPre
                     state_dict[f"blocks.{l}.mlp.W_out"] -= einops.reduce(
-                        state_dict[f"blocks.{l}.mlp.W_out"], 
-                        "d_mlp d_model -> 1 d_model", 
-                        "mean")
+                        state_dict[f"blocks.{l}.mlp.W_out"],
+                        "d_mlp d_model -> 1 d_model",
+                        "mean",
+                    )
                     del (
                         state_dict[f"blocks.{l}.mlp.ln.w"],
                         state_dict[f"blocks.{l}.mlp.ln.b"],
                     )
         # Fold ln_final into Unembed
         if not self.cfg.final_rms:
             # Dumb bug from my old SoLU training code, some models have RMSNorm instead of LayerNorm pre unembed.
@@ -1051,23 +1173,24 @@
             del state_dict[f"ln_final.b"]
         state_dict[f"unembed.W_U"] = (
             state_dict[f"unembed.W_U"] * state_dict[f"ln_final.w"][:, None]
         )
 
         # Center the weights that read in from the LayerNormPre
         state_dict[f"unembed.W_U"] -= einops.reduce(
-            state_dict[f"unembed.W_U"], 
-            "d_model d_vocab -> 1 d_vocab", 
-            "mean")
+            state_dict[f"unembed.W_U"], "d_model d_vocab -> 1 d_vocab", "mean"
+        )
 
         del state_dict[f"ln_final.w"]
         return state_dict
 
     def center_writing_weights(self, state_dict: Dict[str, torch.Tensor]):
-        """Centers the weights of the model that write to the residual stream - W_out, W_E, W_pos and W_out. This is done by subtracting the mean of the weights from the weights themselves. This is done in-place. See fold_layer_norm for more details."""
+        """Centers the weights of the model that write to the residual stream - W_out, W_E, W_pos and W_out. This is
+        done by subtracting the mean of the weights from the weights themselves. This is done in-place. See
+        fold_layer_norm for more details."""
         state_dict["embed.W_E"] = state_dict["embed.W_E"] - state_dict[
             "embed.W_E"
         ].mean(-1, keepdim=True)
         if self.cfg.positional_embedding_type != "rotary":
             state_dict["pos_embed.W_pos"] = state_dict["pos_embed.W_pos"] - state_dict[
                 "pos_embed.W_pos"
             ].mean(-1, keepdim=True)
@@ -1088,63 +1211,87 @@
                 state_dict[f"blocks.{l}.mlp.b_out"] = (
                     state_dict[f"blocks.{l}.mlp.b_out"]
                     - state_dict[f"blocks.{l}.mlp.b_out"].mean()
                 )
         return state_dict
 
     def center_unembed(self, state_dict: Dict[str, torch.Tensor]):
-        """Centers the unembedding weights W_U. This is done by subtracting the mean of the weights from the weights themselves. This is done in-place. As softmax is translation invariant, this changes the logits but not the log probs, and makes the model logits (slightly) more interpretable - when trying to understand how components contribute to the logits, we'll be less misled by components that just add something to every logit."""
+        """Centers the unembedding weights W_U. This is done by subtracting the mean of the weights from the weights
+        themselves. This is done in-place. As softmax is translation invariant, this changes the logits but not the
+        log probs, and makes the model logits (slightly) more interpretable - when trying to understand how components
+        contribute to the logits, we'll be less misled by components that just add something to every logit.
+        """
         state_dict["unembed.W_U"] = state_dict["unembed.W_U"] - state_dict[
             "unembed.W_U"
         ].mean(-1, keepdim=True)
         state_dict["unembed.b_U"] = (
             state_dict["unembed.b_U"] - state_dict["unembed.b_U"].mean()
         )
         return state_dict
-    
+
     def fold_value_biases(self, state_dict: Dict[str, torch.Tensor]):
-        """Fold the value biases into the output bias. Because attention patterns add up to 1, the value biases always have a constant effect on a head's output
-        Further, as the outputs of each head in a layer add together, each head's value bias has a constant effect on the *layer's* output, which can make it harder to interpret the effect of any given head, and it doesn't matter which head a bias is associated with. 
+        """Fold the value biases into the output bias. Because attention patterns add up to 1, the value biases always
+        have a constant effect on a head's output. Further, as the outputs of each head in a layer add together, each
+        head's value bias has a constant effect on the *layer's* output, which can make it harder to interpret the
+        effect of any given head, and it doesn't matter which head a bias is associated with.
         We can factor this all into a single output bias to the layer, and make it easier to interpret the head's output.
         Formally, we take b_O_new = b_O_original + sum_head(b_V_head @ W_O_head)
         """
         for layer in range(self.cfg.n_layers):
             # shape [head_index, d_head]
-            b_V = state_dict[f'blocks.{layer}.attn.b_V']
+            b_V = state_dict[f"blocks.{layer}.attn.b_V"]
             # [head_index, d_head, d_model]
-            W_O = state_dict[f'blocks.{layer}.attn.W_O']
+            W_O = state_dict[f"blocks.{layer}.attn.W_O"]
             # [d_model]
-            b_O_original = state_dict[f'blocks.{layer}.attn.b_O']
+            b_O_original = state_dict[f"blocks.{layer}.attn.b_O"]
+
+            folded_b_O = b_O_original + einsum(
+                "head_index d_head, head_index d_head d_model -> d_model", b_V, W_O
+            )
 
-            folded_b_O = b_O_original + einsum("head_index d_head, head_index d_head d_model -> d_model", b_V, W_O)
-            
-            state_dict[f'blocks.{layer}.attn.b_O'] = folded_b_O 
-            state_dict[f'blocks.{layer}.attn.b_V'] = torch.zeros_like(b_V)
+            state_dict[f"blocks.{layer}.attn.b_O"] = folded_b_O
+            state_dict[f"blocks.{layer}.attn.b_V"] = torch.zeros_like(b_V)
         return state_dict
 
     def refactor_factored_attn_matrices(self, state_dict: Dict[str, torch.Tensor]):
         """
-        Experimental method for managing queries, keys and values. As argued in [A Mathematical Framework for Transformer Circuits](https://transformer-circuits.pub/2021/framework/index.html), queries, keys and values are somewhat arbitrary intermediate terms when computing with the low rank factored matrices W_QK = W_Q @ W_K.T and W_OV = W_V @ W_O, and these matrices are the only thing determining head behaviour. But there are many ways to find a low rank factorization to a given matrix, and hopefully some of these are more interpretable than others! This method is one attempt, which makes all of the matrices have orthogonal rows or columns, W_O into a rotation and W_Q and W_K having the nth column in each having the same norm. The formula is $W_V = U @ S,W_O=Vh.T,W_Q=U@S.sqrt(),W_K=Vh@S.sqrt()$.
+        Experimental method for managing queries, keys and values. As argued in [A Mathematical Framework for Transformer
+        Circuits](https://transformer-circuits.pub/2021/framework/index.html), queries, keys and values are somewhat
+        arbitrary intermediate terms when computing with the low rank factored matrices W_QK = W_Q @ W_K.T and W_OV = W_V @ W_O,
+        and these matrices are the only thing determining head behaviour. But there are many ways to find a low rank
+        factorization to a given matrix, and hopefully some of these are more interpretable than others! This method is
+        one attempt, which makes all of the matrices have orthogonal rows or columns, W_O into a rotation and W_Q and W_K
+        having the nth column in each having the same norm. The formula is $W_V = U @ S,W_O=Vh.T,W_Q=U@S.sqrt(),W_K=Vh@S.sqrt()$.
 
         More details:
 
-        If W_OV = U @ S @ Vh.T in its singular value decomposition, (where S is in R^d_head not R^d_model, as W_OV is low rank), W_OV = (U @ S) @ (Vh.T) is an equivalent low rank factorisation, where rows/columns of each matrix are orthogonal! So setting $W_V=US$ and $W_O=Vh.T$ works just as well. I *think* this is a more interpretable setup, because now $W_O$ is just a rotation, and doesn't change the norm, so $z$ has the same norm as the result of the head.
-
-        For $W_QK = W_Q @ W_K.T$ we use the refactor $W_Q = U @ S.sqrt()$ and $W_K = Vh @ S.sqrt()$, which is also equivalent ($S==S.sqrt() @ S.sqrt()$ as $S$ is diagonal). Here we keep the matrices as having the same norm, since there's not an obvious asymmetry between the keys and queries.
-
-        Biases are more fiddly to deal with. For OV it's pretty easy - we just need (x @ W_V + b_V) @ W_O + b_O to be preserved, so we can set b_V' = 0. and b_O' = b_V @ W_O + b_O (note that b_V in R^{head_index x d_head} while b_O in R^{d_model}, so we need to sum b_V @ W_O along the head_index dimension too).
+        If W_OV = U @ S @ Vh.T in its singular value decomposition, (where S is in R^d_head not R^d_model, as W_OV is low rank),
+        W_OV = (U @ S) @ (Vh.T) is an equivalent low rank factorisation, where rows/columns of each matrix are orthogonal!
+        So setting $W_V=US$ and $W_O=Vh.T$ works just as well. I *think* this is a more interpretable setup, because now
+        $W_O$ is just a rotation, and doesn't change the norm, so $z$ has the same norm as the result of the head.
+
+        For $W_QK = W_Q @ W_K.T$ we use the refactor $W_Q = U @ S.sqrt()$ and $W_K = Vh @ S.sqrt()$, which is also
+        equivalent ($S==S.sqrt() @ S.sqrt()$ as $S$ is diagonal). Here we keep the matrices as having the same norm,
+        since there's not an obvious asymmetry between the keys and queries.
+
+        Biases are more fiddly to deal with. For OV it's pretty easy - we just need (x @ W_V + b_V) @ W_O + b_O to be
+        preserved, so we can set b_V' = 0. and b_O' = b_V @ W_O + b_O (note that b_V in R^{head_index x d_head} while b_O in R^{d_model},
+        so we need to sum b_V @ W_O along the head_index dimension too).
 
         For QK it's messy - we need to preserve the bilinear form of (x @ W_Q +
         b_Q) * (y @ W_K + b_K), which is fairly messy. To deal with the biases,
         we concatenate them to W_Q and W_K to simulate a d_model+1 dimensional
         input (whose final coordinate is always 1), do the SVD factorization on
         this effective matrix, then separate out into final weights and biases
+        """
 
+        assert (
+            self.cfg.positional_embedding_type != "rotary"
+        ), "You can't refactor the QK circuit when using rotary embeddings (as the QK matrix depends on the position of the query and key)"
 
-        """
         for l in range(self.cfg.n_layers):
             # W_QK = W_Q @ W_K.T
             # Concatenate biases to make a d_model+1 input dimension
             W_Q_eff = torch.cat(
                 [
                     state_dict[f"blocks.{l}.attn.W_Q"],
                     state_dict[f"blocks.{l}.attn.b_Q"][:, None, :],
@@ -1186,41 +1333,43 @@
             W_OV = FactoredMatrix(W_V, W_O)
             U, S, Vh = W_OV.svd()
             state_dict[f"blocks.{l}.attn.W_V"] = U @ S.diag_embed()
             state_dict[f"blocks.{l}.attn.W_O"] = utils.transpose(Vh)
 
         return state_dict
 
-    def set_use_attn_result(self, use_attn_result):
+    def set_use_attn_result(self, use_attn_result: bool):
         """
-        Toggles whether to explicitly calculate and expose the result for each attention head - useful for interpretability but can easily burn through GPU memory.
+        Toggles whether to explicitly calculate and expose the result for each attention head - useful for
+        interpretability but can easily burn through GPU memory.
         """
         self.cfg.use_attn_result = use_attn_result
 
-    def set_use_split_qkv_input(self, use_split_qkv_input):
+    def set_use_split_qkv_input(self, use_split_qkv_input: bool):
         """
         Toggles whether to allow editing of inputs to each attention head.
         """
-        self.cfg.use_split_qkv_input = use_split_qkv_input 
+        self.cfg.use_split_qkv_input = use_split_qkv_input
 
     def process_weights_(
         self,
         fold_ln: bool = True,
         center_writing_weights: bool = True,
         center_unembed: bool = True,
         refactor_factored_attn_matrices: bool = False,
         move_state_dict_to_device: bool = True,
     ):
         """
-        Wrapper around load_and_process_state_dict to allow for in-place processing of the weights. This is useful if using HookedTransformer for training, if we then want to analyse a cleaner version of the same model.
+        Wrapper around load_and_process_state_dict to allow for in-place processing of the weights. This is useful if
+        using HookedTransformer for training, if we then want to analyse a cleaner version of the same model.
         """
         state_dict = self.state_dict()
         if fold_ln and self.cfg.normalization_type == "LN":
-            # If we're folding the LN into the weights, we need to replace all of the layernorm layers with LayerNormPres, which do not have learnable parameters.
-            # This is somewhat hacky, but it's the easiest way to do it.
+            # If we're folding the LN into the weights, we need to replace all the layernorm layers with LayerNormPres,
+            # which do not have learnable parameters. This is somewhat hacky, but it's the easiest way to do it.
             self.cfg.normalization_type = "LNPre"
             self.ln_final = LayerNormPre(self.cfg)
             for layer in self.blocks:
                 layer.ln1 = LayerNormPre(self.cfg)
                 layer.ln2 = LayerNormPre(self.cfg)
                 if self.cfg.act_fn.endswith("_ln"):
                     layer.mlp.ln = LayerNormPre(self.cfg)
@@ -1251,17 +1400,21 @@
         prepend_bos=True,
         return_type: Optional[str] = "input",
         verbose: bool = True,
     ) -> Float[torch.Tensor, "batch pos_plus_new_tokens"]:
         """
         Sample tokens from the model until the model outputs eos_token or max_new_tokens is reached.
 
-        To avoid fiddling with ragged tensors, if we input a batch of text and some sequences finish (by producing an EOT token), we keep running the model on the entire batch, but throw away the output for a finished sequence and just keep adding EOTs to pad.
-
-        This supports entering a single string, but not a list of strings - if the strings don't tokenize to exactly the same length, this gets messy. If that functionality is needed, convert them to a batch of tokens and input that instead.
+        To avoid fiddling with ragged tensors, if we input a batch of text and some sequences finish (by producing an
+        EOT token), we keep running the model on the entire batch, but throw away the output for a finished sequence
+        and just keep adding EOTs to pad.
+
+        This supports entering a single string, but not a list of strings - if the strings don't tokenize to exactly the
+        same length, this gets messy. If that functionality is needed, convert them to a batch of tokens and input that
+        instead.
 
         Args:
             input (int): Either a batch of tokens ([batch, pos]) or a text string (this will be converted to a batch of tokens with batch size 1)
             max_new_tokens (int): Maximum number of tokens to generate
             stop_at_eos (bool): If True, stop generating tokens when the model outputs eos_token
             eos_token_id (int, *optional*): The token ID to use for end of sentence. If None, use the tokenizer's eos_token_id - required if using stop_at_eos
             do_sample (bool): If True, sample from the model's output distribution. Otherwise, use greedy search (take the max logit each time).
@@ -1363,137 +1516,160 @@
                 return self.tokenizer.decode(tokens[0])
 
         else:
             return tokens
 
     # Give access to all weights as properties.
     @property
+    @typeguard_ignore
     def W_U(self) -> Float[torch.Tensor, "d_model d_vocab"]:
         """
         Convenience to get the unembedding matrix (ie the linear map from the final residual stream to the output logits)
         """
         return self.unembed.W_U
 
     @property
+    @typeguard_ignore
     def b_U(self) -> Float[torch.Tensor, "d_vocab"]:
         return self.unembed.b_U
 
     @property
+    @typeguard_ignore
     def W_E(self) -> Float[torch.Tensor, "d_vocab d_model"]:
         """
         Convenience to get the embedding matrix
         """
         return self.embed.W_E
 
     @property
+    @typeguard_ignore
     def W_pos(self) -> Float[torch.Tensor, "n_ctx d_model"]:
         """
         Convenience function to get the positional embedding. Only works on models with absolute positional embeddings!
         """
         return self.pos_embed.W_pos
 
     @property
+    @typeguard_ignore
     def W_E_pos(self) -> Float[torch.Tensor, "d_vocab+n_ctx d_model"]:
         """
         Concatenated W_E and W_pos. Used as a full (overcomplete) basis of the input space, useful for full QK and full OV circuits.
         """
         return torch.cat([self.W_E, self.W_pos], dim=0)
 
-    # Layer-specific weights are stacked into one massive tensor and given as properties for convenience and a cache is used to avoid repeated computation. Often a useful convenience when we want to do analysis on weights across all layers. If GPU memory is a bottleneck, don't use these properties!
+    # Layer-specific weights are stacked into one massive tensor and given as properties for convenience and a cache is
+    # used to avoid repeated computation. Often a useful convenience when we want to do analysis on weights across all layers.
+    # If GPU memory is a bottleneck, don't use these properties!
 
     @property
+    @typeguard_ignore
     @lru_cache(maxsize=None)
     def W_K(self) -> Float[torch.Tensor, "n_layers n_heads d_model d_head"]:
         """Stacks the key weights across all layers"""
         return torch.stack([block.attn.W_K for block in self.blocks], dim=0)
 
     @property
+    @typeguard_ignore
     @lru_cache(maxsize=None)
     def W_Q(self) -> Float[torch.Tensor, "n_layers n_heads d_model d_head"]:
         """Stacks the query weights across all layers"""
         return torch.stack([block.attn.W_Q for block in self.blocks], dim=0)
 
     @property
+    @typeguard_ignore
     @lru_cache(maxsize=None)
     def W_V(self) -> Float[torch.Tensor, "n_layers n_heads d_model d_head"]:
         """Stacks the value weights across all layers"""
         return torch.stack([block.attn.W_V for block in self.blocks], dim=0)
 
     @property
+    @typeguard_ignore
     @lru_cache(maxsize=None)
     def W_O(self) -> Float[torch.Tensor, "n_layers n_heads d_head d_model"]:
         """Stacks the attn output weights across all layers"""
         return torch.stack([block.attn.W_O for block in self.blocks], dim=0)
 
     @property
+    @typeguard_ignore
     @lru_cache(maxsize=None)
     def W_in(self) -> Float[torch.Tensor, "n_layers d_model d_mlp"]:
         """Stacks the MLP input weights across all layers"""
         return torch.stack([block.mlp.W_in for block in self.blocks], dim=0)
 
     @property
+    @typeguard_ignore
     @lru_cache(maxsize=None)
     def W_out(self) -> Float[torch.Tensor, "n_layers d_mlp d_model"]:
         """Stacks the MLP output weights across all layers"""
         return torch.stack([block.mlp.W_out for block in self.blocks], dim=0)
 
     @property
+    @typeguard_ignore
     @lru_cache(maxsize=None)
     def b_K(self) -> Float[torch.Tensor, "n_layers n_heads d_head"]:
         """Stacks the key biases across all layers"""
         return torch.stack([block.attn.b_K for block in self.blocks], dim=0)
 
     @property
+    @typeguard_ignore
     @lru_cache(maxsize=None)
     def b_Q(self) -> Float[torch.Tensor, "n_layers n_heads d_head"]:
         """Stacks the query biases across all layers"""
         return torch.stack([block.attn.b_Q for block in self.blocks], dim=0)
 
     @property
+    @typeguard_ignore
     @lru_cache(maxsize=None)
     def b_V(self) -> Float[torch.Tensor, "n_layers n_heads d_head"]:
         """Stacks the value biases across all layers"""
         return torch.stack([block.attn.b_V for block in self.blocks], dim=0)
 
     @property
+    @typeguard_ignore
     @lru_cache(maxsize=None)
     def b_O(self) -> Float[torch.Tensor, "n_layers d_model"]:
         """Stacks the attn output biases across all layers"""
         return torch.stack([block.attn.b_O for block in self.blocks], dim=0)
 
     @property
+    @typeguard_ignore
     @lru_cache(maxsize=None)
     def b_in(self) -> Float[torch.Tensor, "n_layers d_mlp"]:
         """Stacks the MLP input biases across all layers"""
         return torch.stack([block.mlp.b_in for block in self.blocks], dim=0)
 
     @property
+    @typeguard_ignore
     @lru_cache(maxsize=None)
     def b_out(self) -> Float[torch.Tensor, "n_layers d_model"]:
         """Stacks the MLP output biases across all layers"""
         return torch.stack([block.mlp.b_out for block in self.blocks], dim=0)
 
     @property
+    @typeguard_ignore
     def QK(self):
         return FactoredMatrix(self.W_Q, self.W_K.transpose(-2, -1))
 
     @property
+    @typeguard_ignore
     def OV(self):
         return FactoredMatrix(self.W_V, self.W_O)
 
     # Various utility functions
     def accumulated_bias(
         self, layer: int, mlp_input: bool = False, include_mlp_biases=True
     ) -> Float[torch.Tensor, "layers_accumulated_over d_model"]:
         """Returns the accumulated bias from all layer outputs (ie the b_Os and b_outs), up to the input of layer L.
 
         Args:
             layer (int): Layer number, in [0, n_layers]. layer==0 means no layers, layer==n_layers means all layers.
-            mlp_input (bool): If True, we take the bias up to the input of the MLP of layer L (ie we include the bias from the attention output of the current layer, otherwise just biases from previous layers)
-            include_mlp_biases (bool): Whether to include the biases of MLP layers. Often useful to have as False if we're expanding attn_out into individual heads, but keeping mlp_out as is.
+            mlp_input (bool): If True, we take the bias up to the input of the MLP of layer L (ie we include the bias
+            from the attention output of the current layer, otherwise just biases from previous layers)
+            include_mlp_biases (bool): Whether to include the biases of MLP layers. Often useful to have as False if
+            we're expanding attn_out into individual heads, but keeping mlp_out as is.
         Returns:
             bias (torch.Tensor): [d_model], accumulated bias
         """
         accumulated_bias = torch.zeros(self.cfg.d_model, device=self.cfg.device)
 
         for i in range(layer):
             accumulated_bias += self.blocks[i].attn.b_O
@@ -1505,19 +1681,21 @@
             ), "Cannot include attn_bias from beyond the final layer"
             accumulated_bias += self.blocks[layer].attn.b_O
         return accumulated_bias
 
     def all_composition_scores(
         self, mode
     ) -> Float[torch.Tensor, "n_layers n_heads n_layers n_heads"]:
-        """Returns the Composition scores for all pairs of heads, as a L1, H1, L2, H2 tensor (which is upper triangular on the first and third axes)
+        """Returns the Composition scores for all pairs of heads, as a L1, H1, L2, H2 tensor (which is upper triangular
+        on the first and third axes)
 
         mode is one of ["Q", "K", "V"]
 
-        See https://transformer-circuits.pub/2021/framework/index.html#:~:text=The%20above%20diagram%20shows%20Q%2D%2C%20K%2D%2C%20and%20V%2DComposition for three metrics used
+        See https://transformer-circuits.pub/2021/framework/index.html#:~:text=The%20above%20diagram%20shows%20Q%2D%2C%20K%2D%2C%20and%20V%2DComposition
+        for three metrics used
         """
         left = self.OV
         if mode == "Q":
             right = self.QK
         elif mode == "K":
             right = self.QK.T
         elif mode == "V":
@@ -1540,56 +1718,63 @@
         return [
             f"L{l}H{h}"
             for l in range(self.cfg.n_layers)
             for h in range(self.cfg.n_heads)
         ]
 
     def load_sample_training_dataset(self, **kwargs):
-        """ 
-        Helper function to load in a 10K-20K dataset of elements from the model's training data distribution. 
+        """
+        Helper function to load in a 10K-20K dataset of elements from the model's training data distribution.
 
-        Wrapper around utils.get_dataset, which identifies the appropriate dataset the pretrained models. Each dataset has a 'text' field, which contains the relevant info, some have several meta data fields.
+        Wrapper around utils.get_dataset, which identifies the appropriate dataset the pretrained models. Each dataset
+        has a 'text' field, which contains the relevant info, some have several meta data fields.
 
         Kwargs will be passed to utils.get_dataset (e.g. cache_dir to set download location)
 
         Notes:
         * GPT-2's training data is not open source. OpenWebText is a replication (links with >3 karma on Reddit)
-        * OPT's training data is not open source, and is a mess of different things that is hard to replicate. I default to the Pile, which covers some of it, but imperfectly.
+        * OPT's training data is not open source, and is a mess of different things that is hard to replicate. I default
+        to the Pile, which covers some of it, but imperfectly.
 
         (Some models will have actually been trained on the data supplied here, for some it's from the validation set)
         """
         model_dataset_map = {
-            'neel': 'c4_code',
-            'neel-solu-old': 'pile',
-            'GPT2LMHeadModel': 'openwebtext',
-            'GPTNeoForCausalLM': 'pile',
-            'GPTNeoXForCausalLM': 'pile',
-            'GPTJForCausalLM': 'pile',
-            'GPTJForCausalLM': 'pile',
-            'OPTForCausalLM': 'pile',
+            "neel": "c4_code",
+            "neel-solu-old": "pile",
+            "GPT2LMHeadModel": "openwebtext",
+            "GPTNeoForCausalLM": "pile",
+            "GPTNeoXForCausalLM": "pile",
+            "GPTJForCausalLM": "pile",
+            "OPTForCausalLM": "pile",
         }
         if self.cfg.original_architecture in model_dataset_map:
-            self.dataset = utils.get_dataset(model_dataset_map[self.cfg.original_architecture], **kwargs)
+            self.dataset = utils.get_dataset(
+                model_dataset_map[self.cfg.original_architecture], **kwargs
+            )
         else:
             raise ValueError(
                 f"We do not have an available dataset for the relevant model: {self.cfg.original_architecture}"
             )
         return self.dataset
-    
-    def sample_datapoint(self, tokenize=False) -> Union[str, Float[torch.Tensor, "1 pos"]]:
+
+    def sample_datapoint(
+        self, tokenize=False
+    ) -> Union[str, Float[torch.Tensor, "1 pos"]]:
         """
-        Helper function to randomly sample a data point from self.dataset, a small dataset from the data distribution the model was trained on. 
+        Helper function to randomly sample a data point from self.dataset, a small dataset from the data distribution
+        the model was trained on.
 
         Args:
-            tokenize (bool): Whether to return tokens (instead of text). Defaults to False. Note that the returned tokens will be automatically truncated to the model's max context size.
+            tokenize (bool): Whether to return tokens (instead of text). Defaults to False. Note that the returned tokens
+            will be automatically truncated to the model's max context size.
 
-        Implicitly calls self.load_sample_training_dataset if it hasn't already been called. Only works for pretrained models with an associated dataset. But you can manually replace self.dataset with a dataset of your choice if you want.
+        Implicitly calls self.load_sample_training_dataset if it hasn't already been called. Only works for pretrained
+        models with an associated dataset. But you can manually replace self.dataset with a dataset of your choice if you want.
         """
         if self.dataset is None:
             self.load_sample_training_dataset()
         sample_dataset_size = len(self.dataset)
         index = np.random.randint(0, sample_dataset_size)
         if not tokenize:
-            return self.dataset[index]['text']
+            return self.dataset[index]["text"]
         else:
-            return self.to_tokens(self.dataset[index]['text'], truncate=True)
-
+            return self.to_tokens(self.dataset[index]["text"], truncate=True)
```

### Comparing `transformer_lens-1.2.2/transformer_lens/HookedTransformerConfig.py` & `transformer_lens-1.3.0/transformer_lens/HookedTransformerConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from dataclasses import dataclass
-from typing import Union, Tuple, List, Dict, Any, Optional
-import torch
-import torch.nn as nn
-import random
-import numpy as np
+from __future__ import annotations
+
 import logging
-import json
 import pprint
+import random
+from dataclasses import dataclass
+from typing import Any, Dict, List, Optional
+
+import numpy as np
+import torch
 
 SUPPORTED_ACTIVATIONS = ["relu", "gelu", "silu", "gelu_new", "solu_ln", "gelu_fast"]
 
+
 @dataclass
 class HookedTransformerConfig:
     """
     Configuration class to store the configuration of a HookedTransformer model.
 
     See further_comments.md for more details on the more complex arguments.
 
@@ -23,15 +25,15 @@
         n_layers (int): The number of transformer blocks (one block = one attn layer AND one MLP layer).
         n_ctx (int): The maximum sequence length.
         n_heads (int): The number of attention heads. If not
             specified, will be set to d_model // d_head. (This is represented by a default value of -1)
         d_mlp (int, *optional*): The dimensionality of the feedforward mlp
             network. Defaults to 4 * d_model, and in an attn-only model is None.
         d_vocab (int): The size of the vocabulary. Defaults to -1, which means not set. If not set, will be
-            automatically set from the tokenizer's vocab size. 
+            automatically set from the tokenizer's vocab size.
         act_fn (str, *optional*): The activation function to use. Always
             lowercase. Supports ['relu', 'gelu', 'silu', 'gelu_new', 'solu_ln',
             'gelu_fast']. Must be set unless using an attn-only model.
         eps (float): The epsilon value to use for layer normalization. Defaults
             to 1e-5
         use_attn_result (bool): whether to explicitly calculate the amount
             each head adds to the residual stream (with a hook) and THEN add it
@@ -116,15 +118,15 @@
             positional_embedding_type=="rotary" it defaults to d_head.
         n_params (int, *optional*): The number of (hidden weight)
             parameters in the model. This is automatically calculated and not
             intended to be set by the user. (Non embedding parameters, because
             the [scaling laws paper](https://arxiv.org/pdf/2001.08361.pdf) found
             that that was a more meaningful number. Ignoring biases and layer
             norms, for convenience)
-        use_hook_tokens (bool): Will add a hook point on the token input to 
+        use_hook_tokens (bool): Will add a hook point on the token input to
             HookedTransformer.forward, which lets you cache or intervene on the tokens.
             Defaults to False.
     """
 
     n_layers: int
     d_model: int
     n_ctx: int
@@ -134,15 +136,15 @@
     d_mlp: Optional[int] = None
     act_fn: Optional[str] = None
     d_vocab: int = -1
     eps: float = 1e-5
     use_attn_result: bool = False
     use_attn_scale: bool = True
     use_split_qkv_input: bool = False
-    use_local_attn: bool = False 
+    use_local_attn: bool = False
     original_architecture: Optional[str] = None
     from_checkpoint: bool = False
     checkpoint_index: Optional[int] = None
     checkpoint_label_type: Optional[str] = None
     checkpoint_value: Optional[int] = None
     tokenizer_name: Optional[str] = None
     window_size: Optional[int] = None
@@ -163,15 +165,15 @@
     parallel_attn_mlp: bool = False
     rotary_dim: Optional[int] = None
     n_params: Optional[int] = None
     use_hook_tokens: bool = False
     gated_mlp: bool = False
 
     def __post_init__(self):
-        if self.n_heads==-1:
+        if self.n_heads == -1:
             self.n_heads = self.d_model // self.d_head
 
             if not self.d_model % (self.d_head) == 0:
                 logging.warning(
                     f"d_model {self.d_model} is not divisible by d_head {self.d_head}. n_heads was inferred to be {self.n_heads}, rounding down the ratio."
                 )
 
@@ -222,15 +224,15 @@
                 self.device == "cuda"
             ), "n_devices > 1 is only supported on CUDA devices"
             assert (
                 torch.cuda.device_count() >= self.n_devices
             ), f"Not enough CUDA devices to support n_devices {self.n_devices}"
 
     @classmethod
-    def from_dict(cls, config_dict: Dict[str, Any]):
+    def from_dict(cls, config_dict: Dict[str, Any]) -> HookedTransformerConfig:
         """
         Instantiates a `HookedTransformerConfig` from a Python dictionary of
         parameters.
         """
         return cls(**config_dict)
 
     def to_dict(self):
```

### Comparing `transformer_lens-1.2.2/transformer_lens/__init__.py` & `transformer_lens-1.3.0/transformer_lens/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,16 @@
     HookedTransformerKeyValueCacheEntry,
 )
 from . import components
 from .HookedTransformerConfig import HookedTransformerConfig
 from .FactoredMatrix import FactoredMatrix
 from .ActivationCache import ActivationCache
 from .HookedTransformer import HookedTransformer
+from .SVDInterpreter import SVDInterpreter
+from .HookedEncoder import HookedEncoder
 from . import head_detector
 from . import loading_from_pretrained as loading
 from . import patching
 from . import train
 
 from .past_key_value_caching import (
     HookedTransformerKeyValueCache as EasyTransformerKeyValueCache,
```

### Comparing `transformer_lens-1.2.2/transformer_lens/components.py` & `transformer_lens-1.3.0/transformer_lens/components.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-from typing import Union, Dict, Optional, Tuple
+import logging
+from functools import *
+from typing import Dict, Optional, Tuple, Union
+
+import einops
+import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-import numpy as np
-import einops
-import logging
+from fancy_einsum import einsum
 from jaxtyping import Float, Int
+from typeguard import typeguard_ignore
 
-from functools import *
-
+from transformer_lens.FactoredMatrix import FactoredMatrix
 from transformer_lens.hook_points import HookPoint
-from transformer_lens.utils import gelu_new, solu, gelu_fast
 from transformer_lens.HookedTransformerConfig import HookedTransformerConfig
-from transformer_lens.FactoredMatrix import FactoredMatrix
-
-from fancy_einsum import einsum
+from transformer_lens.past_key_value_caching import HookedTransformerKeyValueCacheEntry
+from transformer_lens.utils import gelu_fast, gelu_new, solu
 
-from transformer_lens.past_key_value_caching import (
-    HookedTransformerKeyValueCacheEntry,
-)
 
 # Embed & Unembed
 class Embed(nn.Module):
     def __init__(self, cfg: Union[Dict, HookedTransformerConfig]):
         super().__init__()
         if isinstance(cfg, Dict):
             cfg = HookedTransformerConfig.from_dict(cfg)
@@ -45,15 +43,17 @@
         if isinstance(cfg, Dict):
             cfg = HookedTransformerConfig.from_dict(cfg)
         self.cfg = cfg
         # Note that there's a separate variable for d_vocab_out and d_vocab (the input vocab size). For language tasks these are always the same, but for algorithmic tasks we may want them to be different.
         self.W_U: Float[torch.Tensor, "d_model d_vocab_out"] = nn.Parameter(
             torch.empty(self.cfg.d_model, self.cfg.d_vocab_out)
         )
-        self.b_U: Float[torch.Tensor, "d_vocab_out"] = nn.Parameter(torch.zeros(self.cfg.d_vocab_out))
+        self.b_U: Float[torch.Tensor, "d_vocab_out"] = nn.Parameter(
+            torch.zeros(self.cfg.d_vocab_out)
+        )
 
     def forward(
         self, residual: Float[torch.Tensor, "batch pos d_model"]
     ) -> Float[torch.Tensor, "batch pos d_vocab_out"]:
         return (
             einsum(
                 "batch pos d_model, d_model vocab -> batch pos vocab",
@@ -86,14 +86,105 @@
         ]  # [pos, d_model]
         broadcast_pos_embed = einops.repeat(
             pos_embed, "pos d_model -> batch pos d_model", batch=tokens.size(0)
         )  # [batch, pos, d_model]
         return broadcast_pos_embed.clone()
 
 
+class TokenTypeEmbed(nn.Module):
+    """
+    The token-type embed is a binary ids indicating whether a token belongs to sequence A or B. For example, for two sentences: "[CLS] Sentence A [SEP] Sentence B [SEP]", token_type_ids would be [0, 0, ..., 0, 1, ..., 1, 1]. `0` represents tokens from Sentence A, `1` from Sentence B. If not provided, BERT assumes a single sequence input. Typically, shape is (batch_size, sequence_length).
+
+    See the BERT paper for more information: https://arxiv.org/pdf/1810.04805.pdf
+    """
+
+    def __init__(self, cfg: Union[Dict, HookedTransformerConfig]):
+        super().__init__()
+        if isinstance(cfg, Dict):
+            cfg = HookedTransformerConfig.from_dict(cfg)
+        self.cfg = cfg
+        self.W_token_type = nn.Parameter(torch.empty(2, self.cfg.d_model))
+
+    def forward(self, token_type_ids: Int[torch.Tensor, "batch pos"]):
+        return self.W_token_type[token_type_ids, :]
+
+
+class BertEmbed(nn.Module):
+    """
+    Custom embedding layer for a BERT-like model. This module computes the sum of the token, positional and token-type embeddings and takes the layer norm of the result.
+    """
+
+    def __init__(self, cfg: Union[Dict, HookedTransformerConfig]):
+        super().__init__()
+        if isinstance(cfg, Dict):
+            cfg = HookedTransformerConfig.from_dict(cfg)
+        self.cfg = cfg
+        self.embed = Embed(cfg)
+        self.pos_embed = PosEmbed(cfg)
+        self.token_type_embed = TokenTypeEmbed(cfg)
+        self.ln = LayerNorm(cfg)
+
+        self.hook_embed = HookPoint()
+        self.hook_pos_embed = HookPoint()
+        self.hook_token_type_embed = HookPoint()
+
+    def forward(
+        self,
+        input_ids: Int[torch.Tensor, "batch pos"],
+        token_type_ids: Optional[Int[torch.Tensor, "batch pos"]] = None,
+    ):
+        base_index_id = torch.arange(input_ids.shape[1], device=input_ids.device)
+        index_ids = einops.repeat(
+            base_index_id, "pos -> batch pos", batch=input_ids.shape[0]
+        )
+        if token_type_ids is None:
+            token_type_ids = torch.zeros_like(input_ids)
+
+        word_embeddings_out = self.hook_embed(self.embed(input_ids))
+        position_embeddings_out = self.hook_pos_embed(self.pos_embed(index_ids))
+        token_type_embeddings_out = self.hook_token_type_embed(
+            self.token_type_embed(token_type_ids)
+        )
+
+        embeddings_out = (
+            word_embeddings_out + position_embeddings_out + token_type_embeddings_out
+        )
+        layer_norm_out = self.ln(embeddings_out)
+        return layer_norm_out
+
+
+class BertMLMHead(nn.Module):
+    """
+    Transforms BERT embeddings into logits. The purpose of this module is to predict masked tokens in a sentence.
+    """
+
+    def __init__(self, cfg: Union[Dict, HookedTransformerConfig]):
+        super().__init__()
+        if isinstance(cfg, Dict):
+            cfg = HookedTransformerConfig.from_dict(cfg)
+        self.cfg = cfg
+        self.W = nn.Parameter(torch.empty(cfg.d_model, cfg.d_model))
+        self.b = nn.Parameter(torch.zeros(cfg.d_model))
+        self.act_fn = nn.GELU()
+        self.ln = LayerNorm(cfg)
+
+    def forward(self, resid: Float[torch.Tensor, "batch pos d_model"]) -> torch.Tensor:
+        resid = (
+            einsum(
+                "batch pos d_model_in, d_model_out d_model_in -> batch pos d_model_out",
+                resid,
+                self.W,
+            )
+            + self.b
+        )
+        resid = self.act_fn(resid)
+        resid = self.ln(resid)
+        return resid
+
+
 # LayerNormPre
 # I fold the LayerNorm weights and biases into later weights and biases.
 # This is just the 'center and normalise' part of LayerNorm
 # Centering is equivalent to just deleting one direction of residual space,
 # and is equivalent to centering the weight matrices of everything writing to the residual stream
 # Normalising is a funkier non-linear operation, that projects the residual stream onto the unit hypersphere
 class LayerNormPre(nn.Module):
@@ -109,28 +200,35 @@
 
         # Adds a hook point for the normalisation scale factor
         self.hook_scale = HookPoint()  # [batch, pos]
         # Hook Normalized captures LN output - here it's a vector with std 1 and mean 0
         self.hook_normalized = HookPoint()  # [batch, pos, length]
 
     def forward(
-        self, x: Union[Float[torch.Tensor, "batch pos d_model"], Float[torch.Tensor, "batch pos head_index d_model"]]
-    ) -> Union[Float[torch.Tensor, "batch pos d_model"], Float[torch.Tensor, "batch pos head_index d_model"]]:
+        self,
+        x: Union[
+            Float[torch.Tensor, "batch pos d_model"],
+            Float[torch.Tensor, "batch pos head_index d_model"],
+        ],
+    ) -> Union[
+        Float[torch.Tensor, "batch pos d_model"],
+        Float[torch.Tensor, "batch pos head_index d_model"],
+    ]:
         x = x - x.mean(axis=-1, keepdim=True)  # [batch, pos, length]
-        scale: Float[torch.Tensor, "batch pos 1"] = self.hook_scale(
-            (x.pow(2).mean(-1, keepdim=True) + self.eps).sqrt()
-        )
+        scale: Union[
+            Float[torch.Tensor, "batch pos 1"],
+            Float[torch.Tensor, "batch pos head_index 1"],
+        ] = self.hook_scale((x.pow(2).mean(-1, keepdim=True) + self.eps).sqrt())
         return self.hook_normalized(x / scale)
 
 
 class LayerNorm(nn.Module):
     def __init__(
         self, cfg: Union[Dict, HookedTransformerConfig], length: Optional[int] = None
     ):
-
         """
         LayerNorm with optional length parameter
 
         length (Optional[int]): If the dimension of the LayerNorm. If not provided, assumed to be d_model
         """
         super().__init__()
         if isinstance(cfg, Dict):
@@ -147,16 +245,23 @@
 
         # Adds a hook point for the normalisation scale factor
         self.hook_scale = HookPoint()  # [batch, pos, 1]
         # Hook_normalized is on the LN output
         self.hook_normalized = HookPoint()  # [batch, pos, length]
 
     def forward(
-        self, x: Union[Float[torch.Tensor, "batch pos d_model"], Float[torch.Tensor, "batch pos head_index d_model"]]
-    ) -> Union[Float[torch.Tensor, "batch pos d_model"], Float[torch.Tensor, "batch pos head_index d_model"]]:
+        self,
+        x: Union[
+            Float[torch.Tensor, "batch pos d_model"],
+            Float[torch.Tensor, "batch pos head_index d_model"],
+        ],
+    ) -> Union[
+        Float[torch.Tensor, "batch pos d_model"],
+        Float[torch.Tensor, "batch pos head_index d_model"],
+    ]:
         x = x - x.mean(axis=-1, keepdim=True)  # [batch, pos, length]
         scale: Float[torch.Tensor, "batch pos 1"] = self.hook_scale(
             (x.pow(2).mean(-1, keepdim=True) + self.eps).sqrt()
         )
         x = x / scale  # [batch, pos, length]
         return self.hook_normalized(x * self.w + self.b)
 
@@ -183,15 +288,14 @@
         return self.hook_normalized(x / scale)  # [batch, pos, length]
 
 
 class RMSNorm(nn.Module):
     def __init__(
         self, cfg: Union[Dict, HookedTransformerConfig], length: Optional[int] = None
     ):
-
         """
         RMSNorm - LayerNorm without the centering and bias (RMS = Root Mean Square)
 
         length (Optional[int]): If the dimension of the RMSNorm. If not provided, assumed to be d_model
         """
         super().__init__()
         if isinstance(cfg, Dict):
@@ -302,55 +406,69 @@
             self.hook_rot_k = HookPoint()
             self.hook_rot_q = HookPoint()
             sin, cos = self.calculate_sin_cos_rotary(
                 self.cfg.rotary_dim, self.cfg.n_ctx
             )
             self.register_buffer("rotary_sin", sin)
             self.register_buffer("rotary_cos", cos)
-    
+
     @property
+    @typeguard_ignore
     @lru_cache(maxsize=None)
     def OV(self) -> FactoredMatrix:
-        """ 
+        """
         OV-Circuit, as defined in A Mathematical Framework. Because there's no non-linearity between the value vector and the output of the layer, the output is purely determined by the matrix W_OV = W_V @ W_O, and not W_V or W_O individually. (Mathematically, for a single head, output == pattern @ residual @ W_V @ W_O, see the glossary for more)
 
         Done in the order W_V, W_O because the paper uses left-multiplying weight matrices, and TransformerLens uses right-multiplying, sorry!
 
         lru_cache says "compute this the first time a user runs attn.OV, and then cache it". By not defining this in __init__, this means it's only computed and only consumes memory for investigations that need it.
 
         Returns a FactoredMatrix, with left matrix W_V [head_index, d_model, d_head] and right matrix W_O [head_index, d_head, d_model] - this is a low rank factorisation of the underlying [head_index, d_model, d_model]. FactoredMatrix has helper functions to deal with these large matrices efficiently. To get the OV circuit of a head k, attn.OV[k] works.
         """
         return FactoredMatrix(self.W_V, self.W_O)
-    
+
     @property
+    @typeguard_ignore
     @lru_cache(maxsize=None)
     def QK(self) -> FactoredMatrix:
-        """ 
+        """
         QK-Circuit, as defined in A Mathematical Framework. Because there's no non-linearity in the key-query dot product, the output is purely determined by the matrix W_QK = W_Q.T @ W_K, and not W_Q or W_K individually. (Mathematically, for a single head, pattern = destination_residual.T @ W_Q.T @ W_K @ source-residual, see the glossary for more).
 
         Done in the order Q on the left, K on the right, because the pattern has dimensions [destination_pos, source_pos]
 
         lru_cache says "compute this the first time a user runs attn.QK, and then cache it". By not defining this in __init__, this means it's only computed and only consumes memory for investigations that need it.
 
         Returns a FactoredMatrix, with left matrix W_Q [head_index, d_model, d_head] and right matrix W_K.T [head_index, d_head, d_model] - this is a low rank factorisation of the underlying [head_index, d_model, d_model] matrix. FactoredMatrix has helper functions to deal with these large matrices efficiently. To get the QK circuit of a head k, attn.QK[k] works.
         """
-        W_K_transpose = einops.rearrange(self.W_K , "head_index d_model d_head -> head_index d_head d_model")
+        W_K_transpose = einops.rearrange(
+            self.W_K, "head_index d_model d_head -> head_index d_head d_model"
+        )
         return FactoredMatrix(self.W_Q, W_K_transpose)
 
-
     def forward(
         self,
-        query_input: Union[Float[torch.Tensor, "batch pos d_model"], Float[torch.Tensor, "batch pos head_index d_model"]],
-        key_input: Union[Float[torch.Tensor, "batch pos d_model"], Float[torch.Tensor, "batch pos head_index d_model"]],
-        value_input: Union[Float[torch.Tensor, "batch pos d_model"], Float[torch.Tensor, "batch pos head_index d_model"]],
+        query_input: Union[
+            Float[torch.Tensor, "batch pos d_model"],
+            Float[torch.Tensor, "batch pos head_index d_model"],
+        ],
+        key_input: Union[
+            Float[torch.Tensor, "batch pos d_model"],
+            Float[torch.Tensor, "batch pos head_index d_model"],
+        ],
+        value_input: Union[
+            Float[torch.Tensor, "batch pos d_model"],
+            Float[torch.Tensor, "batch pos head_index d_model"],
+        ],
         past_kv_cache_entry: Optional[HookedTransformerKeyValueCacheEntry] = None,
+        additive_attention_mask: Float[torch.Tensor, "batch 1 1 pos"] = None,
     ) -> Float[torch.Tensor, "batch pos d_model"]:
         """
         shortformer_pos_embed is only used if self.cfg.positional_embedding_type == "shortformer", else defaults to None and is irrelevant. See HookedTransformerConfig for more details
         past_kv_cache_entry is an optional entry of past keys and values for this layer, only relevant if generating text. Defaults to None
+        additive_attention_mask is an optional mask to add to the attention weights. Defaults to None.
         """
 
         if self.cfg.use_split_qkv_input:
             qkv_einops_string = "batch pos head_index d_model"
         else:
             qkv_einops_string = "batch pos d_model"
 
@@ -392,26 +510,29 @@
 
         if self.cfg.positional_embedding_type == "rotary":
             q, k = self.rotary_rotate_qk(q, k, kv_cache_pos_offset)
 
         attn_scores = (
             einsum(
                 "batch query_pos head_index d_head, \
-                batch key_pos head_index d_head \
-                -> batch head_index query_pos key_pos",
+                    batch key_pos head_index d_head \
+                    -> batch head_index query_pos key_pos",
                 q,
                 k,
             )
             / self.attn_scale
         )  # [batch, head_index, query_pos, key_pos]
         if self.cfg.attention_dir == "causal":
             # If causal attention, we mask it to only attend backwards. If bidirectional, we don't mask.
             attn_scores = self.apply_causal_mask(
                 attn_scores, kv_cache_pos_offset
             )  # [batch, head_index, query_pos, key_pos]
+        if additive_attention_mask is not None:
+            attn_scores += additive_attention_mask
+
         attn_scores = self.hook_attn_scores(attn_scores)
         pattern = self.hook_pattern(
             F.softmax(attn_scores, dim=-1)
         )  # [batch, head_index, query_pos, key_pos]
         z = self.hook_z(
             einsum(
                 "batch key_pos head_index d_head, \
@@ -422,16 +543,16 @@
             )
         )  # [batch, pos, head_index, d_head]
         if not self.cfg.use_attn_result:
             out = (
                 (
                     einsum(
                         "batch pos head_index d_head, \
-                        head_index d_head d_model -> \
-                        batch pos d_model",
+                            head_index d_head d_model -> \
+                            batch pos d_model",
                         z,
                         self.W_O,
                     )
                 )
                 + self.b_O
             )  # [batch, pos, d_model]
         else:
@@ -452,15 +573,17 @@
                 )
                 + self.b_O
             )  # [batch, pos, d_model]
         return out
 
     def apply_causal_mask(
         self,
-        attn_scores: Float[torch.Tensor, "batch head_index pos pos_plus_past_kv_pos_offset"],
+        attn_scores: Float[
+            torch.Tensor, "batch head_index pos pos_plus_past_kv_pos_offset"
+        ],
         past_kv_pos_offset: int = 0,
     ):
         # The query context length is the number of positions we take queries from - if not using a past_kv_cache this is just the context length (for the current prompt), but if we're caching it's just a single token.
         query_ctx_length = attn_scores.size(-2)
         # The key context length is the number of positions in the past - this includes all positions in the cache
         # If not caching, query_ctx_length == key_ctx_length
         key_ctx_length = attn_scores.size(-1)
@@ -489,54 +612,66 @@
         # We first apply standard q and k calculation
         q = self.hook_rot_q(self.apply_rotary(q, past_kv_pos_offset))
         k = self.hook_rot_k(self.apply_rotary(k))
         return q, k
 
     def calculate_sin_cos_rotary(
         self, rotary_dim: int, n_ctx: int, base: int = 10000
-    ) -> Tuple[Float[torch.Tensor, "n_ctx rotary_dim"], Float[torch.Tensor, "n_ctx rotary_dim"]]:
+    ) -> Tuple[
+        Float[torch.Tensor, "n_ctx rotary_dim"], Float[torch.Tensor, "n_ctx rotary_dim"]
+    ]:
         """
         Calculate the sine and cosine waves to use in a rotary embedding. See https://blog.eleuther.ai/rotary-embeddings/ for details
 
         Note: For some inexplicable reason, in GPT-J each ADJACENT pair of elements in k and q are rotated, in GPT-NeoX the pair of elements at k and k+n//2 are rotated (ie folding the full length in half, and then looking at pairs accordingly). I have absolutely no clue why, it should be completely equivalent.
         To resolve this, I've coded it to default to the GPT-J mode, but to explicitly check whether it's GPT-NeoX and then do the GPT-NeoX thing if it is.
         """
         pos = torch.arange(n_ctx, dtype=torch.float32)
         dim = torch.arange(rotary_dim // 2, dtype=torch.float32)
         # A set of frequencies evenly spaced in log space
         freq = base ** (dim / (rotary_dim / 2))
-        if self.cfg.original_architecture == "GPTNeoXForCausalLM" or self.cfg.original_architecture == "LLaMAForCausalLM":
+        if (
+            self.cfg.original_architecture == "GPTNeoXForCausalLM"
+            or self.cfg.original_architecture == "LLaMAForCausalLM"
+        ):
             freq = einops.repeat(freq, "d -> (2 d)")
         else:
             freq = einops.repeat(freq, "d -> (d 2)")
         # Create a n_ctx x rotary_dim tensor, where each column is an arithmetic sequence of angles in that frequency
         angles = pos[:, None] / freq[None, :]
         return torch.sin(angles), torch.cos(angles)
 
-    def rotate_every_two(self, x: Float[torch.Tensor, "... rotary_dim"]) -> Float[torch.Tensor, "... rotary_dim"]:
+    def rotate_every_two(
+        self, x: Float[torch.Tensor, "... rotary_dim"]
+    ) -> Float[torch.Tensor, "... rotary_dim"]:
         """
         Rotary helper function, splits x into blocks of size 2 along the final axis and maps [x0, x1] to [-x1, x0]
 
         The final axis of x must have even length.
 
         GPT-NeoX and GPT-J do rotary subtly differently, see calculate_sin_cos_rotary for details.
         """
         rot_x = x.clone()
-        if self.cfg.original_architecture == "GPTNeoXForCausalLM" or self.cfg.original_architecture == "LLaMAForCausalLM":
+        if (
+            self.cfg.original_architecture == "GPTNeoXForCausalLM"
+            or self.cfg.original_architecture == "LLaMAForCausalLM"
+        ):
             n = x.size(-1) // 2
             rot_x[..., :n] = -x[..., n:]
             rot_x[..., n:] = x[..., :n]
         else:
             rot_x[..., ::2] = -x[..., 1::2]
             rot_x[..., 1::2] = x[..., ::2]
 
         return rot_x
 
     def apply_rotary(
-        self, x: Float[torch.Tensor, "batch pos head_index d_head"], past_kv_pos_offset=0
+        self,
+        x: Float[torch.Tensor, "batch pos head_index d_head"],
+        past_kv_pos_offset=0,
     ) -> Float[torch.Tensor, "batch pos head_index d_head"]:
         # Only apply rotary to first rotary_dim dimensions (eg, if rotary_dim=64 and d_head=256, only apply to first 1/4 of dimensions)
         x_pos = x.size(1)
         x_rot = x[..., : self.cfg.rotary_dim]
         x_pass = x[..., self.cfg.rotary_dim :]
         x_flip = self.rotate_every_two(x_rot)
         x_rotated = (
@@ -603,32 +738,33 @@
                 "batch pos d_mlp, d_mlp d_model -> batch pos d_model",
                 post_act,
                 self.W_out,
             )
             + self.b_out
         )
 
+
 # TODO
 # not sure whether to fold this into MLP or not
 class GatedMLP(nn.Module):
     def __init__(self, cfg: Union[Dict, HookedTransformerConfig]):
         super().__init__()
         if isinstance(cfg, Dict):
             cfg = HookedTransformerConfig.from_dict(cfg)
         self.cfg = cfg
         self.W_in = nn.Parameter(torch.empty(self.cfg.d_model, self.cfg.d_mlp))
         self.W_gate = nn.Parameter(torch.empty(self.cfg.d_model, self.cfg.d_mlp))
         self.b_in = nn.Parameter(torch.zeros(self.cfg.d_mlp))
         self.W_out = nn.Parameter(torch.empty(self.cfg.d_mlp, self.cfg.d_model))
         self.b_out = nn.Parameter(torch.zeros(self.cfg.d_model))
 
-        # hook on gate output but before act_fn 
-        self.hook_pre = HookPoint() # [batch, pos, d_mlp]
-        # hook on act_fn(gate_output) * W_in(x) + b_in 
-        self.hook_post = HookPoint() # [batch, pos, d_mlp]
+        # hook on gate output but before act_fn
+        self.hook_pre = HookPoint()  # [batch, pos, d_mlp]
+        # hook on act_fn(gate_output) * W_in(x) + b_in
+        self.hook_post = HookPoint()  # [batch, pos, d_mlp]
 
         if self.cfg.act_fn == "relu":
             self.act_fn = F.relu
         elif self.cfg.act_fn == "gelu":
             self.act_fn = F.gelu
         elif self.cfg.act_fn == "silu":
             self.act_fn = F.silu
@@ -648,18 +784,27 @@
         else:
             raise ValueError(f"Invalid activation function name: {self.cfg.act_fn}")
 
     def forward(
         self, x: Float[torch.Tensor, "batch pos d_model"]
     ) -> Float[torch.Tensor, "batch pos d_model"]:
         # Technically, all these einsums could be done with a single matmul, but this is more readable.
-        pre_act = self.hook_pre(einsum("batch pos d_model, d_model d_mlp -> batch pos d_mlp", x, self.W_gate))  # [batch, pos, d_mlp]
+        pre_act = self.hook_pre(
+            einsum(
+                "batch pos d_model, d_model d_mlp -> batch pos d_mlp", x, self.W_gate
+            )
+        )  # [batch, pos, d_mlp]
         if not self.cfg.act_fn.endswith("_ln"):
-            post_act = self.hook_post(self.act_fn(pre_act) * einsum("batch pos d_model, d_model d_mlp -> batch pos d_mlp", x, self.W_in)
-            + self.b_in)  # [batch, pos, d_mlp]
+            post_act = self.hook_post(
+                self.act_fn(pre_act)
+                * einsum(
+                    "batch pos d_model, d_model d_mlp -> batch pos d_mlp", x, self.W_in
+                )
+                + self.b_in
+            )  # [batch, pos, d_mlp]
         else:
             mid_act = self.hook_mid(self.act_fn(pre_act))  # [batch, pos, d_mlp]
             post_act = self.hook_post(self.ln(mid_act))
         return (
             einsum(
                 "batch pos d_mlp, d_mlp d_model -> batch pos d_model",
                 post_act,
@@ -681,15 +826,15 @@
             if not self.cfg.attn_only:
                 self.ln2 = LayerNorm(cfg)
         elif self.cfg.normalization_type == "LNPre":
             # We've folded in LayerNorm weights, so just need the center + scale parts
             self.ln1 = LayerNormPre(cfg)
             if not self.cfg.attn_only:
                 self.ln2 = LayerNormPre(cfg)
-        elif self.cfg.normalization_type == "RMS": 
+        elif self.cfg.normalization_type == "RMS":
             self.ln1 = RMSNorm(cfg)
             if not self.cfg.attn_only:
                 self.ln2 = RMSNorm(cfg)
         elif self.cfg.normalization_type == "RMSPre":
             self.ln1 = RMSNormPre(cfg)
             if not self.cfg.attn_only:
                 self.ln2 = RMSNormPre(cfg)
@@ -707,32 +852,36 @@
         else:
             assert self.cfg.attn_types is not None
             attn_type = self.cfg.attn_types[block_index]
             self.attn = Attention(cfg, attn_type, block_index)
         if not self.cfg.attn_only:
             if self.cfg.gated_mlp:
                 self.mlp = GatedMLP(cfg)
-            else: 
+            else:
                 self.mlp = MLP(cfg)
 
         self.hook_q_input = HookPoint()  # [batch, pos, d_model]
         self.hook_k_input = HookPoint()  # [batch, pos, d_model]
         self.hook_v_input = HookPoint()  # [batch, pos, d_model]
 
         self.hook_attn_out = HookPoint()  # [batch, pos, d_model]
+
+        self.hook_mlp_in = HookPoint()  # [batch, pos, d_model]
         self.hook_mlp_out = HookPoint()  # [batch, pos, d_model]
         self.hook_resid_pre = HookPoint()  # [batch, pos, d_model]
         if not self.cfg.attn_only and not self.cfg.parallel_attn_mlp:
             self.hook_resid_mid = HookPoint()  # [batch, pos, d_model]
         self.hook_resid_post = HookPoint()  # [batch, pos, d_model]
 
     def forward(
         self,
         resid_pre: Float[torch.Tensor, "batch pos d_model"],
-        shortformer_pos_embed: Optional[Float[torch.Tensor, "batch pos d_model"]] = None,
+        shortformer_pos_embed: Optional[
+            Float[torch.Tensor, "batch pos d_model"]
+        ] = None,
         past_kv_cache_entry: Optional[HookedTransformerKeyValueCacheEntry] = None,
     ) -> Float[torch.Tensor, "batch pos d_model"]:
         """A single Transformer block.
 
         Args:
             resid_pre (torch.Tensor): The residual stream - shape [batch, pos, d_model]
             cache (HookedTransformerKeyValueCache): A cache of previous keys and values, used only when generating text. Defaults to None.
@@ -742,42 +891,49 @@
             _type_: _description_
         """
         resid_pre = self.hook_resid_pre(resid_pre)  # [batch, pos, d_model]
 
         query_input = resid_pre
         key_input = resid_pre
         value_input = resid_pre
-        
+
         if self.cfg.use_split_qkv_input:
+
             def add_head_dimension(tensor):
-                return einops.repeat(tensor, "batch pos d_model -> batch pos n_heads d_model", n_heads=self.cfg.n_heads).clone()
+                return einops.repeat(
+                    tensor,
+                    "batch pos d_model -> batch pos n_heads d_model",
+                    n_heads=self.cfg.n_heads,
+                ).clone()
 
             query_input = self.hook_q_input(add_head_dimension(query_input))
             key_input = self.hook_k_input(add_head_dimension(key_input))
             value_input = self.hook_v_input(add_head_dimension(value_input))
 
             if shortformer_pos_embed is not None:
                 shortformer_pos_embed = add_head_dimension(shortformer_pos_embed)
 
         attn_out = self.hook_attn_out(
-            # hook the residual stream states that are used to calculate the 
-            # queries, keys and values, independently. 
+            # hook the residual stream states that are used to calculate the
+            # queries, keys and values, independently.
             # Then take the layer norm of these inputs, and pass these to the attention module.
             self.attn(
-                query_input = self.ln1(query_input) + (0.0 if shortformer_pos_embed is None else shortformer_pos_embed),
-                key_input = self.ln1(key_input) + (0.0 if shortformer_pos_embed is None else shortformer_pos_embed),
-                value_input = self.ln1(value_input),
+                query_input=self.ln1(query_input)
+                + (0.0 if shortformer_pos_embed is None else shortformer_pos_embed),
+                key_input=self.ln1(key_input)
+                + (0.0 if shortformer_pos_embed is None else shortformer_pos_embed),
+                value_input=self.ln1(value_input),
                 past_kv_cache_entry=past_kv_cache_entry,
             )
         )  # [batch, pos, d_model]
         if not self.cfg.attn_only and not self.cfg.parallel_attn_mlp:
             resid_mid = self.hook_resid_mid(
                 resid_pre + attn_out
             )  # [batch, pos, d_model]
-            normalized_resid_mid = self.ln2(resid_mid)
+            normalized_resid_mid = self.ln2(self.hook_mlp_in(resid_mid))
             mlp_out = self.hook_mlp_out(
                 self.mlp(normalized_resid_mid)
             )  # [batch, pos, d_model]
             resid_post = self.hook_resid_post(
                 resid_mid + mlp_out
             )  # [batch, pos, d_model]
         elif self.cfg.parallel_attn_mlp:
@@ -791,7 +947,75 @@
                 resid_pre + attn_out + mlp_out
             )  # [batch, pos, d_model]
         else:
             resid_post = self.hook_resid_post(
                 resid_pre + attn_out
             )  # [batch, pos, d_model]
         return resid_post
+
+
+class BertBlock(nn.Module):
+    """
+    BERT Block. Similar to the TransformerBlock, except that the LayerNorms are applied after the attention and MLP, rather than before.
+    """
+
+    def __init__(self, cfg: HookedTransformerConfig):
+        super().__init__()
+        self.cfg = cfg
+
+        self.attn = Attention(cfg)
+        self.ln1 = LayerNorm(cfg)
+        self.mlp = MLP(cfg)
+        self.ln2 = LayerNorm(cfg)
+
+        self.hook_q_input = HookPoint()  # [batch, pos, d_model]
+        self.hook_k_input = HookPoint()  # [batch, pos, d_model]
+        self.hook_v_input = HookPoint()  # [batch, pos, d_model]
+
+        self.hook_attn_out = HookPoint()  # [batch, pos, d_model]
+        self.hook_mlp_in = HookPoint()  # [batch, pos, d_model]
+        self.hook_mlp_out = HookPoint()  # [batch, pos, d_model]
+        self.hook_resid_pre = HookPoint()  # [batch, pos, d_model]
+        self.hook_resid_mid = HookPoint()  # [batch, pos, d_model]
+        self.hook_resid_post = HookPoint()  # [batch, pos, d_model]
+        self.hook_normalized_resid_post = HookPoint()  # [batch, pos, d_model]
+
+    def forward(
+        self,
+        resid_pre: Float[torch.Tensor, "batch pos d_model"],
+        additive_attention_mask: Optional[Float[torch.Tensor, "batch 1 1 pos"]] = None,
+    ):
+        resid_pre = self.hook_resid_pre(resid_pre)
+
+        query_input = resid_pre
+        key_input = resid_pre
+        value_input = resid_pre
+
+        if self.cfg.use_split_qkv_input:
+
+            def add_head_dimension(tensor):
+                return einops.repeat(
+                    tensor,
+                    "batch pos d_model -> batch pos n_heads d_model",
+                    n_heads=self.cfg.n_heads,
+                ).clone()
+
+            query_input = self.hook_q_input(add_head_dimension(query_input))
+            key_input = self.hook_k_input(add_head_dimension(key_input))
+            value_input = self.hook_v_input(add_head_dimension(value_input))
+
+        attn_out = self.hook_attn_out(
+            self.attn(
+                query_input,
+                key_input,
+                value_input,
+                additive_attention_mask=additive_attention_mask,
+            )
+        )
+        resid_mid = self.hook_resid_mid(resid_pre + attn_out)
+        normalized_resid_mid = self.ln1(resid_mid)
+
+        mlp_out = self.hook_mlp_out(self.mlp(self.hook_mlp_in(normalized_resid_mid)))
+        resid_post = self.hook_resid_post(normalized_resid_mid + mlp_out)
+        normalized_resid_post = self.hook_normalized_resid_post(self.ln2(resid_post))
+
+        return normalized_resid_post
```

### Comparing `transformer_lens-1.2.2/transformer_lens/evals.py` & `transformer_lens-1.3.0/transformer_lens/evals.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # %%
 """ 
 A file with some rough evals for models - I expect you to be likely better off using the HuggingFace evaluate library if you want to do anything properly, but this is here if you want it and want to eg cheaply and roughly compare models you've trained to baselines.
 """
 
-from typing import List, Dict, Optional
+import random
+from typing import Dict, List, Optional
+
+import einops
 import torch
 import tqdm.auto as tqdm
-import random
 from datasets import load_dataset
-from transformer_lens import HookedTransformer, HookedTransformerConfig, utils
 from torch.utils.data import DataLoader, Dataset
-import einops
+
+from transformer_lens import utils
+
 
 # %%
 def sanity_check(model):
     """
     Very basic eval - just feeds a string into the model (in this case, the first paragraph of Circuits: Zoom In), and returns the loss. It's a rough and quick sanity check - if the loss is <5 the model is probably OK, if the loss is >7 something's gone wrong.
 
     Note that this is a very basic eval, and doesn't really tell you much about the model's performance.
@@ -54,30 +57,34 @@
         dataset, batch_size=batch_size, shuffle=True, drop_last=True
     )
     return data_loader
 
 
 def make_pile_data_loader(tokenizer, batch_size=8):
     """
-    Evaluate on OpenWebText an open source replication of the GPT-2 training corpus (Reddit links with >3 karma)
+    Evaluate on the first 10k texts from The Pile.
 
-    I think the Mistral models were trained on this dataset, so they get very good performance.
+    The Pile is EleutherAI's general-purpose english dataset, made of 22 subsets
+    including academic papers, books, internet content...
     """
     pile_data = load_dataset("NeelNanda/pile-10k", split="train")
     print(len(pile_data))
     dataset = utils.tokenize_and_concatenate(pile_data, tokenizer)
     data_loader = DataLoader(
         dataset, batch_size=batch_size, shuffle=True, drop_last=True
     )
     return data_loader
 
 
 def make_code_data_loader(tokenizer, batch_size=8):
     """
-    Evaluate on the CodeParrot dataset, a dump of Python code. All models seem to get significantly lower loss here (even non-code trained models like GPT-2), presumably code is much easier to predict than natural language?
+    Evaluate on the CodeParrot dataset, a dump of Python code.
+
+    All models seem to get significantly lower loss here (even non-code trained models like GPT-2),
+    presumably code is much easier to predict than natural language?
     """
     code_data = load_dataset("codeparrot/codeparrot-valid-v2-near-dedup", split="train")
     print(len(code_data))
     dataset = utils.tokenize_and_concatenate(
         code_data, tokenizer, column_name="content"
     )
     data_loader = DataLoader(
@@ -90,40 +97,41 @@
 DATASET_LOADERS = [
     make_wiki_data_loader,
     make_owt_data_loader,
     make_pile_data_loader,
     make_code_data_loader,
 ]
 
+
 # %%
 @torch.inference_mode()
-def evaluate_on_dataset(model, data_loader, truncate=100):
+def evaluate_on_dataset(model, data_loader, truncate=100, device="cuda"):
     running_loss = 0
     total = 0
     for batch in tqdm.tqdm(data_loader):
-        loss = model(batch["tokens"].cuda(), return_type="loss").mean()
+        loss = model(batch["tokens"].to(device), return_type="loss").mean()
         running_loss += loss.item()
         total += 1
         if total > truncate:
             break
     return running_loss / total
 
 
 # %%
 @torch.inference_mode()
 def induction_loss(
-    model, tokenizer=None, batch_size=4, subseq_len=384, prepend_bos=True
+    model, tokenizer=None, batch_size=4, subseq_len=384, prepend_bos=True, device="cuda"
 ):
     """
     Generates a batch of random sequences repeated twice, and measures model performance on the second half. Tests whether a model has induction heads.
 
     By default, prepends a beginning of string token (prepend_bos flag), which is useful to give models a resting position, and sometimes models were trained with this.
     """
     # Make the repeated sequence
-    first_half_tokens = torch.randint(100, 20000, (batch_size, subseq_len)).cuda()
+    first_half_tokens = torch.randint(100, 20000, (batch_size, subseq_len)).to(device)
     repeated_tokens = einops.repeat(first_half_tokens, "b p -> b (2 p)")
 
     # Prepend a Beginning Of String token
     if prepend_bos:
         if tokenizer is None:
             tokenizer = model.tokenizer
         repeated_tokens[:, 0] = tokenizer.bos_token_id
@@ -131,14 +139,15 @@
     logits = model(repeated_tokens, return_type="logits")
     correct_log_probs = utils.lm_cross_entropy_loss(
         logits, repeated_tokens, per_token=True
     )
     # Take the loss over the second half of the sequence
     return correct_log_probs[:, subseq_len + 1 :].mean()
 
+
 # %%
 @torch.inference_mode()
 def evaluate(model, truncate=100, batch_size=8, tokenizer=None):
     if tokenizer is None:
         tokenizer = model.tokenizer
     losses = {}
     for data_name, data_loader_fn in zip(DATASET_NAMES, DATASET_LOADERS):
@@ -149,15 +158,15 @@
     return losses
 
 
 # %%
 class IOIDataset(Dataset):
     """
     Dataset for Indirect Object Identification tasks.
-    Paper: https://arxiv.org/pdf/2211.00593.pdf 
+    Paper: https://arxiv.org/pdf/2211.00593.pdf
 
     Example:
     --------
     .. code-block:: python
 
         >>> from transformer_lens.evals import ioi_eval, IOIDataset
         >>> from transformer_lens.HookedTransformer import HookedTransformer
@@ -175,132 +184,142 @@
             templates=['[A] met with [B]. [B] gave the [OBJECT] to [A]'],
             names=['Alice', 'Bob', 'Charlie'],
             nouns={'OBJECT': ['ball', 'book']},
             )
         >>> print(ioi_eval(model, dataset=ds))
         {'Logit Difference': 3.7498160457611083, 'Accuracy': 1.0}
     """
-    def __init__(self,
-                 tokenizer,
-                 templates: Optional[List[str]] = None,
-                 names: Optional[List[str]] = None,
-                 nouns: Optional[Dict[str, List[str]]] = None,
-                 num_samples: int = 1000,
-                 symmetric: bool = False,
-                 prepend_bos: bool = True,
-                 ):
+
+    def __init__(
+        self,
+        tokenizer,
+        templates: Optional[List[str]] = None,
+        names: Optional[List[str]] = None,
+        nouns: Optional[Dict[str, List[str]]] = None,
+        num_samples: int = 1000,
+        symmetric: bool = False,
+        prepend_bos: bool = True,
+    ):
         self.tokenizer = tokenizer
         self.prepend_bos = prepend_bos
 
-        self.templates = templates if templates is not None else self.get_default_templates()
+        self.templates = (
+            templates if templates is not None else self.get_default_templates()
+        )
         self.names = names if names is not None else self.get_default_names()
         self.nouns = nouns if nouns is not None else self.get_default_nouns()
 
         self.samples = []
         for _ in range(num_samples // 2 if symmetric else num_samples):
             # If symmetric, get_sample will return two samples
             self.samples.extend(self.get_sample(symmetric=symmetric))
-    
+
     def __len__(self):
         return len(self.samples)
-    
+
     def __getitem__(self, idx):
         sample = self.samples[idx]
-        prompt = self.tokenizer.encode(sample['text'])
+        prompt = self.tokenizer.encode(sample["text"])
         if self.prepend_bos:
             prompt = [self.tokenizer.bos_token_id] + prompt
 
         return {
-            'prompt': torch.LongTensor(prompt),
-            'IO': torch.LongTensor(self.tokenizer.encode(sample['IO'])),
-            'S': torch.LongTensor(self.tokenizer.encode(sample['S'])),
+            "prompt": torch.LongTensor(prompt),
+            "IO": torch.LongTensor(self.tokenizer.encode(sample["IO"])),
+            "S": torch.LongTensor(self.tokenizer.encode(sample["S"])),
         }
-        
+
     def get_sample(self, symmetric=False) -> List[Dict[str, str]]:
         template: str = random.choice(self.templates)
         for noun_type, noun_list in self.nouns.items():
             template = template.replace(f"[{noun_type}]", random.choice(noun_list))
-        
+
         samples: List[Dict[str, str]] = []
-        
+
         # Sample two names without replacement
         names = random.sample(self.names, 2)
         sample = template.replace("[A]", names[0])
         sample = sample.replace("[B]", names[1])
         # Prepend spaces to IO and S so that the target is e.g. " Mary" and not "Mary"
-        samples.append({'text': sample, 'IO': " " + names[0], 'S': " " + names[1]})
+        samples.append({"text": sample, "IO": " " + names[0], "S": " " + names[1]})
 
         if symmetric:
             sample_2 = template.replace("[A]", names[1])
             sample_2 = sample_2.replace("[B]", names[0])
-            samples.append({'text': sample_2, 'IO': " " + names[1], 'S': " " + names[0]})
+            samples.append(
+                {"text": sample_2, "IO": " " + names[1], "S": " " + names[0]}
+            )
 
         return samples
 
     @staticmethod
     def get_default_names():
         return ["John", "Mary"]
 
     @staticmethod
     def get_default_templates():
         return [
             "[A] and [B] went to the [LOCATION] to buy [OBJECT]. [B] handed the [OBJECT] to [A]",
             "Then, [B] and [A] went to the [LOCATION]. [B] gave the [OBJECT] to [A]",
         ]
-    
+
     @staticmethod
     def get_default_nouns():
         return {
             "LOCATION": ["store", "market"],
             "OBJECT": ["milk", "eggs", "bread"],
         }
 
 
 # %%
 @torch.inference_mode()
-def ioi_eval(model, dataset=None, batch_size=8, num_samples=1000, tokenizer=None, symmetric=False):
+def ioi_eval(
+    model, dataset=None, batch_size=8, num_samples=1000, tokenizer=None, symmetric=False
+):
     """
     Evaluates the model on the Indirect Object Identification task.
 
     dataset must be a torch Dataset that returns a dict:
         {
             'prompt': torch.LongTensor,
             'IO': torch.LongTensor,
             'S': torch.LongTensor
         }
 
     Returns average logit difference and accuracy.
     """
     if tokenizer is None:
         tokenizer = model.tokenizer
-    
+
     if dataset is None:
         dataset = IOIDataset(tokenizer, num_samples=num_samples, symmetric=symmetric)
 
     def collate(samples):
-        prompts = [sample['prompt'] for sample in samples]
+        prompts = [sample["prompt"] for sample in samples]
         padded_prompts = torch.nn.utils.rnn.pad_sequence(prompts, batch_first=True)
         return {
-            'prompt': padded_prompts,
-            'IO': [sample['IO'] for sample in samples],
-            'S': [sample['S'] for sample in samples],
-            'prompt_length': [p.shape[0] for p in prompts],
+            "prompt": padded_prompts,
+            "IO": [sample["IO"] for sample in samples],
+            "S": [sample["S"] for sample in samples],
+            "prompt_length": [p.shape[0] for p in prompts],
         }
 
-    data_loader = DataLoader(dataset, batch_size=batch_size, shuffle=True, collate_fn=collate)
+    data_loader = DataLoader(
+        dataset, batch_size=batch_size, shuffle=True, collate_fn=collate
+    )
 
     total_correct = 0
     total_logit_diff = 0
     for batch in tqdm.tqdm(data_loader):
         batch_logits = model(batch["prompt"], return_type="logits")
 
         for i in range(batch_logits.shape[0]):
-            io = batch['IO'][i]
-            s = batch['S'][i]
-            prefix_length = batch['prompt_length'][i] - io.shape[0]
+            io = batch["IO"][i]
+            s = batch["S"][i]
+            prefix_length = batch["prompt_length"][i] - io.shape[0]
 
             # Trim io and s to the same length
             min_len = min(io.shape[0], s.shape[0])
             io = io[:min_len]
             s = s[:min_len]
 
             # Remove identical prefixes
@@ -315,12 +334,12 @@
             incorrect_logit = logits[s]
 
             # Compute stats
             logit_diff = correct_logit - incorrect_logit
             correct = logit_diff > 0
             total_correct += correct.item()
             total_logit_diff += logit_diff.item()
-    
+
     return {
-        'Logit Difference': total_logit_diff / len(dataset),
-        'Accuracy': total_correct / len(dataset),
-        }
+        "Logit Difference": total_logit_diff / len(dataset),
+        "Accuracy": total_correct / len(dataset),
+    }
```

### Comparing `transformer_lens-1.2.2/transformer_lens/head_detector.py` & `transformer_lens-1.3.0/transformer_lens/head_detector.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,158 +1,271 @@
-import torch
+import logging
+from collections import defaultdict
+from typing import Dict, List, Optional, Tuple, Union, cast
+
 import numpy as np
-from transformer_lens import HookedTransformer, ActivationCache
-from typing import List, Tuple
+import torch
+from typing_extensions import Literal, get_args
 
-HEAD_NAMES = ['previous_token_head', 'duplicate_token_head', 'induction_head']
+from transformer_lens import ActivationCache, HookedTransformer
+from transformer_lens.utils import is_lower_triangular, is_square
 
-def detect_head(model: HookedTransformer, 
-                                sequence: str,
-                                head_name: str = None,
-                                detection_pattern: torch.Tensor = None, 
-                                specific_heads: List[Tuple[int, int]] = None,
-                                cache: ActivationCache = None,
-                                exclude_bos: bool = False,
-                                exclude_current_token: bool = False) -> torch.Tensor:
-  
-    """Searches the model (or a set of specific heads, for circuit analysis) for a particular type of attention head. This head is specified
-    by a detection pattern, a (sequence_length, sequence_length) tensor representing how much attention to keep at each position. We element-wise 
-    multiply the attention pattern by the detection pattern, and our score is how much attention is left, divided by the total attention. 
-    (1 per token other than the first). 
-    
-    For instance, a perfect previous token head would put 1 attention to the previous token and 0 to everything else. To write a detection pattern
-    for this head, we would write a (sequence_length, sequence_length) tensor with 1s below the diagonal and 0s everywhere else. That would then
-    be element-wise multiplied by the attention pattern, zeroing out all attention that did not attend to the previous token. The attention
-    remaining divided by the total attention would then be our score for that attention head. (This particular head is already implemented in HEAD_NAMES)
+HeadName = Literal["previous_token_head", "duplicate_token_head", "induction_head"]
+HEAD_NAMES = cast(List[HeadName], get_args(HeadName))
+ErrorMeasure = Literal["abs", "mul"]
+
+LayerHeadTuple = Tuple[int, int]
+LayerToHead = Dict[int, List[int]]
+
+INVALID_HEAD_NAME_ERR = (
+    f"detection_pattern must be a Tensor or one of head names: {HEAD_NAMES}; got %s"
+)
+
+SEQ_LEN_ERR = (
+    "The sequence must be non-empty and must fit within the model's context window."
+)
+
+DET_PAT_NOT_SQUARE_ERR = "The detection pattern must be a lower triangular matrix of shape (sequence_length, sequence_length); sequence_length=%d; got detection patern of shape %s"
+
+
+def detect_head(
+    model: HookedTransformer,
+    seq: Union[str, List[str]],
+    detection_pattern: Union[torch.Tensor, HeadName],
+    heads: Optional[Union[List[LayerHeadTuple], LayerToHead]] = None,
+    cache: Optional[ActivationCache] = None,
+    *,
+    exclude_bos: bool = False,
+    exclude_current_token: bool = False,
+    error_measure: ErrorMeasure = "mul",
+) -> torch.Tensor:
+    """Searches the model (or a set of specific heads, for circuit analysis) for a particular type of attention head.
+    This head is specified by a detection pattern, a (sequence_length, sequence_length) tensor representing the attention pattern we expect that type of attention head to show.
+    The detection pattern can be also passed not as a tensor, but as a name of one of pre-specified types of attention head (see `HeadName` for available patterns), in which case the tensor is computed within the function itself.
+
+    There are two error measures available for quantifying the match between the detection pattern and the actual attention pattern.
+
+    1. `"mul"` (default) multiplies both tensors element-wise and divides the sum of the result by the sum of the attention pattern.
+    Typically, the detection pattern should in this case contain only ones and zeros, which allows a straightforward interpretation of the score:
+    how big fraction of this head's attention is allocated to these specific query-key pairs?
+    Using values other than 0 or 1 is not prohibited but will raise a warning (which can be disabled, of course).
+    2. `"abs"` calculates the mean element-wise absolute difference between the detection pattern and the actual attention pattern.
+    The "raw result" ranges from 0 to 2 where lower score corresponds to greater accuracy. Subtracting it from 1 maps that range to (-1, 1) interval,
+    with 1 being perfect match and -1 perfect mismatch.
+
+    **Which one should you use?** `"mul"` is likely better for quick or exploratory investigations. For precise examinations where you're trying to
+    reproduce as much functionality as possible or really test your understanding of the attention head, you probably want to switch to `"abs"`.
+
+    The advantage of `"abs"` is that you can make more precise predictions, and have that measured in the score.
+    You can predict, for instance, 0.2 attention to X, and 0.8 attention to Y, and your score will be better if your prediction is closer.
+    The "mul" metric does not allow this, you'll get the same score if attention is 0.2, 0.8 or 0.5, 0.5 or 0.8, 0.2.
 
     Args:
-      model: Model being used.
-      sequence: String being fed to the model.
-      head_name: Name of an existing head in HEAD_NAMES we want to check. Must pass either a head_name or a detection_pattern, but not both!
-      detection_pattern: (sequence_length, sequence_length) Tensor representing what attention pattern corresponds to the head we're looking for.
-      specific_heads: If a specific list of heads is given here, all other heads' score is set to -1. Useful for IOI-style circuit analysis.
-      cache: Include the cache to save time if you want.
-      exclude_bos: Exclude attention paid to the beginning of sequence token.
-      exclude_current_token: Exclude attention paid to the current token.
+    ----------
+        model: Model being used.
+        seq: String or list of strings being fed to the model.
+        head_name: Name of an existing head in HEAD_NAMES we want to check. Must pass either a head_name or a detection_pattern, but not both!
+        detection_pattern: (sequence_length, sequence_length) Tensor representing what attention pattern corresponds to the head we're looking for **or** the name of a pre-specified head. Currently available heads are: `["previous_token_head", "duplicate_token_head", "induction_head"]`.
+        heads: If specific attention heads is given here, all other heads' score is set to -1. Useful for IOI-style circuit analysis. Heads can be spacified as a list tuples (layer, head) or a dictionary mapping a layer to heads within that layer that we want to analyze.
+        cache: Include the cache to save time if you want.
+        exclude_bos: Exclude attention paid to the beginning of sequence token.
+        exclude_current_token: Exclude attention paid to the current token.
+        error_measure: `"mul"` for using element-wise multiplication (default). `"abs"` for using absolute values of element-wise differences as the error measure.
+
+    Returns:
+    ----------
+    A (n_layers, n_heads) Tensor representing the score for each attention head.
 
-    Returns a (n_layers, n_heads) Tensor representing the score for each attention head.
-    
     Example:
     --------
     .. code-block:: python
 
+        >>> from transformer_lens import HookedTransformer,  utils
         >>> from transformer_lens.head_detector import detect_head
-        >>> from transformer_lens.HookedTransformer import HookedTransformer
         >>> import plotly.express as px
-        >>> import transformer_lens.utils as utils
 
         >>> def imshow(tensor, renderer=None, xaxis="", yaxis="", **kwargs):
         >>>     px.imshow(utils.to_numpy(tensor), color_continuous_midpoint=0.0, color_continuous_scale="RdBu", labels={"x":xaxis, "y":yaxis}, **kwargs).show(renderer)
 
-        >>> model = HookedTransformer.from_pretrained('gpt2-small')
+        >>> model = HookedTransformer.from_pretrained("gpt2-small")
         >>> sequence = "This is a test sequence. This is a test sequence."
 
-        >>> attention_score = detect_head(model, sequence, head_type='previous_token_head')
+        >>> attention_score = detect_head(model, sequence, "previous_token_head")
         >>> imshow(attention_score, zmin=-1, zmax=1, xaxis="Head", yaxis="Layer", title="Previous Head Matches")
     """
-    
-    assert (head_name is None) != (detection_pattern is None), "Exactly one of head_name or detection_pattern must be specified."
-    device = model.cfg.device
-
-    if head_name is not None:
-      assert head_name in HEAD_NAMES, "Head name not valid."
-      detection_pattern = eval(f'get_{head_name}_detection_pattern(model, sequence)').to(device)
-
-    sequence = model.to_tokens(sequence).to(device)
 
-    assert 1 < sequence.shape[-1] < model.cfg.n_ctx, "The sequence must be non-empty and must fit within the model's context window."
-    assert sequence.shape[-1] == detection_pattern.shape[0] == detection_pattern.shape[1], "The detection pattern must be a square matrix of shape (sequence_length, sequence_length)."
+    cfg = model.cfg
+    tokens = model.to_tokens(seq).to(cfg.device)
+    seq_len = tokens.shape[-1]
+
+    # Validate error_measure
+
+    assert error_measure in get_args(
+        ErrorMeasure
+    ), f"Invalid error_measure={error_measure}; valid values are {get_args(ErrorMeasure)}"
+
+    # Validate detection pattern if it's a string
+    if isinstance(detection_pattern, str):
+        assert detection_pattern in HEAD_NAMES, (
+            INVALID_HEAD_NAME_ERR % detection_pattern
+        )
+        if isinstance(seq, list):
+            batch_scores = [detect_head(model, seq, detection_pattern) for seq in seq]
+            return torch.stack(batch_scores).mean(0)
+        detection_pattern = cast(
+            torch.Tensor,
+            eval(f"get_{detection_pattern}_detection_pattern(tokens.cpu())"),
+        ).to(cfg.device)
+
+    # if we're using "mul", detection_pattern should consist of zeros and ones
+    if error_measure == "mul" and not set(detection_pattern.unique().tolist()).issubset(
+        {0, 1}
+    ):
+        logging.warning(
+            "Using detection pattern with values other than 0 or 1 with error_measure 'mul'"
+        )
+
+    # Validate inputs and detection pattern shape
+    assert 1 < tokens.shape[-1] < cfg.n_ctx, SEQ_LEN_ERR
+    assert (
+        is_lower_triangular(detection_pattern) and seq_len == detection_pattern.shape[0]
+    ), DET_PAT_NOT_SQUARE_ERR % (seq_len, detection_pattern.shape)
 
     if cache is None:
-        _, cache = model.run_with_cache(sequence, remove_batch_dim=True)
-
-    heads = [(i, j) for i in range(model.cfg.n_layers) for j in range(model.cfg.n_heads)]
+        _, cache = model.run_with_cache(tokens, remove_batch_dim=True)
 
-    # If no specific heads are mentioned, grab all of them.
-    if specific_heads is None:
-        specific_heads = [(i, j) for i in range(model.cfg.n_layers) for j in range(model.cfg.n_heads)]
-
-    matches = []
-
-    for head in heads:
-        if head not in specific_heads:
-            matches.append(-1) # This is kinda ugly, the idea is to be able to still plot this on a 2D grid and everything not in the circuit is red. Ideas?
-        else:
-            attention_pattern = cache["pattern", head[0], "attn"]
-            attention_pattern = attention_pattern[head[1], :, :] # We could batch this, but it only takes a few seconds right now. Can worry about that later. 
-            # It'd be a bit more complex of a batch when using specific heads. Could also just batch-compute all heads if it's faster, then set the non-matching heads to -1 afterwards.
-            
-            if exclude_bos:
-              attention_pattern[:, 0] = 0
-
-            if exclude_current_token:
-              attention_pattern.fill_diagonal_(0)
-
-            # Elementwise multiplication keeps only the parts of the attention pattern that are also in the detection pattern.
-            matched_attention = attention_pattern * detection_pattern
-            matches.append((torch.sum(matched_attention) / torch.sum(attention_pattern))) # Return total percentage of attention which matches the detection pattern.
+    if heads is None:
+        layer2heads = {
+            layer_i: list(range(cfg.n_heads)) for layer_i in range(cfg.n_layers)
+        }
+    elif isinstance(heads, list):
+        layer2heads = defaultdict(list)
+        for layer, head in heads:
+            layer2heads[layer].append(head)
+    else:
+        layer2heads = heads
+
+    matches = -torch.ones(cfg.n_layers, cfg.n_heads)
+
+    for layer, layer_heads in layer2heads.items():
+        # [n_heads q_pos k_pos]
+        layer_attention_patterns = cache["pattern", layer, "attn"]
+        for head in layer_heads:
+            head_attention_pattern = layer_attention_patterns[head, :, :]
+            head_score = compute_head_attention_similarity_score(
+                head_attention_pattern,
+                detection_pattern=detection_pattern,
+                exclude_bos=exclude_bos,
+                exclude_current_token=exclude_current_token,
+                error_measure=error_measure,
+            )
+            matches[layer, head] = head_score
+    return matches
 
-    matches = torch.as_tensor(matches)
-    return matches.reshape(model.cfg.n_layers, model.cfg.n_heads)
 
 # Previous token head
-def get_previous_token_head_detection_pattern(model: HookedTransformer, sequence: str) -> torch.Tensor:
-    """Outputs a detection score for previous token heads. 
-    Previous token head: https://dynalist.io/d/n2ZWtnoYHrU1s4vnFSAQ519J#z=0O5VOHe9xeZn8Ertywkh7ioc
-    
+def get_previous_token_head_detection_pattern(
+    tokens: torch.Tensor,  # [batch (1) x pos]
+) -> torch.Tensor:
+    """Outputs a detection score for [previous token heads](https://dynalist.io/d/n2ZWtnoYHrU1s4vnFSAQ519J#z=0O5VOHe9xeZn8Ertywkh7ioc).
+
     Args:
-      model: Model being used.
-      sequence: String being fed to the model."""
-    
-    sequence = model.to_tokens(sequence)
-    detection_pattern = torch.zeros((sequence.shape[-1], sequence.shape[-1]))
-    detection_pattern[1:, :-1] = torch.eye(sequence.shape[-1] - 1) # Adds a diagonal of 1's below the main diagonal.
+      tokens: Tokens being fed to the model.
+    """
+    detection_pattern = torch.zeros(tokens.shape[-1], tokens.shape[-1])
+    # Adds a diagonal of 1's below the main diagonal.
+    detection_pattern[1:, :-1] = torch.eye(tokens.shape[-1] - 1)
     return torch.tril(detection_pattern)
 
+
 # Duplicate token head
-def get_duplicate_token_head_detection_pattern(model: HookedTransformer, sequence: str) -> torch.Tensor:
-    """Outputs a detection score for duplicate token heads. 
-    Duplicate token head: https://dynalist.io/d/n2ZWtnoYHrU1s4vnFSAQ519J#z=2UkvedzOnghL5UHUgVhROxeo
-    
-    Args:
-      model: Model being used.
-      sequence: String being fed to the model."""
-    
-    sequence = model.to_tokens(sequence).detach().cpu()
+def get_duplicate_token_head_detection_pattern(
+    tokens: torch.Tensor,  # [batch (1) x pos]
+) -> torch.Tensor:
+    """Outputs a detection score for [duplicate token heads](https://dynalist.io/d/n2ZWtnoYHrU1s4vnFSAQ519J#z=2UkvedzOnghL5UHUgVhROxeo).
 
-    # Repeat sequence to create a square matrix.
-    token_pattern = sequence.repeat(sequence.shape[-1], 1).numpy()
+    Args:
+      sequence: String being fed to the model.
+    """
+    # [pos x pos]
+    token_pattern = tokens.repeat(tokens.shape[-1], 1).numpy()
 
     # If token_pattern[i][j] matches its transpose, then token j and token i are duplicates.
     eq_mask = np.equal(token_pattern, token_pattern.T).astype(int)
 
-    np.fill_diagonal(eq_mask, 0) # Current token is always a duplicate of itself. Ignore that.
+    np.fill_diagonal(
+        eq_mask, 0
+    )  # Current token is always a duplicate of itself. Ignore that.
     detection_pattern = eq_mask.astype(int)
     return torch.tril(torch.as_tensor(detection_pattern).float())
 
+
 # Induction head
-def get_induction_head_detection_pattern(model: HookedTransformer, sequence: str) -> torch.Tensor:
-    """Outputs a detection score for induction heads. 
-    Induction head: https://dynalist.io/d/n2ZWtnoYHrU1s4vnFSAQ519J#z=_tFVuP5csv5ORIthmqwj0gSY
-    
+def get_induction_head_detection_pattern(
+    tokens: torch.Tensor,  # [batch (1) x pos]
+) -> torch.Tensor:
+    """Outputs a detection score for [induction heads](https://dynalist.io/d/n2ZWtnoYHrU1s4vnFSAQ519J#z=_tFVuP5csv5ORIthmqwj0gSY).
+
     Args:
-      model: Model being used.
-      sequence: String being fed to the model."""
-    
-    duplicate_pattern = get_duplicate_token_head_detection_pattern(model, sequence)
+      sequence: String being fed to the model.
+    """
+    duplicate_pattern = get_duplicate_token_head_detection_pattern(tokens)
 
     # Shift all items one to the right
     shifted_tensor = torch.roll(duplicate_pattern, shifts=1, dims=1)
 
-    # Replace first column with 0's - we don't care about bos but shifting to the right moves the last column to the first, and the last column might contain non-zero values.
-    zeros_column = torch.zeros((duplicate_pattern.shape[0], 1))
+    # Replace first column with 0's
+    # we don't care about bos but shifting to the right moves the last column to the first,
+    # and the last column might contain non-zero values.
+    zeros_column = torch.zeros(duplicate_pattern.shape[0], 1)
     result_tensor = torch.cat((zeros_column, shifted_tensor[:, 1:]), dim=1)
     return torch.tril(result_tensor)
 
-def get_supported_heads():
+
+def get_supported_heads() -> None:
     """Returns a list of supported heads."""
-    print(f"Supported heads: {HEAD_NAMES}")
+    print(f"Supported heads: {HEAD_NAMES}")
+
+
+def compute_head_attention_similarity_score(
+    attention_pattern: torch.Tensor,  # [q_pos k_pos]
+    detection_pattern: torch.Tensor,  # [seq_len seq_len] (seq_len == q_pos == k_pos)
+    *,
+    exclude_bos: bool,
+    exclude_current_token: bool,
+    error_measure: ErrorMeasure,
+) -> float:
+    """Compute the similarity between `attention_pattern` and `detection_pattern`.
+
+    Args:
+      attention_pattern: Lower triangular matrix (Tensor) representing the attention pattern of a particular attention head.
+      detection_pattern: Lower triangular matrix (Tensor) representing the attention pattern we are looking for.
+      exclude_bos: `True` if the beginning-of-sentence (BOS) token should be omitted from comparison. `False` otherwise.
+      exclude_bcurrent_token: `True` if the current token at each position should be omitted from comparison. `False` otherwise.
+      error_measure: "abs" for using absolute values of element-wise differences as the error measure. "mul" for using element-wise multiplication (legacy code).
+    """
+    assert is_square(
+        attention_pattern
+    ), f"Attention pattern is not square; got shape {attention_pattern.shape}"
+
+    # mul
+
+    if error_measure == "mul":
+        if exclude_bos:
+            attention_pattern[:, 0] = 0
+        if exclude_current_token:
+            attention_pattern.fill_diagonal_(0)
+        score = attention_pattern * detection_pattern
+        return (score.sum() / attention_pattern.sum()).item()
+
+    # abs
+
+    abs_diff = (attention_pattern - detection_pattern).abs()
+    assert (abs_diff - torch.tril(abs_diff).to(abs_diff.device)).sum() == 0
+
+    size = len(abs_diff)
+    if exclude_bos:
+        abs_diff[:, 0] = 0
+    if exclude_current_token:
+        abs_diff.fill_diagonal_(0)
+
+    return 1 - round((abs_diff.mean() * size).item(), 3)
```

### Comparing `transformer_lens-1.2.2/transformer_lens/hook_points.py` & `transformer_lens-1.3.0/transformer_lens/hook_points.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,90 +1,121 @@
 # Import stuff
 import logging
-from typing import Callable, Union, Optional, Sequence, Dict, List, Tuple
-import torch
+from contextlib import contextmanager
+from dataclasses import dataclass
+from typing import Callable, Dict, List, Optional, Sequence, Tuple, Union
+
 import torch.nn as nn
 import torch.utils.hooks as hooks
 
-from functools import *
-from contextlib import contextmanager
-
-from dataclasses import dataclass
 
 @dataclass
 class LensHandle:
     """
     A dataclass that holds information about a PyTorch hook.
 
     Attributes:
         hook (hooks.RemovableHandle): Reference to the hook's RemovableHandle.
         is_permanent (bool, optional): Indicates if the hook is permanent. Defaults to False.
         context_level (Optional[int], optional): Context level associated with the hooks context
             manager for the given hook. Defaults to None.
     """
+
     hook: hooks.RemovableHandle
     is_permanent: bool = False
     context_level: Optional[int] = None
-    
+
 
 # %%
 # Define type aliases
 NamesFilter = Optional[Union[Callable[[str], bool], Sequence[str]]]
 
+
 # %%
 class HookPoint(nn.Module):
     """
     A helper class to access intermediate activations in a PyTorch model (inspired by Garcon).
 
     HookPoint is a dummy module that acts as an identity function by default. By wrapping any
     intermediate activation in a HookPoint, it provides a convenient way to add PyTorch hooks.
     """
+
     def __init__(self):
         super().__init__()
         self.fwd_hooks: List[LensHandle] = []
         self.bwd_hooks: List[LensHandle] = []
         self.ctx = {}
 
         # A variable giving the hook's name (from the perspective of the root
         # module) - this is set by the root module at setup.
         self.name = None
 
     def add_perma_hook(self, hook, dir="fwd") -> None:
         self.add_hook(hook, dir=dir, is_permanent=True)
 
-    def add_hook(self, hook, dir="fwd", is_permanent=False, level=None) -> None:
-        # Hook format is fn(activation, hook_name)
-        # Change it into PyTorch hook format (this includes input and output,
-        # which are the same for a HookPoint)
+    def add_hook(
+        self, hook, dir="fwd", is_permanent=False, level=None, prepend=False
+    ) -> None:
+        """
+        Hook format is fn(activation, hook_name)
+        Change it into PyTorch hook format (this includes input and output,
+        which are the same for a HookPoint)
+        If prepend is True, add this hook before all other hooks
+        """
         if dir == "fwd":
 
             def full_hook(module, module_input, module_output):
                 return hook(module_output, hook=self)
 
+            full_hook.__name__ = (
+                hook.__repr__()
+            )  # annotate the `full_hook` with the string representation of the `hook` function
+
             handle = self.register_forward_hook(full_hook)
             handle = LensHandle(handle, is_permanent, level)
-            self.fwd_hooks.append(handle)
+
+            if prepend:
+                # we could just pass this as an argument in PyTorch 2.0, but for now we manually do this...
+                self._forward_hooks.move_to_end(handle.hook.id, last=False)
+                self.fwd_hooks.insert(0, handle)
+
+            else:
+                self.fwd_hooks.append(handle)
+
         elif dir == "bwd":
             # For a backwards hook, module_output is a tuple of (grad,) - I don't know why.
+
             def full_hook(module, module_input, module_output):
                 return hook(module_output[0], hook=self)
+
+            full_hook.__name__ = (
+                hook.__repr__()
+            )  # annotate the `full_hook` with the string representation of the `hook` function
+
             handle = self.register_full_backward_hook(full_hook)
             handle = LensHandle(handle, is_permanent, level)
-            self.bwd_hooks.append(handle)
+
+            if prepend:
+                # we could just pass this as an argument in PyTorch 2.0, but for now we manually do this...
+                self._backward_hooks.move_to_end(handle.hook.id, last=False)
+                self.bwd_hooks.insert(0, handle)
+            else:
+                self.bwd_hooks.append(handle)
         else:
             raise ValueError(f"Invalid direction {dir}")
 
     def remove_hooks(self, dir="fwd", including_permanent=False, level=None) -> None:
-
         def _remove_hooks(handles: List[LensHandle]) -> List[LensHandle]:
             output_handles = []
             for handle in handles:
                 if including_permanent:
                     handle.hook.remove()
-                elif (not handle.is_permanent) and (level is None or handle.context_level == level):
+                elif (not handle.is_permanent) and (
+                    level is None or handle.context_level == level
+                ):
                     handle.hook.remove()
                 else:
                     output_handles.append(handle)
             return output_handles
 
         if dir == "fwd" or dir == "both":
             self.fwd_hooks = _remove_hooks(self.fwd_hooks)
@@ -132,105 +163,161 @@
         adds a parameter to each module containing its name, and builds a dictionary mapping module
         names to the module instances. It also initializes a hook dictionary for modules of type
         "HookPoint".
         """
         self.mod_dict = {}
         self.hook_dict: Dict[str, HookPoint] = {}
         for name, module in self.named_modules():
+            if name == "":
+                continue
             module.name = name
             self.mod_dict[name] = module
             if "HookPoint" in str(type(module)):
                 self.hook_dict[name] = module
 
     def hook_points(self):
         return self.hook_dict.values()
 
-    def remove_all_hook_fns(self, direction="both", including_permanent=False, level=None):
+    def remove_all_hook_fns(
+        self, direction="both", including_permanent=False, level=None
+    ):
         for hp in self.hook_points():
-            hp.remove_hooks(direction, including_permanent=including_permanent, level=level)
+            hp.remove_hooks(
+                direction, including_permanent=including_permanent, level=level
+            )
 
     def clear_contexts(self):
         for hp in self.hook_points():
             hp.clear_context()
 
-    def reset_hooks(self, clear_contexts=True, direction="both", including_permanent=False, level=None):
+    def reset_hooks(
+        self,
+        clear_contexts=True,
+        direction="both",
+        including_permanent=False,
+        level=None,
+    ):
         if clear_contexts:
             self.clear_contexts()
         self.remove_all_hook_fns(direction, including_permanent, level=level)
         self.is_caching = False
 
-    def check_and_add_hook(self, hook_point, hook_point_name, hook, dir="fwd", is_permanent=False, level=None) -> None:
+    def check_and_add_hook(
+        self,
+        hook_point,
+        hook_point_name,
+        hook,
+        dir="fwd",
+        is_permanent=False,
+        level=None,
+        prepend=False,
+    ) -> None:
         """Runs checks on the hook, and then adds it to the hook point"""
-        self.check_hooks_to_add(hook_point, hook_point_name, hook, dir=dir, is_permanent=is_permanent)
-        hook_point.add_hook(hook, dir=dir, is_permanent=is_permanent, level=level)
-    
-    def check_hooks_to_add(self, hook_point, hook_point_name, hook, dir="fwd", is_permanent=False) -> None:
+        self.check_hooks_to_add(
+            hook_point,
+            hook_point_name,
+            hook,
+            dir=dir,
+            is_permanent=is_permanent,
+            prepend=prepend,
+        )
+        hook_point.add_hook(
+            hook, dir=dir, is_permanent=is_permanent, level=level, prepend=prepend
+        )
+
+    def check_hooks_to_add(
+        self, hook_point, hook_point_name, hook, dir="fwd", is_permanent=False
+    ) -> None:
         """Override this function to add checks on which hooks should be added"""
         pass
 
-    def add_hook(self, name, hook, dir="fwd", is_permanent=False, level=None) -> None:
+    def add_hook(
+        self, name, hook, dir="fwd", is_permanent=False, level=None, prepend=False
+    ) -> None:
         if type(name) == str:
-            self.check_and_add_hook(self.mod_dict[name], name, hook, dir=dir, is_permanent=is_permanent, level=level)
+            self.check_and_add_hook(
+                self.mod_dict[name],
+                name,
+                hook,
+                dir=dir,
+                is_permanent=is_permanent,
+                level=level,
+                prepend=prepend,
+            )
         else:
             # Otherwise, name is a Boolean function on names
             for hook_point_name, hp in self.hook_dict.items():
                 if name(hook_point_name):
-                    self.check_and_add_hook(hp, hook_point_name, hook, dir=dir, is_permanent=is_permanent, level=level)
+                    self.check_and_add_hook(
+                        hp,
+                        hook_point_name,
+                        hook,
+                        dir=dir,
+                        is_permanent=is_permanent,
+                        level=level,
+                        prepend=prepend,
+                    )
 
     def add_perma_hook(self, name, hook, dir="fwd") -> None:
         self.add_hook(name, hook, dir=dir, is_permanent=True)
-    
+
     @contextmanager
     def hooks(
         self,
         fwd_hooks: List[Tuple[Union[str, Callable], Callable]] = [],
         bwd_hooks: List[Tuple[Union[str, Callable], Callable]] = [],
         reset_hooks_end: bool = True,
         clear_contexts: bool = False,
-        ):
+    ):
         """
         A context manager for adding temporary hooks to the model.
 
         Args:
             fwd_hooks: List[Tuple[name, hook]], where name is either the name of a hook point or a
                 Boolean function on hook names and hook is the function to add to that hook point.
             bwd_hooks: Same as fwd_hooks, but for the backward pass.
             reset_hooks_end (bool): If True, removes all hooks added by this context manager when the context manager exits.
             clear_contexts (bool): If True, clears hook contexts whenever hooks are reset.
-        
+
         Example:
         --------
         .. code-block:: python
 
             >>> with model.hooks(fwd_hooks=my_hooks):
             >>>     hooked_loss = model(text, return_type="loss")
         """
         try:
             self.context_level += 1
 
             for name, hook in fwd_hooks:
                 if type(name) == str:
-                    self.mod_dict[name].add_hook(hook, dir="fwd", level=self.context_level)
+                    self.mod_dict[name].add_hook(
+                        hook, dir="fwd", level=self.context_level
+                    )
                 else:
                     # Otherwise, name is a Boolean function on names
                     for hook_name, hp in self.hook_dict.items():
                         if name(hook_name):
                             hp.add_hook(hook, dir="fwd", level=self.context_level)
             for name, hook in bwd_hooks:
                 if type(name) == str:
-                    self.mod_dict[name].add_hook(hook, dir="bwd", level=self.context_level)
+                    self.mod_dict[name].add_hook(
+                        hook, dir="bwd", level=self.context_level
+                    )
                 else:
                     # Otherwise, name is a Boolean function on names
                     for hook_name, hp in self.hook_dict:
                         if name(hook_name):
                             hp.add_hook(hook, dir="bwd", level=self.context_level)
             yield self
         finally:
             if reset_hooks_end:
-                self.reset_hooks(clear_contexts, including_permanent=False, level=self.context_level)
+                self.reset_hooks(
+                    clear_contexts, including_permanent=False, level=self.context_level
+                )
             self.context_level -= 1
 
     def run_with_hooks(
         self,
         *model_args,
         fwd_hooks: List[Tuple[Union[str, Callable], Callable]] = [],
         bwd_hooks: List[Tuple[Union[str, Callable], Callable]] = [],
@@ -260,15 +347,17 @@
             remain active. This function only runs a forward pass.
         """
         if len(bwd_hooks) > 0 and reset_hooks_end:
             logging.warning(
                 "WARNING: Hooks will be reset at the end of run_with_hooks. This removes the backward hooks before a backward pass can occur."
             )
 
-        with self.hooks(fwd_hooks, bwd_hooks, reset_hooks_end, clear_contexts) as hooked_model:
+        with self.hooks(
+            fwd_hooks, bwd_hooks, reset_hooks_end, clear_contexts
+        ) as hooked_model:
             return hooked_model.forward(*model_args, **model_kwargs)
 
     def add_caching_hooks(
         self,
         names_filter: NamesFilter = None,
         incl_bwd: bool = False,
         device=None,
@@ -341,35 +430,40 @@
                 model device. WARNING: Setting a different device than the one used by the model leads to
                 significant performance degradation.
             remove_batch_dim (bool, optional): If True, removes the batch dimension when caching. Only
                 makes sense with batch_size=1 inputs. Defaults to False.
             incl_bwd (bool, optional): If True, calls backward on the model output and caches gradients
                 as well. Assumes that the model outputs a scalar (e.g., return_type="loss"). Custom loss
                 functions are not supported. Defaults to False.
-            reset_hooks_end (bool, optional): If True, removes all hooks added by this function at the 
+            reset_hooks_end (bool, optional): If True, removes all hooks added by this function at the
                 end of the run. Defaults to True.
             clear_contexts (bool, optional): If True, clears hook contexts whenever hooks are reset.
                 Defaults to False.
             **model_kwargs: Keyword arguments for the model.
 
         Returns:
             tuple: A tuple containing the model output and a Cache object.
 
         """
         cache_dict, fwd, bwd = self.get_caching_hooks(
             names_filter, incl_bwd, device, remove_batch_dim=remove_batch_dim
         )
 
-        with self.hooks(fwd_hooks=fwd, bwd_hooks=bwd, reset_hooks_end=reset_hooks_end, clear_contexts=clear_contexts):
+        with self.hooks(
+            fwd_hooks=fwd,
+            bwd_hooks=bwd,
+            reset_hooks_end=reset_hooks_end,
+            clear_contexts=clear_contexts,
+        ):
             model_out = self(*model_args, **model_kwargs)
             if incl_bwd:
                 model_out.backward()
 
         return model_out, cache_dict
-    
+
     def get_caching_hooks(
         self,
         names_filter: NamesFilter = None,
         incl_bwd: bool = False,
         device=None,
         remove_batch_dim: bool = False,
         cache: Optional[dict] = None,
@@ -407,15 +501,15 @@
                 cache[hook.name] = tensor.detach().to(device)
 
         def save_hook_back(tensor, hook):
             if remove_batch_dim:
                 cache[hook.name + "_grad"] = tensor.detach().to(device)[0]
             else:
                 cache[hook.name + "_grad"] = tensor.detach().to(device)
-        
+
         fwd_hooks = []
         bwd_hooks = []
         for name, hp in self.hook_dict.items():
             if names_filter(name):
                 fwd_hooks.append((name, save_hook))
                 if incl_bwd:
                     bwd_hooks.append((name, save_hook_back))
```

### Comparing `transformer_lens-1.2.2/transformer_lens/loading_from_pretrained.py` & `transformer_lens-1.3.0/transformer_lens/loading_from_pretrained.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # %%
-from transformer_lens.HookedTransformerConfig import HookedTransformerConfig
+import dataclasses
+import logging
+import re
+from typing import Dict, Optional
+
 import einops
 import torch
-from transformers import AutoConfig, AutoModelForCausalLM
-import transformer_lens.utils as utils
-from typing import Optional, Dict
-import logging
 from huggingface_hub import HfApi
-import re
+from transformers import AutoConfig, AutoModelForCausalLM, BertForPreTraining
+
+import transformer_lens.utils as utils
+from transformer_lens.HookedTransformerConfig import HookedTransformerConfig
 
 # %% The model names used to access the models on the HuggingFace Hub.
 OFFICIAL_MODEL_NAMES = [
     "gpt2",
     "gpt2-medium",
     "gpt2-large",
     "gpt2-xl",
@@ -95,16 +98,32 @@
     "NeelNanda/Attn_Only_4L512W_C4_Code",
     "NeelNanda/Attn-Only-2L512W-Shortformer-6B-big-lr",
     "NeelNanda/SoLU_1L512W_Wiki_Finetune",
     "NeelNanda/SoLU_4L512W_Wiki_Finetune",
     "ArthurConmy/redwood_attn_2l",
     "llama-7b-hf",
     "llama-13b-hf",
-    "llama-30b-hf", 
+    "llama-30b-hf",
     "llama-65b-hf",
+    "Baidicoot/Othello-GPT-Transformer-Lens",
+    "bert-base-cased",
+    "roneneldan/TinyStories-1M",
+    "roneneldan/TinyStories-3M",
+    "roneneldan/TinyStories-8M",
+    "roneneldan/TinyStories-28M",
+    "roneneldan/TinyStories-33M",
+    "roneneldan/TinyStories-Instruct-1M",
+    "roneneldan/TinyStories-Instruct-3M",
+    "roneneldan/TinyStories-Instruct-8M",
+    "roneneldan/TinyStories-Instruct-28M",
+    "roneneldan/TinyStories-Instruct-33M",
+    "roneneldan/TinyStories-1Layer-21M",
+    "roneneldan/TinyStories-2Layers-33M",
+    "roneneldan/TinyStories-Instuct-1Layer-21M",
+    "roneneldan/TinyStories-Instruct-2Layers-33M",
 ]
 
 # Model Aliases:
 MODEL_ALIASES = {
     "NeelNanda/SoLU_1L_v9_old": ["solu-1l-pile", "solu-1l-old"],
     "NeelNanda/SoLU_2L_v10_old": ["solu-2l-pile", "solu-2l-old"],
     "NeelNanda/SoLU_4L_v11_old": ["solu-4l-pile", "solu-4l-old"],
@@ -156,179 +175,176 @@
         "solu-1l-finetune",
     ],
     "NeelNanda/SoLU_4L512W_Wiki_Finetune": [
         "solu-4l-wiki",
         "solu-4l-wiki-finetune",
         "solu-4l-finetune",
     ],
-
     "EleutherAI/pythia-70m": [
-        "pythia-70m", 
+        "pythia-70m",
         "pythia",
         "EleutherAI/pythia-19m",
-        "pythia-19m", # EleutherAI renamed this model 
+        "pythia-19m",  # EleutherAI renamed this model
     ],
     "EleutherAI/pythia-160m": [
         "pythia-160m",
         "EleutherAI/pythia-125m",
-        "pythia-125m", # EleutherAI renamed this model"        
+        "pythia-125m",  # EleutherAI renamed this model"
     ],
     "EleutherAI/pythia-410m": [
         "pythia-410m",
         "EleutherAI/pythia-350m",
-        "pythia-350m", # EleutherAI renamed this model
+        "pythia-350m",  # EleutherAI renamed this model
     ],
     "EleutherAI/pythia-1b": [
         "pythia-1b",
         "EleutherAI/pythia-800m",
-        "pythia-800m", # EleutherAI renamed this model
+        "pythia-800m",  # EleutherAI renamed this model
     ],
     "EleutherAI/pythia-1.4b": [
         "pythia-1.4b",
         "EleutherAI/pythia-1.3b",
-        "pythia-1.3b", # EleutherAI renamed this model
+        "pythia-1.3b",  # EleutherAI renamed this model
     ],
     "EleutherAI/pythia-2.8b": [
         "pythia-2.8b",
         "EleutherAI/pythia-2.7b",
-        "pythia-2.7b", # EleutherAI renamed this model
+        "pythia-2.7b",  # EleutherAI renamed this model
     ],
     "EleutherAI/pythia-6.9b": [
         "pythia-6.9b",
         "EleutherAI/pythia-6.7b",
-        "pythia-6.7b", # EleutherAI renamed this model
+        "pythia-6.7b",  # EleutherAI renamed this model
     ],
     "EleutherAI/pythia-12b": [
         "pythia-12b",
         "EleutherAI/pythia-13b",
-        "pythia-13b", # EleutherAI renamed this model
+        "pythia-13b",  # EleutherAI renamed this model
     ],
     "EleutherAI/pythia-70m-deduped": [
         "pythia-70m-deduped",
-        "EleutherAI/pythia-19m-deduped", # EleutherAI renamed this model 
+        "EleutherAI/pythia-19m-deduped",  # EleutherAI renamed this model
         "pythia-19m-deduped",
     ],
     "EleutherAI/pythia-160m-deduped": [
         "pythia-160m-deduped",
-        "EleutherAI/pythia-125m-deduped", # EleutherAI renamed this model
+        "EleutherAI/pythia-125m-deduped",  # EleutherAI renamed this model
         "pythia-125m-deduped",
     ],
     "EleutherAI/pythia-410m-deduped": [
         "pythia-410m-deduped",
-        "EleutherAI/pythia-350m-deduped", # EleutherAI renamed this model
+        "EleutherAI/pythia-350m-deduped",  # EleutherAI renamed this model
         "pythia-350m-deduped",
     ],
     "EleutherAI/pythia-1b-deduped": [
         "pythia-1b-deduped",
-        "EleutherAI/pythia-800m-deduped", # EleutherAI renamed this model
+        "EleutherAI/pythia-800m-deduped",  # EleutherAI renamed this model
         "pythia-800m-deduped",
     ],
     "EleutherAI/pythia-1.4b-deduped": [
         "pythia-1.4b-deduped",
-        "EleutherAI/pythia-1.3b-deduped", # EleutherAI renamed this model
+        "EleutherAI/pythia-1.3b-deduped",  # EleutherAI renamed this model
         "pythia-1.3b-deduped",
     ],
     "EleutherAI/pythia-2.8b-deduped": [
         "pythia-2.8b-deduped",
-        "EleutherAI/pythia-2.7b-deduped", # EleutherAI renamed this model
+        "EleutherAI/pythia-2.7b-deduped",  # EleutherAI renamed this model
         "pythia-2.7b-deduped",
     ],
     "EleutherAI/pythia-6.9b-deduped": [
         "pythia-6.9b-deduped",
-        "EleutherAI/pythia-6.7b-deduped", # EleutherAI renamed this model
+        "EleutherAI/pythia-6.7b-deduped",  # EleutherAI renamed this model
         "pythia-6.7b-deduped",
     ],
     "EleutherAI/pythia-12b-deduped": [
         "pythia-12b-deduped",
-        "EleutherAI/pythia-13b-deduped", # EleutherAI renamed this model
+        "EleutherAI/pythia-13b-deduped",  # EleutherAI renamed this model
         "pythia-13b-deduped",
     ],
-
     "EleutherAI/pythia-70m-v0": [
-        "pythia-70m-v0", 
+        "pythia-70m-v0",
         "pythia-v0",
         "EleutherAI/pythia-19m-v0",
-        "pythia-19m-v0", # EleutherAI renamed this model 
+        "pythia-19m-v0",  # EleutherAI renamed this model
     ],
     "EleutherAI/pythia-160m-v0": [
         "pythia-160m-v0",
         "EleutherAI/pythia-125m-v0",
-        "pythia-125m-v0", # EleutherAI renamed this model"        
+        "pythia-125m-v0",  # EleutherAI renamed this model"
     ],
     "EleutherAI/pythia-410m-v0": [
         "pythia-410m-v0",
         "EleutherAI/pythia-350m-v0",
-        "pythia-350m-v0", # EleutherAI renamed this model
+        "pythia-350m-v0",  # EleutherAI renamed this model
     ],
     "EleutherAI/pythia-1b-v0": [
         "pythia-1b-v0",
         "EleutherAI/pythia-800m-v0",
-        "pythia-800m-v0", # EleutherAI renamed this model
+        "pythia-800m-v0",  # EleutherAI renamed this model
     ],
     "EleutherAI/pythia-1.4b-v0": [
         "pythia-1.4b-v0",
         "EleutherAI/pythia-1.3b-v0",
-        "pythia-1.3b-v0", # EleutherAI renamed this model
+        "pythia-1.3b-v0",  # EleutherAI renamed this model
     ],
     "EleutherAI/pythia-2.8b-v0": [
         "pythia-2.8b-v0",
         "EleutherAI/pythia-2.7b-v0",
-        "pythia-2.7b-v0", # EleutherAI renamed this model
+        "pythia-2.7b-v0",  # EleutherAI renamed this model
     ],
     "EleutherAI/pythia-6.9b-v0": [
         "pythia-6.9b-v0",
         "EleutherAI/pythia-6.7b-v0",
-        "pythia-6.7b-v0", # EleutherAI renamed this model
+        "pythia-6.7b-v0",  # EleutherAI renamed this model
     ],
     "EleutherAI/pythia-12b-v0": [
         "pythia-12b-v0",
         "EleutherAI/pythia-13b-v0",
-        "pythia-13b-v0", # EleutherAI renamed this model
+        "pythia-13b-v0",  # EleutherAI renamed this model
     ],
     "EleutherAI/pythia-70m-deduped-v0": [
         "pythia-70m-deduped-v0",
-        "EleutherAI/pythia-19m-deduped-v0", # EleutherAI renamed this model 
+        "EleutherAI/pythia-19m-deduped-v0",  # EleutherAI renamed this model
         "pythia-19m-deduped-v0",
     ],
     "EleutherAI/pythia-160m-deduped-v0": [
         "pythia-160m-deduped-v0",
-        "EleutherAI/pythia-125m-deduped-v0", # EleutherAI renamed this model
+        "EleutherAI/pythia-125m-deduped-v0",  # EleutherAI renamed this model
         "pythia-125m-deduped-v0",
     ],
     "EleutherAI/pythia-410m-deduped-v0": [
         "pythia-410m-deduped-v0",
-        "EleutherAI/pythia-350m-deduped-v0", # EleutherAI renamed this model
+        "EleutherAI/pythia-350m-deduped-v0",  # EleutherAI renamed this model
         "pythia-350m-deduped-v0",
     ],
     "EleutherAI/pythia-1b-deduped-v0": [
         "pythia-1b-deduped-v0",
-        "EleutherAI/pythia-800m-deduped-v0", # EleutherAI renamed this model
+        "EleutherAI/pythia-800m-deduped-v0",  # EleutherAI renamed this model
         "pythia-800m-deduped-v0",
     ],
     "EleutherAI/pythia-1.4b-deduped-v0": [
         "pythia-1.4b-deduped-v0",
-        "EleutherAI/pythia-1.3b-deduped-v0", # EleutherAI renamed this model
+        "EleutherAI/pythia-1.3b-deduped-v0",  # EleutherAI renamed this model
         "pythia-1.3b-deduped-v0",
     ],
     "EleutherAI/pythia-2.8b-deduped-v0": [
         "pythia-2.8b-deduped-v0",
-        "EleutherAI/pythia-2.7b-deduped-v0", # EleutherAI renamed this model
+        "EleutherAI/pythia-2.7b-deduped-v0",  # EleutherAI renamed this model
         "pythia-2.7b-deduped-v0",
     ],
     "EleutherAI/pythia-6.9b-deduped-v0": [
         "pythia-6.9b-deduped-v0",
-        "EleutherAI/pythia-6.7b-deduped-v0", # EleutherAI renamed this model
+        "EleutherAI/pythia-6.7b-deduped-v0",  # EleutherAI renamed this model
         "pythia-6.7b-deduped-v0",
     ],
     "EleutherAI/pythia-12b-deduped-v0": [
         "pythia-12b-deduped-v0",
-        "EleutherAI/pythia-13b-deduped-v0", # EleutherAI renamed this model
+        "EleutherAI/pythia-13b-deduped-v0",  # EleutherAI renamed this model
         "pythia-13b-deduped-v0",
     ],
-    
     "gpt2": ["gpt2-small"],
     "distilgpt2": ["distillgpt2", "distill-gpt2", "distil-gpt2", "gpt2-xs"],
     "facebook/opt-125m": ["opt-125m", "opt-small", "opt"],
     "facebook/opt-1.3b": ["opt-1.3b", "opt-medium"],
     "facebook/opt-2.7b": ["opt-2.7b", "opt-large"],
     "facebook/opt-6.7b": ["opt-6.7b", "opt-xl"],
     "facebook/opt-13b": ["opt-13b", "opt-xxl"],
@@ -396,22 +412,41 @@
     "stanford-crfm/eowyn-gpt2-medium-x777": [
         "stanford-gpt2-medium-e",
         "eowyn-gpt2-medium-x777",
         "gpt2-medium-small-e",
         "gpt2-stanford-medium-e",
     ],
     "ArthurConmy/redwood_attn_2l": ["redwood_attn_2l"],
-    "llama-7b-hf": ["llama-7b"], 
+    "llama-7b-hf": ["llama-7b"],
     "llama-13b-hf": ["llama-13b"],
     "llama-30b-hf": ["llama-30b"],
     "llama-65b-hf": ["llama-65b"],
+    "Baidicoot/Othello-GPT-Transformer-Lens": ["othello-gpt"],
+    "roneneldan/TinyStories-1M": ["tiny-stories-1M"],
+    "roneneldan/TinyStories-3M": ["tiny-stories-3M"],
+    "roneneldan/TinyStories-8M": ["tiny-stories-8M"],
+    "roneneldan/TinyStories-28M": ["tiny-stories-28M"],
+    "roneneldan/TinyStories-33M": ["tiny-stories-33M"],
+    "roneneldan/TinyStories-Instruct-1M": ["tiny-stories-instruct-1M"],
+    "roneneldan/TinyStories-Instruct-3M": ["tiny-stories-instruct-3M"],
+    "roneneldan/TinyStories-Instruct-8M": ["tiny-stories-instruct-8M"],
+    "roneneldan/TinyStories-Instruct-28M": ["tiny-stories-instruct-28M"],
+    "roneneldan/TinyStories-Instruct-33M": ["tiny-stories-instruct-33M"],
+    "roneneldan/TinyStories-1Layer-21M": ["tiny-stories-1L-21M"],
+    "roneneldan/TinyStories-2Layers-33M": ["tiny-stories-2L-33M"],
+    "roneneldan/TinyStories-Instuct-1Layer-21M": ["tiny-stories-instruct-1L-21M"],
+    "roneneldan/TinyStories-Instruct-2Layers-33M": ["tiny-stories-instruct-2L-33M"],
 }
 
 # Sets a default model alias, by convention the first one in the model alias table, else the official name if it has no aliases
-DEFAULT_MODEL_ALIASES = [MODEL_ALIASES[name][0] if name in MODEL_ALIASES else name for name in OFFICIAL_MODEL_NAMES]
+DEFAULT_MODEL_ALIASES = [
+    MODEL_ALIASES[name][0] if name in MODEL_ALIASES else name
+    for name in OFFICIAL_MODEL_NAMES
+]
+
 
 def make_model_alias_map():
     """
     Converts OFFICIAL_MODEL_NAMES (the list of actual model names on
     HuggingFace) and MODEL_ALIASES (a dictionary mapping official model names to
     aliases) into a dictionary mapping all aliases to the official model name.
     """
@@ -433,96 +468,96 @@
     if official_model_name is None:
         raise ValueError(
             f"{model_name} not found. Valid official model names (excl aliases): {OFFICIAL_MODEL_NAMES}"
         )
     return official_model_name
 
 
-def convert_hf_model_config(official_model_name: str):
+def convert_hf_model_config(model_name: str, **kwargs):
     """
     Returns the model config for a HuggingFace model, converted to a dictionary
     in the HookedTransformerConfig format.
 
     Takes the official_model_name as an input.
     """
     # In case the user passed in an alias
-    official_model_name = get_official_model_name(official_model_name)
+    official_model_name = get_official_model_name(model_name)
     # Load HuggingFace model config
-    if 'llama' not in official_model_name:
-        hf_config = AutoConfig.from_pretrained(official_model_name)
+    if "llama" not in official_model_name:
+        hf_config = AutoConfig.from_pretrained(official_model_name, **kwargs)
         architecture = hf_config.architectures[0]
-    else: 
+    else:
         architecture = "LLaMAForCausalLM"
-    if 'llama-7b' in official_model_name:
+    if "llama-7b" in official_model_name:
         cfg_dict = {
             "d_model": 4096,
             "d_head": 4096 // 32,
             "n_heads": 32,
             "d_mlp": 11008,
             "n_layers": 32,
             "n_ctx": 2048,
-            "eps": 1e-6, 
+            "eps": 1e-6,
             "d_vocab": 32000,
-            "act_fn": "silu", 
-            "normalization_type": "RMS", 
+            "act_fn": "silu",
+            "normalization_type": "RMS",
             "positional_embedding_type": "rotary",
-            "rotary_dim": 4096 // 32, 
-            "final_rms": True, 
-            "gated_mlp": True, 
+            "rotary_dim": 4096 // 32,
+            "final_rms": True,
+            "gated_mlp": True,
         }
-    elif 'llama-13b' in official_model_name:
+    elif "llama-13b" in official_model_name:
         cfg_dict = {
             "d_model": 5120,
             "d_head": 5120 // 40,
             "n_heads": 40,
             "d_mlp": 13824,
             "n_layers": 40,
             "n_ctx": 2048,
-            "eps": 1e-6, 
+            "eps": 1e-6,
             "d_vocab": 32000,
-            "act_fn": "silu", 
-            "normalization_type": "RMS", 
+            "act_fn": "silu",
+            "normalization_type": "RMS",
             "positional_embedding_type": "rotary",
-            "rotary_dim": 5120 // 40, 
-            "final_rms": True, 
-            "gated_mlp": True, 
+            "rotary_dim": 5120 // 40,
+            "final_rms": True,
+            "gated_mlp": True,
         }
-    elif 'llama-30b' in official_model_name:
+    elif "llama-30b" in official_model_name:
         cfg_dict = {
             "d_model": 6656,
             "d_head": 6656 // 52,
             "n_heads": 52,
             "d_mlp": 17920,
             "n_layers": 60,
             "n_ctx": 2048,
-            "eps": 1e-6, 
+            "eps": 1e-6,
             "d_vocab": 32000,
-            "act_fn": "silu", 
-            "normalization_type": "RMS", 
+            "act_fn": "silu",
+            "normalization_type": "RMS",
             "positional_embedding_type": "rotary",
-            "rotary_dim": 6656 // 52, 
-            "final_rms": True, 
-            "gated_mlp": True, 
+            "rotary_dim": 6656 // 52,
+            "final_rms": True,
+            "gated_mlp": True,
         }
-    elif 'llama-65b' in official_model_name:
+    elif "llama-65b" in official_model_name:
         cfg_dict = {
             "d_model": 8192,
             "d_head": 8192 // 64,
             "n_heads": 64,
             "d_mlp": 22016,
             "n_layers": 80,
             "n_ctx": 2048,
-            "eps": 1e-6, 
+            "eps": 1e-6,
             "d_vocab": 32000,
-            "act_fn": "silu", 
-            "normalization_type": "RMS", 
+            "act_fn": "silu",
+            "normalization_type": "RMS",
             "positional_embedding_type": "rotary",
-            "rotary_dim": 8192 // 64, 
-            "final_rms": True, 
-            "gated_mlp": True, 
+            "rotary_dim": 8192 // 64,
+            "final_rms": True,
+            "gated_mlp": True,
         }
     elif architecture == "GPTNeoForCausalLM":
         cfg_dict = {
             "d_model": hf_config.hidden_size,
             "d_head": hf_config.hidden_size // hf_config.num_heads,
             "n_heads": hf_config.num_heads,
             "d_mlp": hf_config.hidden_size * 4,
@@ -532,15 +567,15 @@
             "d_vocab": hf_config.vocab_size,
             "attn_types": hf_config.attention_layers,
             "act_fn": hf_config.activation_function,
             "use_attn_scale": False,
             "use_local_attn": True,
             "window_size": hf_config.window_size,
             "scale_attn_by_inverse_layer_idx": False,
-            "normalization_type": "LN", 
+            "normalization_type": "LN",
         }
     elif architecture == "GPT2LMHeadModel":
         cfg_dict = {
             "d_model": hf_config.n_embd,
             "d_head": hf_config.n_embd // hf_config.n_head,
             "n_heads": hf_config.n_head,
             "d_mlp": hf_config.n_embd * 4,
@@ -548,15 +583,15 @@
             "n_ctx": hf_config.n_ctx,
             "eps": hf_config.layer_norm_epsilon,
             "d_vocab": hf_config.vocab_size,
             "act_fn": hf_config.activation_function,
             "use_attn_scale": True,
             "use_local_attn": False,
             "scale_attn_by_inverse_layer_idx": hf_config.scale_attn_by_inverse_layer_idx,
-            "normalization_type": "LN", 
+            "normalization_type": "LN",
         }
     elif architecture == "OPTForCausalLM":
         cfg_dict = {
             "d_model": hf_config.hidden_size,
             "d_head": hf_config.hidden_size // hf_config.num_attention_heads,
             "n_heads": hf_config.num_attention_heads,
             "d_mlp": hf_config.ffn_dim,
@@ -564,15 +599,15 @@
             "n_ctx": hf_config.max_position_embeddings,
             "eps": 1e-5,
             "d_vocab": hf_config.vocab_size,
             "act_fn": hf_config.activation_function,
             "use_attn_scale": True,
             "use_local_attn": False,
             "scale_attn_by_inverse_layer_idx": False,
-            "normalization_type": "LN", 
+            "normalization_type": "LN",
         }
     elif architecture == "GPTJForCausalLM":
         cfg_dict = {
             "d_model": hf_config.n_embd,
             "d_head": hf_config.n_embd // hf_config.n_head,
             "n_heads": hf_config.n_head,
             "d_mlp": 4 * hf_config.n_embd,
@@ -583,15 +618,15 @@
             "act_fn": hf_config.activation_function,
             "use_attn_scale": True,
             "use_local_attn": False,
             "scale_attn_by_inverse_layer_idx": False,
             "parallel_attn_mlp": True,
             "positional_embedding_type": "rotary",
             "rotary_dim": hf_config.rotary_dim,
-            "normalization_type": "LN", 
+            "normalization_type": "LN",
         }
     elif architecture == "GPTNeoXForCausalLM":
         cfg_dict = {
             "d_model": hf_config.hidden_size,
             "d_head": hf_config.hidden_size // hf_config.num_attention_heads,
             "n_heads": hf_config.num_attention_heads,
             "d_mlp": hf_config.intermediate_size,
@@ -601,51 +636,67 @@
             "d_vocab": hf_config.vocab_size,
             "act_fn": hf_config.hidden_act,
             "use_attn_scale": True,
             "use_local_attn": False,
             "scale_attn_by_inverse_layer_idx": False,
             "parallel_attn_mlp": True,
             "positional_embedding_type": "rotary",
-            "normalization_type": "LN", 
+            "normalization_type": "LN",
         }
         rotary_pct = hf_config.rotary_pct
         cfg_dict["rotary_dim"] = round(rotary_pct * cfg_dict["d_head"])
+    elif architecture == "BertForMaskedLM":
+        cfg_dict = {
+            "d_model": hf_config.hidden_size,
+            "d_head": hf_config.hidden_size // hf_config.num_attention_heads,
+            "n_heads": hf_config.num_attention_heads,
+            "d_mlp": hf_config.intermediate_size,
+            "n_layers": hf_config.num_hidden_layers,
+            "n_ctx": hf_config.max_position_embeddings,
+            "eps": hf_config.layer_norm_eps,
+            "d_vocab": hf_config.vocab_size,
+            "act_fn": "gelu",
+            "attention_dir": "bidirectional",
+        }
     else:
         raise NotImplementedError(f"{architecture} is not currently supported.")
     # All of these models use LayerNorm
     cfg_dict["original_architecture"] = architecture
     # The name such that AutoTokenizer.from_pretrained works
     cfg_dict["tokenizer_name"] = official_model_name
     return cfg_dict
 
 
-def convert_neel_model_config(official_model_name: str):
+def convert_neel_model_config(official_model_name: str, **kwargs):
     """
     Loads the config for a model trained by me (NeelNanda), converted to a dictionary
     in the HookedTransformerConfig format.
 
     AutoConfig is not supported, because these models are in the HookedTransformer format, so we directly download and load the json.
     """
     official_model_name = get_official_model_name(official_model_name)
-    cfg_json: dict = utils.download_file_from_hf(official_model_name, "config.json")
+    cfg_json: dict = utils.download_file_from_hf(
+        official_model_name, "config.json", **kwargs
+    )
+    cfg_arch = cfg_json.get(
+        "architecture", "neel" if "_old" not in official_model_name else "neel-solu-old"
+    )
     cfg_dict = {
         "d_model": cfg_json["d_model"],
         "n_layers": cfg_json["n_layers"],
         "d_mlp": cfg_json["d_mlp"],
         "d_head": cfg_json["d_head"],
         "n_heads": cfg_json["n_heads"],
         "n_ctx": cfg_json["n_ctx"],
         "d_vocab": cfg_json["d_vocab"],
-        "tokenizer_name": cfg_json["tokenizer_name"],
+        "tokenizer_name": cfg_json.get("tokenizer_name", None),
         "act_fn": cfg_json["act_fn"],
         "attn_only": cfg_json["attn_only"],
         "final_rms": cfg_json.get("final_rms", False),
-        "original_architecture": (
-            "neel" if "_old" not in official_model_name else "neel-solu-old"
-        ),
+        "original_architecture": cfg_arch,
     }
     if "normalization" in cfg_json:
         cfg_dict["normalization_type"] = cfg_json["normalization"]
     else:
         cfg_dict["normalization_type"] = cfg_json["normalization_type"]
     if "shortformer_pos" in cfg_json:
         cfg_dict["positional_embedding_type"] = (
@@ -659,14 +710,15 @@
 def get_pretrained_model_config(
     model_name: str,
     checkpoint_index: Optional[int] = None,
     checkpoint_value: Optional[int] = None,
     fold_ln: bool = False,
     device: Optional[str] = None,
     n_devices: int = 1,
+    **kwargs,
 ):
     """Returns the pretrained model config as an HookedTransformerConfig object.
 
     There are two types of pretrained models: HuggingFace models (where
     AutoModel and AutoConfig work), and models trained by me (NeelNanda) which
     aren't as integrated with HuggingFace infrastructure.
 
@@ -682,47 +734,65 @@
             checkpoints labelled with exactly one of these). Defaults to None.
         fold_ln (bool, optional): Whether to fold the layer norm into the
             subsequent linear layers (see HookedTransformer.fold_layer_norm for
             details). Defaults to False.
         device (str, optional): The device to load the model onto. By
             default will load to CUDA if available, else CPU.
         n_devices (int): The number of devices to split the model across. Defaults to 1.
+        kwargs: Other optional arguments passed to HuggingFace's from_pretrained.
+            Also given to other HuggingFace functions when compatible.
 
     """
     official_model_name = get_official_model_name(model_name)
-    if official_model_name.startswith("NeelNanda") or official_model_name.startswith("ArthurConmy"):
-        cfg_dict = convert_neel_model_config(official_model_name)
+    if (
+        official_model_name.startswith("NeelNanda")
+        or official_model_name.startswith("ArthurConmy")
+        or official_model_name.startswith("Baidicoot")
+    ):
+        cfg_dict = convert_neel_model_config(official_model_name, **kwargs)
     else:
-        cfg_dict = convert_hf_model_config(official_model_name)
+        cfg_dict = convert_hf_model_config(official_model_name, **kwargs)
     # Processing common to both model types
     # Remove any prefix, saying the organization who made a model.
     cfg_dict["model_name"] = official_model_name.split("/")[-1]
     # Don't need to initialize weights, we're loading from pretrained
     cfg_dict["init_weights"] = False
 
+    if (
+        "positional_embedding_type" in cfg_dict
+        and cfg_dict["positional_embedding_type"] == "shortformer"
+        and fold_ln
+    ):
+        logging.warning(
+            "You tried to specify fold_ln=True for a shortformer model, but this can't be done! Setting fold_ln=False instead."
+        )
+        fold_ln = False
+
     if device is not None:
         cfg_dict["device"] = device
     if fold_ln:
         if cfg_dict["normalization_type"] in ["LN", "LNPre"]:
             cfg_dict["normalization_type"] = "LNPre"
         else:
             logging.warning("Cannot fold in layer norm, normalization_type is not LN.")
-            pass
 
     if checkpoint_index is not None or checkpoint_value is not None:
         checkpoint_labels, checkpoint_label_type = get_checkpoint_labels(
-            official_model_name
+            official_model_name,
+            **kwargs,
         )
         cfg_dict["from_checkpoint"] = True
         cfg_dict["checkpoint_label_type"] = checkpoint_label_type
         if checkpoint_index is not None:
             cfg_dict["checkpoint_index"] = checkpoint_index
             cfg_dict["checkpoint_value"] = checkpoint_labels[checkpoint_index]
         elif checkpoint_value is not None:
-            assert checkpoint_value in checkpoint_labels, f"Checkpoint value {checkpoint_value} is not in list of available checkpoints"
+            assert (
+                checkpoint_value in checkpoint_labels
+            ), f"Checkpoint value {checkpoint_value} is not in list of available checkpoints"
             cfg_dict["checkpoint_value"] = checkpoint_value
             cfg_dict["checkpoint_index"] = checkpoint_labels.index(checkpoint_value)
     else:
         cfg_dict["from_checkpoint"] = False
 
     cfg_dict["device"] = device
     cfg_dict["n_devices"] = n_devices
@@ -744,39 +814,43 @@
 STANFORD_CRFM_CHECKPOINTS = (
     list(range(0, 100, 10))
     + list(range(100, 2000, 50))
     + list(range(2000, 20000, 100))
     + list(range(20000, 400000 + 1, 1000))
 )
 
-# Linearly spaced checkpoints for Pythia models, taken every 1000 steps. 
+# Linearly spaced checkpoints for Pythia models, taken every 1000 steps.
 # Batch size 2,097,152 tokens, so checkpoints every 2.1B tokens
-PYTHIA_CHECKPOINTS = (
-    [0, 1, 2, 4, 8, 16, 32, 64, 128, 256, 512]
-    + list(range(1000, 143000+1, 1000))
+PYTHIA_CHECKPOINTS = [0, 1, 2, 4, 8, 16, 32, 64, 128, 256, 512] + list(
+    range(1000, 143000 + 1, 1000)
 )
 # Pythia V1 has log-spaced early checkpoints (see line above), but V0 doesn't
-PYTHIA_V0_CHECKPOINTS = list(range(1000, 143000+1, 1000))
+PYTHIA_V0_CHECKPOINTS = list(range(1000, 143000 + 1, 1000))
 
 
-def get_checkpoint_labels(model_name: str):
+def get_checkpoint_labels(model_name: str, **kwargs):
     """Returns the checkpoint labels for a given model, and the label_type
     (step or token). Raises an error for models that are not checkpointed."""
     official_model_name = get_official_model_name(model_name)
     if official_model_name.startswith("stanford-crfm/"):
         return STANFORD_CRFM_CHECKPOINTS, "step"
     elif official_model_name.startswith("EleutherAI/pythia"):
         if "v0" in official_model_name:
             return PYTHIA_V0_CHECKPOINTS, "step"
         else:
-            logging.warning("Pythia models on HF were updated on 4/3/23! add '-v0' to model name to access the old models.")
+            logging.warning(
+                "Pythia models on HF were updated on 4/3/23! add '-v0' to model name to access the old models."
+            )
             return PYTHIA_CHECKPOINTS, "step"
     elif official_model_name.startswith("NeelNanda/"):
         api = HfApi()
-        files_list = api.list_repo_files(official_model_name)
+        files_list = api.list_repo_files(
+            official_model_name,
+            **utils.select_compatible_kwargs(kwargs, api.list_repo_files),
+        )
         labels = []
         for file_name in files_list:
             match = re.match(r"checkpoints/.*_(\d*)\.pth", file_name)
             if match:
                 labels.append(int(match.group(1)))
         if labels[-1] > 1e9:
             label_type = "token"
@@ -790,101 +864,140 @@
 # %% Loading state dicts
 
 
 def get_pretrained_state_dict(
     official_model_name: str,
     cfg: HookedTransformerConfig,
     hf_model=None,
+    **kwargs,
 ) -> Dict[str, torch.Tensor]:
     """
     Loads in the model weights for a pretrained model, and processes them to
     have the HookedTransformer parameter names and shapes. Supports checkpointed
     models (and expects the checkpoint info to be stored in the config object)
 
     hf_model: Optionally, a HuggingFace model object. If provided, we will use
-    these weights rather than reloading the model.
+        these weights rather than reloading the model.
+    kwargs: Other optional arguments passed to HuggingFace's from_pretrained.
+        Also given to other HuggingFace functions when compatible.
     """
     official_model_name = get_official_model_name(official_model_name)
-    if official_model_name.startswith("NeelNanda") or official_model_name.startswith("ArthurConmy"):
+    if (
+        official_model_name.startswith("NeelNanda")
+        or official_model_name.startswith("ArthurConmy")
+        or official_model_name.startswith("Baidicoot")
+    ):
         api = HfApi()
-        repo_files = api.list_repo_files(official_model_name)
+        repo_files = api.list_repo_files(
+            official_model_name,
+            **utils.select_compatible_kwargs(kwargs, api.list_repo_files),
+        )
         if cfg.from_checkpoint:
             file_name = list(
                 filter(lambda x: x.endswith(f"{cfg.checkpoint_value}.pth"), repo_files)
             )[0]
         else:
             file_name = list(filter(lambda x: x.endswith("final.pth"), repo_files))[0]
-        state_dict = utils.download_file_from_hf(official_model_name, file_name)
+        state_dict = utils.download_file_from_hf(
+            official_model_name, file_name, **kwargs
+        )
+        dtype = kwargs.get("torch_dtype", None)
+        if dtype is not None:
+            state_dict = {k: v.to(dtype) for k, v in state_dict.items()}
+
         if cfg.original_architecture == "neel-solu-old":
             state_dict = convert_neel_solu_old_weights(state_dict, cfg)
+        elif cfg.original_architecture == "mingpt":
+            state_dict = convert_mingpt_weights(state_dict, cfg)
         return state_dict
     else:
         if cfg.from_checkpoint:
             if official_model_name.startswith("stanford-crfm"):
                 hf_model = AutoModelForCausalLM.from_pretrained(
-                    official_model_name, revision=f"checkpoint-{cfg.checkpoint_value}"
+                    official_model_name,
+                    revision=f"checkpoint-{cfg.checkpoint_value}",
+                    **kwargs,
                 )
             elif official_model_name.startswith("EleutherAI/pythia"):
                 hf_model = AutoModelForCausalLM.from_pretrained(
-                    official_model_name, revision=f"step{cfg.checkpoint_value}"
+                    official_model_name,
+                    revision=f"step{cfg.checkpoint_value}",
+                    **kwargs,
                 )
             else:
-                raise ValueError(f"Checkpoints for model {official_model_name} are not supported")
+                raise ValueError(
+                    f"Checkpoints for model {official_model_name} are not supported"
+                )
         elif hf_model is None:
             if "llama" in official_model_name:
                 raise NotImplementedError("Must pass in hf_model for LLaMA models")
-            else: 
-                hf_model = AutoModelForCausalLM.from_pretrained(official_model_name)
+            elif "bert" in official_model_name:
+                hf_model = BertForPreTraining.from_pretrained(
+                    official_model_name, **kwargs
+                )
+            else:
+                hf_model = AutoModelForCausalLM.from_pretrained(
+                    official_model_name, **kwargs
+                )
 
             # Load model weights, and fold in layer norm weights
+
+        for param in hf_model.parameters():
+            param.requires_grad = False
+
         if cfg.original_architecture == "GPT2LMHeadModel":
             state_dict = convert_gpt2_weights(hf_model, cfg)
         elif cfg.original_architecture == "GPTNeoForCausalLM":
             state_dict = convert_neo_weights(hf_model, cfg)
         elif cfg.original_architecture == "OPTForCausalLM":
             state_dict = convert_opt_weights(hf_model, cfg)
         elif cfg.original_architecture == "GPTJForCausalLM":
             state_dict = convert_gptj_weights(hf_model, cfg)
         elif cfg.original_architecture == "GPTNeoXForCausalLM":
             state_dict = convert_neox_weights(hf_model, cfg)
-        elif cfg.original_architecture == "LLaMAForCausalLM": 
+        elif cfg.original_architecture == "LLaMAForCausalLM":
             state_dict = convert_llama_weights(hf_model, cfg)
+        elif cfg.original_architecture == "BertForMaskedLM":
+            state_dict = convert_bert_weights(hf_model, cfg)
         else:
             raise ValueError(
                 f"Loading weights from the architecture is not currently supported: {cfg.original_architecture}, generated from model name {cfg.model_name}. Feel free to open an issue on GitHub to request this feature."
             )
 
         return state_dict
 
 
-# %%
-def convert_state_dict(
-    state_dict: dict,
-    cfg: HookedTransformerConfig,
-):
-    """Converts a state_dict from a HuggingFace model to a state_dict
-    compatible with HookedTransformer."""
-    official_model_name = get_official_model_name(official_model_name)
+def fill_missing_keys(model, state_dict):
+    """Takes in a state dict from a pretrained model, and fills in any missing keys with the default initialization.
 
-    if cfg["original_architecture"] == "gpt2":
-        return convert_gpt2_weights(state_dict, cfg)
-    elif cfg["original_architecture"] == "neo":
-        return convert_neo_weights(state_dict, cfg)
-    elif cfg["original_architecture"] == "gptj":
-        return convert_gptj_weights(state_dict, cfg)
-    elif cfg["original_architecture"] == "neox":
-        return convert_neox_weights(state_dict, cfg)
-    elif cfg["original_architecture"] == "opt":
-        return convert_opt_weights(state_dict, cfg)
-    elif cfg["original_architecture"] == "neel-solu-old":
-        return convert_neel_solu_old_weights(state_dict, cfg)
-    elif cfg["original_architecture"] == "neel":
-        return state_dict
-    else:
-        raise ValueError(f"Unknown architecture {cfg['original_architecture']}")
+    This function is assumed to be run before weights are initialized.
+
+    Args:
+        state_dict (dict): State dict from a pretrained model
+
+    Returns:
+        dict: State dict with missing keys filled in
+    """
+    # Get the default state dict
+    default_state_dict = model.state_dict()
+    # Get the keys that are missing from the pretrained model
+    missing_keys = set(default_state_dict.keys()) - set(state_dict.keys())
+    # Fill in the missing keys with the default initialization
+    for key in missing_keys:
+        if "hf_model" in key:
+            # Skip keys that are from the HuggingFace model, if loading from HF.
+            continue
+        if "W_" in key:
+            logging.warning(
+                "Missing key for a weight matrix in pretrained, filled in with an empty tensor: {}".format(
+                    key
+                )
+            )
+        state_dict[key] = default_state_dict[key]
+    return state_dict
 
 
 # Convert state dicts
 def convert_gpt2_weights(gpt2, cfg: HookedTransformerConfig):
     state_dict = {}
 
     state_dict["embed.W_E"] = gpt2.transformer.wte.weight
@@ -929,15 +1042,15 @@
         W_in = gpt2.transformer.h[l].mlp.c_fc.weight
         state_dict[f"blocks.{l}.mlp.W_in"] = W_in
         state_dict[f"blocks.{l}.mlp.b_in"] = gpt2.transformer.h[l].mlp.c_fc.bias
 
         W_out = gpt2.transformer.h[l].mlp.c_proj.weight
         state_dict[f"blocks.{l}.mlp.W_out"] = W_out
         state_dict[f"blocks.{l}.mlp.b_out"] = gpt2.transformer.h[l].mlp.c_proj.bias
-    state_dict[f"unembed.W_U"] = gpt2.lm_head.weight.T
+    state_dict["unembed.W_U"] = gpt2.lm_head.weight.T
 
     state_dict["ln_final.w"] = gpt2.transformer.ln_f.weight
     state_dict["ln_final.b"] = gpt2.transformer.ln_f.bias
     return state_dict
 
 
 def convert_neo_weights(neo, cfg: HookedTransformerConfig):
@@ -1097,24 +1210,24 @@
     state_dict["ln_final.w"] = neox.gpt_neox.final_layer_norm.weight
     state_dict["ln_final.b"] = neox.gpt_neox.final_layer_norm.bias
 
     state_dict["unembed.W_U"] = neox.embed_out.weight.T
     state_dict["unembed.b_U"] = torch.zeros(cfg.d_vocab)
     return state_dict
 
-def convert_llama_weights(llama, cfg: HookedTransformerConfig): 
+
+def convert_llama_weights(llama, cfg: HookedTransformerConfig):
     state_dict = {}
 
     state_dict["embed.W_E"] = llama.model.embed_tokens.weight
 
     # llama has no biases anywhere and deals with everything else roughly like
     # GPTNeoX with different names
-    
-    for l in range(cfg.n_layers):
 
+    for l in range(cfg.n_layers):
         state_dict[f"blocks.{l}.ln1.w"] = llama.model.layers[l].input_layernorm.weight
 
         W_Q = llama.model.layers[l].self_attn.q_proj.weight
         W_K = llama.model.layers[l].self_attn.k_proj.weight
         W_V = llama.model.layers[l].self_attn.v_proj.weight
         W_Q = einops.rearrange(W_Q, "(n h) m->n m h", n=cfg.n_heads)
         W_K = einops.rearrange(W_K, "(n h) m->n m h", n=cfg.n_heads)
@@ -1129,30 +1242,37 @@
 
         W_O = llama.model.layers[l].self_attn.o_proj.weight
         W_O = einops.rearrange(W_O, "m (n h)->n h m", n=cfg.n_heads)
         state_dict[f"blocks.{l}.attn.W_O"] = W_O
 
         state_dict[f"blocks.{l}.attn.b_O"] = torch.zeros(cfg.d_model)
 
-        state_dict[f"blocks.{l}.ln2.w"] = llama.model.layers[l].post_attention_layernorm.weight
+        state_dict[f"blocks.{l}.ln2.w"] = llama.model.layers[
+            l
+        ].post_attention_layernorm.weight
 
         state_dict[f"blocks.{l}.mlp.W_in"] = llama.model.layers[l].mlp.up_proj.weight.T
-        state_dict[f"blocks.{l}.mlp.W_gate"] = llama.model.layers[l].mlp.gate_proj.weight.T
+        state_dict[f"blocks.{l}.mlp.W_gate"] = llama.model.layers[
+            l
+        ].mlp.gate_proj.weight.T
         state_dict[f"blocks.{l}.mlp.b_in"] = torch.zeros(cfg.d_mlp)
 
-        state_dict[f"blocks.{l}.mlp.W_out"] = llama.model.layers[l].mlp.down_proj.weight.T
+        state_dict[f"blocks.{l}.mlp.W_out"] = llama.model.layers[
+            l
+        ].mlp.down_proj.weight.T
         state_dict[f"blocks.{l}.mlp.b_out"] = torch.zeros(cfg.d_model)
-    
+
     state_dict["ln_final.w"] = llama.model.norm.weight
 
     state_dict["unembed.W_U"] = llama.lm_head.weight.T
     state_dict["unembed.b_U"] = torch.zeros(cfg.d_vocab)
 
     return state_dict
 
+
 def convert_opt_weights(opt, cfg: HookedTransformerConfig):
     state_dict = {}
 
     state_dict["embed.W_E"] = opt.model.decoder.embed_tokens.weight
     state_dict["pos_embed.W_pos"] = opt.model.decoder.embed_positions.weight[2:, :]
 
     for l in range(cfg.n_layers):
@@ -1228,16 +1348,16 @@
         ].final_layer_norm.bias
 
         state_dict[f"blocks.{l}.mlp.W_in"] = opt.model.decoder.layers[l].fc1.weight.T
         state_dict[f"blocks.{l}.mlp.W_out"] = opt.model.decoder.layers[l].fc2.weight.T
 
         state_dict[f"blocks.{l}.mlp.b_in"] = opt.model.decoder.layers[l].fc1.bias
         state_dict[f"blocks.{l}.mlp.b_out"] = opt.model.decoder.layers[l].fc2.bias
-    state_dict[f"ln_final.w"] = opt.model.decoder.final_layer_norm.weight
-    state_dict[f"ln_final.b"] = opt.model.decoder.final_layer_norm.bias
+    state_dict["ln_final.w"] = opt.model.decoder.final_layer_norm.weight
+    state_dict["ln_final.b"] = opt.model.decoder.final_layer_norm.bias
     state_dict["unembed.W_U"] = opt.lm_head.weight.T
     state_dict["unembed.b_U"] = torch.zeros(cfg.d_vocab)
     return state_dict
 
 
 def convert_neel_solu_old_weights(state_dict: dict, cfg: HookedTransformerConfig):
     """
@@ -1271,8 +1391,169 @@
         new_state_dict["pos_embed.W_pos"] = new_state_dict["pos_embed.W_pos"].T
     if reverse_weights:
         for k, v in new_state_dict.items():
             if "W_" in k and "W_pos" not in k:
                 new_state_dict[k] = v.transpose(-2, -1)
     return new_state_dict
 
-# %%
+
+def convert_mingpt_weights(old_state_dict, cfg: HookedTransformerConfig):
+    # mingpt (https://github.com/karpathy/minGPT) is mostly similar to GPT-2,
+    # but doesn't concat the QKV matrices.
+    state_dict = {}
+
+    state_dict["embed.W_E"] = old_state_dict["tok_emb.weight"]
+    state_dict["pos_embed.W_pos"] = old_state_dict["pos_emb"].squeeze()
+
+    for l in range(cfg.n_layers):
+        state_dict[f"blocks.{l}.ln1.w"] = old_state_dict[f"blocks.{l}.ln1.weight"]
+        state_dict[f"blocks.{l}.ln1.b"] = old_state_dict[f"blocks.{l}.ln1.bias"]
+
+        W_Q = old_state_dict[f"blocks.{l}.attn.query.weight"]
+        W_K = old_state_dict[f"blocks.{l}.attn.key.weight"]
+        W_V = old_state_dict[f"blocks.{l}.attn.value.weight"]
+        W_Q = einops.rearrange(W_Q, "(i h) m->i m h", i=cfg.n_heads)
+        W_K = einops.rearrange(W_K, "(i h) m->i m h", i=cfg.n_heads)
+        W_V = einops.rearrange(W_V, "(i h) m->i m h", i=cfg.n_heads)
+        state_dict[f"blocks.{l}.attn.W_Q"] = W_Q
+        state_dict[f"blocks.{l}.attn.W_K"] = W_K
+        state_dict[f"blocks.{l}.attn.W_V"] = W_V
+
+        q_bias = einops.rearrange(
+            old_state_dict[f"blocks.{l}.attn.query.bias"], "(i h)->i h", i=cfg.n_heads
+        )
+        k_bias = einops.rearrange(
+            old_state_dict[f"blocks.{l}.attn.key.bias"], "(i h)->i h", i=cfg.n_heads
+        )
+        v_bias = einops.rearrange(
+            old_state_dict[f"blocks.{l}.attn.value.bias"], "(i h)->i h", i=cfg.n_heads
+        )
+
+        state_dict[f"blocks.{l}.attn.b_Q"] = q_bias
+        state_dict[f"blocks.{l}.attn.b_K"] = k_bias
+        state_dict[f"blocks.{l}.attn.b_V"] = v_bias
+
+        W_O = old_state_dict[f"blocks.{l}.attn.proj.weight"]
+        W_O = einops.rearrange(W_O, "m (i h)->i h m", i=cfg.n_heads)
+        state_dict[f"blocks.{l}.attn.W_O"] = W_O
+        state_dict[f"blocks.{l}.attn.b_O"] = old_state_dict[
+            f"blocks.{l}.attn.proj.bias"
+        ]
+
+        state_dict[f"blocks.{l}.ln2.w"] = old_state_dict[f"blocks.{l}.ln2.weight"]
+        state_dict[f"blocks.{l}.ln2.b"] = old_state_dict[f"blocks.{l}.ln2.bias"]
+
+        W_in = old_state_dict[f"blocks.{l}.mlp.0.weight"]
+        state_dict[f"blocks.{l}.mlp.W_in"] = W_in.T
+        state_dict[f"blocks.{l}.mlp.b_in"] = old_state_dict[f"blocks.{l}.mlp.0.bias"]
+
+        W_out = old_state_dict[f"blocks.{l}.mlp.2.weight"]
+        state_dict[f"blocks.{l}.mlp.W_out"] = W_out.T
+        state_dict[f"blocks.{l}.mlp.b_out"] = old_state_dict[f"blocks.{l}.mlp.2.bias"]
+
+    state_dict["unembed.W_U"] = old_state_dict["head.weight"].T
+
+    state_dict["ln_final.w"] = old_state_dict["ln_f.weight"]
+    state_dict["ln_final.b"] = old_state_dict["ln_f.bias"]
+
+    return state_dict
+
+
+def convert_bert_weights(bert, cfg: HookedTransformerConfig):
+    embeddings = bert.bert.embeddings
+    state_dict = {
+        "embed.embed.W_E": embeddings.word_embeddings.weight,
+        "embed.pos_embed.W_pos": embeddings.position_embeddings.weight,
+        "embed.token_type_embed.W_token_type": embeddings.token_type_embeddings.weight,
+        "embed.ln.w": embeddings.LayerNorm.weight,
+        "embed.ln.b": embeddings.LayerNorm.bias,
+    }
+
+    for l in range(cfg.n_layers):
+        block = bert.bert.encoder.layer[l]
+        state_dict[f"blocks.{l}.attn.W_Q"] = einops.rearrange(
+            block.attention.self.query.weight, "(i h) m -> i m h", i=cfg.n_heads
+        )
+        state_dict[f"blocks.{l}.attn.b_Q"] = einops.rearrange(
+            block.attention.self.query.bias, "(i h) -> i h", i=cfg.n_heads
+        )
+        state_dict[f"blocks.{l}.attn.W_K"] = einops.rearrange(
+            block.attention.self.key.weight, "(i h) m -> i m h", i=cfg.n_heads
+        )
+        state_dict[f"blocks.{l}.attn.b_K"] = einops.rearrange(
+            block.attention.self.key.bias, "(i h) -> i h", i=cfg.n_heads
+        )
+        state_dict[f"blocks.{l}.attn.W_V"] = einops.rearrange(
+            block.attention.self.value.weight, "(i h) m -> i m h", i=cfg.n_heads
+        )
+        state_dict[f"blocks.{l}.attn.b_V"] = einops.rearrange(
+            block.attention.self.value.bias, "(i h) -> i h", i=cfg.n_heads
+        )
+        state_dict[f"blocks.{l}.attn.W_O"] = einops.rearrange(
+            block.attention.output.dense.weight,
+            "m (i h) -> i h m",
+            i=cfg.n_heads,
+        )
+        state_dict[f"blocks.{l}.attn.b_O"] = block.attention.output.dense.bias
+        state_dict[f"blocks.{l}.ln1.w"] = block.attention.output.LayerNorm.weight
+        state_dict[f"blocks.{l}.ln1.b"] = block.attention.output.LayerNorm.bias
+        state_dict[f"blocks.{l}.mlp.W_in"] = einops.rearrange(
+            block.intermediate.dense.weight, "mlp model -> model mlp"
+        )
+        state_dict[f"blocks.{l}.mlp.b_in"] = block.intermediate.dense.bias
+        state_dict[f"blocks.{l}.mlp.W_out"] = einops.rearrange(
+            block.output.dense.weight, "model mlp -> mlp model"
+        )
+        state_dict[f"blocks.{l}.mlp.b_out"] = block.output.dense.bias
+        state_dict[f"blocks.{l}.ln2.w"] = block.output.LayerNorm.weight
+        state_dict[f"blocks.{l}.ln2.b"] = block.output.LayerNorm.bias
+
+    mlm_head = bert.cls.predictions
+    state_dict["mlm_head.W"] = mlm_head.transform.dense.weight
+    state_dict["mlm_head.b"] = mlm_head.transform.dense.bias
+    state_dict["mlm_head.ln.w"] = mlm_head.transform.LayerNorm.weight
+    state_dict["mlm_head.ln.b"] = mlm_head.transform.LayerNorm.bias
+    # Note: BERT uses tied embeddings
+    state_dict["unembed.W_U"] = embeddings.word_embeddings.weight.T
+    # "unembed.W_U": mlm_head.decoder.weight.T,
+    state_dict["unembed.b_U"] = mlm_head.bias
+
+    return state_dict
+
+
+@dataclasses.dataclass
+class Config:
+    d_model: int = 768
+    debug: bool = True
+    layer_norm_eps: float = 1e-5
+    d_vocab: int = 50257
+    init_range: float = 0.02
+    n_ctx: int = 1024
+    d_head: int = 64
+    d_mlp: int = 3072
+    n_heads: int = 12
+    n_layers: int = 12
+
+
+# Returns the configuration parameters of the model as a basic Config dataclass
+def get_basic_config(model_name: str, **kwargs) -> Config:
+    return Config(
+        **{
+            k: v
+            for k, v in get_pretrained_model_config(model_name, **kwargs)
+            .to_dict()
+            .items()
+            if k
+            in [
+                "d_model",
+                "debug",
+                "layer_norm_eps",
+                "d_vocab",
+                "init_range",
+                "n_ctx",
+                "d_head",
+                "d_mlp",
+                "n_heads",
+                "n_layers",
+            ]
+        }
+    )
```

### Comparing `transformer_lens-1.2.2/transformer_lens/make_docs.py` & `transformer_lens-1.3.0/transformer_lens/make_docs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 # %%
-from easy_transformer import loading
-from easy_transformer import utils
 from functools import lru_cache
+
+from easy_transformer import loading
+
 # %%
 # cfg = (loading.get_pretrained_model_config("solu-1l"))
 # print(cfg)
 # %%
 """ 
 Structure:
 d_model, d_mlp, d_head, d_vocab, act_fn, n_heads, n_layers, n_ctx, n_params, 
 Make an architecture table separately probs
 tokenizer_name, training_data, has checkpoints
 act_fn includes attn_only
 architecture
 Architecture should list weird shit to be aware of.
 """
 import pandas as pd
-import numpy as np
+
+
 # df = pd.DataFrame(np.random.randn(2, 2))
 # print(df.to_markdown(open("test.md", "w")))
 # %%
 @lru_cache(maxsize=None)
 def get_config(model_name):
     return loading.get_pretrained_model_config(model_name)
 
+
 def get_property(name, model_name):
     cfg = get_config(model_name)
-    if name=="act_fn":
+    if name == "act_fn":
         if cfg.attn_only:
             return "attn_only"
-        elif cfg.act_fn=="gelu_new":
+        elif cfg.act_fn == "gelu_new":
             return "gelu"
-        elif cfg.act_fn=="gelu_fast":
+        elif cfg.act_fn == "gelu_fast":
             return "gelu"
-        elif cfg.act_fn=="solu_ln":
+        elif cfg.act_fn == "solu_ln":
             return "solu"
         else:
             return cfg.act_fn
-    if name=="n_params":
+    if name == "n_params":
         n_params = cfg.n_params
         if n_params < 1e4:
             return f"{n_params/1e3:.1f}K"
         elif n_params < 1e6:
             return f"{round(n_params/1e3)}K"
         elif n_params < 1e7:
             return f"{n_params/1e6:.1f}M"
@@ -54,12 +57,21 @@
         else:
             raise ValueError(f"Passed in {n_params} above 1T?")
     else:
         return cfg.to_dict()[name]
 
 
 if __name__ == "__main__":
-    column_names = "n_params, n_layers, d_model, n_heads, act_fn, n_ctx, d_vocab, d_head, d_mlp".split(", ")
-    df = pd.DataFrame({name:[get_property(name, model_name) for model_name in loading.DEFAULT_MODEL_ALIASES] for name in column_names}, index=loading.DEFAULT_MODEL_ALIASES)
-    df.to_markdown(
-        open("model_properties_table.md", "w"))
-
+    column_names = "n_params, n_layers, d_model, n_heads, act_fn, n_ctx, d_vocab, d_head, d_mlp".split(
+        ", "
+    )
+    df = pd.DataFrame(
+        {
+            name: [
+                get_property(name, model_name)
+                for model_name in loading.DEFAULT_MODEL_ALIASES
+            ]
+            for name in column_names
+        },
+        index=loading.DEFAULT_MODEL_ALIASES,
+    )
+    df.to_markdown(open("model_properties_table.md", "w"))
```

### Comparing `transformer_lens-1.2.2/transformer_lens/model_properties_table.md` & `transformer_lens-1.3.0/transformer_lens/model_properties_table.md`

 * *Files identical despite different names*

### Comparing `transformer_lens-1.2.2/transformer_lens/past_key_value_caching.py` & `transformer_lens-1.3.0/transformer_lens/past_key_value_caching.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-import torch
 from dataclasses import dataclass
 from typing import List
+
+import torch
+from jaxtyping import Float
+
 from transformer_lens.HookedTransformerConfig import HookedTransformerConfig
 from transformer_lens.utilities.devices import get_device_for_block_index
-from jaxtyping import Float
 
 
 @dataclass
 class HookedTransformerKeyValueCacheEntry:
     past_keys: Float[torch.Tensor, "batch pos_so_far n_heads d_head"]
     past_values: Float[torch.Tensor, "batch pos_so_far n_heads d_head"]
```

### Comparing `transformer_lens-1.2.2/transformer_lens/patching.py` & `transformer_lens-1.3.0/transformer_lens/patching.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,91 +1,102 @@
-
 # %%
 """
 A module for patching activations in a transformer model, and measuring the effect of the patch on the output.
 This implements the activation patching technique for a range of types of activation. 
 The structure is to have a single generic_activation_patch function that does everything, and to have a range of specialised functions for specific types of activation.
 
 See this explanation for more https://dynalist.io/d/n2ZWtnoYHrU1s4vnFSAQ519J#z=qeWBvs-R-taFfcCq-S_hgMqx
 And check out the Activation Patching in TransformerLens Demo notebook for a demo of how to use this module.
 """
 
 from __future__ import annotations
-import torch
-from typing import Optional, Union, Dict, Callable, Sequence, Optional, Tuple
-from typing_extensions import Literal
 
-from transformer_lens import HookedTransformer, ActivationCache
-import transformer_lens.utils as utils
-import pandas as pd
 import itertools
 from functools import partial
-from tqdm.auto import tqdm
-from jaxtyping import Float, Int 
+from typing import Callable, Optional, Sequence, Tuple, Union
 
 import einops
+import pandas as pd
+import torch
+from jaxtyping import Float, Int
+from tqdm.auto import tqdm
+from typing_extensions import Literal
+
+import transformer_lens.utils as utils
+from transformer_lens import ActivationCache, HookedTransformer
 
 # %%
 Logits = torch.Tensor
 AxisNames = Literal["layer", "pos", "head_index", "head", "src_pos", "dest_pos"]
 
 
 # %%
 from typing import Sequence
-def make_df_from_ranges(column_max_ranges: Sequence[int], column_names: Sequence[str]) -> pd.DataFrame:
+
+
+def make_df_from_ranges(
+    column_max_ranges: Sequence[int], column_names: Sequence[str]
+) -> pd.DataFrame:
     """
     Takes in a list of column names and max ranges for each column, and returns a dataframe with the cartesian product of the range for each column (ie iterating through all combinations from zero to column_max_range - 1, in order, incrementing the final column first)
     """
-    rows = list(itertools.product(*[
-        range(axis_max_range) for axis_max_range in column_max_ranges
-    ]))
+    rows = list(
+        itertools.product(
+            *[range(axis_max_range) for axis_max_range in column_max_ranges]
+        )
+    )
     df = pd.DataFrame(rows, columns=column_names)
     return df
 
 
 # %%
 CorruptedActivation = torch.Tensor
 PatchedActivation = torch.Tensor
 
+
 def generic_activation_patch(
     model: HookedTransformer,
     corrupted_tokens: Int[torch.Tensor, "batch pos"],
     clean_cache: ActivationCache,
-    patching_metric: Callable[[Float[torch.Tensor, "batch pos d_vocab"]], Float[torch.Tensor, ""]],
-    patch_setter: Callable[[CorruptedActivation, Sequence[int], ActivationCache], PatchedActivation],
+    patching_metric: Callable[
+        [Float[torch.Tensor, "batch pos d_vocab"]], Float[torch.Tensor, ""]
+    ],
+    patch_setter: Callable[
+        [CorruptedActivation, Sequence[int], ActivationCache], PatchedActivation
+    ],
     activation_name: str,
     index_axis_names: Optional[Sequence[AxisNames]] = None,
     index_df: Optional[pd.DataFrame] = None,
     return_index_df: bool = False,
 ) -> Union[torch.Tensor, Tuple[torch.Tensor, pd.DataFrame]]:
     """
     A generic function to do activation patching, will be specialised to specific use cases.
 
     Activation patching is about studying the counterfactual effect of a specific activation between a clean run and a corrupted run. The idea is have two inputs, clean and corrupted, which have two different outputs, and differ in some key detail. Eg "The Eiffel Tower is in" vs "The Colosseum is in". Then to take a cached set of activations from the "clean" run, and a set of corrupted.
 
     Internally, the key function comes from three things: A list of tuples of indices (eg (layer, position, head_index)), a index_to_act_name function which identifies the right activation for each index, a patch_setter function which takes the corrupted activation, the index and the clean cache, and a metric for how well the patched model has recovered.
-    
+
     The indices can either be given explicitly as a pandas dataframe, or by listing the relevant axis names and having them inferred from the tokens and the model config. It is assumed that the first column is always layer.
 
-    This function then iterates over every tuple of indices, does the relevant patch, and stores it 
+    This function then iterates over every tuple of indices, does the relevant patch, and stores it
 
-    Params
-    model: The relevant model
-    corrupted_tokens: The input tokens for the corrupted run
-    clean_cache: The cached activations from the clean run
-    patching_metric: A function from the model's output logits to some metric (eg loss, logit diff, etc)
-    patch_setter: A function which acts on (corrupted_activation, index, clean_cache) to edit the activation and patch in the relevant chunk of the clean activation
-    activation_name: The name of the activation being patched
-    index_axis_names: The names of the axes to (fully) iterate over, implicitly fills in index_df
-    index_df: The dataframe of indices, columns are axis names and each row is a tuple of indices. Will be inferred from index_axis_names if not given. When this is input, the output will be a flattened tensor with an element per row of index_df
-    return_index_df: A Boolean flag for whether to return the dataframe of indices too
-
-    Returns
-    patched_output: The tensor of the patching metric for each patch. By default it has one dimension for each index dimension, via index_df set explicitly it is flattened with one element per row.
-    index_df *optional*: The dataframe of indices
+    Args:
+        model: The relevant model
+        corrupted_tokens: The input tokens for the corrupted run
+        clean_cache: The cached activations from the clean run
+        patching_metric: A function from the model's output logits to some metric (eg loss, logit diff, etc)
+        patch_setter: A function which acts on (corrupted_activation, index, clean_cache) to edit the activation and patch in the relevant chunk of the clean activation
+        activation_name: The name of the activation being patched
+        index_axis_names: The names of the axes to (fully) iterate over, implicitly fills in index_df
+        index_df: The dataframe of indices, columns are axis names and each row is a tuple of indices. Will be inferred from index_axis_names if not given. When this is input, the output will be a flattened tensor with an element per row of index_df
+        return_index_df: A Boolean flag for whether to return the dataframe of indices too
+
+    Returns:
+        patched_output: The tensor of the patching metric for each patch. By default it has one dimension for each index dimension, via index_df set explicitly it is flattened with one element per row.
+        index_df *optional*: The dataframe of indices
     """
 
     if index_df is None:
         assert index_axis_names is not None
 
         # Get the max range for all possible axes
         max_axis_range = {
@@ -94,15 +105,17 @@
             "head_index": model.cfg.n_heads,
         }
         max_axis_range["src_pos"] = max_axis_range["pos"]
         max_axis_range["dest_pos"] = max_axis_range["pos"]
         max_axis_range["head"] = max_axis_range["head_index"]
 
         # Get the max range for each axis we iterate over
-        index_axis_max_range = [max_axis_range[axis_name] for axis_name in index_axis_names]
+        index_axis_max_range = [
+            max_axis_range[axis_name] for axis_name in index_axis_names
+        ]
 
         # Get the dataframe where each row is a tuple of indices
         index_df = make_df_from_ranges(index_axis_max_range, index_axis_names)
 
         flattened_output = False
     else:
         # A dataframe of indices was provided. Verify that we did not *also* receive index_axis_names
@@ -111,15 +124,17 @@
 
         flattened_output = True
 
     # Create an empty tensor to show the patched metric for each patch
     if flattened_output:
         patched_metric_output = torch.zeros(len(index_df), device=model.cfg.device)
     else:
-        patched_metric_output = torch.zeros(index_axis_max_range, device=model.cfg.device)
+        patched_metric_output = torch.zeros(
+            index_axis_max_range, device=model.cfg.device
+        )
 
     # A generic patching hook - for each index, it applies the patch_setter appropriately to patch the activation
     def patching_hook(corrupted_activation, hook, index, clean_activation):
         return patch_setter(corrupted_activation, index, clean_activation)
 
     # Iterate over every list of indices, and make the appropriate patch!
     for c, index_row in enumerate(tqdm((list(index_df.iterrows())))):
@@ -127,135 +142,144 @@
 
         # The current activation name is just the activation name plus the layer (assumed to be the first element of the input)
         current_activation_name = utils.get_act_name(activation_name, layer=index[0])
 
         # The hook function cannot receive additional inputs, so we use partial to include the specific index and the corresponding clean activation
         current_hook = partial(
             patching_hook,
-            index = index,
-            clean_activation = clean_cache[current_activation_name]
-        )                 
+            index=index,
+            clean_activation=clean_cache[current_activation_name],
+        )
 
         # Run the model with the patching hook and get the logits!
-        patched_logits = model.run_with_hooks(corrupted_tokens, fwd_hooks=[(current_activation_name, current_hook)])
+        patched_logits = model.run_with_hooks(
+            corrupted_tokens, fwd_hooks=[(current_activation_name, current_hook)]
+        )
 
         # Calculate the patching metric and store
         if flattened_output:
             patched_metric_output[c] = patching_metric(patched_logits).item()
         else:
             patched_metric_output[tuple(index)] = patching_metric(patched_logits).item()
-    
+
     if return_index_df:
         return patched_metric_output, index_df
     else:
         return patched_metric_output
 
+
 # %%
 # Defining patch setters for various shapes of activations
-def layer_pos_patch_setter(
-    corrupted_activation, 
-    index, 
-    clean_activation
-    ):
+def layer_pos_patch_setter(corrupted_activation, index, clean_activation):
     """
     Applies the activation patch where index = [layer, pos]
 
-    Impliitly assumes that the activation axis order is [batch, pos, ...], which is true of everything that is not an attention pattern shaped tensor.
+    Implicitly assumes that the activation axis order is [batch, pos, ...], which is true of everything that is not an attention pattern shaped tensor.
     """
-    assert len(index)==2
+    assert len(index) == 2
     layer, pos = index
     corrupted_activation[:, pos, ...] = clean_activation[:, pos, ...]
     return corrupted_activation
 
+
 def layer_pos_head_vector_patch_setter(
-    corrupted_activation, 
-    index, 
+    corrupted_activation,
+    index,
     clean_activation,
 ):
     """
     Applies the activation patch where index = [layer, pos, head_index]
 
-    Impliitly assumes that the activation axis order is [batch, pos, head_index, ...], which is true of all attention head vector activations (q, k, v, z, result) but *not* of attention patterns.
+    Implicitly assumes that the activation axis order is [batch, pos, head_index, ...], which is true of all attention head vector activations (q, k, v, z, result) but *not* of attention patterns.
     """
-    assert len(index)==3
+    assert len(index) == 3
     layer, pos, head_index = index
     corrupted_activation[:, pos, head_index] = clean_activation[:, pos, head_index]
     return corrupted_activation
 
+
 def layer_head_vector_patch_setter(
-    corrupted_activation, 
-    index, 
+    corrupted_activation,
+    index,
     clean_activation,
 ):
     """
     Applies the activation patch where index = [layer,  head_index]
 
-    Impliitly assumes that the activation axis order is [batch, pos, head_index, ...], which is true of all attention head vector activations (q, k, v, z, result) but *not* of attention patterns.
+    Implicitly assumes that the activation axis order is [batch, pos, head_index, ...], which is true of all attention head vector activations (q, k, v, z, result) but *not* of attention patterns.
     """
-    assert len(index)==2
+    assert len(index) == 2
     layer, head_index = index
     corrupted_activation[:, :, head_index] = clean_activation[:, :, head_index]
-    
+
     return corrupted_activation
 
+
 def layer_head_pattern_patch_setter(
-    corrupted_activation, 
-    index, 
+    corrupted_activation,
+    index,
     clean_activation,
 ):
     """
     Applies the activation patch where index = [layer,  head_index]
 
-    Impliitly assumes that the activation axis order is [batch, head_index, dest_pos, src_pos], which is true of attention scores and patterns.
+    Implicitly assumes that the activation axis order is [batch, head_index, dest_pos, src_pos], which is true of attention scores and patterns.
     """
-    assert len(index)==2
+    assert len(index) == 2
     layer, head_index = index
     corrupted_activation[:, head_index, :, :] = clean_activation[:, head_index, :, :]
-    
+
     return corrupted_activation
 
+
 def layer_head_pos_pattern_patch_setter(
-    corrupted_activation, 
-    index, 
+    corrupted_activation,
+    index,
     clean_activation,
 ):
     """
     Applies the activation patch where index = [layer,  head_index, dest_pos]
 
-    Impliitly assumes that the activation axis order is [batch, head_index, dest_pos, src_pos], which is true of attention scores and patterns.
+    Implicitly assumes that the activation axis order is [batch, head_index, dest_pos, src_pos], which is true of attention scores and patterns.
     """
-    assert len(index)==3
+    assert len(index) == 3
     layer, head_index, dest_pos = index
-    corrupted_activation[:, head_index, dest_pos, :] = clean_activation[:, head_index, dest_pos, :]
-    
+    corrupted_activation[:, head_index, dest_pos, :] = clean_activation[
+        :, head_index, dest_pos, :
+    ]
+
     return corrupted_activation
 
+
 def layer_head_dest_src_pos_pattern_patch_setter(
-    corrupted_activation, 
-    index, 
+    corrupted_activation,
+    index,
     clean_activation,
 ):
     """
     Applies the activation patch where index = [layer,  head_index, dest_pos, src_pos]
 
-    Impliitly assumes that the activation axis order is [batch, head_index, dest_pos, src_pos], which is true of attention scores and patterns.
+    Implicitly assumes that the activation axis order is [batch, head_index, dest_pos, src_pos], which is true of attention scores and patterns.
     """
-    assert len(index)==4
+    assert len(index) == 4
     layer, head_index, dest_pos, src_pos = index
-    corrupted_activation[:, head_index, dest_pos, src_pos] = clean_activation[:, head_index, dest_pos, src_pos]
-    
+    corrupted_activation[:, head_index, dest_pos, src_pos] = clean_activation[
+        :, head_index, dest_pos, src_pos
+    ]
+
     return corrupted_activation
 
+
 # %%
 # Defining activation patching functions for a range of common activation patches.
 get_act_patch_resid_pre = partial(
     generic_activation_patch,
-    patch_setter = layer_pos_patch_setter,
-    activation_name = "resid_pre",
-    index_axis_names = ("layer", "pos")
+    patch_setter=layer_pos_patch_setter,
+    activation_name="resid_pre",
+    index_axis_names=("layer", "pos"),
 )
 get_act_patch_resid_pre.__doc__ = """
     Function to get activation patching results for the residual stream (at the start of each block) (by position). Returns a tensor of shape [n_layers, pos]
 
     See generic_activation_patch for a more detailed explanation of activation patching 
 
     Args:
@@ -266,23 +290,38 @@
 
     Returns:
         patched_output (torch.Tensor): The tensor of the patching metric for each resid_pre patch. Has shape [n_layers, pos]
     """
 
 get_act_patch_resid_mid = partial(
     generic_activation_patch,
-    patch_setter = layer_pos_patch_setter,
-    activation_name = "resid_mid",
-    index_axis_names = ("layer", "pos")
+    patch_setter=layer_pos_patch_setter,
+    activation_name="resid_mid",
+    index_axis_names=("layer", "pos"),
 )
+get_act_patch_resid_mid.__doc__ = """
+    Function to get activation patching results for the residual stream (between the attn and MLP layer of each block) (by position). Returns a tensor of shape [n_layers, pos]
+
+    See generic_activation_patch for a more detailed explanation of activation patching 
+
+    Args:
+        model: The relevant model
+        corrupted_tokens (torch.Tensor): The input tokens for the corrupted run. Has shape [batch, pos]
+        clean_cache (ActivationCache): The cached activations from the clean run
+        patching_metric: A function from the model's output logits to some metric (eg loss, logit diff, etc)
+
+    Returns:
+        patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [n_layers, pos]
+    """
+
 get_act_patch_attn_out = partial(
     generic_activation_patch,
-    patch_setter = layer_pos_patch_setter,
-    activation_name = "attn_out",
-    index_axis_names = ("layer", "pos")
+    patch_setter=layer_pos_patch_setter,
+    activation_name="attn_out",
+    index_axis_names=("layer", "pos"),
 )
 get_act_patch_attn_out.__doc__ = """
     Function to get activation patching results for the output of each Attention layer (by position). Returns a tensor of shape [n_layers, pos]
 
     See generic_activation_patch for a more detailed explanation of activation patching 
 
     Args:
@@ -293,17 +332,17 @@
 
     Returns:
         patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [n_layers, pos]
     """
 
 get_act_patch_mlp_out = partial(
     generic_activation_patch,
-    patch_setter = layer_pos_patch_setter,
-    activation_name = "mlp_out",
-    index_axis_names = ("layer", "pos")
+    patch_setter=layer_pos_patch_setter,
+    activation_name="mlp_out",
+    index_axis_names=("layer", "pos"),
 )
 get_act_patch_mlp_out.__doc__ = """
     Function to get activation patching results for the output of each MLP layer (by position). Returns a tensor of shape [n_layers, pos]
 
     See generic_activation_patch for a more detailed explanation of activation patching 
 
     Args:
@@ -314,56 +353,144 @@
 
     Returns:
         patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [n_layers, pos]
     """
 # %%
 get_act_patch_attn_head_out_by_pos = partial(
     generic_activation_patch,
-    patch_setter = layer_pos_head_vector_patch_setter,
-    activation_name = "z",
-    index_axis_names = ("layer", "pos", "head")
+    patch_setter=layer_pos_head_vector_patch_setter,
+    activation_name="z",
+    index_axis_names=("layer", "pos", "head"),
 )
+get_act_patch_attn_head_out_by_pos.__doc__ = """
+    Function to get activation patching results for the output of each Attention Head (by position). Returns a tensor of shape [n_layers, pos, n_heads]
+
+    See generic_activation_patch for a more detailed explanation of activation patching 
+
+    Args:
+        model: The relevant model
+        corrupted_tokens (torch.Tensor): The input tokens for the corrupted run. Has shape [batch, pos]
+        clean_cache (ActivationCache): The cached activations from the clean run
+        patching_metric: A function from the model's output logits to some metric (eg loss, logit diff, etc)
+
+    Returns:
+        patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [n_layers, pos, n_heads]
+    """
+
 get_act_patch_attn_head_q_by_pos = partial(
     generic_activation_patch,
-    patch_setter = layer_pos_head_vector_patch_setter,
-    activation_name = "q",
-    index_axis_names = ("layer", "pos", "head")
+    patch_setter=layer_pos_head_vector_patch_setter,
+    activation_name="q",
+    index_axis_names=("layer", "pos", "head"),
 )
+get_act_patch_attn_head_q_by_pos.__doc__ = """
+    Function to get activation patching results for the queries of each Attention Head (by position). Returns a tensor of shape [n_layers, pos, n_heads]
+
+    See generic_activation_patch for a more detailed explanation of activation patching 
+
+    Args:
+        model: The relevant model
+        corrupted_tokens (torch.Tensor): The input tokens for the corrupted run. Has shape [batch, pos]
+        clean_cache (ActivationCache): The cached activations from the clean run
+        patching_metric: A function from the model's output logits to some metric (eg loss, logit diff, etc)
+
+    Returns:
+        patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [n_layers, pos, n_heads]
+    """
+
 get_act_patch_attn_head_k_by_pos = partial(
     generic_activation_patch,
-    patch_setter = layer_pos_head_vector_patch_setter,
-    activation_name = "k",
-    index_axis_names = ("layer", "pos", "head")
+    patch_setter=layer_pos_head_vector_patch_setter,
+    activation_name="k",
+    index_axis_names=("layer", "pos", "head"),
 )
+get_act_patch_attn_head_k_by_pos.__doc__ = """
+    Function to get activation patching results for the keys of each Attention Head (by position). Returns a tensor of shape [n_layers, pos, n_heads]
+
+    See generic_activation_patch for a more detailed explanation of activation patching 
+
+    Args:
+        model: The relevant model
+        corrupted_tokens (torch.Tensor): The input tokens for the corrupted run. Has shape [batch, pos]
+        clean_cache (ActivationCache): The cached activations from the clean run
+        patching_metric: A function from the model's output logits to some metric (eg loss, logit diff, etc)
+
+    Returns:
+        patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [n_layers, pos, n_heads]
+    """
+
 get_act_patch_attn_head_v_by_pos = partial(
     generic_activation_patch,
-    patch_setter = layer_pos_head_vector_patch_setter,
-    activation_name = "v",
-    index_axis_names = ("layer", "pos", "head")
+    patch_setter=layer_pos_head_vector_patch_setter,
+    activation_name="v",
+    index_axis_names=("layer", "pos", "head"),
 )
+get_act_patch_attn_head_v_by_pos.__doc__ = """
+    Function to get activation patching results for the values of each Attention Head (by position). Returns a tensor of shape [n_layers, pos, n_heads]
+
+    See generic_activation_patch for a more detailed explanation of activation patching 
+
+    Args:
+        model: The relevant model
+        corrupted_tokens (torch.Tensor): The input tokens for the corrupted run. Has shape [batch, pos]
+        clean_cache (ActivationCache): The cached activations from the clean run
+        patching_metric: A function from the model's output logits to some metric (eg loss, logit diff, etc)
+
+    Returns:
+        patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [n_layers, pos, n_heads]
+    """
 # %%
 get_act_patch_attn_head_pattern_by_pos = partial(
     generic_activation_patch,
-    patch_setter = layer_head_pos_pattern_patch_setter,
-    activation_name = "pattern",
-    index_axis_names = ("layer", "head_index", "dest_pos")
+    patch_setter=layer_head_pos_pattern_patch_setter,
+    activation_name="pattern",
+    index_axis_names=("layer", "head_index", "dest_pos"),
 )
+get_act_patch_attn_head_pattern_by_pos.__doc__ = """
+    Function to get activation patching results for the attention pattern of each Attention Head (by destination position). Returns a tensor of shape [n_layers, n_heads, dest_pos]
+
+    See generic_activation_patch for a more detailed explanation of activation patching 
+
+    Args:
+        model: The relevant model
+        corrupted_tokens (torch.Tensor): The input tokens for the corrupted run. Has shape [batch, pos]
+        clean_cache (ActivationCache): The cached activations from the clean run
+        patching_metric: A function from the model's output logits to some metric (eg loss, logit diff, etc)
+
+    Returns:
+        patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [n_layers, n_heads, dest_pos]
+    """
+
 get_act_patch_attn_head_pattern_dest_src_pos = partial(
     generic_activation_patch,
-    patch_setter = layer_head_dest_src_pos_pattern_patch_setter,
-    activation_name = "pattern",
-    index_axis_names = ("layer", "head_index", "dest_pos", "src_pos")
+    patch_setter=layer_head_dest_src_pos_pattern_patch_setter,
+    activation_name="pattern",
+    index_axis_names=("layer", "head_index", "dest_pos", "src_pos"),
 )
+get_act_patch_attn_head_pattern_dest_src_pos.__doc__ = """
+    Function to get activation patching results for each destination, source entry of the attention pattern for each Attention Head. Returns a tensor of shape [n_layers, n_heads, dest_pos, src_pos]
+
+    See generic_activation_patch for a more detailed explanation of activation patching 
+
+    Args:
+        model: The relevant model
+        corrupted_tokens (torch.Tensor): The input tokens for the corrupted run. Has shape [batch, pos]
+        clean_cache (ActivationCache): The cached activations from the clean run
+        patching_metric: A function from the model's output logits to some metric (eg loss, logit diff, etc)
+
+    Returns:
+        patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [n_layers, n_heads, dest_pos, src_pos]
+    """
 
 # %%
 get_act_patch_attn_head_out_all_pos = partial(
     generic_activation_patch,
-    patch_setter = layer_head_vector_patch_setter,
-    activation_name = "z",
-    index_axis_names = ("layer", "head")
+    patch_setter=layer_head_vector_patch_setter,
+    activation_name="z",
+    index_axis_names=("layer", "head"),
 )
 get_act_patch_attn_head_out_all_pos.__doc__ = """
     Function to get activation patching results for the outputs of each Attention Head (across all positions). Returns a tensor of shape [n_layers, n_heads]
 
     See generic_activation_patch for a more detailed explanation of activation patching 
 
     Args:
@@ -374,17 +501,17 @@
 
     Returns:
         patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [n_layers, n_heads]
     """
 
 get_act_patch_attn_head_q_all_pos = partial(
     generic_activation_patch,
-    patch_setter = layer_head_vector_patch_setter,
-    activation_name = "q",
-    index_axis_names = ("layer", "head")
+    patch_setter=layer_head_vector_patch_setter,
+    activation_name="q",
+    index_axis_names=("layer", "head"),
 )
 get_act_patch_attn_head_q_all_pos.__doc__ = """
     Function to get activation patching results for the queries of each Attention Head (across all positions). Returns a tensor of shape [n_layers, n_heads]
 
     See generic_activation_patch for a more detailed explanation of activation patching 
 
     Args:
@@ -395,17 +522,17 @@
 
     Returns:
         patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [n_layers, n_heads]
     """
 
 get_act_patch_attn_head_k_all_pos = partial(
     generic_activation_patch,
-    patch_setter = layer_head_vector_patch_setter,
-    activation_name = "k",
-    index_axis_names = ("layer", "head")
+    patch_setter=layer_head_vector_patch_setter,
+    activation_name="k",
+    index_axis_names=("layer", "head"),
 )
 get_act_patch_attn_head_k_all_pos.__doc__ = """
     Function to get activation patching results for the keys of each Attention Head (across all positions). Returns a tensor of shape [n_layers, n_heads]
 
     See generic_activation_patch for a more detailed explanation of activation patching 
 
     Args:
@@ -416,17 +543,17 @@
 
     Returns:
         patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [n_layers, n_heads]
     """
 
 get_act_patch_attn_head_v_all_pos = partial(
     generic_activation_patch,
-    patch_setter = layer_head_vector_patch_setter,
-    activation_name = "v",
-    index_axis_names = ("layer", "head")
+    patch_setter=layer_head_vector_patch_setter,
+    activation_name="v",
+    index_axis_names=("layer", "head"),
 )
 get_act_patch_attn_head_v_all_pos.__doc__ = """
     Function to get activation patching results for the values of each Attention Head (across all positions). Returns a tensor of shape [n_layers, n_heads]
 
     See generic_activation_patch for a more detailed explanation of activation patching 
 
     Args:
@@ -437,17 +564,17 @@
 
     Returns:
         patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [n_layers, n_heads]
     """
 
 get_act_patch_attn_head_pattern_all_pos = partial(
     generic_activation_patch,
-    patch_setter = layer_head_pattern_patch_setter,
-    activation_name = "pattern",
-    index_axis_names = ("layer", "head_index")
+    patch_setter=layer_head_pattern_patch_setter,
+    activation_name="pattern",
+    index_axis_names=("layer", "head_index"),
 )
 get_act_patch_attn_head_pattern_all_pos.__doc__ = """
     Function to get activation patching results for the attention pattern of each Attention Head (across all positions). Returns a tensor of shape [n_layers, n_heads]
 
     See generic_activation_patch for a more detailed explanation of activation patching 
 
     Args:
@@ -458,58 +585,108 @@
 
     Returns:
         patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [n_layers, n_heads]
     """
 
 # %%
 
-def get_act_patch_attn_head_all_pos_every(model, corrupted_tokens, clean_cache, metric) -> Float[torch.Tensor, "patch_type layer head"]:
+
+def get_act_patch_attn_head_all_pos_every(
+    model, corrupted_tokens, clean_cache, metric
+) -> Float[torch.Tensor, "patch_type layer head"]:
     """Helper function to get activation patching results for every head (across all positions) for every act type (output, query, key, value, pattern). Wrapper around each's patching function, returns a stacked tensor of shape [5, n_layers, n_heads]
 
     Args:
         model: The relevant model
         corrupted_tokens (torch.Tensor): The input tokens for the corrupted run. Has shape [batch, pos]
         clean_cache (ActivationCache): The cached activations from the clean run
         metric: A function from the model's output logits to some metric (eg loss, logit diff, etc)
 
     Returns:
         patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [5, n_layers, n_heads]
     """
     act_patch_results = []
-    act_patch_results.append(get_act_patch_attn_head_out_all_pos(model, corrupted_tokens, clean_cache, metric))
-    act_patch_results.append(get_act_patch_attn_head_q_all_pos(model, corrupted_tokens, clean_cache, metric))
-    act_patch_results.append(get_act_patch_attn_head_k_all_pos(model, corrupted_tokens, clean_cache, metric))
-    act_patch_results.append(get_act_patch_attn_head_v_all_pos(model, corrupted_tokens, clean_cache, metric))
-    act_patch_results.append(get_act_patch_attn_head_pattern_all_pos(model, corrupted_tokens, clean_cache, metric))
+    act_patch_results.append(
+        get_act_patch_attn_head_out_all_pos(
+            model, corrupted_tokens, clean_cache, metric
+        )
+    )
+    act_patch_results.append(
+        get_act_patch_attn_head_q_all_pos(model, corrupted_tokens, clean_cache, metric)
+    )
+    act_patch_results.append(
+        get_act_patch_attn_head_k_all_pos(model, corrupted_tokens, clean_cache, metric)
+    )
+    act_patch_results.append(
+        get_act_patch_attn_head_v_all_pos(model, corrupted_tokens, clean_cache, metric)
+    )
+    act_patch_results.append(
+        get_act_patch_attn_head_pattern_all_pos(
+            model, corrupted_tokens, clean_cache, metric
+        )
+    )
     return torch.stack(act_patch_results, dim=0)
 
-def get_act_patch_attn_head_by_pos_every(model, corrupted_tokens, clean_cache, metric) -> Float[torch.Tensor, "patch_type layer pos head"]:
-    """Helper function to get activation patching results for every head (across all positions) for every act type (output, query, key, value, pattern). Wrapper around each's patching function, returns a stacked tensor of shape [5, n_layers, pos, n_heads]
+
+def get_act_patch_attn_head_by_pos_every(
+    model, corrupted_tokens, clean_cache, metric
+) -> Float[torch.Tensor, "patch_type layer pos head"]:
+    """Helper function to get activation patching results for every head (by position) for every act type (output, query, key, value, pattern). Wrapper around each's patching function, returns a stacked tensor of shape [5, n_layers, pos, n_heads]
+
+    Args:
+        model: The relevant model
+        corrupted_tokens (torch.Tensor): The input tokens for the corrupted run. Has shape [batch, pos]
+        clean_cache (ActivationCache): The cached activations from the clean run
+        metric: A function from the model's output logits to some metric (eg loss, logit diff, etc)
+
+    Returns:
+        patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [5, n_layers, pos, n_heads]
     """
     act_patch_results = []
-    act_patch_results.append(get_act_patch_attn_head_out_by_pos(model, corrupted_tokens, clean_cache, metric))
-    act_patch_results.append(get_act_patch_attn_head_q_by_pos(model, corrupted_tokens, clean_cache, metric))
-    act_patch_results.append(get_act_patch_attn_head_k_by_pos(model, corrupted_tokens, clean_cache, metric))
-    act_patch_results.append(get_act_patch_attn_head_v_by_pos(model, corrupted_tokens, clean_cache, metric))
-    
+    act_patch_results.append(
+        get_act_patch_attn_head_out_by_pos(model, corrupted_tokens, clean_cache, metric)
+    )
+    act_patch_results.append(
+        get_act_patch_attn_head_q_by_pos(model, corrupted_tokens, clean_cache, metric)
+    )
+    act_patch_results.append(
+        get_act_patch_attn_head_k_by_pos(model, corrupted_tokens, clean_cache, metric)
+    )
+    act_patch_results.append(
+        get_act_patch_attn_head_v_by_pos(model, corrupted_tokens, clean_cache, metric)
+    )
+
     # Reshape pattern to be compatible with the rest of the results
-    pattern_results = (get_act_patch_attn_head_pattern_by_pos(model, corrupted_tokens, clean_cache, metric))
-    act_patch_results.append(einops.rearrange(pattern_results, "batch head pos -> batch pos head"))
+    pattern_results = get_act_patch_attn_head_pattern_by_pos(
+        model, corrupted_tokens, clean_cache, metric
+    )
+    act_patch_results.append(
+        einops.rearrange(pattern_results, "batch head pos -> batch pos head")
+    )
     return torch.stack(act_patch_results, dim=0)
 
-def get_act_patch_block_every(model, corrupted_tokens, clean_cache, metric) -> Float[torch.Tensor, "patch_type layer pos"]:
+
+def get_act_patch_block_every(
+    model, corrupted_tokens, clean_cache, metric
+) -> Float[torch.Tensor, "patch_type layer pos"]:
     """Helper function to get activation patching results for the residual stream (at the start of each block), output of each Attention layer and output of each MLP layer. Wrapper around each's patching function, returns a stacked tensor of shape [3, n_layers, pos]
 
     Args:
         model: The relevant model
         corrupted_tokens (torch.Tensor): The input tokens for the corrupted run. Has shape [batch, pos]
         clean_cache (ActivationCache): The cached activations from the clean run
         metric: A function from the model's output logits to some metric (eg loss, logit diff, etc)
 
     Returns:
         patched_output (torch.Tensor): The tensor of the patching metric for each patch. Has shape [3, n_layers, pos]
     """
     act_patch_results = []
-    act_patch_results.append(get_act_patch_resid_pre(model, corrupted_tokens, clean_cache, metric))
-    act_patch_results.append(get_act_patch_attn_out(model, corrupted_tokens, clean_cache, metric))
-    act_patch_results.append(get_act_patch_mlp_out(model, corrupted_tokens, clean_cache, metric))
-    return torch.stack(act_patch_results, dim=0)
+    act_patch_results.append(
+        get_act_patch_resid_pre(model, corrupted_tokens, clean_cache, metric)
+    )
+    act_patch_results.append(
+        get_act_patch_attn_out(model, corrupted_tokens, clean_cache, metric)
+    )
+    act_patch_results.append(
+        get_act_patch_mlp_out(model, corrupted_tokens, clean_cache, metric)
+    )
+    return torch.stack(act_patch_results, dim=0)
```

### Comparing `transformer_lens-1.2.2/transformer_lens/train.py` & `transformer_lens-1.3.0/transformer_lens/train.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from transformer_lens import HookedTransformer
-from transformer_lens import HookedTransformerConfig
 from dataclasses import dataclass
-from typing import Optional, Callable
-from torch.utils.data import Dataset, DataLoader
+from typing import Optional
+
+import torch
 import torch.optim as optim
 import wandb
-import torch
-import torch.nn as nn
+from torch.utils.data import DataLoader, Dataset
 from tqdm.auto import tqdm
-from einops import rearrange
+
+from transformer_lens import HookedTransformer
 
 
 @dataclass
 class HookedTransformerTrainConfig:
     """
     Configuration class to store training hyperparameters for a training run of
     an HookedTransformer model.
```

### Comparing `transformer_lens-1.2.2/transformer_lens/utils.py` & `transformer_lens-1.3.0/transformer_lens/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,108 @@
 from __future__ import annotations
+
+import inspect
+import json
+import re
+import shutil
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union, cast
+
+import einops
 import numpy as np
 import torch
 import torch.nn.functional as F
-from datasets.arrow_dataset import Dataset
-import einops
-from transformers import AutoTokenizer
-from typing import Optional, Union, Tuple, List, Dict, Type
 import transformers
-from huggingface_hub import hf_hub_download
-import re
-from rich import print as rprint
 from datasets.arrow_dataset import Dataset
 from datasets.load import load_dataset
+from huggingface_hub import hf_hub_download
+from jaxtyping import Float, Int
+from rich import print as rprint
+from transformers import AutoTokenizer
 
 from transformer_lens import FactoredMatrix
 
 CACHE_DIR = transformers.TRANSFORMERS_CACHE
-import json
-from jaxtyping import Float, Int
+
+
+def select_compatible_kwargs(
+    kwargs_dict: Dict[str, Any], callable: Callable
+) -> Dict[str, Any]:
+    """Return a dict with the elements kwargs_dict that are parameters of callable"""
+    return {
+        k: v
+        for k, v in kwargs_dict.items()
+        if k in inspect.getfullargspec(callable).args
+    }
 
 
 def download_file_from_hf(
-    repo_name, file_name, subfolder=".", cache_dir=CACHE_DIR, force_is_torch=False
+    repo_name,
+    file_name,
+    subfolder=".",
+    cache_dir=CACHE_DIR,
+    force_is_torch=False,
+    **kwargs,
 ):
     """
     Helper function to download files from the HuggingFace Hub, from subfolder/file_name in repo_name, saving locally to cache_dir and returning the loaded file (if a json or Torch object) and the file path otherwise.
 
     If it's a Torch file without the ".pth" extension, set force_is_torch=True to load it as a Torch object.
     """
     file_path = hf_hub_download(
-        repo_id=repo_name, filename=file_name, subfolder=subfolder, cache_dir=cache_dir
+        repo_id=repo_name,
+        filename=file_name,
+        subfolder=subfolder,
+        cache_dir=cache_dir,
+        **select_compatible_kwargs(kwargs, hf_hub_download),
     )
 
     # Load to the CPU device if CUDA is not available
-    map_location = None if torch.cuda.is_available() else torch.device('cpu')
+    map_location = None if torch.cuda.is_available() else torch.device("cpu")
 
     if file_path.endswith(".pth") or force_is_torch:
         return torch.load(file_path, map_location=map_location)
     elif file_path.endswith(".json"):
         return json.load(open(file_path, "r"))
     else:
         print("File type not supported:", file_path.split(".")[-1])
         return file_path
 
+
+def clear_huggingface_cache():
+    """
+    Deletes the Hugging Face cache directory and all its contents.
+
+    This function deletes the Hugging Face cache directory, which is used to store downloaded models and their associated files. Deleting the cache directory will remove all the downloaded models and their files, so you will need to download them again if you want to use them in your code.
+
+    Parameters:
+    None
+
+    Returns:
+    None
+    """
+    print("Deleting Hugging Face cache directory and all its contents.")
+    shutil.rmtree(CACHE_DIR)
+
+
 def print_gpu_mem(step_name=""):
     print(
         f"{step_name} ~ {np.round(torch.cuda.memory_allocated()/2e30, 2)} GiB allocated on GPU."
     )
 
 
 def get_corner(tensor, n=3):
     # Prints the top left corner of the tensor
     if isinstance(tensor, torch.Tensor):
         return tensor[tuple(slice(n) for _ in range(tensor.ndim))]
     elif isinstance(tensor, FactoredMatrix):
         return tensor[tuple(slice(n) for _ in range(tensor.ndim))].AB
+
+
 def to_numpy(tensor):
-    """ 
+    """
     Helper function to convert a tensor to a numpy array. Also works on lists, tuples, and numpy arrays.
     """
     if isinstance(tensor, np.ndarray):
         return tensor
     elif isinstance(tensor, (list, tuple)):
         array = np.array(tensor)
         return array
@@ -110,37 +152,43 @@
     correct_matches = top_prediction[:, :-1] == tokens[:, 1:]
     if per_token:
         return correct_matches
     else:
         return correct_matches.sum() / correct_matches.numel()
 
 
-def gelu_new(input: Float[torch.Tensor, "batch pos d_mlp"]) -> Float[torch.Tensor, "batch pos d_mlp"]:
+def gelu_new(
+    input: Float[torch.Tensor, "batch pos d_mlp"]
+) -> Float[torch.Tensor, "batch pos d_mlp"]:
     # Implementation of GeLU used by GPT2 - subtly different from PyTorch's
     return (
         0.5
         * input
         * (
             1.0
             + torch.tanh(
                 np.sqrt(2.0 / np.pi) * (input + 0.044715 * torch.pow(input, 3.0))
             )
         )
     )
 
 
-def gelu_fast(input: Float[torch.Tensor, "batch pos d_mlp"]) -> Float[torch.Tensor, "batch pos d_mlp"]:
+def gelu_fast(
+    input: Float[torch.Tensor, "batch pos d_mlp"]
+) -> Float[torch.Tensor, "batch pos d_mlp"]:
     return (
         0.5
         * input
         * (1.0 + torch.tanh(input * 0.7978845608 * (1.0 + 0.044715 * input * input)))
     )
 
 
-def solu(input: Float[torch.Tensor, "batch pos d_mlp"]) -> Float[torch.Tensor, "batch pos d_mlp"]:
+def solu(
+    input: Float[torch.Tensor, "batch pos d_mlp"]
+) -> Float[torch.Tensor, "batch pos d_mlp"]:
     """
     SoLU activation function as described by
     https://transformer-circuits.pub/2022/solu/index.html.
 
     LayerNorm implemented by the MLP class.
     """
     return input * F.softmax(input, dim=-1)
@@ -236,14 +284,15 @@
 
 data = Dataset.from_dict({"text":[str(i) for i in range(1000)]})
 tokenizer = AutoTokenizer.from_pretrained("NeelNanda/gpt-neox-tokenizer-digits")
 print(data)
 tokenize_and_concatenate(data, tokenizer, streaming=False, column_name="text")
 """
 
+
 def sample_logits(
     final_logits: Float[torch.Tensor, "batch d_vocab"],
     top_k: Optional[int] = None,
     top_p: Optional[float] = None,
     temperature: float = 1.0,
     freq_penalty: float = 0.0,
     tokens: Optional[Int[torch.Tensor, "batch pos"]] = None,
@@ -282,15 +331,15 @@
                 )
         if top_k is not None:
             assert top_k > 0, "top_k has to be greater than 0"
             top_logits, top_idx = final_logits.topk(top_k, dim=-1)
             indices_to_remove = final_logits < top_logits[..., -1].unsqueeze(-1)
             final_logits = final_logits.masked_fill(indices_to_remove, -float("inf"))
         elif top_p is not None:
-            assert 1.0 >= top_p > 0.0, "top_p has to be in [0, 1)"
+            assert 1.0 >= top_p > 0.0, "top_p has to be in (0, 1]"
             sorted_logits, sorted_indices = torch.sort(final_logits, descending=True)
             cumulative_probs = sorted_logits.softmax(dim=-1).cumsum(dim=-1)
             # We round up - we want prob >= top_p not <top_p
             sorted_indices_to_remove = cumulative_probs > top_p
             sorted_indices_to_remove[..., 1:] = sorted_indices_to_remove[
                 ..., :-1
             ].clone()
@@ -301,15 +350,23 @@
             final_logits = final_logits.masked_fill(indices_to_remove, -float("inf"))
         return torch.distributions.categorical.Categorical(logits=final_logits).sample()
 
 
 # %%
 # Type alias
 SliceInput: Type = Optional[
-    Union[int, Tuple[int,], Tuple[int, int], Tuple[int, int, int], List[int], torch.Tensor, np.ndarray]
+    Union[
+        int,
+        Tuple[int,],
+        Tuple[int, int],
+        Tuple[int, int, int],
+        List[int],
+        torch.Tensor,
+        np.ndarray,
+    ]
 ]
 """
 An optional type alias for a slice input used in the `ActivationCache` module.
 
 A `SliceInput` can be one of the following types:
     - `int`: an integer representing a single position
     - `Tuple[int, int]`: a tuple of two integers representing a range of positions
@@ -352,23 +409,23 @@
         input_slice: SliceInput = None,
     ):
         """
         Modular component for slicing tensors. Can be used to slice a tensor along a given dimension, or to index into a tensor along a given dimension.
 
         Args:
             input_slice (SliceInput): The slice to apply. Can be an int, a tuple, a list, a torch.Tensor, or None. If None, do nothing.
-            
+
         Returns:
             Slice: A Slice object that can be applied to a tensor.
-        
+
         Raises:
             ValueError: If the input_slice is not one of the above types.
         """
         if type(input_slice) == tuple:
-            input_slice = slice(*input_slice)
+            input_slice: slice = slice(*input_slice)
             self.slice = input_slice
             self.mode = "slice"
         elif type(input_slice) == int:
             self.slice = input_slice
             self.mode = "int"
         elif type(input_slice) == slice:
             self.slice = input_slice
@@ -382,15 +439,15 @@
         else:
             raise ValueError(f"Invalid input_slice {input_slice}")
 
     def apply(
         self,
         tensor: torch.Tensor,
         dim: int = 0,
-        ) -> torch.Tensor:
+    ) -> torch.Tensor:
         """
         Takes in a tensor and a slice, and applies the slice to the given dimension (supports positive and negative dimension syntax). Returns the sliced tensor.
 
         Args:
             tensor (torch.Tensor): The tensor to slice.
             dim (int, optional): The dimension to slice along. Supports positive and negative dimension syntax.
 
@@ -401,36 +458,36 @@
         slices = [slice(None)] * ndim
         slices[dim] = self.slice
         return tensor[tuple(slices)]
 
     def indices(
         self,
         max_ctx: Optional[int] = None,
-        ) -> Union[np.ndarray, np.int64]:
+    ) -> Union[np.ndarray, np.int64]:
         """
         Returns the indices when this slice is applied to an axis of size max_ctx. Returns them as a numpy array, for integer slicing it is eg array([4])
 
         Args:
             max_ctx (int, optional): The size of the axis to slice. Only used if the slice is not an integer.
 
         Returns:
             np.ndarray: The indices that this slice will select.
 
         Raises:
             ValueError: If the slice is not an integer and max_ctx is not specified.
         """
         if self.mode == "int":
-            return np.array([self.slice])
+            return np.array([self.slice], dtype=np.int64)
         if max_ctx is None:
             raise ValueError("max_ctx must be specified if slice is not an integer")
-        return np.arange(max_ctx)[self.slice]
+        return np.arange(max_ctx, dtype=np.int64)[self.slice]
 
     def __repr__(
         self,
-        ) -> str:
+    ) -> str:
         return f"Slice: {self.slice} Mode: {self.mode} "
 
 
 # %%
 
 
 def get_act_name(
@@ -488,33 +545,43 @@
         "b": "",
         "block": "",
         "blocks": "",
         "attention": "attn",
     }
 
     act_name_alias = {
-        "attn":"pattern",
-        "attn_logits":"attn_scores",
-        "key":"k",
-        "query":"q",
-        "value":"v",
-        "mlp_pre":"pre",
-        "mlp_mid":"mid",
-        "mlp_post":"post",
+        "attn": "pattern",
+        "attn_logits": "attn_scores",
+        "key": "k",
+        "query": "q",
+        "value": "v",
+        "mlp_pre": "pre",
+        "mlp_mid": "mid",
+        "mlp_post": "post",
     }
 
     layer_norm_names = ["scale", "normalized"]
 
     if name in act_name_alias:
         name = act_name_alias[name]
 
     full_act_name = ""
     if layer is not None:
         full_act_name += f"blocks.{layer}."
-    if name in ["k", "v", "q", "z", "rot_k", "rot_q", "result", "pattern", "attn_scores"]:
+    if name in [
+        "k",
+        "v",
+        "q",
+        "z",
+        "rot_k",
+        "rot_q",
+        "result",
+        "pattern",
+        "attn_scores",
+    ]:
         layer_type = "attn"
     elif name in ["pre", "post", "mid"]:
         layer_type = "mlp"
     elif layer_type in layer_type_alias:
         layer_type = layer_type_alias[layer_type]
 
     if layer_type:
@@ -522,15 +589,17 @@
     full_act_name += f"hook_{name}"
 
     if name in layer_norm_names and layer is None:
         full_act_name = f"ln_final.{full_act_name}"
     return full_act_name
 
 
-def remove_batch_dim(tensor: Float[torch.Tensor, "1 ..."]) -> Float[torch.Tensor, "..."]:
+def remove_batch_dim(
+    tensor: Float[torch.Tensor, "1 ..."]
+) -> Float[torch.Tensor, "..."]:
     """
     Removes the first dimension of a tensor if it is size 1, otherwise returns the tensor unchanged
     """
     if tensor.shape[0] == 1:
         return tensor.squeeze(0)
     else:
         return tensor
@@ -593,18 +662,20 @@
 # %%
 def transpose(tensor: Float[torch.Tensor, "... a b"]) -> Float[torch.Tensor, "... b a"]:
     """
     Utility to swap the last two dimensions of a tensor, regardless of the number of leading dimensions
     """
     return tensor.transpose(-1, -2)
 
+
 def composition_scores(
     left: FactoredMatrix, right: FactoredMatrix, broadcast_dims=True
 ) -> Union[
-    Float[torch.Tensor, "*leading_dims"], Float[torch.Tensor, "*leading_dims_left *T.leading_dims_right"]
+    Float[torch.Tensor, "*leading_dims"],
+    Float[torch.Tensor, "*leading_dims_left *T.leading_dims_right"],
 ]:
     """
     See `HookedTransformer.all_composition_scores` for documentation.
     """
     if broadcast_dims:
         r_leading = right.ndim - 2
         l_leading = left.ndim - 2
@@ -623,37 +694,95 @@
     comp_norms = (left @ right).norm(dim=[-2, -1])
     return comp_norms / r_norms / l_norms
 
 
 # %%
 def get_dataset(dataset_name: str, **kwargs) -> Dataset:
     """
-    Returns a small HuggingFace dataset, for easy testing and exploration. Accesses several convenience datasets with 10,000 elements (dealing with the enormous 100GB - 2TB datasets is a lot of effort!). Note that it returns a dataset (ie a dictionary containing all the data), *not* a DataLoader (iterator over the data + some fancy features). But you can easily convert it to a DataLoader. 
-    
+    Returns a small HuggingFace dataset, for easy testing and exploration. Accesses several convenience datasets with 10,000 elements (dealing with the enormous 100GB - 2TB datasets is a lot of effort!). Note that it returns a dataset (ie a dictionary containing all the data), *not* a DataLoader (iterator over the data + some fancy features). But you can easily convert it to a DataLoader.
+
     Each dataset has a 'text' field, which contains the relevant info, some also have several meta data fields
 
     Kwargs will be passed to the huggingface dataset loading function, e.g. "data_dir"
-    
+
     Possible inputs:
     * openwebtext (approx the GPT-2 training data https://huggingface.co/datasets/openwebtext)
     * pile (The Pile, a big mess of tons of diverse data https://pile.eleuther.ai/)
     * c4 (Colossal, Cleaned, Common Crawl - basically openwebtext but bigger https://huggingface.co/datasets/c4)
     * code (Codeparrot Clean, a Python code dataset https://huggingface.co/datasets/codeparrot/codeparrot-clean )
     * c4_code (c4 + code - the 20K data points from c4-10k and code-10k. This is the mix of datasets used to train my interpretability-friendly models, though note that they are *not* in the correct ratio! There's 10K texts for each, but about 22M tokens of code and 5M tokens of C4)
     * wiki (Wikipedia, generated from the 20220301.en split of https://huggingface.co/datasets/wikipedia )
     """
     dataset_aliases = {
-        'openwebtext': 'stas/openwebtext-10k',
-        'owt': 'stas/openwebtext-10k',
-        'pile': 'NeelNanda/pile-10k',
-        'c4': 'NeelNanda/c4-10k',
-        'code': 'NeelNanda/code-10k',
-        'python': 'NeelNanda/code-10k',
-        'c4_code': 'NeelNanda/c4-code-20k',
-        'c4-code': 'NeelNanda/c4-code-20k',
-        'wiki': 'NeelNanda/wiki-10k'
+        "openwebtext": "stas/openwebtext-10k",
+        "owt": "stas/openwebtext-10k",
+        "pile": "NeelNanda/pile-10k",
+        "c4": "NeelNanda/c4-10k",
+        "code": "NeelNanda/code-10k",
+        "python": "NeelNanda/code-10k",
+        "c4_code": "NeelNanda/c4-code-20k",
+        "c4-code": "NeelNanda/c4-code-20k",
+        "wiki": "NeelNanda/wiki-10k",
     }
     if dataset_name in dataset_aliases:
-        dataset = load_dataset(dataset_aliases[dataset_name], split='train', **kwargs)
+        dataset = load_dataset(dataset_aliases[dataset_name], split="train", **kwargs)
     else:
         raise ValueError(f"Dataset {dataset_name} not supported")
     return dataset
+
+
+def is_square(x: torch.Tensor) -> bool:
+    """Checks if `x` is a square matrix."""
+    return x.ndim == 2 and x.shape[0] == x.shape[1]
+
+
+def is_lower_triangular(x: torch.Tensor) -> bool:
+    """Checks if `x` is a lower triangular matrix."""
+    if not is_square(x):
+        return False
+    return x.equal(x.tril())
+
+
+def check_structure(
+    t1: torch.Tensor, t2: torch.Tensor, *, verbose: bool = False
+) -> None:
+    """Validate that the two square tensors have the same structure, i.e.,
+    that the directionality of comparisons points in the same directions both
+    row-wise and column-wise.
+
+    This function is not used anywhere in the code right now, just for debugging tests.
+    """
+    assert t1.ndim == 2
+    assert t1.shape == t2.shape
+    n_rows, n_cols = cast(Tuple[int, int], t1.shape)
+
+    if verbose:
+        print("Checking rows")
+    row_mismatch = []
+    for row_i in range(n_rows - 1):
+        t1_result = t1[row_i].ge(t1[row_i + 1])
+        t2_result = t2[row_i].ge(t2[row_i + 1])
+        if any(t1_result != t2_result):
+            row_mismatch.append(row_i)
+            if verbose:
+                print(f"\trows {row_i}:{row_i + 1}")
+                print(f"\tt1: {t1_result.tolist()}")
+                print(f"\tt2: {t2_result.tolist()}")
+
+    if verbose:
+        print("Checking columns")
+    col_mismatch = []
+    for col_i in range(n_cols - 1):
+        t1_result = t1[:, col_i].ge(t1[:, col_i + 1])
+        t2_result = t2[:, col_i].ge(t2[:, col_i + 1])
+        if any(t1_result != t2_result):
+            col_mismatch.append(col_i)
+            if verbose:
+                print(f"\trows {col_i}:{col_i + 1}")
+                print(f"\tt1: {t1_result.tolist()}")
+                print(f"\tt2: {t2_result.tolist()}")
+    if not row_mismatch and not col_mismatch:
+        print("PASSED")
+    elif row_mismatch:
+        print(f"row mismatch: {row_mismatch}")
+    elif col_mismatch:
+        print(f"column mismatch: {col_mismatch}")
```

### Comparing `transformer_lens-1.2.2/PKG-INFO` & `transformer_lens-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: transformer-lens
-Version: 1.2.2
+Version: 1.3.0
 Summary: An implementation of transformers tailored for mechanistic interpretability.
 License: MIT
 Author: Neel Nanda
 Author-email: 77788841+neelnanda-io@users.noreply.github.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7.4,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: datasets (>=2.7.1)
 Requires-Dist: einops (>=0.6.0)
@@ -27,19 +26,22 @@
 Requires-Dist: sphinx (==5.2.3) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "docs")
 Requires-Dist: sphinx-autobuild (>=2021.3.14) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "docs")
 Requires-Dist: sphinxcontrib-napoleon (>=0.7) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "docs")
 Requires-Dist: tabulate (>=0.9.0) ; (python_version >= "3.8" and python_version < "3.10") and (extra == "docs")
 Requires-Dist: torch (>=1.10)
 Requires-Dist: tqdm (>=4.64.1)
 Requires-Dist: transformers (>=4.25.1)
+Requires-Dist: typeguard (>=3.0.2,<4.0.0)
 Requires-Dist: wandb (>=0.13.5)
 Description-Content-Type: text/markdown
 
 # TransformerLens
 
+![TransformerLens](assets/rm_transformer_lens_logo.png)
+
 [![Pypi](https://img.shields.io/pypi/v/transformer-lens)](https://pypi.org/project/transformer-lens/)
 
 (Formerly known as EasyTransformer)
 
 ## [Read the Docs Here](https://neelnanda-io.github.io/TransformerLens/)
 
 ## [Main Tutorial Here](https://neelnanda.io/transformer-lens-demo)
@@ -110,14 +112,21 @@
 
 #### Running the tests
 
 - All tests via `make test`
 - Unit tests only via `make unit-test`
 - Acceptance tests only via `make acceptance-test`
 
+### Formatting
+
+This project uses `pycln`, `isort` and `black` for formatting, pull requests are checked in github actions.
+
+- Format all files via `make format`
+- Only check the formatting via `make check-format`
+
 ### Demos
 
 If adding a feature, please add it to the demo notebook in the `demos` folder, and check that it works in the demo format. This can be tested by replacing `pip install git+https://github.com/JayBaileyCS/TransformerLens.git` with `pip install git+https://github.com/<YOUR_USERNAME_HERE>/TransformerLens.git` in the demo notebook, and running it in a fresh environment.
 
 ## Citation
 
 Please cite this library as:
```

