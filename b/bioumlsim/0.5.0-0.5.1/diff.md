# Comparing `tmp/bioumlsim-0.5.0.tar.gz` & `tmp/bioumlsim-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioumlsim-0.5.0.tar", last modified: Fri Jun 23 13:06:52 2023, max compression
+gzip compressed data, was "bioumlsim-0.5.1.tar", last modified: Mon Jun 26 18:49:54 2023, max compression
```

## Comparing `bioumlsim-0.5.0.tar` & `bioumlsim-0.5.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 13:06:52.510912 bioumlsim-0.5.0/
--rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.5.0/LICENSE
--rw-rw-rw-   0        0        0      771 2023-06-23 13:06:52.511931 bioumlsim-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 13:06:52.408338 bioumlsim-0.5.0/bioumlsim/
--rw-rw-rw-   0        0        0     5166 2023-06-23 12:58:48.000000 bioumlsim-0.5.0/bioumlsim/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 13:06:52.507335 bioumlsim-0.5.0/bioumlsim/jars/
--rw-rw-rw-   0        0        0   386547 2023-05-26 08:30:49.000000 bioumlsim-0.5.0/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar
--rw-rw-rw-   0        0        0   615951 2023-05-26 08:30:49.000000 bioumlsim-0.5.0/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar
--rw-rw-rw-   0        0        0  2085692 2023-05-26 08:30:49.000000 bioumlsim-0.5.0/bioumlsim/jars/biouml.workbench_0.9.10.jar
--rw-rw-rw-   0        0        0   581945 2023-05-26 08:30:49.000000 bioumlsim-0.5.0/bioumlsim/jars/colt.jar
--rw-rw-rw-   0        0        0   396595 2023-05-26 08:30:49.000000 bioumlsim-0.5.0/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar
--rw-rw-rw-   0        0        0    94331 2023-05-26 08:30:48.000000 bioumlsim-0.5.0/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar
--rw-rw-rw-   0        0        0    31222 2023-05-26 08:30:49.000000 bioumlsim-0.5.0/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar
--rw-rw-rw-   0        0        0   575606 2023-05-26 08:30:49.000000 bioumlsim-0.5.0/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar
--rw-rw-rw-   0        0        0   262026 2023-05-26 08:30:48.000000 bioumlsim-0.5.0/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar
--rw-rw-rw-   0        0        0   421287 2023-05-26 08:30:49.000000 bioumlsim-0.5.0/bioumlsim/jars/org.apache.velocity_1.6.2.jar
--rw-rw-rw-   0        0        0    58013 2023-05-26 08:30:48.000000 bioumlsim-0.5.0/bioumlsim/jars/org.json-20170516.jar
--rw-rw-rw-   0        0        0  1251757 2023-05-26 08:30:49.000000 bioumlsim-0.5.0/bioumlsim/jars/ru.biosoft.access_0.9.10.jar
--rw-rw-rw-   0        0        0    14541 2023-05-26 08:30:49.000000 bioumlsim-0.5.0/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar
--rw-rw-rw-   0        0        0   231950 2023-05-26 08:30:48.000000 bioumlsim-0.5.0/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar
--rw-rw-rw-   0        0        0   197773 2023-05-26 08:30:48.000000 bioumlsim-0.5.0/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar
--rw-rw-rw-   0        0        0    26578 2023-05-26 08:30:49.000000 bioumlsim-0.5.0/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar
--rw-rw-rw-   0        0        0   163699 2023-05-26 08:30:48.000000 bioumlsim-0.5.0/bioumlsim/jars/ru.biosoft.math_0.9.10.jar
--rw-rw-rw-   0        0        0    20343 2023-05-26 08:30:49.000000 bioumlsim-0.5.0/bioumlsim/jars/src.jar
--rw-rw-rw-   0        0        0   299064 2023-05-26 08:30:49.000000 bioumlsim-0.5.0/bioumlsim/jars/streamex-0.7.0.jar
--rw-rw-rw-   0        0        0      323 2023-05-30 05:53:42.000000 bioumlsim-0.5.0/bioumlsim/test.py
--rw-rw-rw-   0        0        0     1496 2023-05-30 07:46:26.000000 bioumlsim-0.5.0/bioumlsim/test.xml
-drwxrwxrwx   0        0        0        0 2023-06-23 13:06:52.433598 bioumlsim-0.5.0/bioumlsim.egg-info/
--rw-rw-rw-   0        0        0      771 2023-06-23 13:06:52.000000 bioumlsim-0.5.0/bioumlsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1134 2023-06-23 13:06:52.000000 bioumlsim-0.5.0/bioumlsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 13:06:52.000000 bioumlsim-0.5.0/bioumlsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-23 13:06:51.000000 bioumlsim-0.5.0/bioumlsim.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2023-06-23 13:06:52.000000 bioumlsim-0.5.0/bioumlsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-23 13:06:52.000000 bioumlsim-0.5.0/bioumlsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      185 2023-05-27 18:48:00.000000 bioumlsim-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0      895 2023-06-23 13:06:52.525250 bioumlsim-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 18:49:54.169586 bioumlsim-0.5.1/
+-rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0      771 2023-06-26 18:49:54.169586 bioumlsim-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 18:49:54.019773 bioumlsim-0.5.1/bioumlsim/
+-rw-rw-rw-   0        0        0     6237 2023-06-26 18:34:34.000000 bioumlsim-0.5.1/bioumlsim/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:49:54.164537 bioumlsim-0.5.1/bioumlsim/jars/
+-rw-rw-rw-   0        0        0   386547 2023-05-26 08:30:49.000000 bioumlsim-0.5.1/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar
+-rw-rw-rw-   0        0        0   615951 2023-05-26 08:30:49.000000 bioumlsim-0.5.1/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar
+-rw-rw-rw-   0        0        0  2085692 2023-05-26 08:30:49.000000 bioumlsim-0.5.1/bioumlsim/jars/biouml.workbench_0.9.10.jar
+-rw-rw-rw-   0        0        0   581945 2023-05-26 08:30:49.000000 bioumlsim-0.5.1/bioumlsim/jars/colt.jar
+-rw-rw-rw-   0        0        0   396595 2023-05-26 08:30:49.000000 bioumlsim-0.5.1/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar
+-rw-rw-rw-   0        0        0    94331 2023-05-26 08:30:48.000000 bioumlsim-0.5.1/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar
+-rw-rw-rw-   0        0        0    31222 2023-05-26 08:30:49.000000 bioumlsim-0.5.1/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar
+-rw-rw-rw-   0        0        0   575606 2023-05-26 08:30:49.000000 bioumlsim-0.5.1/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar
+-rw-rw-rw-   0        0        0   262026 2023-05-26 08:30:48.000000 bioumlsim-0.5.1/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar
+-rw-rw-rw-   0        0        0   421287 2023-05-26 08:30:49.000000 bioumlsim-0.5.1/bioumlsim/jars/org.apache.velocity_1.6.2.jar
+-rw-rw-rw-   0        0        0    58013 2023-05-26 08:30:48.000000 bioumlsim-0.5.1/bioumlsim/jars/org.json-20170516.jar
+-rw-rw-rw-   0        0        0  1251757 2023-05-26 08:30:49.000000 bioumlsim-0.5.1/bioumlsim/jars/ru.biosoft.access_0.9.10.jar
+-rw-rw-rw-   0        0        0    14541 2023-05-26 08:30:49.000000 bioumlsim-0.5.1/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar
+-rw-rw-rw-   0        0        0   231950 2023-05-26 08:30:48.000000 bioumlsim-0.5.1/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar
+-rw-rw-rw-   0        0        0   197773 2023-05-26 08:30:48.000000 bioumlsim-0.5.1/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar
+-rw-rw-rw-   0        0        0    26578 2023-05-26 08:30:49.000000 bioumlsim-0.5.1/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar
+-rw-rw-rw-   0        0        0   163699 2023-05-26 08:30:48.000000 bioumlsim-0.5.1/bioumlsim/jars/ru.biosoft.math_0.9.10.jar
+-rw-rw-rw-   0        0        0    20343 2023-05-26 08:30:49.000000 bioumlsim-0.5.1/bioumlsim/jars/src.jar
+-rw-rw-rw-   0        0        0   299064 2023-05-26 08:30:49.000000 bioumlsim-0.5.1/bioumlsim/jars/streamex-0.7.0.jar
+-rw-rw-rw-   0        0        0      323 2023-05-30 05:53:42.000000 bioumlsim-0.5.1/bioumlsim/test.py
+-rw-rw-rw-   0        0        0     1496 2023-05-30 07:46:26.000000 bioumlsim-0.5.1/bioumlsim/test.xml
+drwxrwxrwx   0        0        0        0 2023-06-26 18:49:54.076069 bioumlsim-0.5.1/bioumlsim.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-06-26 18:49:53.000000 bioumlsim-0.5.1/bioumlsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1134 2023-06-26 18:49:53.000000 bioumlsim-0.5.1/bioumlsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 18:49:53.000000 bioumlsim-0.5.1/bioumlsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-26 18:49:52.000000 bioumlsim-0.5.1/bioumlsim.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2023-06-26 18:49:53.000000 bioumlsim-0.5.1/bioumlsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-26 18:49:53.000000 bioumlsim-0.5.1/bioumlsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      185 2023-05-27 18:48:00.000000 bioumlsim-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0      895 2023-06-26 18:49:54.188758 bioumlsim-0.5.1/setup.cfg
```

### Comparing `bioumlsim-0.5.0/LICENSE` & `bioumlsim-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/PKG-INFO` & `bioumlsim-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bioumlsim-0.5.0/bioumlsim/__init__.py` & `bioumlsim-0.5.1/bioumlsim/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,68 +14,96 @@
     rtol = 1E-8
     engine = None
 
     def getJVMVersion(self):
         return '.'.join(map(str, jpype.getJVMVersion()))
         
     def checkJDKVersion(self, release):
