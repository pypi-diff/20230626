# Comparing `tmp/mowgli-0.2.0.tar.gz` & `tmp/mowgli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mowgli-0.2.0.tar", max compression
+gzip compressed data, was "mowgli-0.3.0.tar", max compression
```

## Comparing `mowgli-0.2.0.tar` & `mowgli-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-02-09 12:53:58.500041 mowgli-0.2.0/LICENSE
--rw-r--r--   0        0        0     2946 2023-03-01 13:00:03.556043 mowgli-0.2.0/README.md
--rw-r--r--   0        0        0      117 2023-03-01 14:00:58.668054 mowgli-0.2.0/mowgli/__init__.py
--rw-r--r--   0        0        0    18191 2023-02-09 15:03:01.828064 mowgli-0.2.0/mowgli/models.py
--rw-r--r--   0        0        0     4615 2023-03-01 13:47:36.644052 mowgli-0.2.0/mowgli/pl.py
--rw-r--r--   0        0        0     4094 2023-02-09 13:41:10.760049 mowgli-0.2.0/mowgli/score.py
--rw-r--r--   0        0        0     3866 2023-02-09 13:41:08.064049 mowgli-0.2.0/mowgli/tl.py
--rw-r--r--   0        0        0     5644 2023-02-09 15:02:54.928064 mowgli-0.2.0/mowgli/utils.py
--rw-r--r--   0        0        0      957 2023-03-01 14:00:10.108054 mowgli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4192 1970-01-01 00:00:00.000000 mowgli-0.2.0/setup.py
--rw-r--r--   0        0        0     4316 1970-01-01 00:00:00.000000 mowgli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-09 12:53:58.500041 mowgli-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3154 2023-06-01 15:21:42.484001 mowgli-0.3.0/README.md
+-rw-r--r--   0        0        0      118 2023-06-26 19:12:11.004001 mowgli-0.3.0/mowgli/__init__.py
+-rw-r--r--   0        0        0    18573 2023-06-26 19:12:46.704001 mowgli-0.3.0/mowgli/models.py
+-rw-r--r--   0        0        0     4693 2023-03-01 14:45:34.724062 mowgli-0.3.0/mowgli/pl.py
+-rw-r--r--   0        0        0     3798 2023-03-01 14:48:01.628063 mowgli-0.3.0/mowgli/score.py
+-rw-r--r--   0        0        0     3866 2023-02-09 13:41:08.064049 mowgli-0.3.0/mowgli/tl.py
+-rw-r--r--   0        0        0     5638 2023-03-01 14:47:36.876062 mowgli-0.3.0/mowgli/utils.py
+-rw-r--r--   0        0        0     1032 2023-06-26 19:11:51.028001 mowgli-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4439 1970-01-01 00:00:00.000000 mowgli-0.3.0/setup.py
+-rw-r--r--   0        0        0     4604 1970-01-01 00:00:00.000000 mowgli-0.3.0/PKG-INFO
```

### Comparing `mowgli-0.2.0/LICENSE` & `mowgli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mowgli-0.2.0/README.md` & `mowgli-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Mowgli: Multi Omics Wasserstein inteGrative anaLysIs
 [![Tests](https://github.com/gjhuizing/Mowgli/actions/workflows/main.yml/badge.svg)](https://github.com/gjhuizing/Mowgli/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/gjhuizing/Mowgli/branch/main/graph/badge.svg?token=UBUJF7098Q)](https://codecov.io/gh/gjhuizing/Mowgli)
+[![codecov](https://codecov.io/gh/cantinilab/Mowgli/branch/main/graph/badge.svg?token=UBUJF7098Q)](https://codecov.io/gh/cantinilab/Mowgli)
 [![Documentation Status](https://readthedocs.org/projects/mowgli/badge/?version=latest)](https://mowgli.readthedocs.io/en/latest/?badge=latest)
-[![PyPI version](https://badge.fury.io/py/mowgli.svg)](https://badge.fury.io/py/mowgli)
+[![PyPI version](https://img.shields.io/pypi/v/mowgli?color=blue)](https://img.shields.io/pypi/v/mowgli?color=blue)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Mowgli is a novel method for the integration of paired multi-omics data with any type and number of omics, combining integrative Nonnegative Matrix Factorization and Optimal Transport. [Read the preprint!](https://www.biorxiv.org/content/10.1101/2023.02.02.526825v2)
 
 ![figure](figure.png)
 
 ## Install the package
 
@@ -29,15 +30,15 @@
 
 ## Getting started
 
 Mowgli takes as an input a Muon object and populates its `obsm` and `uns` fiels with the embeddings and dictionaries, respectively. Visit [mowgli.rtfd.io](https://mowgli.rtfd.io/) for more documentation and tutorials.
 
 You may download a preprocessed 10X Multiome demo dataset [here](https://figshare.com/s/4c8e72cbb188d8e1cce8).
 
-A GPU is not required for small datasets, but is strongly recommmended above 1,000 cells. On CPU, the [cell lines demo](https://mowgli.readthedocs.io/en/latest/vignettes/Liu%20cell%20lines.html) (206 cells) should run in under 5 minutes and the [PBMC demo](https://mowgli.readthedocs.io/en/latest/vignettes/PBMC.html) (500 cells) should run in under 10 minutes.
+A GPU is not required for small datasets, but is strongly recommmended above 1,000 cells. On CPU, the [cell lines demo](https://mowgli.readthedocs.io/en/latest/vignettes/Liu%20cell%20lines.html) (206 cells) should run in under 5 minutes and the [PBMC demo](https://mowgli.readthedocs.io/en/latest/vignettes/PBMC.html) (500 cells) should run in under 10 minutes (tested on a Ubuntu 20.04 machine with an 11th gen i7 processor).
 
 ```python
 import mowgli
 import mudata as md
 import scanpy as sc
 
 # Load data into a Muon object.
```

### Comparing `mowgli-0.2.0/mowgli/models.py` & `mowgli-0.3.0/mowgli/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-import torch
-from torch import optim
-import torch.nn.functional as F
+from typing import Callable, List
 
+import mudata as md
 import numpy as np
+import torch
+import torch.nn.functional as F
+from mowgli import utils
 from sklearn.decomposition import PCA
-
-from typing import Callable, List
-import mudata as md
+from torch import optim
 from tqdm import tqdm
 
-from mowgli import utils
-
 
 class MowgliModel:
     def __init__(
         self,
-        latent_dim: int = 15,
+        latent_dim: int = 50,
         use_mod_weight: bool = False,
-        h_regularization: float = 5e-2,
-        w_regularization: float = 5e-2,
+        h_regularization: float = {
+            "rna": 1e-2,
+            "adt": 1e-2,
+            "prot": 1e-2,
+            "atac": 1e-1,
+        },
+        w_regularization: float = 1e-3,
         eps: float = 5e-2,
         cost: str = "cosine",
         pca_cost: bool = False,
         cost_path: dict = None,
     ):
         """Initialize the Mowgli model, which performs integrative NMF with an
         Optimal Transport loss.
@@ -31,19 +34,22 @@
             latent_dim (int, optional):
                 The latent dimension of the model. Defaults to 15.
             use_mod_weight (bool, optional):
                 Whether to use a different weight for each modality and each
                 cell. If `True`, the weights are expected in the `mod_weight`
                 obs field of each modality. Defaults to False.
             h_regularization (float, optional):
-                The entropy parameter for the dictionary. Small values mean
-                sparse dictionaries. Defaults to 5e-2.
+                The entropy parameter for the dictionary. Defaults to 0.01 for RNA
+                and ADT and 0.1 for ATAC. If needed, other modalities should be
+                specified by the user. We advise setting values between 0.001
+                (biological signal driven by very few features) and 1.0 (very
+                diffuse biological signals).
             w_regularization (float, optional):
-                The entropy parameter for the embedding. Small values mean
-                sparse vectors. Defaults to 5e-2.
+                The entropy parameter for the embedding. As with `h_regularization`,
+                small values mean sparse vectors. Defaults to 1e-3.
             eps (float, optional):
                 The entropy parameter for epsilon transport. Large values
                 decrease importance of individual genes. Defaults to 5e-2.
             cost (str, optional):
                 The function used to compute an emprical ground cost. All
                 metrics from Scipy's `cdist` are allowed. Defaults to 'cosine'.
             pca_cost (bool, optional):
@@ -144,15 +150,15 @@
                 self.A[mod] /= self.A[mod].sum(1).reshape(-1, 1) * mean_row_sum
             self.A[mod] /= self.A[mod].sum(0)
 
             # Determine which cost function to use.
             cost = self.cost if isinstance(self.cost, str) else self.cost[mod]
             try:
                 cost_path = self.cost_path[mod]
-            except:
+            except Exception:
                 cost_path = None
 
             # Define the features that the ground cost will be computed on.
             features = 1e-6 + self.A[mod].cpu().numpy()
             if self.pca_cost:
                 pca = PCA(n_components=self.latent_dim)
                 features = pca.fit_transform(features)
@@ -180,19 +186,19 @@
 
     def train(
         self,
         mdata: md.MuData,
         max_iter_inner: int = 1_000,
         max_iter: int = 100,
         device: torch.device = "cpu",
-        dtype: torch.dtype = torch.float,
+        dtype: torch.dtype = torch.double,
         lr: float = 1,
         optim_name: str = "lbfgs",
-        tol_inner: float = 1e-9,
-        tol_outer: float = 1e-3,
+        tol_inner: float = 1e-12,
+        tol_outer: float = 1e-4,
         normalize_rows: bool = False,
     ) -> None:
         """Train the Mowgli model on an input MuData object.
 
         Args:
             mdata (md.MuData):
                 The input MuData object.
@@ -201,39 +207,39 @@
                 (optimizing H, or W). Defaults to 1_000.
             max_iter (int, optional):
                 How many interations for the outer optimization loop (how
                 many successive optimizations of H and W). Defaults to 100.
             device (torch.device, optional):
                 The device to work on. Defaults to 'cpu'.
             dtype (torch.dtype, optional):
-                The dtype to work with. Defaults to torch.float.
+                The dtype to work with. Defaults to torch.double.
             lr (float, optional):
                 The learning rate for the optimizer. The default is set
                 for LBFGS and should be changed otherwise. Defaults to 1.
             optim_name (str, optional):
                 The optimizer to use (`lbfgs`, `sgd` or `adam`). LBFGS
                 is advised, but requires more memory. Defaults to "lbfgs".
             tol_inner (float, optional):
                 The tolerance for the inner iterations before early stopping.
-                Defaults to 1e-9.
+                Defaults to 1e-12.
             tol_outer (float, optional):
                 The tolerance for the outer iterations before early stopping.
-                Defaults to 1e-3.
+                Defaults to 1e-4.
         """
 
         # First, initialize the different parameters.
         self.init_parameters(
             mdata,
             dtype=dtype,
             device=device,
             normalize_rows=normalize_rows,
         )
 
         # This is needed to save things in uns if it doesn't exist.
-        if mdata.uns == None:
+        if mdata.uns is None:
             mdata.uns = {}
 
         self.lr = lr
         self.optim_name = optim_name
 
         # Initialize the loss histories.
         self.losses_w, self.losses_h, self.losses = [], [], []
@@ -345,15 +351,15 @@
         loss_fn: Callable,
         max_iter: int,
         history: List,
         tol: float,
         pbar,
         device: str,
     ) -> None:
-        """Optimize a fiven function.
+        """Optimize a given function.
 
         Args:
             loss_fn (Callable): The function to optimize.
             max_iter (int): The maximum number of iterations.
             history (List): A list to append the losses to.
             tol (float): The tolerance before early stopping.
             pbar (A tqdm progress bar): The progress bar.
```

### Comparing `mowgli-0.2.0/mowgli/pl.py` & `mowgli-0.3.0/mowgli/pl.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,29 +72,31 @@
     # Create an AnnData with the joint embedding.
     joint_embedding = ad.AnnData(mdata.obsm[obsm], obs=mdata.obs)
 
     # Try to compute a dendrogram.
     try:
         sc.pp.pca(joint_embedding)
         sc.tl.dendrogram(joint_embedding, groupby=groupby, use_rep="X_pca")
-    except:
+    except Exception:
+        print("Dendrogram not computed.")
         pass
 
     # Get the dimension names to show.
     if sort_var:
         idx = joint_embedding.X.std(0).argsort()[::-1]
         var_names = joint_embedding.var_names[idx]
     else:
         var_names = joint_embedding.var_names
 
     # PLot the heatmap.
     return sc.pl.heatmap(
         joint_embedding, var_names, groupby=groupby, cmap=cmap, save=save, **kwds
     )
 
+
 def enrich(enr: pd.DataFrame, query_name: str, n_terms: int = 10):
     """Display a list of enriched terms.
 
     Args:
         enr (pd.DataFrame): The enrichment object returned by mowgli.tl.enrich()
         query_name (str): The name of the query, e.g. "dimension 0".
     """
@@ -126,14 +128,15 @@
     )
 
     ax.set_xlabel("$-log_{10}(p)$")
     ax.set_ylabel("Enriched terms")
 
     plt.show()
 
+
 def top_features(
     mdata: md.MuData,
     mod: str = "rna",
     uns: str = "H_OT",
     dim: int = 0,
     n_top: int = 10,
 ):
@@ -142,20 +145,22 @@
     Args:
         mdata (md.MuData): The input data
         mod (str, optional): The modality to consider. Defaults to 'rna'.
         uns (str, optional): The uns field to consider. Defaults to 'H_OT'.
         dim (int, optional): The latent dimension. Defaults to 0.
         n_top (int, optional): The number of top features to display. Defaults to 10.
     """
-    
+
     # Get the variable names.
     var_names = mdata[mod].var_names[mdata[mod].var.highly_variable]
 
     # Get the top features.
     idx_top_features = np.argsort(mdata[mod].uns[uns][:, dim])[::-1][:n_top]
-    df = pd.DataFrame({
-        "features": var_names[idx_top_features],
-        "weights": mdata[mod].uns[uns][idx_top_features, dim]
-    })
+    df = pd.DataFrame(
+        {
+            "features": var_names[idx_top_features],
+            "weights": mdata[mod].uns[uns][idx_top_features, dim],
+        }
+    )
 
     # Display the top features.
-    sns.barplot(data=df, x="weights", y="features", palette="Blues_r")
+    sns.barplot(data=df, x="weights", y="features", palette="Blues_r")
```

### Comparing `mowgli-0.2.0/mowgli/score.py` & `mowgli-0.3.0/mowgli/score.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from typing import Iterable
+
+import anndata as ad
 import numpy as np
-from scipy.stats import pearsonr, spearmanr
-from sklearn.metrics import silhouette_score
+import scanpy as sc
 from scipy.spatial.distance import cdist
 from sklearn.metrics import adjusted_rand_score as ARI
 from sklearn.metrics import normalized_mutual_info_score as NMI
-import anndata as ad
-import scanpy as sc
+from sklearn.metrics import silhouette_score
 from tqdm import tqdm
 
-############################ BASED ON AN EMBEDDING ############################
-
 
 def embedding_silhouette_score(
     embedding: np.ndarray,
     labels: np.ndarray,
     metric: str = "euclidean",
 ) -> float:
     """Compute the silhouette score for an embedding.
@@ -62,17 +60,14 @@
         aris.append(ARI(joint_embedding.obs["leiden"], labels))
         nmis.append(NMI(joint_embedding.obs["leiden"], labels))
 
     # Return ARI and NMI for various resolutions.
     return resolutions, aris, nmis
 
 
-################################ BASED ON A KNN ###############################
-
-
 def knn_purity_score(knn: np.ndarray, labels: np.ndarray) -> float:
     """Compute the kNN purity score, averaged over all observations.
     For one observation, the purity score is the percentage of
     nearest neighbors that share its label.
 
     Args:
         knn (np.ndarray):
@@ -93,21 +88,19 @@
     # Iterate over the observations.
     for i, neighbors in enumerate(knn):
 
         # Do the neighbors have the same label as the observation?
         matches = labels[neighbors] == labels[i]
 
         # Add the purity rate to the scores.
-        score += np.mean(matches)/knn.shape[0]
+        score += np.mean(matches) / knn.shape[0]
 
     # Return the average purity.
     return score
 
-#################################### EMBEDDING TO KNN ####################################
-
 
 def embedding_to_knn(
     embedding: np.ndarray, k: int = 15, metric: str = "euclidean"
 ) -> np.ndarray:
     """Convert embedding to knn
 
     Args:
```

### Comparing `mowgli-0.2.0/mowgli/tl.py` & `mowgli-0.3.0/mowgli/tl.py`

 * *Files identical despite different names*

### Comparing `mowgli-0.2.0/mowgli/utils.py` & `mowgli-0.3.0/mowgli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Iterable, List
+from typing import Iterable, List
 import torch
 from scipy.spatial.distance import cdist
 import numpy as np
 
 
 def reference_dataset(
     X, dtype: torch.dtype, device: torch.device, keep_idx: Iterable
```

### Comparing `mowgli-0.2.0/pyproject.toml` & `mowgli-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mowgli"
-version = "0.2.0"
+version = "0.3.0"
 description = "Mowgli is a novel method for the integration of paired multi-omics data with any type and number of omics, combining integrative Nonnegative Matrix Factorization and Optimal Transport."
 authors = ["Geert-Jan Huizing <huizing@ens.fr>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
@@ -18,15 +18,17 @@
 scikit-learn = "^1.0.0"
 scipy = "^1.0.0"
 
 nbsphinx = { version = "^0.8.12", optional = true }
 furo = { version = "^2022.12.7", optional = true }
 gprofiler-official = { version = "^1.0.0", optional = true }
 leidenalg = { version = "^0.9.1", optional = true }
+pre-commit = { version = "^3.1.1", optional = true }
 
 [tool.poetry.extras]
 docs = ["nbsphinx", "furo"]
+dev = ["pre-commit"]
 full = ["gprofiler-official", "leidenalg"]
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `mowgli-0.2.0/setup.py` & `mowgli-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,22 +15,23 @@
  'scanpy>=1.0.0,<2.0.0',
  'scikit-learn>=1.0.0,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'torch>=1.0.0,<2.0.0',
  'tqdm>=4.0.0,<5.0.0']
 
 extras_require = \
-{'docs': ['nbsphinx>=0.8.12,<0.9.0', 'furo>=2022.12.7,<2023.0.0'],
+{'dev': ['pre-commit>=3.1.1,<4.0.0'],
+ 'docs': ['nbsphinx>=0.8.12,<0.9.0', 'furo>=2022.12.7,<2023.0.0'],
  'full': ['gprofiler-official>=1.0.0,<2.0.0', 'leidenalg>=0.9.1,<0.10.0']}
 
 setup_kwargs = {
     'name': 'mowgli',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'Mowgli is a novel method for the integration of paired multi-omics data with any type and number of omics, combining integrative Nonnegative Matrix Factorization and Optimal Transport.',
-    'long_description': '# Mowgli: Multi Omics Wasserstein inteGrative anaLysIs\n[![Tests](https://github.com/gjhuizing/Mowgli/actions/workflows/main.yml/badge.svg)](https://github.com/gjhuizing/Mowgli/actions/workflows/main.yml)\n[![codecov](https://codecov.io/gh/gjhuizing/Mowgli/branch/main/graph/badge.svg?token=UBUJF7098Q)](https://codecov.io/gh/gjhuizing/Mowgli)\n[![Documentation Status](https://readthedocs.org/projects/mowgli/badge/?version=latest)](https://mowgli.readthedocs.io/en/latest/?badge=latest)\n[![PyPI version](https://badge.fury.io/py/mowgli.svg)](https://badge.fury.io/py/mowgli)\n\nMowgli is a novel method for the integration of paired multi-omics data with any type and number of omics, combining integrative Nonnegative Matrix Factorization and Optimal Transport. [Read the preprint!](https://www.biorxiv.org/content/10.1101/2023.02.02.526825v2)\n\n![figure](figure.png)\n\n## Install the package\n\nMowgli is implemented as a Python package seamlessly integrated within the scverse ecosystem, in particular Muon and Scanpy.\n\n### via PyPI (recommended)\n\nOn all operating systems, the easiest way to install Mowgli is via PyPI. Installation should typically take a minute and is continuously tested with Python 3.8 on an Ubuntu virtual machine.\n\n```bash\npip install mowgli\n```\n\n### via GitHub (development version)\n\n```bash\ngit clone git@github.com:cantinilab/Mowgli.git\npip install ./Mowgli/\n```\n\n## Getting started\n\nMowgli takes as an input a Muon object and populates its `obsm` and `uns` fiels with the embeddings and dictionaries, respectively. Visit [mowgli.rtfd.io](https://mowgli.rtfd.io/) for more documentation and tutorials.\n\nYou may download a preprocessed 10X Multiome demo dataset [here](https://figshare.com/s/4c8e72cbb188d8e1cce8).\n\nA GPU is not required for small datasets, but is strongly recommmended above 1,000 cells. On CPU, the [cell lines demo](https://mowgli.readthedocs.io/en/latest/vignettes/Liu%20cell%20lines.html) (206 cells) should run in under 5 minutes and the [PBMC demo](https://mowgli.readthedocs.io/en/latest/vignettes/PBMC.html) (500 cells) should run in under 10 minutes.\n\n```python\nimport mowgli\nimport mudata as md\nimport scanpy as sc\n\n# Load data into a Muon object.\nmdata = md.read_h5mu("my_data.h5mu")\n\n# Initialize and train the model.\nmodel = mowgli.models.MowgliModel(latent_dim=15)\nmodel.train(mdata)\n\n# Visualize the embedding with UMAP.\nsc.pp.neighbors(mdata, use_rep="W_OT")\nsc.tl.umap(mdata)\nsc.pl.umap(mdata)\n```\n\n## Our preprint\n\n```bibtex\n@article{huizing2023paired,\n  title={Paired single-cell multi-omics data integration with Mowgli},\n  author={Huizing, Geert-Jan and Deutschmann, Ina Maria and Peyre, Gabriel and Cantini, Laura},\n  journal={bioRxiv},\n  pages={2023--02},\n  year={2023},\n  publisher={Cold Spring Harbor Laboratory}\n}\n```\n\nIf you\'re looking for the repository with code to reproduce the experiments in our preprint, [here is is!](https://github.com/cantinilab/mowgli_reproducibility)\n',
+    'long_description': '# Mowgli: Multi Omics Wasserstein inteGrative anaLysIs\n[![Tests](https://github.com/gjhuizing/Mowgli/actions/workflows/main.yml/badge.svg)](https://github.com/gjhuizing/Mowgli/actions/workflows/main.yml)\n[![codecov](https://codecov.io/gh/cantinilab/Mowgli/branch/main/graph/badge.svg?token=UBUJF7098Q)](https://codecov.io/gh/cantinilab/Mowgli)\n[![Documentation Status](https://readthedocs.org/projects/mowgli/badge/?version=latest)](https://mowgli.readthedocs.io/en/latest/?badge=latest)\n[![PyPI version](https://img.shields.io/pypi/v/mowgli?color=blue)](https://img.shields.io/pypi/v/mowgli?color=blue)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nMowgli is a novel method for the integration of paired multi-omics data with any type and number of omics, combining integrative Nonnegative Matrix Factorization and Optimal Transport. [Read the preprint!](https://www.biorxiv.org/content/10.1101/2023.02.02.526825v2)\n\n![figure](figure.png)\n\n## Install the package\n\nMowgli is implemented as a Python package seamlessly integrated within the scverse ecosystem, in particular Muon and Scanpy.\n\n### via PyPI (recommended)\n\nOn all operating systems, the easiest way to install Mowgli is via PyPI. Installation should typically take a minute and is continuously tested with Python 3.8 on an Ubuntu virtual machine.\n\n```bash\npip install mowgli\n```\n\n### via GitHub (development version)\n\n```bash\ngit clone git@github.com:cantinilab/Mowgli.git\npip install ./Mowgli/\n```\n\n## Getting started\n\nMowgli takes as an input a Muon object and populates its `obsm` and `uns` fiels with the embeddings and dictionaries, respectively. Visit [mowgli.rtfd.io](https://mowgli.rtfd.io/) for more documentation and tutorials.\n\nYou may download a preprocessed 10X Multiome demo dataset [here](https://figshare.com/s/4c8e72cbb188d8e1cce8).\n\nA GPU is not required for small datasets, but is strongly recommmended above 1,000 cells. On CPU, the [cell lines demo](https://mowgli.readthedocs.io/en/latest/vignettes/Liu%20cell%20lines.html) (206 cells) should run in under 5 minutes and the [PBMC demo](https://mowgli.readthedocs.io/en/latest/vignettes/PBMC.html) (500 cells) should run in under 10 minutes (tested on a Ubuntu 20.04 machine with an 11th gen i7 processor).\n\n```python\nimport mowgli\nimport mudata as md\nimport scanpy as sc\n\n# Load data into a Muon object.\nmdata = md.read_h5mu("my_data.h5mu")\n\n# Initialize and train the model.\nmodel = mowgli.models.MowgliModel(latent_dim=15)\nmodel.train(mdata)\n\n# Visualize the embedding with UMAP.\nsc.pp.neighbors(mdata, use_rep="W_OT")\nsc.tl.umap(mdata)\nsc.pl.umap(mdata)\n```\n\n## Our preprint\n\n```bibtex\n@article{huizing2023paired,\n  title={Paired single-cell multi-omics data integration with Mowgli},\n  author={Huizing, Geert-Jan and Deutschmann, Ina Maria and Peyre, Gabriel and Cantini, Laura},\n  journal={bioRxiv},\n  pages={2023--02},\n  year={2023},\n  publisher={Cold Spring Harbor Laboratory}\n}\n```\n\nIf you\'re looking for the repository with code to reproduce the experiments in our preprint, [here is is!](https://github.com/cantinilab/mowgli_reproducibility)\n',
     'author': 'Geert-Jan Huizing',
     'author_email': 'huizing@ens.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mowgli-0.2.0/PKG-INFO` & `mowgli-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 Metadata-Version: 2.1
 Name: mowgli
-Version: 0.2.0
+Version: 0.3.0
 Summary: Mowgli is a novel method for the integration of paired multi-omics data with any type and number of omics, combining integrative Nonnegative Matrix Factorization and Optimal Transport.
 License: GPL-3.0-only
 Author: Geert-Jan Huizing
 Author-email: huizing@ens.fr
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: full
 Requires-Dist: anndata (>=0.8.0,<0.9.0)
 Requires-Dist: furo (>=2022.12.7,<2023.0.0) ; extra == "docs"
 Requires-Dist: gprofiler-official (>=1.0.0,<2.0.0) ; extra == "full"
 Requires-Dist: leidenalg (>=0.9.1,<0.10.0) ; extra == "full"
 Requires-Dist: matplotlib (>=3.0.0,<4.0.0)
 Requires-Dist: mudata (>=0.2.1,<0.3.0)
 Requires-Dist: nbsphinx (>=0.8.12,<0.9.0) ; extra == "docs"
 Requires-Dist: numpy (>=1.0.0,<2.0.0)
+Requires-Dist: pre-commit (>=3.1.1,<4.0.0) ; extra == "dev"
 Requires-Dist: scanpy (>=1.0.0,<2.0.0)
 Requires-Dist: scikit-learn (>=1.0.0,<2.0.0)
 Requires-Dist: scipy (>=1.0.0,<2.0.0)
 Requires-Dist: torch (>=1.0.0,<2.0.0)
 Requires-Dist: tqdm (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Mowgli: Multi Omics Wasserstein inteGrative anaLysIs
 [![Tests](https://github.com/gjhuizing/Mowgli/actions/workflows/main.yml/badge.svg)](https://github.com/gjhuizing/Mowgli/actions/workflows/main.yml)
-[![codecov](https://codecov.io/gh/gjhuizing/Mowgli/branch/main/graph/badge.svg?token=UBUJF7098Q)](https://codecov.io/gh/gjhuizing/Mowgli)
+[![codecov](https://codecov.io/gh/cantinilab/Mowgli/branch/main/graph/badge.svg?token=UBUJF7098Q)](https://codecov.io/gh/cantinilab/Mowgli)
 [![Documentation Status](https://readthedocs.org/projects/mowgli/badge/?version=latest)](https://mowgli.readthedocs.io/en/latest/?badge=latest)
-[![PyPI version](https://badge.fury.io/py/mowgli.svg)](https://badge.fury.io/py/mowgli)
+[![PyPI version](https://img.shields.io/pypi/v/mowgli?color=blue)](https://img.shields.io/pypi/v/mowgli?color=blue)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Mowgli is a novel method for the integration of paired multi-omics data with any type and number of omics, combining integrative Nonnegative Matrix Factorization and Optimal Transport. [Read the preprint!](https://www.biorxiv.org/content/10.1101/2023.02.02.526825v2)
 
 ![figure](figure.png)
 
 ## Install the package
 
@@ -60,15 +63,15 @@
 
 ## Getting started
 
 Mowgli takes as an input a Muon object and populates its `obsm` and `uns` fiels with the embeddings and dictionaries, respectively. Visit [mowgli.rtfd.io](https://mowgli.rtfd.io/) for more documentation and tutorials.
 
 You may download a preprocessed 10X Multiome demo dataset [here](https://figshare.com/s/4c8e72cbb188d8e1cce8).
 
-A GPU is not required for small datasets, but is strongly recommmended above 1,000 cells. On CPU, the [cell lines demo](https://mowgli.readthedocs.io/en/latest/vignettes/Liu%20cell%20lines.html) (206 cells) should run in under 5 minutes and the [PBMC demo](https://mowgli.readthedocs.io/en/latest/vignettes/PBMC.html) (500 cells) should run in under 10 minutes.
+A GPU is not required for small datasets, but is strongly recommmended above 1,000 cells. On CPU, the [cell lines demo](https://mowgli.readthedocs.io/en/latest/vignettes/Liu%20cell%20lines.html) (206 cells) should run in under 5 minutes and the [PBMC demo](https://mowgli.readthedocs.io/en/latest/vignettes/PBMC.html) (500 cells) should run in under 10 minutes (tested on a Ubuntu 20.04 machine with an 11th gen i7 processor).
 
 ```python
 import mowgli
 import mudata as md
 import scanpy as sc
 
 # Load data into a Muon object.
```

