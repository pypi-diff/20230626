# Comparing `tmp/pygame_ecs-0.1.0.tar.gz` & `tmp/pygame_ecs-0.2.0.tar.gz`

## Comparing `pygame_ecs-0.1.0.tar` & `pygame_ecs-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/.gitattributes
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/pygame_ecs/__init__.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/pygame_ecs/entity.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/pygame_ecs/exceptions.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/pygame_ecs/components/base_component.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/pygame_ecs/managers/component_manager.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/pygame_ecs/managers/entity_manager.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/pygame_ecs/managers/system_manager.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/pygame_ecs/systems/base_system.py
--rw-r--r--   0        0        0    30680 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/test/circle.png
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/test/particle_test_cpu.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/test/particle_test_gpu.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/test/speed_test.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/test/tester.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/LICENSE
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/README.md
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 pygame_ecs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/.gitattributes
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/__init__.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/entity.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/exceptions.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/components/base_component.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/managers/component_manager.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/managers/entity_manager.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/managers/system_manager.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pygame_ecs/systems/base_system.py
+-rw-r--r--   0        0        0    30680 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/test/circle.png
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/test/draw_test.py
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/test/particle_test_cpu.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/test/particle_test_gpu.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/test/speed_test.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/test/tester.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/README.md
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 pygame_ecs-0.2.0/PKG-INFO
```

### Comparing `pygame_ecs-0.1.0/pygame_ecs/managers/component_manager.py` & `pygame_ecs-0.2.0/pygame_ecs/managers/component_manager.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.1.0/pygame_ecs/managers/entity_manager.py` & `pygame_ecs-0.2.0/pygame_ecs/managers/entity_manager.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.1.0/pygame_ecs/managers/system_manager.py` & `pygame_ecs-0.2.0/pygame_ecs/managers/system_manager.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.1.0/pygame_ecs/systems/base_system.py` & `pygame_ecs-0.2.0/pygame_ecs/systems/base_system.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.1.0/test/circle.png` & `pygame_ecs-0.2.0/test/circle.png`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.1.0/test/particle_test_cpu.py` & `pygame_ecs-0.2.0/test/particle_test_cpu.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.1.0/test/particle_test_gpu.py` & `pygame_ecs-0.2.0/test/particle_test_gpu.py`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.1.0/test/speed_test.py` & `pygame_ecs-0.2.0/test/speed_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,15 @@
 
 entities = []
 entity_manager = pygame_ecs.EntityManager()
 component_manager = pygame_ecs.ComponentManager()
 system_manager = pygame_ecs.SystemManager()
 ball_physics = BallPhysics()
 
-component_manager.add_component_type(Position)
-component_manager.add_component_type(Velocity)
+component_manager.init_components()
 
 for _ in range(ENTITY_AMOUNT):
     center = (
         random.randint(0, WIDTH),
         random.randint(0, HEIGHT),
     )
     radius = random.randint(2, 12)
```

### Comparing `pygame_ecs-0.1.0/.gitignore` & `pygame_ecs-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.1.0/LICENSE` & `pygame_ecs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame_ecs-0.1.0/pyproject.toml` & `pygame_ecs-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 
 [project]
 name = "pygame_ecs"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Notenlish", email="71970100+Notenlish@users.noreply.github.com" },
 ]
-description = "Pure Python, simple to use Entity Component System for pygame"
+description = "Pure Python, simple to use Entity Component System(ECS) for pygame"
 packages=["pygame_ecs", "pygame_ecs.components", "pygame_ecs.managers", "pygame_ecs.systems"]
 readme = "README.md"
 requires-python = ">=3.7"
 license="MIT"
 keywords = [
     "pygame",
     "ECS",
     "ecs",
     "pygame-ce",
     "entity",
     "component",
     "system",
     "entity component system",
+    "pygame_ecs"
 ]
 classifiers = [
-    "Development Status :: 3 - Alpha",  # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
+    "Development Status :: 5 - Production/Stable",  # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
```