+        if not os.path.isfile(release):
+            return False
         f = open(release,'r')
         lines = f.readlines()
         for line in lines :
             if line.startswith('JAVA_VERSION=\"1.8') or line.startswith('JAVA_VERSION=\"11'):
                 return True
         return False
-      
+    
+    def isMac(self):
+        systemName = platform.system()
+        if systemName == 'Windows' or systemName == 'Linux':
+            return False
+        return True
+  
     def findJDK(self):
         jdkBasePath = ospath.join(ospath.expanduser("~"), ".jdk")
+        if self.isMac():
+            jdkBasePath = ospath.join(jdkBasePath,'Contents','Home')
+        print(jdkBasePath)
+        if not os.path.isdir(jdkBasePath):
+            print('Can not find appropriate JDK in '+jdkBasePath)
+            return ''              
         for name in os.listdir(jdkBasePath):
-            jdkPath = jdkBasePath+'/'+name
-            if os.path.isdir(jdkPath) and self.checkJDKVersion(jdkPath+'/release'):
+            print("NAME: "+name)
+            jdkPath = ospath.join(jdkBasePath,name)
+            print("BASE "+jdkBasePath)
+            print("Look for JDK at "+jdkPath)
+            if ospath.isdir(jdkPath) and self.checkJDKVersion(ospath.join(jdkPath,'release')):
                 return jdkPath
         print('Can not find appropriate JDK in '+jdkBasePath)
         return '' 
          
     def findJVM(self, possiblePathes, jdkLocation = ''):
         jdk = jdkLocation
         if jdk == '':
             jdk = self.findJDK()
