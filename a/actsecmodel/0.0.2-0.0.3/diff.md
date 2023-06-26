# Comparing `tmp/actsecmodel-0.0.2.tar.gz` & `tmp/actsecmodel-0.0.3.tar.gz`

## Comparing `actsecmodel-0.0.2.tar` & `actsecmodel-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actsecmodel-0.0.2/src/actsecmodel/__init__.py
--rw-r--r--   0        0        0    11678 2020-02-02 00:00:00.000000 actsecmodel-0.0.2/src/actsecmodel/actsecmodel.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 actsecmodel-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 actsecmodel-0.0.2/README.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 actsecmodel-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8936 2020-02-02 00:00:00.000000 actsecmodel-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 actsecmodel-0.0.3/src/actsecmodel/__init__.py
+-rw-r--r--   0        0        0    11678 2020-02-02 00:00:00.000000 actsecmodel-0.0.3/src/actsecmodel/actsecmodel.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 actsecmodel-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 actsecmodel-0.0.3/README.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 actsecmodel-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8936 2020-02-02 00:00:00.000000 actsecmodel-0.0.3/PKG-INFO
```

### Comparing `actsecmodel-0.0.2/src/actsecmodel/actsecmodel.py` & `actsecmodel-0.0.3/src/actsecmodel/actsecmodel.py`

 * *Files identical despite different names*

### Comparing `actsecmodel-0.0.2/LICENSE.txt` & `actsecmodel-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `actsecmodel-0.0.2/README.md` & `actsecmodel-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -29,99 +29,99 @@
 I used matplotlib and Gephi for all the graphing and visuals. A tutorial for the 95% confidence elipses is under this link https://matplotlib.org/stable/gallery/statistics/confidence_ellipse.html, since that took me longer to find on account of being in the examples section of the documentation, rather than the reference. 
 
 
 # FUNCTION DOCUMENTATION
 
 ### ACTIVATION FUNCTIONS
 
-##### activation(binsList):
+***activation(binsList):***
 
 A fucntion that choses an actor for activation. 
 - *binslist.* A list containing the probability bins for each actor to fall into. Each item in the list should be the cumulative probability of the respective actor being chosen. 
 - RETURNS: The integer index of the actor chosen for activation (in my program, each actor was assigned a number from 0 upwards, so this index was also the actor's ID, and later code relfects this. The same was not true for comments)
 
-##### uniform_bins(n):
+***uniform_bins(n):***
 
 A fucntion that creates the binsList for uniform activation.
 - *n.* The number of actors. 
 - RETURNS: The list binsList for uniform activation
 
-##### zipfs_bins(n, s):
+***zipfs_bins(n, s):***
 
 A fucntion that creates the binsList for Zipf's Law activation.
 - *n.* The number of actors. 
 - *s.* The Zipf's constant. 
 - RETURNS: The list binsList for Zipf's Law activation
 
 
 ### SELECTION FUNCTIONS
 
-##### uniform_selection(allCurrentComments):
+***uniform_selection(allCurrentComments):***
 
 A function for choosing a comment with uniform selection. 
 - *allCurrentComments.* A list containing all comments that have currently been made
 - RETURNS: The integer index of the comment chosen for selection
 
-##### barabasi_albert_selection(commentNetwork, allCurrentComments):
+***barabasi_albert_selection(commentNetwork, allCurrentComments):***
 
 A function for choosing a comment with Barabasi-Albert selection. 
 - *commentNetwork.* The discussion layer of the current NetworkX network
 - *allCurrentComments.* A list containing all comments that have currently been made
 - RETURNS: The integer index of the comment chosen for selection
 
-##### bianconi_barabasi_layer_selection(commentNetwork, allCurrentComments):
+***bianconi_barabasi_layer_selection(commentNetwork, allCurrentComments):***
 
 A function for choosing a comment with level selection. 
 - *commentNetwork.* The discussion layer of the current NetworkX network
 - *allCurrentComments.* A list containing all comments that have currently been made
 - RETURNS: The index of the comment chosen for selection
 
-##### bianconi_barabasi_recency_selection(commentNetwork, allCurrentComments):
+***bianconi_barabasi_recency_selection(commentNetwork, allCurrentComments):***
 
 A function for choosing a comment with recency selection. 
 - *commentNetwork.* The discussion layer of the current NetworkX network
 - *allCurrentComments.* A list containing all comments that have currently been made
 - RETURNS: The integer index of the comment chosen for selection
 
 
 ### GENERAL FUNCTIONS
 
-##### generalised_harmonic_sum(N,s):
+***generalised_harmonic_sum(N,s):***
 
 A function to find the generalised harmonic sum. 
 - *N.* The number of values to be summed over
 - *s.* The power of the denominator
 - RETURNS: The float value of the generalised harmonic sum over the first N terms. 
 
-##### initialise_lists(nActors, tSteps):
+***initialise_lists(nActors, tSteps):***
 
 A function to initialise the actor and comments lists for a predetermined number of actors and comments. 
 - *nActors.* The total number of actors
 - *tSteps.* The total number of timesteps (and thus total number of comments)
 - RETURNS: The actor and comments lists, in that order, separated by a comma. 
 
-##### iterate_reddit_network(currentTimeStep, adjacencyMatrix, activatedActor, selectedCommentValue, commentOwnersList, commentsList):
+***iterate_reddit_network(currentTimeStep, adjacencyMatrix, activatedActor, selectedCommentValue, commentOwnersList, commentsList):***
 
 A function that receives the activated actor and selected commennt and updates the adjacency matrix accordingly.
 - *currentTimeStep.* An integer for the current timestep
 - *adjacencyMatrix.* The current adjacency matrix for the multilayer network
 - *activatedActor.* The actor chosen for activation. In my case, the index and actor ID were identical, so I simply fed in the index
 - *selectedCommentValue.* The index in the commentsList for the selected comment
 - *commentOwnersList.* The list of comment owners (see top)
 - *commentsList.* The commentsList list representing the list of all comments
 - RETURNS: The updated adjacency matrix. 
 
-##### width_and_depth(rootNode, commentsGraph):
+***width_and_depth(rootNode, commentsGraph):***
 
 A function to find the mean and maximum width and depth measures from a discussion layer graph. 
 - *rootNode.* The root node/initial post of the discussion layer graph. 
 - *commentsGraph.* The NetworkX graph for the discussion layer. 
 - RETURNS: The following list: [maxWidth, meanWidth, maxDepth, meanDepth]
 
-##### standard_actsecmodel(tSteps, nActors, aBinsList, selectionType):
+***standard_actsecmodel(tSteps, nActors, aBinsList, selectionType):***
 
 The function I used in my model, that completely iterates through a set number of timesteps, for a set number of actors, for the activation and selection types available in this package. 
 - *tStepss.* The number of timesteps to run for. 
 - *nActors.* The number of actors in the actor layer (note that not all actors may participate)
 - *aBinsList.* The binsList list for the activation type being used 
 - *selectionType.* A string to determine which selection type to be used, choosing from 'uniform', 'barabsi', 'layer', or 'recency'
 - RETURNS: The following list: [maxWidth, meanWidth, maxDepth, meanDepth, developmentArray, cliques, transitivity, reciprocity, clustering, actorDevelopmentArray]. The maxWidth, meanWidth, maxDepth, meanDepth, cliques, transitivity, reciprocity, and clustering measures are all terminal. developmentArray is a Numpy array that contains the development of the discussion layer measures over time. actorDevelopmentArray is a Numpy array that contains the development of the actor layer measures over time.
```