+        print('JDK found at' + jdk)
         for possiblePath in possiblePathes:
-            jvm = jdk+possiblePath;
-            if os.path.isfile(jvm):
+            print("JDK "+jdk+", PATH "+possiblePath)
+            print("Look at "+ospath.join(jdk,possiblePath))
+            jvm = ospath.join(jdk,possiblePath)
+            if ospath.isfile(jvm):
                 return jvm;
         print('Can not find appropriate JVM. Please install 1.8 or 11 Java')
         return '' 
     
     def guessJVMLocations(self):
         systemName = platform.system()
         if systemName == 'Windows':
-            return ['/jre/bin/server/jvm.dll','/bin/server/jvm.dll']
+            return ['jre/bin/server/jvm.dll','bin/server/jvm.dll']
         elif systemName == 'Linux':
-            return ['/lib/server/libjvm.so','/jre/lib/amd64/server/libjvm.so']
+            return ['lib/server/libjvm.so','jre/lib/amd64/server/libjvm.so']
         else:
-            return ['/Contents/Home/jre/lib/server/libjvm.dylib', '/Contents/Home/lib/server/libjvm.dylib',
-                    '/Contents/MacOS/libjli.dylib','/Contents/Home/jre/lib/jli/libjvm.dylib']
+            return ['jre/lib/server/libjvm.dylib', 'lib/server/libjvm.dylib',
+                    'jre/lib/jli/libjvm.dylib']
     
     def isJavaSet(self):
          try:
              p = subprocess.check_output(["java", "-version"], stderr=subprocess.STDOUT)
              version = str(p.splitlines()[0].split()[-1])[3:]
              return version.startswith('1.8') or version.startswith('11')
          except FileNotFoundError:
              return False 
+    
+    def isJavaHomeSet(self):
+        try:
+            os.environ['JAVA_HOME']
+            print('Java home: '+os.environ['JAVA_HOME'])
+            return True
+        except KeyError:
+            return False
      
     def __init__(self, jdk = ''):