### Comparing `actsecmodel-0.0.2/pyproject.toml` & `actsecmodel-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "actsecmodel"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Aiden Littlewood-Johnson", email="aidenlittlewoodjohnson@gmail.com" },
 ]
 description = "A package designed to be used to research the development of multilayer Reddit discussion networks"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `actsecmodel-0.0.2/PKG-INFO` & `actsecmodel-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actsecmodel
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package designed to be used to research the development of multilayer Reddit discussion networks
 Author-email: Aiden Littlewood-Johnson <aidenlittlewoodjohnson@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -41,99 +41,99 @@
 I used matplotlib and Gephi for all the graphing and visuals. A tutorial for the 95% confidence elipses is under this link https://matplotlib.org/stable/gallery/statistics/confidence_ellipse.html, since that took me longer to find on account of being in the examples section of the documentation, rather than the reference. 
 
 
 # FUNCTION DOCUMENTATION
 
 ### ACTIVATION FUNCTIONS
 
-##### activation(binsList):
+***activation(binsList):***
 
 A fucntion that choses an actor for activation. 
 - *binslist.* A list containing the probability bins for each actor to fall into. Each item in the list should be the cumulative probability of the respective actor being chosen. 
 - RETURNS: The integer index of the actor chosen for activation (in my program, each actor was assigned a number from 0 upwards, so this index was also the actor's ID, and later code relfects this. The same was not true for comments)
 
-##### uniform_bins(n):
+***uniform_bins(n):***
 
 A fucntion that creates the binsList for uniform activation.
 - *n.* The number of actors. 
 - RETURNS: The list binsList for uniform activation
 
-##### zipfs_bins(n, s):
+***zipfs_bins(n, s):***
 
 A fucntion that creates the binsList for Zipf's Law activation.
 - *n.* The number of actors. 
 - *s.* The Zipf's constant. 
 - RETURNS: The list binsList for Zipf's Law activation
 
 
 ### SELECTION FUNCTIONS
 
-##### uniform_selection(allCurrentComments):
+***uniform_selection(allCurrentComments):***
 
 A function for choosing a comment with uniform selection. 
 - *allCurrentComments.* A list containing all comments that have currently been made
 - RETURNS: The integer index of the comment chosen for selection
 
-##### barabasi_albert_selection(commentNetwork, allCurrentComments):
+***barabasi_albert_selection(commentNetwork, allCurrentComments):***
 
 A function for choosing a comment with Barabasi-Albert selection. 
 - *commentNetwork.* The discussion layer of the current NetworkX network
 - *allCurrentComments.* A list containing all comments that have currently been made
 - RETURNS: The integer index of the comment chosen for selection
 
-##### bianconi_barabasi_layer_selection(commentNetwork, allCurrentComments):
+***bianconi_barabasi_layer_selection(commentNetwork, allCurrentComments):***
 
 A function for choosing a comment with level selection. 
 - *commentNetwork.* The discussion layer of the current NetworkX network
 - *allCurrentComments.* A list containing all comments that have currently been made
 - RETURNS: The index of the comment chosen for selection
 
-##### bianconi_barabasi_recency_selection(commentNetwork, allCurrentComments):
+***bianconi_barabasi_recency_selection(commentNetwork, allCurrentComments):***
 
 A function for choosing a comment with recency selection. 
 - *commentNetwork.* The discussion layer of the current NetworkX network
 - *allCurrentComments.* A list containing all comments that have currently been made
 - RETURNS: The integer index of the comment chosen for selection
 
 
 ### GENERAL FUNCTIONS
 
-##### generalised_harmonic_sum(N,s):
+***generalised_harmonic_sum(N,s):***
 
 A function to find the generalised harmonic sum. 
 - *N.* The number of values to be summed over
 - *s.* The power of the denominator
 - RETURNS: The float value of the generalised harmonic sum over the first N terms. 
 
-##### initialise_lists(nActors, tSteps):
+***initialise_lists(nActors, tSteps):***
 
 A function to initialise the actor and comments lists for a predetermined number of actors and comments. 
 - *nActors.* The total number of actors
 - *tSteps.* The total number of timesteps (and thus total number of comments)
 - RETURNS: The actor and comments lists, in that order, separated by a comma. 
 
-##### iterate_reddit_network(currentTimeStep, adjacencyMatrix, activatedActor, selectedCommentValue, commentOwnersList, commentsList):
+***iterate_reddit_network(currentTimeStep, adjacencyMatrix, activatedActor, selectedCommentValue, commentOwnersList, commentsList):***
 
 A function that receives the activated actor and selected commennt and updates the adjacency matrix accordingly.
 - *currentTimeStep.* An integer for the current timestep
 - *adjacencyMatrix.* The current adjacency matrix for the multilayer network
 - *activatedActor.* The actor chosen for activation. In my case, the index and actor ID were identical, so I simply fed in the index
 - *selectedCommentValue.* The index in the commentsList for the selected comment
 - *commentOwnersList.* The list of comment owners (see top)
 - *commentsList.* The commentsList list representing the list of all comments
 - RETURNS: The updated adjacency matrix. 
 
-##### width_and_depth(rootNode, commentsGraph):
+***width_and_depth(rootNode, commentsGraph):***
 
 A function to find the mean and maximum width and depth measures from a discussion layer graph. 
 - *rootNode.* The root node/initial post of the discussion layer graph. 
 - *commentsGraph.* The NetworkX graph for the discussion layer. 
 - RETURNS: The following list: [maxWidth, meanWidth, maxDepth, meanDepth]
 
-##### standard_actsecmodel(tSteps, nActors, aBinsList, selectionType):
+***standard_actsecmodel(tSteps, nActors, aBinsList, selectionType):***
 
 The function I used in my model, that completely iterates through a set number of timesteps, for a set number of actors, for the activation and selection types available in this package. 
 - *tStepss.* The number of timesteps to run for. 
 - *nActors.* The number of actors in the actor layer (note that not all actors may participate)
 - *aBinsList.* The binsList list for the activation type being used 
 - *selectionType.* A string to determine which selection type to be used, choosing from 'uniform', 'barabsi', 'layer', or 'recency'
 - RETURNS: The following list: [maxWidth, meanWidth, maxDepth, meanDepth, developmentArray, cliques, transitivity, reciprocity, clustering, actorDevelopmentArray]. The maxWidth, meanWidth, maxDepth, meanDepth, cliques, transitivity, reciprocity, and clustering measures are all terminal. developmentArray is a Numpy array that contains the development of the discussion layer measures over time. actorDevelopmentArray is a Numpy array that contains the development of the actor layer measures over time.
```