-        path = os.path.dirname(__file__)+'/jars'
+        path = ospath.join(ospath.dirname(__file__),'jars')
         self.bioUMLPath = path
         jvmPath = ''
         possiblePathes = self.guessJVMLocations()
         if jdk != '':
             jvmPath = self.findJVM(possiblePathes, jdkLocation = jdk)
             print('JVM is starting up on given path '+jvmPath)
-        elif self.isJavaSet():    
+        elif self.isJavaSet() and self.isJavaHomeSet():    
             print('JVM is starting on path provided by system')
         else:
             jvmPath = self.findJVM(possiblePathes)
             print('JVM is starting, will try to find jvm automatically: '+ jvmPath) 
         if jvmPath == '':
            jpype.startJVM(classpath=[path+'/*'], convertStrings=True)
         else :
@@ -91,27 +119,28 @@
             model
         """
         if (verbose):
              print(f"SBML file is loading: {file}")
         diagram = jpype.JClass("biouml.plugins.sbml.SbmlModelFactory").readDiagram(file, False)
         self.engine = jpype.JClass("biouml.plugins.simulation.java.JavaSimulationEngine")()
         self.engine.setDiagram(diagram)
-        self.engine.setClassPath(self.bioUMLPath +'/src.jar')
+        print(ospath.join(self.bioUMLPath,'src.jar'))
+        self.engine.setClassPath(ospath.join(self.bioUMLPath,'src.jar'))
         self.engine.disableLog()
         self.engine.setAbsTolerance(self.atol)
         self.engine.setRelTolerance(self.rtol)
         return Model(self.engine, self.engine.createModel())
     
     def plot(self, df):
         import matplotlib.pyplot as plt
         plt.plot(df)
         plt.show()
     
     def loadTest(self):
-        path = os.path.dirname(__file__)+'/test.xml'
+        path = ospath.join(ospath.dirname(__file__),'test.xml')
         return self.load(path)
          
 class Model:
     
     def __init__(self, engine, model):
         self.engine = engine
         self.model = model
```

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar` & `bioumlsim-0.5.1/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar` & `bioumlsim-0.5.1/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/biouml.workbench_0.9.10.jar` & `bioumlsim-0.5.1/bioumlsim/jars/biouml.workbench_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/colt.jar` & `bioumlsim-0.5.1/bioumlsim/jars/colt.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar` & `bioumlsim-0.5.1/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar` & `bioumlsim-0.5.1/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar` & `bioumlsim-0.5.1/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar` & `bioumlsim-0.5.1/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar` & `bioumlsim-0.5.1/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/org.apache.velocity_1.6.2.jar` & `bioumlsim-0.5.1/bioumlsim/jars/org.apache.velocity_1.6.2.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/org.json-20170516.jar` & `bioumlsim-0.5.1/bioumlsim/jars/org.json-20170516.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/ru.biosoft.access_0.9.10.jar` & `bioumlsim-0.5.1/bioumlsim/jars/ru.biosoft.access_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar` & `bioumlsim-0.5.1/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar` & `bioumlsim-0.5.1/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar` & `bioumlsim-0.5.1/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar` & `bioumlsim-0.5.1/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/ru.biosoft.math_0.9.10.jar` & `bioumlsim-0.5.1/bioumlsim/jars/ru.biosoft.math_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/src.jar` & `bioumlsim-0.5.1/bioumlsim/jars/src.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/jars/streamex-0.7.0.jar` & `bioumlsim-0.5.1/bioumlsim/jars/streamex-0.7.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim/test.xml` & `bioumlsim-0.5.1/bioumlsim/test.xml`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/bioumlsim.egg-info/PKG-INFO` & `bioumlsim-0.5.1/bioumlsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bioumlsim-0.5.0/bioumlsim.egg-info/SOURCES.txt` & `bioumlsim-0.5.1/bioumlsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.5.0/setup.cfg` & `bioumlsim-0.5.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 696f 756d 6c73 696d 0d0a 7665   = bioumlsim..ve
-00000020: 7273 696f 6e20 3d20 302e 352e 300d 0a61  rsion = 0.5.0..a
+00000020: 7273 696f 6e20 3d20 302e 352e 310d 0a61  rsion = 0.5.1..a
 00000030: 7574 686f 7220 3d20 496c 7961 204b 6973  uthor = Ilya Kis
 00000040: 656c 6576 2c20 4269 6f73 6f66 742e 7275  elev, Biosoft.ru
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2034 7833 6375 7430 7240 676d 6169 6c2e   4x3cut0r@gmail.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2050 7974 686f 6e20 696e 7465 7266   = Python interf
 00000090: 6163 6520 666f 7220 7369 6d75 6c61 7469  ace for simulati
```

