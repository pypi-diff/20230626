# Comparing `tmp/grassmanntn-1.0.tar.gz` & `tmp/grassmanntn-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grassmanntn-1.0.tar", last modified: Mon Jun 26 02:39:23 2023, max compression
+gzip compressed data, was "grassmanntn-1.1.tar", last modified: Mon Jun 26 03:26:24 2023, max compression
```

## Comparing `grassmanntn-1.0.tar` & `grassmanntn-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-06-26 02:39:23.347060 grassmanntn-1.0/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.0/LICENSE.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      728 2023-06-26 02:39:23.347060 grassmanntn-1.0/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     4373 2023-06-26 02:27:00.000000 grassmanntn-1.0/README.md
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-06-26 02:39:23.347060 grassmanntn-1.0/grassmanntn/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      107 2023-06-26 02:11:32.000000 grassmanntn-1.0/grassmanntn/__init__.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132851 2023-06-26 01:30:01.000000 grassmanntn-1.0/grassmanntn/gauge2d.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109643 2023-06-26 01:29:03.000000 grassmanntn-1.0/grassmanntn/grassmanntn.py
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.0/grassmanntn/param.py
-drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-06-26 02:39:23.347060 grassmanntn-1.0/grassmanntn.egg-info/
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      728 2023-06-26 02:39:23.000000 grassmanntn-1.0/grassmanntn.egg-info/PKG-INFO
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      309 2023-06-26 02:39:23.000000 grassmanntn-1.0/grassmanntn.egg-info/SOURCES.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-06-26 02:39:23.000000 grassmanntn-1.0/grassmanntn.egg-info/dependency_links.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-06-26 02:39:23.000000 grassmanntn-1.0/grassmanntn.egg-info/requires.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-06-26 02:39:23.000000 grassmanntn-1.0/grassmanntn.egg-info/top_level.txt
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-06-26 02:39:23.347060 grassmanntn-1.0/setup.cfg
--rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1678 2023-06-26 02:39:15.000000 grassmanntn-1.0/setup.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-06-26 03:26:24.741714 grassmanntn-1.1/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)    11357 2023-06-26 02:27:06.000000 grassmanntn-1.1/LICENSE.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      728 2023-06-26 03:26:24.741714 grassmanntn-1.1/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     4373 2023-06-26 02:27:00.000000 grassmanntn-1.1/README.md
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-06-26 03:26:24.741714 grassmanntn-1.1/grassmanntn/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      107 2023-06-26 02:11:32.000000 grassmanntn-1.1/grassmanntn/__init__.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   132612 2023-06-26 03:15:27.000000 grassmanntn-1.1/grassmanntn/gauge2d.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   109252 2023-06-26 03:15:02.000000 grassmanntn-1.1/grassmanntn/grassmanntn.py
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)   693592 2023-05-29 12:33:44.000000 grassmanntn-1.1/grassmanntn/param.py
+drwxrwxr-x   0 ayosp     (1000) ayosp     (1000)        0 2023-06-26 03:26:24.741714 grassmanntn-1.1/grassmanntn.egg-info/
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      728 2023-06-26 03:26:24.000000 grassmanntn-1.1/grassmanntn.egg-info/PKG-INFO
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)      309 2023-06-26 03:26:24.000000 grassmanntn-1.1/grassmanntn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)        1 2023-06-26 03:26:24.000000 grassmanntn-1.1/grassmanntn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       24 2023-06-26 03:26:24.000000 grassmanntn-1.1/grassmanntn.egg-info/requires.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       12 2023-06-26 03:26:24.000000 grassmanntn-1.1/grassmanntn.egg-info/top_level.txt
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)       79 2023-06-26 03:26:24.741714 grassmanntn-1.1/setup.cfg
+-rw-rw-r--   0 ayosp     (1000) ayosp     (1000)     1678 2023-06-26 03:26:18.000000 grassmanntn-1.1/setup.py
```

### Comparing `grassmanntn-1.0/LICENSE.txt` & `grassmanntn-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.0/PKG-INFO` & `grassmanntn-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.0
+Version: 1.1
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_10.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_11.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.0/README.md` & `grassmanntn-1.1/README.md`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.0/grassmanntn/gauge2d.py` & `grassmanntn-1.1/grassmanntn/gauge2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,20 +63,14 @@
     return T, trace_error
 
 def myQuadrature(beta, Nf, npoints):
         
     xi = np.array( [ i*2*np.pi/npoints           for i in range(npoints) ] )
     wi = np.array( [ (2*np.pi/npoints)**(1.0/Nf) for i in range(npoints) ] )
 
-    #xi = np.zeros([npoints],dtype=float)
-    #wi = np.zeros([npoints],dtype=float)
-    #for i in range(npoints):
-    #    xi[i] = i*2*np.pi/npoints #-np.pi + 2*np.pi*(i+0.5)/npoints
-    #    wi[i] = (2*np.pi/npoints)**(1.0/Nf)
-    
     return xi, wi
 
 def get_ABtensors(Nphi=2, beta=1, Nf=1, spacing=1, mass=1, charge=1, mu=1):
     Npsi = 16 #this value is probably always fixed to 16
     Bshape = (Npsi,Npsi,Npsi,Npsi,Nphi,Nphi,Nphi,Nphi)
     A = np.zeros([Nphi,Nphi,Nphi,Nphi],dtype=float)
     psi1 = []
@@ -1015,15 +1009,15 @@
     return A, B
 
 def fcompress_B(B,cutoff=64,mute=True):
 
     process_name = "B compression (1)"
     process_length = 16
     s00 = time.time()
-    print()
+    gtn.progress_space()
 
     if not mute:
         B.info("B (uncompressed)")
 
     # μ = 1 ===========================================================================
 
     step = 1
@@ -1098,27 +1092,27 @@
         U2 = Um.copy()
         cU2 = cUm.copy()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     B = gtn.einsum('JB,AJCLijkl->ABCLijkl',U2,B)
     B = gtn.einsum('DL,ABCLijkl->ABCDijkl',cU2,B)
     gtn.clear_progress()
-    sys.stdout.write("\033[F")
+    gtn.tab_up()
     
     if not mute:
         U2.info("U2")
 
     return B
 
 def compress_B(B,cutoff=64,mute=True):
 
     process_name = "B compression (2)"
     process_length = 4*8
     s00 = time.time()
-    print()
+    gtn.progress_space()
 
     Npsi = B.shape[0]
     Nphi = B.shape[4]
     δ = np.zeros([Nphi,Nphi],dtype=int)
     for i in range(Nphi):
         δ[i,i] = 1
     δ = gtn.sparse(δ,statistic=(0,0))
@@ -1273,30 +1267,30 @@
         U4 = Up.copy()
     else:
         U4 = Um.copy()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Bfin = gtn.einsum('ABCLl,DLl->ABCD',Bfin,U4.hconjugate('ij k'))
     gtn.clear_progress()
-    sys.stdout.write("\033[F")
+    gtn.tab_up()
     
     if not mute:
         U1.info("U4")
         Bfin.info("B (compressed)")
 
     return Bfin, [U1,U2,U3,U4]
 
 def compress_A(A,Upack,mute=True):
     
     [U1,U2,U3,U4] = Upack
 
     process_name = "A compression"
     process_length = 3
     s00 = time.time()
-    print()
+    gtn.progress_space()
 
     Nphi = A.shape[0]
     δ = np.zeros([Nphi,Nphi],dtype=int)
     for i in range(Nphi):
         δ[i,i] = 1
     δ = gtn.sparse(δ,statistic=(0,0))
 
@@ -1308,27 +1302,27 @@
     Ix = gtn.einsum('KXj,XjI->KIj',U1.hconjugate('ij k'),U3)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Iy = gtn.einsum('LYj,YjJ->LJj',U2.hconjugate('ij k'),U4)
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Afin = gtn.einsum('ijkl,KIl,LJk,km,ln->IJKLijklmn',A,Ix,Iy,δ,δ)
     gtn.clear_progress()
-    sys.stdout.write("\033[F")
+    gtn.tab_up()
 
     if not mute:
         Afin.info("A (compressed)")
 
     return Afin
 
 def compress_T(T,cutoff=64,mute=True):
 
     process_name = "T compression"
     process_length = 16
     s00 = time.time()
-    print()
+    gtn.progress_space()
 
     # x direction =====================================================================
 
     step = 1
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Txp = gtn.einsum('IJKLijklmn -> JKLjklmn Ii',T)
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
@@ -1392,15 +1386,15 @@
         U = Up.copy()
     else:
         U = Um.copy()
 
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",time=time.time()-s00)
     Tfin = gtn.einsum('ACJLjlmn,JjB,DLl->ABCDmn',Tfin,U,U.hconjugate('ij k'))
     gtn.clear_progress()
-    sys.stdout.write("\033[F")
+    gtn.tab_up()
 
     if not mute:
         Tfin.info("T (y-compression)")
 
     return Tfin
 
 ####################################################
@@ -1560,15 +1554,15 @@
     process_name = "atrg2d"+alignment
     if iternum != None:
         process_name = process_name+"["+str(iternum)+"]"
     process_length = 8
     process_color = "purple"
     step = 1
     s00 = time.time()
-    print() # << Don't remove this. This is for the gtn.show_progress!
+    gtn.progress_space() # << Don't remove this. This is for the gtn.show_progress!
 
     if intermediate_dcut==None:
         intermediate_dcut=dcut
 
     T1 = gtn.einsum("ijkl->li jk",T1)
     T2 = gtn.einsum("ijkl->li jk",T2)
 
@@ -1648,15 +1642,15 @@
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00)
     if error_test :
         Z1 = gtn.einsum('IJIK,iKiJ',T1ori,T2ori)
         Z2 = gtn.einsum('IJIJ',T)
         error = np.abs(1-Z2/Z1)
     
     gtn.clear_progress()
-    sys.stdout.write("\033[F")
+    gtn.tab_up()
     
     Tnorm = T.norm
     T.data = T.data/Tnorm
 
     if error_test :
         return T, Tnorm, error
     else :
@@ -1701,15 +1695,15 @@
     process_name = "hotrg3d"
     if iternum != None:
         process_name = process_name+"["+str(iternum)+"]"
     process_color = "purple"
     process_length = 38
     step = 1
     s00 = time.time()
-    print() # << Don't remove this. This is for the gtn.show_progress!
+    gtn.progress_space() # << Don't remove this. This is for the gtn.show_progress!
 
     if intermediate_dcut==None:
         intermediate_dcut=dcut
 
     #=================================================================================================
     step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00) #1
     T1 = gtn.einsum('i1 i2 i3 i4 mn-> i1 i3 mn i2 i4',T1)
@@ -1883,15 +1877,15 @@
         step = gtn.show_progress(step,process_length,process_name+" "+"<"+gtn.current_memory_display()+">",color=process_color,time=time.time()-s00) #37
         T = gtn.einsum(' t1 t3 kl m, n lk t2 t4 -> t1 t2 t3 t4 mn ',Xprime,Yprime)
         del Xprime.data,Yprime.data
         del Xprime,Yprime
         gc.collect()
     
     gtn.clear_progress()
-    sys.stdout.write("\033[F")
+    gtn.tab_up()
 
     if print_svd :
         Sx = np.sort(np.diag(Sx.force_format("matrix").data))[::-1]
         Sy = np.sort(np.diag(Sy.force_format("matrix").data))[::-1]
 
         Sxmax = 0
         for s in Sx:
```

### Comparing `grassmanntn-1.0/grassmanntn/grassmanntn.py` & `grassmanntn-1.1/grassmanntn/grassmanntn.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,888 +35,888 @@
 00000220: 6722 290d 0a66 6f72 6d61 745f 7479 7065  g")..format_type
 00000230: 203d 2028 2273 7461 6e64 6172 6422 2c22   = ("standard","
 00000240: 6d61 7472 6978 2229 0d0a 6e75 6d65 725f  matrix")..numer_
 00000250: 6375 746f 6666 203d 2031 2e30 652d 3134  cutoff = 1.0e-14
 00000260: 0d0a 6e75 6d65 725f 6469 7370 6c61 795f  ..numer_display_
 00000270: 6375 746f 6666 203d 2031 3030 302a 6e75  cutoff = 1000*nu
 00000280: 6d65 725f 6375 746f 6666 0d0a 6368 6172  mer_cutoff..char
-00000290: 5f6c 6973 7420 3d20 2822 6122 2c22 6222  _list = ("a","b"
-000002a0: 2c22 6322 2c22 6422 2c22 6522 2c22 6622  ,"c","d","e","f"
-000002b0: 2c22 6722 2c22 6822 2c22 6922 2c22 6a22  ,"g","h","i","j"
-000002c0: 2c22 6b22 2c22 6c22 2c22 6d22 2c22 6e22  ,"k","l","m","n"
-000002d0: 2c22 6f22 2c22 7022 2c22 7122 2c22 7222  ,"o","p","q","r"
-000002e0: 2c22 7322 2c22 7422 2c22 7522 2c22 7622  ,"s","t","u","v"
-000002f0: 2c22 7722 2c22 7822 2c22 7922 2c22 7a22  ,"w","x","y","z"
-00000300: 2c22 4122 2c22 4222 2c22 4322 2c22 4422  ,"A","B","C","D"
-00000310: 2c22 4522 2c22 4622 2c22 4722 2c22 4822  ,"E","F","G","H"
-00000320: 2c22 4922 2c22 4a22 2c22 4b22 2c22 4c22  ,"I","J","K","L"
-00000330: 2c22 4d22 2c22 4e22 2c22 4f22 2c22 5022  ,"M","N","O","P"
-00000340: 2c22 5122 2c22 5222 2c22 5322 2c22 5422  ,"Q","R","S","T"
-00000350: 2c22 5522 2c22 5622 2c22 5722 2c22 5822  ,"U","V","W","X"
-00000360: 2c22 5922 2c22 5a22 290d 0a0d 0a23 2323  ,"Y","Z")....###
-00000370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000390: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000003a0: 230d 0a23 2320 2020 2020 2020 2020 2020  #..##           
-000003b0: 2020 2020 2052 616e 646f 6d20 5574 696c       Random Util
-000003c0: 6974 6965 7320 2020 2020 2020 2020 2020  ities           
-000003d0: 2020 2020 2023 230d 0a23 2323 2323 2323       ##..#######
-000003e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000003f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000400: 2323 2323 2323 2323 2323 2323 230d 0a0d  #############...
-00000410: 0a64 6566 206d 616b 655f 7475 706c 6528  .def make_tuple(
-00000420: 6f62 6a29 3a0d 0a20 2020 2069 6620 6e70  obj):..    if np
-00000430: 2e69 7373 6361 6c61 7228 6f62 6a29 3a0d  .isscalar(obj):.
-00000440: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000450: 7475 706c 6528 5b6f 626a 5d29 0d0a 2020  tuple([obj])..  
-00000460: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00000470: 2072 6574 7572 6e20 7475 706c 6528 6c69   return tuple(li
-00000480: 7374 286f 626a 2929 0d0a 0d0a 6465 6620  st(obj))....def 
-00000490: 6d61 6b65 5f6c 6973 7428 6f62 6a29 3a0d  make_list(obj):.
-000004a0: 0a20 2020 2069 6620 6e70 2e69 7373 6361  .    if np.issca
-000004b0: 6c61 7228 6f62 6a29 3a0d 0a20 2020 2020  lar(obj):..     
-000004c0: 2020 2072 6574 7572 6e20 5b6f 626a 5d0d     return [obj].
-000004d0: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
-000004e0: 2020 2020 7265 7475 726e 206c 6973 7428      return list(
-000004f0: 6f62 6a29 0d0a 0d0a 6465 6620 6572 726f  obj)....def erro
-00000500: 7228 7465 7874 3d22 4572 726f 725b 5d3a  r(text="Error[]:
-00000510: 2055 6e6b 6e6f 776e 2065 7272 6f72 2e22   Unknown error."
-00000520: 293a 0d0a 2020 2020 7072 696e 7428 290d  ):..    print().
-00000530: 0a20 2020 2070 7269 6e74 2874 6578 7429  .    print(text)
-00000540: 0d0a 2020 2020 7072 696e 7428 290d 0a20  ..    print().. 
-00000550: 2020 2070 7269 6e74 2822 5c74 5f5f 5f5f     print("\t____
-00000560: 5f5f 5f5f 5f5f 6c6f 6f6b 5f62 656c 6f77  ______look_below
-00000570: 5f66 6f72 5f74 6865 5f65 7272 6f72 5f69  _for_the_error_i
-00000580: 6e66 6f72 6d61 7469 6f6e 5f5f 5f5f 5f5f  nformation______
-00000590: 5f5f 5f5f 2229 0d0a 2020 2020 2369 6e74  ____")..    #int
-000005a0: 656e 7469 6f6e 616c 2073 6162 6f74 6167  entional sabotag
-000005b0: 6521 2121 0d0a 2020 2020 5f5f 5f5f 5f5f  e!!!..    ______
-000005c0: 5f5f 5f5f 6c6f 6f6b 5f61 626f 7665 5f66  ____look_above_f
-000005d0: 6f72 5f74 6865 5f65 7272 6f72 5f69 6e66  or_the_error_inf
-000005e0: 6f72 6d61 7469 6f6e 5f5f 5f5f 5f5f 5f5f  ormation________
-000005f0: 5f5f 0d0a 0d0a 6465 6620 6765 745f 6368  __....def get_ch
-00000600: 6172 2873 7472 696e 6729 3a0d 0a20 2020  ar(string):..   
-00000610: 2066 6f72 2063 6861 7220 696e 2063 6861   for char in cha
-00000620: 725f 6c69 7374 3a0d 0a20 2020 2020 2020  r_list:..       
-00000630: 2069 6620 6368 6172 206e 6f74 2069 6e20   if char not in 
-00000640: 7374 7269 6e67 3a0d 0a20 2020 2020 2020  string:..       
-00000650: 2020 2020 2072 6574 7572 6e20 6368 6172       return char
-00000660: 0d0a 2020 2020 6572 726f 7228 2245 7272  ..    error("Err
-00000670: 6f72 5b67 6574 5f63 6861 725d 3a20 5275  or[get_char]: Ru
-00000680: 6e6e 696e 6720 6f75 7420 6f66 2069 6e64  nning out of ind
-00000690: 6578 2063 6861 7261 6374 6572 2122 2920  ex character!") 
-000006a0: 2020 200d 0a0d 0a64 6566 2073 686f 775f     ....def show_
-000006b0: 7072 6f67 7265 7373 2873 7465 705f 696e  progress(step_in
-000006c0: 702c 746f 7461 6c5f 696e 702c 7072 6f63  p,total_inp,proc
-000006d0: 6573 735f 6e61 6d65 203d 2022 222c 2072  ess_name = "", r
-000006e0: 6174 696f 3d54 7275 652c 2063 6f6c 6f72  atio=True, color
-000006f0: 3d22 626c 7565 222c 2074 696d 653d 3029  ="blue", time=0)
-00000700: 3a0d 0a0d 0a20 2020 2062 6172 5f6c 656e  :....    bar_len
-00000710: 6774 6820 3d20 3337 0d0a 2020 2020 7374  gth = 37..    st
-00000720: 6570 203d 2069 6e74 286e 702e 666c 6f6f  ep = int(np.floo
-00000730: 7228 6261 725f 6c65 6e67 7468 2a73 7465  r(bar_length*ste
-00000740: 705f 696e 702f 746f 7461 6c5f 696e 7029  p_inp/total_inp)
-00000750: 290d 0a20 2020 2074 6f74 616c 203d 2062  )..    total = b
-00000760: 6172 5f6c 656e 6774 680d 0a0d 0a20 2020  ar_length....   
-00000770: 2063 6f6c 6f72 203d 2063 6f6c 6f72 2e6c   color = color.l
-00000780: 6f77 6572 2829 0d0a 2020 2020 6966 2020  ower()..    if  
-00000790: 2063 6f6c 6f72 3d3d 2262 6c61 636b 223a   color=="black":
-000007a0: 0d0a 2020 2020 2020 2020 636f 6c6f 723d  ..        color=
-000007b0: 2230 220d 0a20 2020 2065 6c69 6620 636f  "0"..    elif co
-000007c0: 6c6f 723d 3d22 7265 6422 3a0d 0a20 2020  lor=="red":..   
-000007d0: 2020 2020 2063 6f6c 6f72 3d22 3122 0d0a       color="1"..
-000007e0: 2020 2020 656c 6966 2063 6f6c 6f72 3d3d      elif color==
-000007f0: 2267 7265 656e 223a 0d0a 2020 2020 2020  "green":..      
-00000800: 2020 636f 6c6f 723d 2232 220d 0a20 2020    color="2"..   
-00000810: 2065 6c69 6620 636f 6c6f 723d 3d22 7965   elif color=="ye
-00000820: 6c6c 6f77 223a 0d0a 2020 2020 2020 2020  llow":..        
-00000830: 636f 6c6f 723d 2233 220d 0a20 2020 2065  color="3"..    e
-00000840: 6c69 6620 636f 6c6f 723d 3d22 626c 7565  lif color=="blue
-00000850: 223a 0d0a 2020 2020 2020 2020 636f 6c6f  ":..        colo
-00000860: 723d 2234 220d 0a20 2020 2065 6c69 6620  r="4"..    elif 
-00000870: 636f 6c6f 723d 3d22 7075 7270 6c65 223a  color=="purple":
-00000880: 0d0a 2020 2020 2020 2020 636f 6c6f 723d  ..        color=
-00000890: 2235 220d 0a20 2020 2065 6c69 6620 636f  "5"..    elif co
-000008a0: 6c6f 723d 3d22 6379 616e 223a 0d0a 2020  lor=="cyan":..  
-000008b0: 2020 2020 2020 636f 6c6f 723d 2236 220d        color="6".
-000008c0: 0a0d 0a20 2020 2069 6620 7374 6570 203e  ...    if step >
-000008d0: 2074 6f74 616c 3a0d 0a20 2020 2020 2020   total:..       
-000008e0: 2023 6774 6e2e 6572 726f 7228 2245 7272   #gtn.error("Err
-000008f0: 6f72 5b73 686f 775f 7072 6f67 7265 7373  or[show_progress
-00000900: 5d3a 203c 7374 6570 3e20 6361 6e6e 6f74  ]: <step> cannot
-00000910: 2062 6520 6c61 7267 6572 2074 6861 6e20   be larger than 
-00000920: 3c74 6f74 616c 3e21 2229 0d0a 2020 2020  <total>!")..    
-00000930: 2020 2020 7374 6570 203d 2074 6f74 616c      step = total
-00000940: 0d0a 2020 2020 7072 696e 7428 225c 7222  ..    print("\r"
-00000950: 2c65 6e64 3d22 2229 0d0a 0d0a 2020 2020  ,end="")....    
-00000960: 6966 2072 6174 696f 203a 0d0a 2020 2020  if ratio :..    
-00000970: 2020 2020 7072 6f67 7265 7373 203d 2073      progress = s
-00000980: 7472 2873 7465 705f 696e 7029 2b22 2f22  tr(step_inp)+"/"
-00000990: 2b73 7472 2874 6f74 616c 5f69 6e70 290d  +str(total_inp).
-000009a0: 0a20 2020 2065 6c73 6520 3a0d 0a20 2020  .    else :..   
-000009b0: 2020 2020 2070 726f 6772 6573 7320 3d20       progress = 
-000009c0: 277b 3a2e 3467 7d20 2527 2e66 6f72 6d61  '{:.4g} %'.forma
-000009d0: 7428 7374 6570 5f69 6e70 2f74 6f74 616c  t(step_inp/total
-000009e0: 5f69 6e70 2a31 3030 290d 0a0d 0a20 2020  _inp*100)....   
-000009f0: 2074 696d 655f 7465 7874 203d 2022 220d   time_text = "".
-00000a00: 0a20 2020 2069 6620 7469 6d65 3e31 2e30  .    if time>1.0
-00000a10: 652d 3130 203a 0d0a 2020 2020 2020 2020  e-10 :..        
-00000a20: 7469 6d65 5f74 6578 7420 3d20 2228 222b  time_text = "("+
-00000a30: 7469 6d65 5f64 6973 706c 6179 2874 696d  time_display(tim
-00000a40: 6529 2b22 2922 0d0a 0d0a 2020 2020 6966  e)+")"....    if
-00000a50: 2073 7465 705f 696e 702f 746f 7461 6c5f   step_inp/total_
-00000a60: 696e 7020 3e20 302e 3735 203a 0d0a 2020  inp > 0.75 :..  
-00000a70: 2020 2020 2020 6c65 6674 5f74 6578 7420        left_text 
-00000a80: 3d20 7072 6f67 7265 7373 2b22 2022 2b74  = progress+" "+t
-00000a90: 696d 655f 7465 7874 2b22 2022 2b70 726f  ime_text+" "+pro
-00000aa0: 6365 7373 5f6e 616d 652b 2220 220d 0a20  cess_name+" ".. 
-00000ab0: 2020 2020 2020 2072 6768 745f 7465 7874         rght_text
-00000ac0: 203d 2022 220d 0a20 2020 2065 6c69 6620   = ""..    elif 
-00000ad0: 7374 6570 5f69 6e70 2f74 6f74 616c 5f69  step_inp/total_i
-00000ae0: 6e70 203e 2030 2e35 3a0d 0a20 2020 2020  np > 0.5:..     
-00000af0: 2020 206c 6566 745f 7465 7874 203d 2074     left_text = t
-00000b00: 696d 655f 7465 7874 2b22 2022 2b70 726f  ime_text+" "+pro
-00000b10: 6365 7373 5f6e 616d 652b 2220 220d 0a20  cess_name+" ".. 
-00000b20: 2020 2020 2020 2072 6768 745f 7465 7874         rght_text
-00000b30: 203d 2022 2022 2b70 726f 6772 6573 730d   = " "+progress.
-00000b40: 0a20 2020 2065 6c69 6620 7374 6570 5f69  .    elif step_i
-00000b50: 6e70 2f74 6f74 616c 5f69 6e70 203e 2030  np/total_inp > 0
-00000b60: 2e32 353a 0d0a 2020 2020 2020 2020 6c65  .25:..        le
-00000b70: 6674 5f74 6578 7420 3d20 7072 6f63 6573  ft_text = proces
-00000b80: 735f 6e61 6d65 2b22 2022 0d0a 2020 2020  s_name+" "..    
-00000b90: 2020 2020 7267 6874 5f74 6578 7420 3d20      rght_text = 
-00000ba0: 2220 222b 7072 6f67 7265 7373 2b22 2022  " "+progress+" "
-00000bb0: 2b74 696d 655f 7465 7874 0d0a 2020 2020  +time_text..    
-00000bc0: 656c 7365 3a0d 0a20 2020 2020 2020 206c  else:..        l
-00000bd0: 6566 745f 7465 7874 203d 2022 220d 0a20  eft_text = "".. 
-00000be0: 2020 2020 2020 2072 6768 745f 7465 7874         rght_text
-00000bf0: 203d 2022 2022 2b70 726f 6365 7373 5f6e   = " "+process_n
-00000c00: 616d 652b 2220 222b 7072 6f67 7265 7373  ame+" "+progress
-00000c10: 2b22 2022 2b74 696d 655f 7465 7874 0d0a  +" "+time_text..
-00000c20: 0d0a 2020 2020 6966 206c 656e 286c 6566  ..    if len(lef
-00000c30: 745f 7465 7874 2920 3e20 322a 7374 6570  t_text) > 2*step
-00000c40: 203a 0d0a 2020 2020 2020 2020 6c65 6674   :..        left
-00000c50: 5f74 6578 7420 3d20 6c65 6674 5f74 6578  _text = left_tex
-00000c60: 745b 286c 656e 286c 6566 745f 7465 7874  t[(len(left_text
-00000c70: 292d 322a 7374 6570 293a 5d0d 0a0d 0a20  )-2*step):].... 
-00000c80: 2020 2027 2727 0d0a 2020 2020 7072 6f63     '''..    proc
-00000c90: 6573 735f 6e61 6d65 203d 2070 726f 6365  ess_name = proce
-00000ca0: 7373 5f6e 616d 6520 2b20 2220 220d 0a20  ss_name + " ".. 
-00000cb0: 2020 2069 6628 6c65 6e28 7072 6f63 6573     if(len(proces
-00000cc0: 735f 6e61 6d65 293e 322a 746f 7461 6c29  s_name)>2*total)
-00000cd0: 3a0d 0a20 2020 2020 2020 2070 726f 6365  :..        proce
-00000ce0: 7373 5f6e 616d 6520 3d20 2220 220d 0a20  ss_name = " ".. 
-00000cf0: 2020 2069 6620 7261 7469 6f20 3a0d 0a20     if ratio :.. 
-00000d00: 2020 2020 2020 2070 726f 6772 6573 735f         progress_
-00000d10: 6e75 6d62 6572 203d 2022 2022 2b73 7472  number = " "+str
-00000d20: 2873 7465 705f 696e 7029 2b22 2f22 2b73  (step_inp)+"/"+s
-00000d30: 7472 2874 6f74 616c 5f69 6e70 290d 0a20  tr(total_inp).. 
-00000d40: 2020 2065 6c73 6520 3a0d 0a20 2020 2020     else :..     
-00000d50: 2020 2070 726f 6772 6573 735f 6e75 6d62     progress_numb
-00000d60: 6572 203d 2022 2022 2b27 7b3a 2e34 677d  er = " "+'{:.4g}
-00000d70: 2025 272e 666f 726d 6174 2873 7465 705f   %'.format(step_
-00000d80: 696e 702f 746f 7461 6c5f 696e 702a 3130  inp/total_inp*10
-00000d90: 3029 0d0a 0d0a 2020 2020 6966 2074 696d  0)....    if tim
-00000da0: 653e 312e 3065 2d31 3020 3a0d 0a20 2020  e>1.0e-10 :..   
-00000db0: 2020 2020 2069 6620 7374 6570 5f69 6e70       if step_inp
-00000dc0: 2a32 203c 2074 6f74 616c 5f69 6e70 3a0d  *2 < total_inp:.
-00000dd0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00000de0: 6772 6573 735f 6e75 6d62 6572 202b 3d20  gress_number += 
-00000df0: 2220 2822 2b74 696d 655f 6469 7370 6c61  " ("+time_displa
-00000e00: 7928 7469 6d65 292b 2229 220d 0a20 2020  y(time)+")"..   
-00000e10: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00000e20: 2020 2020 2020 2020 7072 6f63 6573 735f          process_
-00000e30: 6e61 6d65 203d 2022 2822 2b74 696d 655f  name = "("+time_
-00000e40: 6469 7370 6c61 7928 7469 6d65 292b 2229  display(time)+")
-00000e50: 2022 2b70 726f 6365 7373 5f6e 616d 650d   "+process_name.
-00000e60: 0a0d 0a20 2020 2069 6620 7374 6570 5f69  ...    if step_i
-00000e70: 6e70 2a34 203e 2074 6f74 616c 5f69 6e70  np*4 > total_inp
-00000e80: 2a33 3a0d 0a20 2020 2020 2020 2070 726f  *3:..        pro
-00000e90: 6365 7373 5f6e 616d 6520 3d20 7072 6f67  cess_name = prog
-00000ea0: 7265 7373 5f6e 756d 6265 722b 2220 222b  ress_number+" "+
-00000eb0: 7072 6f63 6573 735f 6e61 6d65 0d0a 2020  process_name..  
-00000ec0: 2020 2020 2020 7072 6f67 7265 7373 5f6e        progress_n
-00000ed0: 756d 6265 7220 3d20 2222 0d0a 0d0a 2020  umber = ""....  
-00000ee0: 2020 6966 206c 656e 2870 726f 6365 7373    if len(process
-00000ef0: 5f6e 616d 6529 203e 2032 2a73 7465 7020  _name) > 2*step 
-00000f00: 3a0d 0a20 2020 2020 2020 2070 726f 6365  :..        proce
-00000f10: 7373 5f6e 616d 6520 3d20 7072 6f63 6573  ss_name = proces
-00000f20: 735f 6e61 6d65 5b28 6c65 6e28 7072 6f63  s_name[(len(proc
-00000f30: 6573 735f 6e61 6d65 292d 322a 7374 6570  ess_name)-2*step
-00000f40: 293a 5d0d 0a20 2020 2027 2727 0d0a 0d0a  ):]..    '''....
-00000f50: 2020 2020 7374 796c 6564 5f6c 6566 745f      styled_left_
-00000f60: 7465 7874 203d 2022 5c75 3030 3162 5b31  text = "\u001b[1
-00000f70: 3b33 373b 3422 2b63 6f6c 6f72 2b22 6d22  ;37;4"+color+"m"
-00000f80: 2b6c 6566 745f 7465 7874 2b22 5c75 3030  +left_text+"\u00
-00000f90: 3162 5b30 3b30 6d22 0d0a 0d0a 2020 2020  1b[0;0m"....    
-00000fa0: 6966 2032 2a73 7465 702d 6c65 6e28 6c65  if 2*step-len(le
-00000fb0: 6674 5f74 6578 7429 2b6c 656e 286c 6566  ft_text)+len(lef
-00000fc0: 745f 7465 7874 292b 6c65 6e28 7267 6874  t_text)+len(rght
-00000fd0: 5f74 6578 7429 203e 2032 2a74 6f74 616c  _text) > 2*total
-00000fe0: 203a 0d0a 2020 2020 2020 2020 7267 6874   :..        rght
-00000ff0: 5f74 6578 7420 3d20 7267 6874 5f74 6578  _text = rght_tex
-00001000: 745b 3a28 322a 746f 7461 6c2d 322a 7374  t[:(2*total-2*st
-00001010: 6570 295d 0d0a 2020 2020 7374 796c 6564  ep)]..    styled
-00001020: 5f72 6768 745f 7465 7874 203d 2022 5c75  _rght_text = "\u
-00001030: 3030 3162 5b31 3b33 222b 636f 6c6f 722b  001b[1;3"+color+
-00001040: 223b 3437 6d22 2b72 6768 745f 7465 7874  ";47m"+rght_text
-00001050: 2b22 5c75 3030 3162 5b30 3b30 6d22 0d0a  +"\u001b[0;0m"..
-00001060: 0d0a 2020 2020 6669 6c6c 6564 5f62 6172  ..    filled_bar
-00001070: 203d 2022 5c75 3030 3162 5b30 3b3b 3422   = "\u001b[0;;4"
-00001080: 2b63 6f6c 6f72 2b22 6d20 5c75 3030 3162  +color+"m \u001b
-00001090: 5b30 3b30 6d22 0d0a 2020 2020 626c 616e  [0;0m"..    blan
-000010a0: 6b5f 6261 7220 3d20 225c 7530 3031 625b  k_bar = "\u001b[
-000010b0: 303b 3b34 376d 205c 7530 3031 625b 303b  0;;47m \u001b[0;
-000010c0: 306d 220d 0a0d 0a0d 0a20 2020 206e 5f66  0m"......    n_f
-000010d0: 696c 6c65 6420 3d20 322a 7374 6570 2d6c  illed = 2*step-l
-000010e0: 656e 286c 6566 745f 7465 7874 290d 0a20  en(left_text).. 
-000010f0: 2020 206e 5f62 6c61 6e6b 2020 3d20 322a     n_blank  = 2*
-00001100: 746f 7461 6c2d 6e5f 6669 6c6c 6564 2d6c  total-n_filled-l
-00001110: 656e 286c 6566 745f 7465 7874 292d 6c65  en(left_text)-le
-00001120: 6e28 7267 6874 5f74 6578 7429 0d0a 0d0a  n(rght_text)....
-00001130: 2020 2020 746f 7461 6c20 3d20 6e5f 6669      total = n_fi
-00001140: 6c6c 6564 2b6c 656e 286c 6566 745f 7465  lled+len(left_te
-00001150: 7874 292b 6c65 6e28 7267 6874 5f74 6578  xt)+len(rght_tex
-00001160: 7429 2b6e 5f62 6c61 6e6b 0d0a 0d0a 2020  t)+n_blank....  
-00001170: 2020 2370 7269 6e74 2822 2020 2070 726f    #print("   pro
-00001180: 6772 6573 733a 2022 2c65 6e64 3d22 2229  gress: ",end="")
-00001190: 0d0a 2020 2020 7072 696e 7428 2220 2020  ..    print("   
-000011a0: 222c 656e 643d 2222 290d 0a20 2020 2066  ",end="")..    f
-000011b0: 6f72 2069 2069 6e20 7261 6e67 6528 6e5f  or i in range(n_
-000011c0: 6669 6c6c 6564 293a 0d0a 2020 2020 2020  filled):..      
-000011d0: 2020 7072 696e 7428 6669 6c6c 6564 5f62    print(filled_b
-000011e0: 6172 2c65 6e64 3d22 2229 0d0a 2020 2020  ar,end="")..    
-000011f0: 0d0a 2020 2020 7072 696e 7428 7374 796c  ..    print(styl
-00001200: 6564 5f6c 6566 745f 7465 7874 2c65 6e64  ed_left_text,end
-00001210: 3d22 2229 0d0a 2020 2020 7072 696e 7428  ="")..    print(
-00001220: 7374 796c 6564 5f72 6768 745f 7465 7874  styled_rght_text
-00001230: 2c65 6e64 3d22 2229 0d0a 0d0a 2020 2020  ,end="")....    
-00001240: 666f 7220 6920 696e 2072 616e 6765 286e  for i in range(n
-00001250: 5f62 6c61 6e6b 293a 0d0a 2020 2020 2020  _blank):..      
-00001260: 2020 7072 696e 7428 626c 616e 6b5f 6261    print(blank_ba
-00001270: 722c 656e 643d 2222 290d 0a20 2020 2072  r,end="")..    r
-00001280: 6574 7572 6e20 7374 6570 5f69 6e70 2b31  eturn step_inp+1
-00001290: 0d0a 0d0a 6465 6620 636c 6561 725f 7072  ....def clear_pr
-000012a0: 6f67 7265 7373 2829 3a0d 0a20 2020 2070  ogress():..    p
-000012b0: 7269 6e74 2822 5c72 222c 656e 643d 2222  rint("\r",end=""
-000012c0: 290d 0a20 2020 2066 6f72 2069 2069 6e20  )..    for i in 
-000012d0: 7261 6e67 6528 3930 293a 0d0a 2020 2020  range(90):..    
-000012e0: 2020 2020 7072 696e 7428 2220 222c 656e      print(" ",en
-000012f0: 643d 2222 290d 0a20 2020 2070 7269 6e74  d="")..    print
-00001300: 2822 5c72 222c 656e 643d 2222 290d 0a20  ("\r",end="").. 
-00001310: 2020 2072 6574 7572 6e20 310d 0a0d 0a64     return 1....d
-00001320: 6566 2074 696d 655f 6469 7370 6c61 7928  ef time_display(
-00001330: 7469 6d65 5f73 6563 6f6e 6473 293a 0d0a  time_seconds):..
-00001340: 0d0a 2020 2020 6966 2074 696d 655f 7365  ..    if time_se
-00001350: 636f 6e64 7320 3c20 3630 203a 0d0a 2020  conds < 60 :..  
-00001360: 2020 2020 2020 7265 7420 3d20 277b 3a2e        ret = '{:.
-00001370: 3467 7d27 2e66 6f72 6d61 7428 7469 6d65  4g}'.format(time
-00001380: 5f73 6563 6f6e 6473 292b 2220 7322 0d0a  _seconds)+" s"..
-00001390: 2020 2020 656c 6966 2074 696d 655f 7365      elif time_se
-000013a0: 636f 6e64 7320 3c20 3630 2a36 3020 3a0d  conds < 60*60 :.
-000013b0: 0a20 2020 2020 2020 206d 696e 7574 6573  .        minutes
-000013c0: 203d 2069 6e74 286e 702e 666c 6f6f 7228   = int(np.floor(
-000013d0: 7469 6d65 5f73 6563 6f6e 6473 2f36 3029  time_seconds/60)
-000013e0: 290d 0a20 2020 2020 2020 2073 6563 6f6e  )..        secon
-000013f0: 6473 203d 2074 696d 655f 7365 636f 6e64  ds = time_second
-00001400: 732d 3630 2a6d 696e 7574 6573 0d0a 2020  s-60*minutes..  
-00001410: 2020 2020 2020 7265 7420 3d20 7374 7228        ret = str(
-00001420: 6d69 6e75 7465 7329 2b22 206d 2022 2b27  minutes)+" m "+'
-00001430: 7b3a 2e34 677d 272e 666f 726d 6174 2873  {:.4g}'.format(s
-00001440: 6563 6f6e 6473 292b 2220 7322 0d0a 2020  econds)+" s"..  
-00001450: 2020 656c 6966 2074 696d 655f 7365 636f    elif time_seco
-00001460: 6e64 7320 3c20 3630 2a36 302a 3234 203a  nds < 60*60*24 :
-00001470: 0d0a 2020 2020 2020 2020 686f 7572 7320  ..        hours 
-00001480: 3d20 696e 7428 6e70 2e66 6c6f 6f72 2874  = int(np.floor(t
-00001490: 696d 655f 7365 636f 6e64 732f 3630 2f36  ime_seconds/60/6
-000014a0: 3029 290d 0a20 2020 2020 2020 206d 696e  0))..        min
-000014b0: 7574 6573 203d 2069 6e74 286e 702e 666c  utes = int(np.fl
-000014c0: 6f6f 7228 7469 6d65 5f73 6563 6f6e 6473  oor(time_seconds
-000014d0: 2f36 302d 3630 2a68 6f75 7273 2929 0d0a  /60-60*hours))..
-000014e0: 2020 2020 2020 2020 7365 636f 6e64 7320          seconds 
-000014f0: 3d20 7469 6d65 5f73 6563 6f6e 6473 2d36  = time_seconds-6
-00001500: 302a 6d69 6e75 7465 732d 3630 2a36 302a  0*minutes-60*60*
-00001510: 686f 7572 730d 0a20 2020 2020 2020 2072  hours..        r
-00001520: 6574 203d 2073 7472 2868 6f75 7273 292b  et = str(hours)+
-00001530: 2220 6872 2022 2b73 7472 286d 696e 7574  " hr "+str(minut
-00001540: 6573 292b 2220 6d20 222b 277b 3a2e 3467  es)+" m "+'{:.4g
-00001550: 7d27 2e66 6f72 6d61 7428 7365 636f 6e64  }'.format(second
-00001560: 7329 2b22 2073 220d 0a20 2020 2065 6c73  s)+" s"..    els
-00001570: 653a 0d0a 2020 2020 2020 2020 6461 7973  e:..        days
-00001580: 203d 2069 6e74 286e 702e 666c 6f6f 7228   = int(np.floor(
-00001590: 7469 6d65 5f73 6563 6f6e 6473 2f36 302f  time_seconds/60/
-000015a0: 3630 2f32 3429 290d 0a20 2020 2020 2020  60/24))..       
-000015b0: 2068 6f75 7273 203d 2069 6e74 286e 702e   hours = int(np.
-000015c0: 666c 6f6f 7228 7469 6d65 5f73 6563 6f6e  floor(time_secon
-000015d0: 6473 2f36 302f 3630 2d32 342a 6461 7973  ds/60/60-24*days
-000015e0: 2929 0d0a 2020 2020 2020 2020 6d69 6e75  ))..        minu
-000015f0: 7465 7320 3d20 696e 7428 6e70 2e66 6c6f  tes = int(np.flo
-00001600: 6f72 2874 696d 655f 7365 636f 6e64 732f  or(time_seconds/
-00001610: 3630 2d36 302a 686f 7572 732d 3630 2a32  60-60*hours-60*2
-00001620: 342a 6461 7973 2929 0d0a 2020 2020 2020  4*days))..      
-00001630: 2020 7365 636f 6e64 7320 3d20 7469 6d65    seconds = time
-00001640: 5f73 6563 6f6e 6473 2d36 302a 6d69 6e75  _seconds-60*minu
-00001650: 7465 732d 3630 2a36 302a 686f 7572 732d  tes-60*60*hours-
-00001660: 3630 2a36 302a 3234 2a64 6179 730d 0a20  60*60*24*days.. 
-00001670: 2020 2020 2020 2072 6574 203d 2073 7472         ret = str
-00001680: 2864 6179 7329 2b22 2064 2022 2b73 7472  (days)+" d "+str
-00001690: 2868 6f75 7273 292b 2220 6872 2022 2b73  (hours)+" hr "+s
-000016a0: 7472 286d 696e 7574 6573 292b 2220 6d20  tr(minutes)+" m 
-000016b0: 222b 277b 3a2e 3467 7d27 2e66 6f72 6d61  "+'{:.4g}'.forma
-000016c0: 7428 7365 636f 6e64 7329 2b22 2073 220d  t(seconds)+" s".
-000016d0: 0a0d 0a20 2020 2072 6574 7572 6e20 7265  ...    return re
-000016e0: 740d 0a0d 0a64 6566 2063 6c65 616e 5f66  t....def clean_f
-000016f0: 6f72 6d61 7428 6e75 6d62 6572 293a 0d0a  ormat(number):..
-00001700: 2020 2020 6f72 6465 7220 3d20 2d69 6e74      order = -int
-00001710: 286e 702e 6c6f 6731 3028 6e75 6d65 725f  (np.log10(numer_
-00001720: 6469 7370 6c61 795f 6375 746f 6666 2929  display_cutoff))
-00001730: 0d0a 2020 2020 6966 206e 702e 6162 7328  ..    if np.abs(
-00001740: 6e70 2e72 6561 6c28 6e75 6d62 6572 2929  np.real(number))
-00001750: 3e6e 756d 6572 5f63 7574 6f66 6620 616e  >numer_cutoff an
-00001760: 6420 6e70 2e61 6273 286e 702e 696d 6167  d np.abs(np.imag
-00001770: 286e 756d 6265 7229 293c 6e75 6d65 725f  (number))<numer_
-00001780: 6375 746f 6666 3a0d 0a20 2020 2020 2020  cutoff:..       
-00001790: 2072 6574 7572 6e20 726f 756e 6428 6e70   return round(np
-000017a0: 2e72 6561 6c28 6e75 6d62 6572 292c 6f72  .real(number),or
-000017b0: 6465 7229 0d0a 2020 2020 656c 6966 206e  der)..    elif n
-000017c0: 702e 6162 7328 6e70 2e72 6561 6c28 6e75  p.abs(np.real(nu
-000017d0: 6d62 6572 2929 3c6e 756d 6572 5f63 7574  mber))<numer_cut
-000017e0: 6f66 6620 616e 6420 6e70 2e61 6273 286e  off and np.abs(n
-000017f0: 702e 696d 6167 286e 756d 6265 7229 293e  p.imag(number))>
-00001800: 6e75 6d65 725f 6375 746f 6666 3a0d 0a20  numer_cutoff:.. 
-00001810: 2020 2020 2020 2072 6574 7572 6e20 726f         return ro
-00001820: 756e 6428 6e70 2e69 6d61 6728 6e75 6d62  und(np.imag(numb
-00001830: 6572 292c 6f72 6465 7229 2a63 6f6d 706c  er),order)*compl
-00001840: 6578 2830 2c31 290d 0a20 2020 2065 6c69  ex(0,1)..    eli
-00001850: 6620 6e70 2e61 6273 286e 702e 7265 616c  f np.abs(np.real
-00001860: 286e 756d 6265 7229 293c 6e75 6d65 725f  (number))<numer_
-00001870: 6375 746f 6666 2061 6e64 206e 702e 6162  cutoff and np.ab
-00001880: 7328 6e70 2e69 6d61 6728 6e75 6d62 6572  s(np.imag(number
-00001890: 2929 3c6e 756d 6572 5f63 7574 6f66 663a  ))<numer_cutoff:
-000018a0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000018b0: 2030 0d0a 2020 2020 656c 7365 3a0d 0a20   0..    else:.. 
-000018c0: 2020 2020 2020 2072 6574 7572 6e20 726f         return ro
-000018d0: 756e 6428 6e70 2e72 6561 6c28 6e75 6d62  und(np.real(numb
-000018e0: 6572 292c 6f72 6465 7229 2b72 6f75 6e64  er),order)+round
-000018f0: 286e 702e 696d 6167 286e 756d 6265 7229  (np.imag(number)
-00001900: 2c6f 7264 6572 292a 636f 6d70 6c65 7828  ,order)*complex(
-00001910: 302c 3129 0d0a 0d0a 6465 6620 6d65 6d6f  0,1)....def memo
-00001920: 7279 5f64 6973 706c 6179 2872 6177 5f6d  ry_display(raw_m
-00001930: 656d 6f72 7929 3a0d 0a20 2020 2069 6620  emory):..    if 
-00001940: 7261 775f 6d65 6d6f 7279 3c32 2a2a 3130  raw_memory<2**10
-00001950: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-00001960: 6e20 277b 3a2e 3467 7d27 2e66 6f72 6d61  n '{:.4g}'.forma
-00001970: 7428 7261 775f 6d65 6d6f 7279 292b 2220  t(raw_memory)+" 
-00001980: 4222 0d0a 2020 2020 656c 6966 2072 6177  B"..    elif raw
-00001990: 5f6d 656d 6f72 793c 322a 2a32 303a 0d0a  _memory<2**20:..
-000019a0: 2020 2020 2020 2020 7265 7475 726e 2027          return '
-000019b0: 7b3a 2e34 677d 272e 666f 726d 6174 2872  {:.4g}'.format(r
-000019c0: 6177 5f6d 656d 6f72 792f 2832 2a2a 3130  aw_memory/(2**10
-000019d0: 2929 2b22 204b 6942 220d 0a20 2020 2065  ))+" KiB"..    e
-000019e0: 6c69 6620 7261 775f 6d65 6d6f 7279 3c32  lif raw_memory<2
-000019f0: 2a2a 3330 3a0d 0a20 2020 2020 2020 2072  **30:..        r
-00001a00: 6574 7572 6e20 277b 3a2e 3467 7d27 2e66  eturn '{:.4g}'.f
-00001a10: 6f72 6d61 7428 7261 775f 6d65 6d6f 7279  ormat(raw_memory
-00001a20: 2f28 322a 2a32 3029 292b 2220 4d69 4222  /(2**20))+" MiB"
-00001a30: 0d0a 2020 2020 656c 6966 2072 6177 5f6d  ..    elif raw_m
-00001a40: 656d 6f72 793c 322a 2a34 303a 0d0a 2020  emory<2**40:..  
-00001a50: 2020 2020 2020 7265 7475 726e 2027 7b3a        return '{:
-00001a60: 2e34 677d 272e 666f 726d 6174 2872 6177  .4g}'.format(raw
-00001a70: 5f6d 656d 6f72 792f 2832 2a2a 3330 2929  _memory/(2**30))
-00001a80: 2b22 2047 6942 220d 0a20 2020 2065 6c73  +" GiB"..    els
-00001a90: 653a 0d0a 2020 2020 2020 2020 7265 7475  e:..        retu
-00001aa0: 726e 2027 7b3a 2e34 677d 272e 666f 726d  rn '{:.4g}'.form
-00001ab0: 6174 2872 6177 5f6d 656d 6f72 792f 2832  at(raw_memory/(2
-00001ac0: 2a2a 3430 2929 2b22 2054 6942 220d 0a0d  **40))+" TiB"...
-00001ad0: 0a64 6566 2063 7572 7265 6e74 5f6d 656d  .def current_mem
-00001ae0: 6f72 795f 6469 7370 6c61 7928 293a 0d0a  ory_display():..
-00001af0: 2020 2020 7265 7475 726e 206d 656d 6f72      return memor
-00001b00: 795f 6469 7370 6c61 7928 7472 6163 656d  y_display(tracem
-00001b10: 616c 6c6f 632e 6765 745f 7472 6163 6564  alloc.get_traced
-00001b20: 5f6d 656d 6f72 7928 295b 305d 292b 222f  _memory()[0])+"/
-00001b30: 222b 6d65 6d6f 7279 5f64 6973 706c 6179  "+memory_display
-00001b40: 2874 7261 6365 6d61 6c6c 6f63 2e67 6574  (tracemalloc.get
-00001b50: 5f74 7261 6365 645f 6d65 6d6f 7279 2829  _traced_memory()
-00001b60: 5b31 5d29 0d0a 0d0a 6465 6620 6765 7473  [1])....def gets
-00001b70: 697a 6528 7368 6170 6529 3a0d 0a20 2020  ize(shape):..   
-00001b80: 2072 6574 203d 2031 0d0a 2020 2020 666f   ret = 1..    fo
-00001b90: 7220 6420 696e 2073 6861 7065 3a0d 0a20  r d in shape:.. 
-00001ba0: 2020 2020 2020 2072 6574 202a 3d20 640d         ret *= d.
-00001bb0: 0a20 2020 2072 6574 7572 6e20 7265 740d  .    return ret.
-00001bc0: 0a0d 0a23 2323 2323 2323 2323 2323 2323  ...#############
+00000290: 5f6c 6973 7420 3d20 280d 0a20 2020 2022  _list = (..    "
+000002a0: 6122 2c22 6222 2c22 6322 2c22 6422 2c22  a","b","c","d","
+000002b0: 6522 2c22 6622 2c22 6722 2c22 6822 2c22  e","f","g","h","
+000002c0: 6922 2c22 6a22 2c22 6b22 2c22 6c22 2c22  i","j","k","l","
+000002d0: 6d22 2c22 6e22 2c22 6f22 2c22 7022 2c22  m","n","o","p","
+000002e0: 7122 2c22 7222 2c22 7322 2c22 7422 2c22  q","r","s","t","
+000002f0: 7522 2c22 7622 2c22 7722 2c22 7822 2c22  u","v","w","x","
+00000300: 7922 2c22 7a22 0d0a 2020 2020 2c22 4122  y","z"..    ,"A"
+00000310: 2c22 4222 2c22 4322 2c22 4422 2c22 4522  ,"B","C","D","E"
+00000320: 2c22 4622 2c22 4722 2c22 4822 2c22 4922  ,"F","G","H","I"
+00000330: 2c22 4a22 2c22 4b22 2c22 4c22 2c22 4d22  ,"J","K","L","M"
+00000340: 2c22 4e22 2c22 4f22 2c22 5022 2c22 5122  ,"N","O","P","Q"
+00000350: 2c22 5222 2c22 5322 2c22 5422 2c22 5522  ,"R","S","T","U"
+00000360: 2c22 5622 2c22 5722 2c22 5822 2c22 5922  ,"V","W","X","Y"
+00000370: 2c22 5a22 0d0a 2020 2020 2c22 ceb1 222c  ,"Z"..    ,"..",
+00000380: 22ce b222 2c22 ce93 222c 22ce b322 2c22  "..","..","..","
+00000390: ce94 222c 22ce b422 2c22 ceb5 222c 22ce  ..","..","..",".
+000003a0: b622 2c22 ceb7 222c 22ce 9822 2c22 ceb8  .","..","..","..
+000003b0: 222c 22ce b922 2c22 ceba 222c 22ce bb22  ","..","..",".."
+000003c0: 2c22 cebc 222c 22ce bd22 2c22 ce9e 222c  ,"..","..","..",
+000003d0: 22ce be22 2c22 cea0 222c 22cf 8022 2c22  "..","..","..","
+000003e0: cf81 222c 22ce a322 2c22 cf83 222c 22cf  ..","..","..",".
+000003f0: 8222 2c22 cf84 222c 22cf 8522 2c22 cea6  .","..","..","..
+00000400: 222c 22cf 9522 2c22 cf86 222c 22cf 8722  ","..","..",".."
+00000410: 2c22 cea8 222c 22cf 8822 2c22 cea9 222c  ,"..","..","..",
+00000420: 22cf 8922 0d0a 2020 2020 290d 0a0d 0a70  ".."..    )....p
+00000430: 726f 6772 6573 735f 6261 725f 656e 6162  rogress_bar_enab
+00000440: 6c65 6420 3d20 5472 7565 0d0a 0d0a 2323  led = True....##
+00000450: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000460: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000470: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000480: 2323 0d0a 2323 2020 2020 2020 2020 2020  ##..##          
+00000490: 2020 2020 2020 5261 6e64 6f6d 2055 7469        Random Uti
+000004a0: 6c69 7469 6573 2020 2020 2020 2020 2020  lities          
+000004b0: 2020 2020 2020 2323 0d0a 2323 2323 2323        ##..######
+000004c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000004d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000004e0: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
+000004f0: 0d0a 6465 6620 6d61 6b65 5f74 7570 6c65  ..def make_tuple
+00000500: 286f 626a 293a 0d0a 2020 2020 6966 206e  (obj):..    if n
+00000510: 702e 6973 7363 616c 6172 286f 626a 293a  p.isscalar(obj):
+00000520: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000530: 2074 7570 6c65 285b 6f62 6a5d 290d 0a20   tuple([obj]).. 
+00000540: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00000550: 2020 7265 7475 726e 2074 7570 6c65 286c    return tuple(l
+00000560: 6973 7428 6f62 6a29 290d 0a0d 0a64 6566  ist(obj))....def
+00000570: 206d 616b 655f 6c69 7374 286f 626a 293a   make_list(obj):
+00000580: 0d0a 2020 2020 6966 206e 702e 6973 7363  ..    if np.issc
+00000590: 616c 6172 286f 626a 293a 0d0a 2020 2020  alar(obj):..    
+000005a0: 2020 2020 7265 7475 726e 205b 6f62 6a5d      return [obj]
+000005b0: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
+000005c0: 2020 2020 2072 6574 7572 6e20 6c69 7374       return list
+000005d0: 286f 626a 290d 0a0d 0a64 6566 2065 7272  (obj)....def err
+000005e0: 6f72 2874 6578 743d 2245 7272 6f72 5b5d  or(text="Error[]
+000005f0: 3a20 556e 6b6e 6f77 6e20 6572 726f 722e  : Unknown error.
+00000600: 2229 3a0d 0a20 2020 2070 7269 6e74 2829  "):..    print()
+00000610: 0d0a 2020 2020 7072 696e 7428 7465 7874  ..    print(text
+00000620: 290d 0a20 2020 2070 7269 6e74 2829 0d0a  )..    print()..
+00000630: 2020 2020 7072 696e 7428 225c 745f 5f5f      print("\t___
+00000640: 5f5f 5f5f 5f5f 5f6c 6f6f 6b5f 6265 6c6f  _______look_belo
+00000650: 775f 666f 725f 7468 655f 6572 726f 725f  w_for_the_error_
+00000660: 696e 666f 726d 6174 696f 6e5f 5f5f 5f5f  information_____
+00000670: 5f5f 5f5f 5f22 290d 0a20 2020 2023 696e  _____")..    #in
+00000680: 7465 6e74 696f 6e61 6c20 7361 626f 7461  tentional sabota
+00000690: 6765 2121 210d 0a20 2020 205f 5f5f 5f5f  ge!!!..    _____
+000006a0: 5f5f 5f5f 5f6c 6f6f 6b5f 6162 6f76 655f  _____look_above_
+000006b0: 666f 725f 7468 655f 6572 726f 725f 696e  for_the_error_in
+000006c0: 666f 726d 6174 696f 6e5f 5f5f 5f5f 5f5f  formation_______
+000006d0: 5f5f 5f0d 0a0d 0a64 6566 2067 6574 5f63  ___....def get_c
+000006e0: 6861 7228 7374 7269 6e67 293a 0d0a 2020  har(string):..  
+000006f0: 2020 666f 7220 6368 6172 2069 6e20 6368    for char in ch
+00000700: 6172 5f6c 6973 743a 0d0a 2020 2020 2020  ar_list:..      
+00000710: 2020 6966 2063 6861 7220 6e6f 7420 696e    if char not in
+00000720: 2073 7472 696e 673a 0d0a 2020 2020 2020   string:..      
+00000730: 2020 2020 2020 7265 7475 726e 2063 6861        return cha
+00000740: 720d 0a20 2020 2065 7272 6f72 2822 4572  r..    error("Er
+00000750: 726f 725b 6765 745f 6368 6172 5d3a 2052  ror[get_char]: R
+00000760: 756e 6e69 6e67 206f 7574 206f 6620 696e  unning out of in
+00000770: 6465 7820 6368 6172 6163 7465 7221 2229  dex character!")
+00000780: 2020 2020 0d0a 0d0a 6465 6620 7368 6f77      ....def show
+00000790: 5f70 726f 6772 6573 7328 7374 6570 5f69  _progress(step_i
+000007a0: 6e70 2c74 6f74 616c 5f69 6e70 2c70 726f  np,total_inp,pro
+000007b0: 6365 7373 5f6e 616d 6520 3d20 2222 2c20  cess_name = "", 
+000007c0: 7261 7469 6f3d 5472 7565 2c20 636f 6c6f  ratio=True, colo
+000007d0: 723d 2262 6c75 6522 2c20 7469 6d65 3d30  r="blue", time=0
+000007e0: 293a 0d0a 0d0a 2020 2020 6966 2070 726f  ):....    if pro
+000007f0: 6772 6573 735f 6261 725f 656e 6162 6c65  gress_bar_enable
+00000800: 643a 0d0a 0d0a 2020 2020 2020 2020 6261  d:....        ba
+00000810: 725f 6c65 6e67 7468 203d 2033 370d 0a20  r_length = 37.. 
+00000820: 2020 2020 2020 2073 7465 7020 3d20 696e         step = in
+00000830: 7428 6e70 2e66 6c6f 6f72 2862 6172 5f6c  t(np.floor(bar_l
+00000840: 656e 6774 682a 7374 6570 5f69 6e70 2f74  ength*step_inp/t
+00000850: 6f74 616c 5f69 6e70 2929 0d0a 2020 2020  otal_inp))..    
+00000860: 2020 2020 746f 7461 6c20 3d20 6261 725f      total = bar_
+00000870: 6c65 6e67 7468 0d0a 0d0a 2020 2020 2020  length....      
+00000880: 2020 636f 6c6f 7220 3d20 636f 6c6f 722e    color = color.
+00000890: 6c6f 7765 7228 290d 0a20 2020 2020 2020  lower()..       
+000008a0: 2069 6620 2020 636f 6c6f 723d 3d22 626c   if   color=="bl
+000008b0: 6163 6b22 3a0d 0a20 2020 2020 2020 2020  ack":..         
+000008c0: 2020 2063 6f6c 6f72 3d22 3022 0d0a 2020     color="0"..  
+000008d0: 2020 2020 2020 656c 6966 2063 6f6c 6f72        elif color
+000008e0: 3d3d 2272 6564 223a 0d0a 2020 2020 2020  =="red":..      
+000008f0: 2020 2020 2020 636f 6c6f 723d 2231 220d        color="1".
+00000900: 0a20 2020 2020 2020 2065 6c69 6620 636f  .        elif co
+00000910: 6c6f 723d 3d22 6772 6565 6e22 3a0d 0a20  lor=="green":.. 
+00000920: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
+00000930: 3d22 3222 0d0a 2020 2020 2020 2020 656c  ="2"..        el
+00000940: 6966 2063 6f6c 6f72 3d3d 2279 656c 6c6f  if color=="yello
+00000950: 7722 3a0d 0a20 2020 2020 2020 2020 2020  w":..           
+00000960: 2063 6f6c 6f72 3d22 3322 0d0a 2020 2020   color="3"..    
+00000970: 2020 2020 656c 6966 2063 6f6c 6f72 3d3d      elif color==
+00000980: 2262 6c75 6522 3a0d 0a20 2020 2020 2020  "blue":..       
+00000990: 2020 2020 2063 6f6c 6f72 3d22 3422 0d0a       color="4"..
+000009a0: 2020 2020 2020 2020 656c 6966 2063 6f6c          elif col
+000009b0: 6f72 3d3d 2270 7572 706c 6522 3a0d 0a20  or=="purple":.. 
+000009c0: 2020 2020 2020 2020 2020 2063 6f6c 6f72             color
+000009d0: 3d22 3522 0d0a 2020 2020 2020 2020 656c  ="5"..        el
+000009e0: 6966 2063 6f6c 6f72 3d3d 2263 7961 6e22  if color=="cyan"
+000009f0: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
+00000a00: 6f6c 6f72 3d22 3622 0d0a 0d0a 2020 2020  olor="6"....    
+00000a10: 2020 2020 6966 2073 7465 7020 3e20 746f      if step > to
+00000a20: 7461 6c3a 0d0a 2020 2020 2020 2020 2020  tal:..          
+00000a30: 2020 2367 746e 2e65 7272 6f72 2822 4572    #gtn.error("Er
+00000a40: 726f 725b 7368 6f77 5f70 726f 6772 6573  ror[show_progres
+00000a50: 735d 3a20 3c73 7465 703e 2063 616e 6e6f  s]: <step> canno
+00000a60: 7420 6265 206c 6172 6765 7220 7468 616e  t be larger than
+00000a70: 203c 746f 7461 6c3e 2122 290d 0a20 2020   <total>!")..   
+00000a80: 2020 2020 2020 2020 2073 7465 7020 3d20           step = 
+00000a90: 746f 7461 6c0d 0a20 2020 2020 2020 2070  total..        p
+00000aa0: 7269 6e74 2822 5c72 222c 656e 643d 2222  rint("\r",end=""
+00000ab0: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
+00000ac0: 7261 7469 6f20 3a0d 0a20 2020 2020 2020  ratio :..       
+00000ad0: 2020 2020 2070 726f 6772 6573 7320 3d20       progress = 
+00000ae0: 7374 7228 7374 6570 5f69 6e70 292b 222f  str(step_inp)+"/
+00000af0: 222b 7374 7228 746f 7461 6c5f 696e 7029  "+str(total_inp)
+00000b00: 0d0a 2020 2020 2020 2020 656c 7365 203a  ..        else :
+00000b10: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00000b20: 6f67 7265 7373 203d 2027 7b3a 2e34 677d  ogress = '{:.4g}
+00000b30: 2025 272e 666f 726d 6174 2873 7465 705f   %'.format(step_
+00000b40: 696e 702f 746f 7461 6c5f 696e 702a 3130  inp/total_inp*10
+00000b50: 3029 0d0a 0d0a 2020 2020 2020 2020 7469  0)....        ti
+00000b60: 6d65 5f74 6578 7420 3d20 2222 0d0a 2020  me_text = ""..  
+00000b70: 2020 2020 2020 6966 2074 696d 653e 312e        if time>1.
+00000b80: 3065 2d31 3020 3a0d 0a20 2020 2020 2020  0e-10 :..       
+00000b90: 2020 2020 2074 696d 655f 7465 7874 203d       time_text =
+00000ba0: 2022 2822 2b74 696d 655f 6469 7370 6c61   "("+time_displa
+00000bb0: 7928 7469 6d65 292b 2229 220d 0a0d 0a20  y(time)+")".... 
+00000bc0: 2020 2020 2020 2069 6620 7374 6570 5f69         if step_i
+00000bd0: 6e70 2f74 6f74 616c 5f69 6e70 203e 2030  np/total_inp > 0
+00000be0: 2e37 3520 3a0d 0a20 2020 2020 2020 2020  .75 :..         
+00000bf0: 2020 206c 6566 745f 7465 7874 203d 2070     left_text = p
+00000c00: 726f 6772 6573 732b 2220 222b 7469 6d65  rogress+" "+time
+00000c10: 5f74 6578 742b 2220 222b 7072 6f63 6573  _text+" "+proces
+00000c20: 735f 6e61 6d65 2b22 2022 0d0a 2020 2020  s_name+" "..    
+00000c30: 2020 2020 2020 2020 7267 6874 5f74 6578          rght_tex
+00000c40: 7420 3d20 2222 0d0a 2020 2020 2020 2020  t = ""..        
+00000c50: 656c 6966 2073 7465 705f 696e 702f 746f  elif step_inp/to
+00000c60: 7461 6c5f 696e 7020 3e20 302e 353a 0d0a  tal_inp > 0.5:..
+00000c70: 2020 2020 2020 2020 2020 2020 6c65 6674              left
+00000c80: 5f74 6578 7420 3d20 7469 6d65 5f74 6578  _text = time_tex
+00000c90: 742b 2220 222b 7072 6f63 6573 735f 6e61  t+" "+process_na
+00000ca0: 6d65 2b22 2022 0d0a 2020 2020 2020 2020  me+" "..        
+00000cb0: 2020 2020 7267 6874 5f74 6578 7420 3d20      rght_text = 
+00000cc0: 2220 222b 7072 6f67 7265 7373 0d0a 2020  " "+progress..  
+00000cd0: 2020 2020 2020 656c 6966 2073 7465 705f        elif step_
+00000ce0: 696e 702f 746f 7461 6c5f 696e 7020 3e20  inp/total_inp > 
+00000cf0: 302e 3235 3a0d 0a20 2020 2020 2020 2020  0.25:..         
+00000d00: 2020 206c 6566 745f 7465 7874 203d 2070     left_text = p
+00000d10: 726f 6365 7373 5f6e 616d 652b 2220 220d  rocess_name+" ".
+00000d20: 0a20 2020 2020 2020 2020 2020 2072 6768  .            rgh
+00000d30: 745f 7465 7874 203d 2022 2022 2b70 726f  t_text = " "+pro
+00000d40: 6772 6573 732b 2220 222b 7469 6d65 5f74  gress+" "+time_t
+00000d50: 6578 740d 0a20 2020 2020 2020 2065 6c73  ext..        els
+00000d60: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000d70: 6c65 6674 5f74 6578 7420 3d20 2222 0d0a  left_text = ""..
+00000d80: 2020 2020 2020 2020 2020 2020 7267 6874              rght
+00000d90: 5f74 6578 7420 3d20 2220 222b 7072 6f63  _text = " "+proc
+00000da0: 6573 735f 6e61 6d65 2b22 2022 2b70 726f  ess_name+" "+pro
+00000db0: 6772 6573 732b 2220 222b 7469 6d65 5f74  gress+" "+time_t
+00000dc0: 6578 740d 0a0d 0a20 2020 2020 2020 2069  ext....        i
+00000dd0: 6620 6c65 6e28 6c65 6674 5f74 6578 7429  f len(left_text)
+00000de0: 203e 2032 2a73 7465 7020 3a0d 0a20 2020   > 2*step :..   
+00000df0: 2020 2020 2020 2020 206c 6566 745f 7465           left_te
+00000e00: 7874 203d 206c 6566 745f 7465 7874 5b28  xt = left_text[(
+00000e10: 6c65 6e28 6c65 6674 5f74 6578 7429 2d32  len(left_text)-2
+00000e20: 2a73 7465 7029 3a5d 0d0a 0d0a 2020 2020  *step):]....    
+00000e30: 2020 2020 7374 796c 6564 5f6c 6566 745f      styled_left_
+00000e40: 7465 7874 203d 2022 5c75 3030 3162 5b31  text = "\u001b[1
+00000e50: 3b33 373b 3422 2b63 6f6c 6f72 2b22 6d22  ;37;4"+color+"m"
+00000e60: 2b6c 6566 745f 7465 7874 2b22 5c75 3030  +left_text+"\u00
+00000e70: 3162 5b30 3b30 6d22 0d0a 0d0a 2020 2020  1b[0;0m"....    
+00000e80: 2020 2020 6966 2032 2a73 7465 702d 6c65      if 2*step-le
+00000e90: 6e28 6c65 6674 5f74 6578 7429 2b6c 656e  n(left_text)+len
+00000ea0: 286c 6566 745f 7465 7874 292b 6c65 6e28  (left_text)+len(
+00000eb0: 7267 6874 5f74 6578 7429 203e 2032 2a74  rght_text) > 2*t
+00000ec0: 6f74 616c 203a 0d0a 2020 2020 2020 2020  otal :..        
+00000ed0: 2020 2020 7267 6874 5f74 6578 7420 3d20      rght_text = 
+00000ee0: 7267 6874 5f74 6578 745b 3a28 322a 746f  rght_text[:(2*to
+00000ef0: 7461 6c2d 322a 7374 6570 295d 0d0a 2020  tal-2*step)]..  
+00000f00: 2020 2020 2020 7374 796c 6564 5f72 6768        styled_rgh
+00000f10: 745f 7465 7874 203d 2022 5c75 3030 3162  t_text = "\u001b
+00000f20: 5b31 3b33 222b 636f 6c6f 722b 223b 3437  [1;3"+color+";47
+00000f30: 6d22 2b72 6768 745f 7465 7874 2b22 5c75  m"+rght_text+"\u
+00000f40: 3030 3162 5b30 3b30 6d22 0d0a 0d0a 2020  001b[0;0m"....  
+00000f50: 2020 2020 2020 6669 6c6c 6564 5f62 6172        filled_bar
+00000f60: 203d 2022 5c75 3030 3162 5b30 3b3b 3422   = "\u001b[0;;4"
+00000f70: 2b63 6f6c 6f72 2b22 6d20 5c75 3030 3162  +color+"m \u001b
+00000f80: 5b30 3b30 6d22 0d0a 2020 2020 2020 2020  [0;0m"..        
+00000f90: 626c 616e 6b5f 6261 7220 3d20 225c 7530  blank_bar = "\u0
+00000fa0: 3031 625b 303b 3b34 376d 205c 7530 3031  01b[0;;47m \u001
+00000fb0: 625b 303b 306d 220d 0a0d 0a0d 0a20 2020  b[0;0m"......   
+00000fc0: 2020 2020 206e 5f66 696c 6c65 6420 3d20       n_filled = 
+00000fd0: 322a 7374 6570 2d6c 656e 286c 6566 745f  2*step-len(left_
+00000fe0: 7465 7874 290d 0a20 2020 2020 2020 206e  text)..        n
+00000ff0: 5f62 6c61 6e6b 2020 3d20 322a 746f 7461  _blank  = 2*tota
+00001000: 6c2d 6e5f 6669 6c6c 6564 2d6c 656e 286c  l-n_filled-len(l
+00001010: 6566 745f 7465 7874 292d 6c65 6e28 7267  eft_text)-len(rg
+00001020: 6874 5f74 6578 7429 0d0a 0d0a 2020 2020  ht_text)....    
+00001030: 2020 2020 746f 7461 6c20 3d20 6e5f 6669      total = n_fi
+00001040: 6c6c 6564 2b6c 656e 286c 6566 745f 7465  lled+len(left_te
+00001050: 7874 292b 6c65 6e28 7267 6874 5f74 6578  xt)+len(rght_tex
+00001060: 7429 2b6e 5f62 6c61 6e6b 0d0a 0d0a 2020  t)+n_blank....  
+00001070: 2020 2020 2020 2370 7269 6e74 2822 2020        #print("  
+00001080: 2070 726f 6772 6573 733a 2022 2c65 6e64   progress: ",end
+00001090: 3d22 2229 0d0a 2020 2020 2020 2020 7072  ="")..        pr
+000010a0: 696e 7428 2220 2020 222c 656e 643d 2222  int("   ",end=""
+000010b0: 290d 0a20 2020 2020 2020 2066 6f72 2069  )..        for i
+000010c0: 2069 6e20 7261 6e67 6528 6e5f 6669 6c6c   in range(n_fill
+000010d0: 6564 293a 0d0a 2020 2020 2020 2020 2020  ed):..          
+000010e0: 2020 7072 696e 7428 6669 6c6c 6564 5f62    print(filled_b
+000010f0: 6172 2c65 6e64 3d22 2229 0d0a 2020 2020  ar,end="")..    
+00001100: 2020 2020 0d0a 2020 2020 2020 2020 7072      ..        pr
+00001110: 696e 7428 7374 796c 6564 5f6c 6566 745f  int(styled_left_
+00001120: 7465 7874 2c65 6e64 3d22 2229 0d0a 2020  text,end="")..  
+00001130: 2020 2020 2020 7072 696e 7428 7374 796c        print(styl
+00001140: 6564 5f72 6768 745f 7465 7874 2c65 6e64  ed_rght_text,end
+00001150: 3d22 2229 0d0a 0d0a 2020 2020 2020 2020  ="")....        
+00001160: 666f 7220 6920 696e 2072 616e 6765 286e  for i in range(n
+00001170: 5f62 6c61 6e6b 293a 0d0a 2020 2020 2020  _blank):..      
+00001180: 2020 2020 2020 7072 696e 7428 626c 616e        print(blan
+00001190: 6b5f 6261 722c 656e 643d 2222 290d 0a20  k_bar,end="").. 
+000011a0: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+000011b0: 6570 5f69 6e70 2b31 0d0a 0d0a 6465 6620  ep_inp+1....def 
+000011c0: 636c 6561 725f 7072 6f67 7265 7373 2829  clear_progress()
+000011d0: 3a0d 0a0d 0a20 2020 2069 6620 7072 6f67  :....    if prog
+000011e0: 7265 7373 5f62 6172 5f65 6e61 626c 6564  ress_bar_enabled
+000011f0: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
+00001200: 2822 5c72 222c 656e 643d 2222 290d 0a20  ("\r",end="").. 
+00001210: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+00001220: 7261 6e67 6528 3930 293a 0d0a 2020 2020  range(90):..    
+00001230: 2020 2020 2020 2020 7072 696e 7428 2220          print(" 
+00001240: 222c 656e 643d 2222 290d 0a20 2020 2020  ",end="")..     
+00001250: 2020 2070 7269 6e74 2822 5c72 222c 656e     print("\r",en
+00001260: 643d 2222 290d 0a20 2020 2020 2020 2072  d="")..        r
+00001270: 6574 7572 6e20 310d 0a0d 0a64 6566 2070  eturn 1....def p
+00001280: 726f 6772 6573 735f 7370 6163 6528 293a  rogress_space():
+00001290: 0d0a 2020 2020 6966 2070 726f 6772 6573  ..    if progres
+000012a0: 735f 6261 725f 656e 6162 6c65 643a 0d0a  s_bar_enabled:..
+000012b0: 2020 2020 2020 2020 7072 696e 7428 290d          print().
+000012c0: 0a0d 0a64 6566 2074 6162 5f75 7028 293a  ...def tab_up():
+000012d0: 0d0a 2020 2020 6966 2070 726f 6772 6573  ..    if progres
+000012e0: 735f 6261 725f 656e 6162 6c65 643a 0d0a  s_bar_enabled:..
+000012f0: 2020 2020 2020 2020 7379 732e 7374 646f          sys.stdo
+00001300: 7574 2e77 7269 7465 2822 5c30 3333 5b46  ut.write("\033[F
+00001310: 2229 0d0a 0d0a 6465 6620 7469 6d65 5f64  ")....def time_d
+00001320: 6973 706c 6179 2874 696d 655f 7365 636f  isplay(time_seco
+00001330: 6e64 7329 3a0d 0a0d 0a20 2020 2069 6620  nds):....    if 
+00001340: 7469 6d65 5f73 6563 6f6e 6473 203c 2036  time_seconds < 6
+00001350: 3020 3a0d 0a20 2020 2020 2020 2072 6574  0 :..        ret
+00001360: 203d 2027 7b3a 2e34 677d 272e 666f 726d   = '{:.4g}'.form
+00001370: 6174 2874 696d 655f 7365 636f 6e64 7329  at(time_seconds)
+00001380: 2b22 2073 220d 0a20 2020 2065 6c69 6620  +" s"..    elif 
+00001390: 7469 6d65 5f73 6563 6f6e 6473 203c 2036  time_seconds < 6
+000013a0: 302a 3630 203a 0d0a 2020 2020 2020 2020  0*60 :..        
+000013b0: 6d69 6e75 7465 7320 3d20 696e 7428 6e70  minutes = int(np
+000013c0: 2e66 6c6f 6f72 2874 696d 655f 7365 636f  .floor(time_seco
+000013d0: 6e64 732f 3630 2929 0d0a 2020 2020 2020  nds/60))..      
+000013e0: 2020 7365 636f 6e64 7320 3d20 7469 6d65    seconds = time
+000013f0: 5f73 6563 6f6e 6473 2d36 302a 6d69 6e75  _seconds-60*minu
+00001400: 7465 730d 0a20 2020 2020 2020 2072 6574  tes..        ret
+00001410: 203d 2073 7472 286d 696e 7574 6573 292b   = str(minutes)+
+00001420: 2220 6d20 222b 277b 3a2e 3467 7d27 2e66  " m "+'{:.4g}'.f
+00001430: 6f72 6d61 7428 7365 636f 6e64 7329 2b22  ormat(seconds)+"
+00001440: 2073 220d 0a20 2020 2065 6c69 6620 7469   s"..    elif ti
+00001450: 6d65 5f73 6563 6f6e 6473 203c 2036 302a  me_seconds < 60*
+00001460: 3630 2a32 3420 3a0d 0a20 2020 2020 2020  60*24 :..       
+00001470: 2068 6f75 7273 203d 2069 6e74 286e 702e   hours = int(np.
+00001480: 666c 6f6f 7228 7469 6d65 5f73 6563 6f6e  floor(time_secon
+00001490: 6473 2f36 302f 3630 2929 0d0a 2020 2020  ds/60/60))..    
+000014a0: 2020 2020 6d69 6e75 7465 7320 3d20 696e      minutes = in
+000014b0: 7428 6e70 2e66 6c6f 6f72 2874 696d 655f  t(np.floor(time_
+000014c0: 7365 636f 6e64 732f 3630 2d36 302a 686f  seconds/60-60*ho
+000014d0: 7572 7329 290d 0a20 2020 2020 2020 2073  urs))..        s
+000014e0: 6563 6f6e 6473 203d 2074 696d 655f 7365  econds = time_se
+000014f0: 636f 6e64 732d 3630 2a6d 696e 7574 6573  conds-60*minutes
+00001500: 2d36 302a 3630 2a68 6f75 7273 0d0a 2020  -60*60*hours..  
+00001510: 2020 2020 2020 7265 7420 3d20 7374 7228        ret = str(
+00001520: 686f 7572 7329 2b22 2068 7220 222b 7374  hours)+" hr "+st
+00001530: 7228 6d69 6e75 7465 7329 2b22 206d 2022  r(minutes)+" m "
+00001540: 2b27 7b3a 2e34 677d 272e 666f 726d 6174  +'{:.4g}'.format
+00001550: 2873 6563 6f6e 6473 292b 2220 7322 0d0a  (seconds)+" s"..
+00001560: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00001570: 2020 2064 6179 7320 3d20 696e 7428 6e70     days = int(np
+00001580: 2e66 6c6f 6f72 2874 696d 655f 7365 636f  .floor(time_seco
+00001590: 6e64 732f 3630 2f36 302f 3234 2929 0d0a  nds/60/60/24))..
+000015a0: 2020 2020 2020 2020 686f 7572 7320 3d20          hours = 
+000015b0: 696e 7428 6e70 2e66 6c6f 6f72 2874 696d  int(np.floor(tim
+000015c0: 655f 7365 636f 6e64 732f 3630 2f36 302d  e_seconds/60/60-
+000015d0: 3234 2a64 6179 7329 290d 0a20 2020 2020  24*days))..     
+000015e0: 2020 206d 696e 7574 6573 203d 2069 6e74     minutes = int
+000015f0: 286e 702e 666c 6f6f 7228 7469 6d65 5f73  (np.floor(time_s
+00001600: 6563 6f6e 6473 2f36 302d 3630 2a68 6f75  econds/60-60*hou
+00001610: 7273 2d36 302a 3234 2a64 6179 7329 290d  rs-60*24*days)).
+00001620: 0a20 2020 2020 2020 2073 6563 6f6e 6473  .        seconds
+00001630: 203d 2074 696d 655f 7365 636f 6e64 732d   = time_seconds-
+00001640: 3630 2a6d 696e 7574 6573 2d36 302a 3630  60*minutes-60*60
+00001650: 2a68 6f75 7273 2d36 302a 3630 2a32 342a  *hours-60*60*24*
+00001660: 6461 7973 0d0a 2020 2020 2020 2020 7265  days..        re
+00001670: 7420 3d20 7374 7228 6461 7973 292b 2220  t = str(days)+" 
+00001680: 6420 222b 7374 7228 686f 7572 7329 2b22  d "+str(hours)+"
+00001690: 2068 7220 222b 7374 7228 6d69 6e75 7465   hr "+str(minute
+000016a0: 7329 2b22 206d 2022 2b27 7b3a 2e34 677d  s)+" m "+'{:.4g}
+000016b0: 272e 666f 726d 6174 2873 6563 6f6e 6473  '.format(seconds
+000016c0: 292b 2220 7322 0d0a 0d0a 2020 2020 7265  )+" s"....    re
+000016d0: 7475 726e 2072 6574 0d0a 0d0a 6465 6620  turn ret....def 
+000016e0: 636c 6561 6e5f 666f 726d 6174 286e 756d  clean_format(num
+000016f0: 6265 7229 3a0d 0a20 2020 206f 7264 6572  ber):..    order
+00001700: 203d 202d 696e 7428 6e70 2e6c 6f67 3130   = -int(np.log10
+00001710: 286e 756d 6572 5f64 6973 706c 6179 5f63  (numer_display_c
+00001720: 7574 6f66 6629 290d 0a20 2020 2069 6620  utoff))..    if 
+00001730: 6e70 2e61 6273 286e 702e 7265 616c 286e  np.abs(np.real(n
+00001740: 756d 6265 7229 293e 6e75 6d65 725f 6375  umber))>numer_cu
+00001750: 746f 6666 2061 6e64 206e 702e 6162 7328  toff and np.abs(
+00001760: 6e70 2e69 6d61 6728 6e75 6d62 6572 2929  np.imag(number))
+00001770: 3c6e 756d 6572 5f63 7574 6f66 663a 0d0a  <numer_cutoff:..
+00001780: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00001790: 6f75 6e64 286e 702e 7265 616c 286e 756d  ound(np.real(num
+000017a0: 6265 7229 2c6f 7264 6572 290d 0a20 2020  ber),order)..   
+000017b0: 2065 6c69 6620 6e70 2e61 6273 286e 702e   elif np.abs(np.
+000017c0: 7265 616c 286e 756d 6265 7229 293c 6e75  real(number))<nu
+000017d0: 6d65 725f 6375 746f 6666 2061 6e64 206e  mer_cutoff and n
+000017e0: 702e 6162 7328 6e70 2e69 6d61 6728 6e75  p.abs(np.imag(nu
+000017f0: 6d62 6572 2929 3e6e 756d 6572 5f63 7574  mber))>numer_cut
+00001800: 6f66 663a 0d0a 2020 2020 2020 2020 7265  off:..        re
+00001810: 7475 726e 2072 6f75 6e64 286e 702e 696d  turn round(np.im
+00001820: 6167 286e 756d 6265 7229 2c6f 7264 6572  ag(number),order
+00001830: 292a 636f 6d70 6c65 7828 302c 3129 0d0a  )*complex(0,1)..
+00001840: 2020 2020 656c 6966 206e 702e 6162 7328      elif np.abs(
+00001850: 6e70 2e72 6561 6c28 6e75 6d62 6572 2929  np.real(number))
+00001860: 3c6e 756d 6572 5f63 7574 6f66 6620 616e  <numer_cutoff an
+00001870: 6420 6e70 2e61 6273 286e 702e 696d 6167  d np.abs(np.imag
+00001880: 286e 756d 6265 7229 293c 6e75 6d65 725f  (number))<numer_
+00001890: 6375 746f 6666 3a0d 0a20 2020 2020 2020  cutoff:..       
+000018a0: 2072 6574 7572 6e20 300d 0a20 2020 2065   return 0..    e
+000018b0: 6c73 653a 0d0a 2020 2020 2020 2020 7265  lse:..        re
+000018c0: 7475 726e 2072 6f75 6e64 286e 702e 7265  turn round(np.re
+000018d0: 616c 286e 756d 6265 7229 2c6f 7264 6572  al(number),order
+000018e0: 292b 726f 756e 6428 6e70 2e69 6d61 6728  )+round(np.imag(
+000018f0: 6e75 6d62 6572 292c 6f72 6465 7229 2a63  number),order)*c
+00001900: 6f6d 706c 6578 2830 2c31 290d 0a0d 0a64  omplex(0,1)....d
+00001910: 6566 206d 656d 6f72 795f 6469 7370 6c61  ef memory_displa
+00001920: 7928 7261 775f 6d65 6d6f 7279 293a 0d0a  y(raw_memory):..
+00001930: 2020 2020 6966 2072 6177 5f6d 656d 6f72      if raw_memor
+00001940: 793c 322a 2a31 303a 0d0a 2020 2020 2020  y<2**10:..      
+00001950: 2020 7265 7475 726e 2027 7b3a 2e34 677d    return '{:.4g}
+00001960: 272e 666f 726d 6174 2872 6177 5f6d 656d  '.format(raw_mem
+00001970: 6f72 7929 2b22 2042 220d 0a20 2020 2065  ory)+" B"..    e
+00001980: 6c69 6620 7261 775f 6d65 6d6f 7279 3c32  lif raw_memory<2
+00001990: 2a2a 3230 3a0d 0a20 2020 2020 2020 2072  **20:..        r
+000019a0: 6574 7572 6e20 277b 3a2e 3467 7d27 2e66  eturn '{:.4g}'.f
+000019b0: 6f72 6d61 7428 7261 775f 6d65 6d6f 7279  ormat(raw_memory
+000019c0: 2f28 322a 2a31 3029 292b 2220 4b69 4222  /(2**10))+" KiB"
+000019d0: 0d0a 2020 2020 656c 6966 2072 6177 5f6d  ..    elif raw_m
+000019e0: 656d 6f72 793c 322a 2a33 303a 0d0a 2020  emory<2**30:..  
+000019f0: 2020 2020 2020 7265 7475 726e 2027 7b3a        return '{:
+00001a00: 2e34 677d 272e 666f 726d 6174 2872 6177  .4g}'.format(raw
+00001a10: 5f6d 656d 6f72 792f 2832 2a2a 3230 2929  _memory/(2**20))
+00001a20: 2b22 204d 6942 220d 0a20 2020 2065 6c69  +" MiB"..    eli
+00001a30: 6620 7261 775f 6d65 6d6f 7279 3c32 2a2a  f raw_memory<2**
+00001a40: 3430 3a0d 0a20 2020 2020 2020 2072 6574  40:..        ret
+00001a50: 7572 6e20 277b 3a2e 3467 7d27 2e66 6f72  urn '{:.4g}'.for
+00001a60: 6d61 7428 7261 775f 6d65 6d6f 7279 2f28  mat(raw_memory/(
+00001a70: 322a 2a33 3029 292b 2220 4769 4222 0d0a  2**30))+" GiB"..
+00001a80: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00001a90: 2020 2072 6574 7572 6e20 277b 3a2e 3467     return '{:.4g
+00001aa0: 7d27 2e66 6f72 6d61 7428 7261 775f 6d65  }'.format(raw_me
+00001ab0: 6d6f 7279 2f28 322a 2a34 3029 292b 2220  mory/(2**40))+" 
+00001ac0: 5469 4222 0d0a 0d0a 6465 6620 6375 7272  TiB"....def curr
+00001ad0: 656e 745f 6d65 6d6f 7279 5f64 6973 706c  ent_memory_displ
+00001ae0: 6179 2829 3a0d 0a20 2020 2072 6574 7572  ay():..    retur
+00001af0: 6e20 6d65 6d6f 7279 5f64 6973 706c 6179  n memory_display
+00001b00: 2874 7261 6365 6d61 6c6c 6f63 2e67 6574  (tracemalloc.get
+00001b10: 5f74 7261 6365 645f 6d65 6d6f 7279 2829  _traced_memory()
+00001b20: 5b30 5d29 2b22 2f22 2b6d 656d 6f72 795f  [0])+"/"+memory_
+00001b30: 6469 7370 6c61 7928 7472 6163 656d 616c  display(tracemal
+00001b40: 6c6f 632e 6765 745f 7472 6163 6564 5f6d  loc.get_traced_m
+00001b50: 656d 6f72 7928 295b 315d 290d 0a0d 0a64  emory()[1])....d
+00001b60: 6566 2067 6574 7369 7a65 2873 6861 7065  ef getsize(shape
+00001b70: 293a 0d0a 2020 2020 7265 7420 3d20 310d  ):..    ret = 1.
+00001b80: 0a20 2020 2066 6f72 2064 2069 6e20 7368  .    for d in sh
+00001b90: 6170 653a 0d0a 2020 2020 2020 2020 7265  ape:..        re
+00001ba0: 7420 2a3d 2064 0d0a 2020 2020 7265 7475  t *= d..    retu
+00001bb0: 726e 2072 6574 0d0a 0d0a 2323 2323 2323  rn ret....######
+00001bc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00001bd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001be0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001bf0: 2323 2323 2323 230d 0a23 2320 2020 2020  #######..##     
-00001c00: 2020 2020 2020 2020 4465 6e73 6564 2047          Densed G
-00001c10: 7261 7373 6d61 6e6e 2041 7272 6179 2020  rassmann Array  
-00001c20: 2020 2020 2020 2020 2020 2023 230d 0a23             ##..#
+00001be0: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
+00001bf0: 2323 2020 2020 2020 2020 2020 2020 2044  ##             D
+00001c00: 656e 7365 6420 4772 6173 736d 616e 6e20  ensed Grassmann 
+00001c10: 4172 7261 7920 2020 2020 2020 2020 2020  Array           
+00001c20: 2020 2323 0d0a 2323 2323 2323 2323 2323    ##..##########
 00001c30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00001c40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001c50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00001c60: 2323 230d 0a0d 0a63 6c61 7373 2064 656e  ###....class den
-00001c70: 7365 3a0d 0a20 2020 2064 6566 205f 5f69  se:..    def __i
-00001c80: 6e69 745f 5f28 7365 6c66 2c20 6461 7461  nit__(self, data
-00001c90: 3d4e 6f6e 652c 2065 6e63 6f64 6572 203d  =None, encoder =
-00001ca0: 2022 6361 6e6f 6e69 6361 6c22 2c20 666f   "canonical", fo
-00001cb0: 726d 6174 203d 2022 7374 616e 6461 7264  rmat = "standard
-00001cc0: 222c 2073 7461 7469 7374 6963 3d4e 6f6e  ", statistic=Non
-00001cd0: 6529 3a0d 0a20 2020 200d 0a20 2020 2020  e):..    ..     
-00001ce0: 2020 2023 636f 7079 2064 656e 7365 2070     #copy dense p
-00001cf0: 726f 7065 7274 6965 730d 0a20 2020 2020  roperties..     
-00001d00: 2020 2073 656c 662e 6461 7461 203d 204e     self.data = N
-00001d10: 6f6e 650d 0a20 2020 2020 2020 2073 656c  one..        sel
-00001d20: 662e 7374 6174 6973 7469 6320 3d20 4e6f  f.statistic = No
-00001d30: 6e65 0d0a 2020 2020 2020 2020 7365 6c66  ne..        self
-00001d40: 2e66 6f72 6d61 7420 3d20 666f 726d 6174  .format = format
-00001d50: 0d0a 2020 2020 2020 2020 7365 6c66 2e65  ..        self.e
-00001d60: 6e63 6f64 6572 203d 2065 6e63 6f64 6572  ncoder = encoder
-00001d70: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
-00001d80: 6465 6661 756c 7420 3d20 5472 7565 0d0a  default = True..
-00001d90: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
-00001da0: 2865 6e63 6f64 6572 206e 6f74 2069 6e20  (encoder not in 
-00001db0: 656e 636f 6465 725f 7479 7065 293a 0d0a  encoder_type):..
-00001dc0: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-00001dd0: 7228 2245 7272 6f72 5b64 656e 7365 5d3a  r("Error[dense]:
-00001de0: 2055 6e6b 6e6f 776e 2065 6e63 6f64 6572   Unknown encoder
-00001df0: 2e22 290d 0a20 2020 2020 2020 2020 2020  .")..           
-00001e00: 200d 0a20 2020 2020 2020 2069 6628 666f   ..        if(fo
-00001e10: 726d 6174 206e 6f74 2069 6e20 666f 726d  rmat not in form
-00001e20: 6174 5f74 7970 6529 3a0d 0a20 2020 2020  at_type):..     
-00001e30: 2020 2020 2020 2065 7272 6f72 2822 4572         error("Er
-00001e40: 726f 725b 6465 6e73 655d 3a20 556e 6b6e  ror[dense]: Unkn
-00001e50: 6f77 6e20 666f 726d 6174 2e22 290d 0a20  own format.").. 
-00001e60: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00001e70: 2020 2020 2069 6628 7479 7065 2864 6174       if(type(dat
-00001e80: 6129 3d3d 6e70 2e61 7272 6179 206f 7220  a)==np.array or 
-00001e90: 7479 7065 2864 6174 6129 3d3d 6e70 2e6e  type(data)==np.n
-00001ea0: 6461 7272 6179 206f 7220 7479 7065 2864  darray or type(d
-00001eb0: 6174 6129 3d3d 6c69 7374 293a 0d0a 2020  ata)==list):..  
-00001ec0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00001ed0: 6174 6120 3d20 6e70 2e61 7272 6179 2864  ata = np.array(d
-00001ee0: 6174 6129 0d0a 2020 2020 2020 2020 2020  ata)..          
-00001ef0: 2020 6465 6661 756c 7420 3d20 4661 6c73    default = Fals
-00001f00: 650d 0a20 2020 2020 2020 2065 6c69 6628  e..        elif(
-00001f10: 7479 7065 2864 6174 6129 3d3d 7370 2e43  type(data)==sp.C
-00001f20: 4f4f 293a 0d0a 2020 2020 2020 2020 2020  OO):..          
-00001f30: 2020 7365 6c66 2e64 6174 6120 203d 2064    self.data  = d
-00001f40: 6174 612e 746f 6465 6e73 6528 290d 0a20  ata.todense().. 
-00001f50: 2020 2020 2020 2020 2020 2064 6566 6175             defau
-00001f60: 6c74 203d 2046 616c 7365 0d0a 2020 2020  lt = False..    
-00001f70: 2020 2020 656c 6966 2874 7970 6528 6461      elif(type(da
-00001f80: 7461 293d 3d73 7061 7273 6529 3a0d 0a20  ta)==sparse):.. 
-00001f90: 2020 2020 2020 2020 2020 2023 636f 7079             #copy
-00001fa0: 2064 656e 7365 2070 726f 7065 7274 6965   dense propertie
-00001fb0: 730d 0a20 2020 2020 2020 2020 2020 2073  s..            s
-00001fc0: 656c 662e 6461 7461 203d 2064 6174 612e  elf.data = data.
-00001fd0: 6461 7461 2e74 6f64 656e 7365 2829 0d0a  data.todense()..
-00001fe0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001ff0: 2e73 7461 7469 7374 6963 203d 2064 6174  .statistic = dat
-00002000: 612e 7374 6174 6973 7469 630d 0a20 2020  a.statistic..   
-00002010: 2020 2020 2020 2020 2073 656c 662e 666f           self.fo
-00002020: 726d 6174 203d 2064 6174 612e 666f 726d  rmat = data.form
-00002030: 6174 0d0a 2020 2020 2020 2020 2020 2020  at..            
-00002040: 7365 6c66 2e65 6e63 6f64 6572 203d 2064  self.encoder = d
-00002050: 6174 612e 656e 636f 6465 720d 0a20 2020  ata.encoder..   
-00002060: 2020 2020 2020 2020 2064 6566 6175 6c74           default
-00002070: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
-00002080: 2020 656c 6966 2874 7970 6528 6461 7461    elif(type(data
-00002090: 293d 3d64 656e 7365 293a 0d0a 2020 2020  )==dense):..    
-000020a0: 2020 2020 2020 2020 2363 6f70 7920 6465          #copy de
-000020b0: 6e73 6520 7072 6f70 6572 7469 6573 0d0a  nse properties..
-000020c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000020d0: 2e64 6174 6120 3d20 6461 7461 2e64 6174  .data = data.dat
-000020e0: 612e 636f 7079 2829 0d0a 2020 2020 2020  a.copy()..      
-000020f0: 2020 2020 2020 7365 6c66 2e73 7461 7469        self.stati
-00002100: 7374 6963 203d 2064 6174 612e 7374 6174  stic = data.stat
-00002110: 6973 7469 630d 0a20 2020 2020 2020 2020  istic..         
-00002120: 2020 2073 656c 662e 666f 726d 6174 203d     self.format =
-00002130: 2064 6174 612e 666f 726d 6174 0d0a 2020   data.format..  
-00002140: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-00002150: 6e63 6f64 6572 203d 2064 6174 612e 656e  ncoder = data.en
-00002160: 636f 6465 720d 0a20 2020 2020 2020 2020  coder..         
-00002170: 2020 2064 6566 6175 6c74 203d 2046 616c     default = Fal
-00002180: 7365 0d0a 2020 2020 2020 2020 656c 6966  se..        elif
-00002190: 286e 702e 6973 7363 616c 6172 2864 6174  (np.isscalar(dat
-000021a0: 6129 293a 0d0a 2020 2020 2020 2020 2020  a)):..          
-000021b0: 2020 7365 6c66 2e64 6174 6120 3d20 6e70    self.data = np
-000021c0: 2e61 7272 6179 286c 6973 7428 5b64 6174  .array(list([dat
-000021d0: 615d 2929 0d0a 2020 2020 2020 2020 2020  a]))..          
-000021e0: 2020 6465 6661 756c 7420 3d20 4661 6c73    default = Fals
-000021f0: 650d 0a20 2020 2020 2020 2065 6c69 6628  e..        elif(
-00002200: 6461 7461 3d3d 4e6f 6e65 293a 0d0a 2020  data==None):..  
-00002210: 2020 2020 2020 2020 2020 226e 6f74 6869            "nothi
-00002220: 6e67 2074 6f20 7365 6520 6865 7265 220d  ng to see here".
-00002230: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00002240: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-00002250: 7228 2245 7272 6f72 5b64 656e 7365 5d3a  r("Error[dense]:
-00002260: 2049 6e76 616c 6964 2069 6e69 7469 616c   Invalid initial
-00002270: 697a 6564 2064 6174 612e 2229 0d0a 2020  ized data.")..  
-00002280: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00002290: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
-000022a0: 2073 7461 7469 7374 6963 2021 3d20 4e6f   statistic != No
-000022b0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-000022c0: 2073 656c 662e 7374 6174 6973 7469 6320   self.statistic 
-000022d0: 3d20 6d61 6b65 5f74 7570 6c65 2873 7461  = make_tuple(sta
-000022e0: 7469 7374 6963 290d 0a20 2020 2020 2020  tistic)..       
-000022f0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-00002300: 6620 6e6f 7420 6465 6661 756c 7420 616e  f not default an
-00002310: 6420 6e6f 7420 736b 6970 5f70 6f77 6572  d not skip_power
-00002320: 5f6f 665f 7477 6f5f 6368 6563 6b3a 0d0a  _of_two_check:..
-00002330: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00002340: 692c 6469 6d20 696e 2065 6e75 6d65 7261  i,dim in enumera
-00002350: 7465 2873 656c 662e 6461 7461 2e73 6861  te(self.data.sha
-00002360: 7065 293a 0d0a 2020 2020 2020 2020 2020  pe):..          
-00002370: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-00002380: 6174 6973 7469 635b 695d 2069 6e20 6665  atistic[i] in fe
-00002390: 726d 695f 7479 7065 2061 6e64 2064 696d  rmi_type and dim
-000023a0: 2021 3d20 696e 7428 322a 2a6d 6174 682e   != int(2**math.
-000023b0: 666c 6f6f 7228 6e70 2e6c 6f67 3228 6469  floor(np.log2(di
-000023c0: 6d29 2929 3a0d 0a20 2020 2020 2020 2020  m))):..         
-000023d0: 2020 2020 2020 2020 2020 2065 7272 6f72             error
-000023e0: 2822 4572 726f 725b 6465 6e73 655d 3a20  ("Error[dense]: 
-000023f0: 536f 6d65 206f 6620 7468 6520 6665 726d  Some of the ferm
-00002400: 696f 6e69 6320 7465 6e73 6f72 2073 6861  ionic tensor sha
-00002410: 7065 7320 6172 6520 6e6f 7420 6120 706f  pes are not a po
-00002420: 7765 7220 6f66 2074 776f 2e5c 6e20 2020  wer of two.\n   
-00002430: 2020 2020 2020 2020 2020 2048 6176 6520             Have 
-00002440: 796f 7520 6164 6465 6420 7468 6520 3c73  you added the <s
-00002450: 7461 7469 7374 6963 3e20 6172 6775 6d65  tatistic> argume
-00002460: 6e74 2077 6865 6e20 6361 6c6c 696e 6720  nt when calling 
-00002470: 7468 6973 2066 756e 6374 696f 6e3f 2229  this function?")
-00002480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002490: 2020 0d0a 2020 2020 6465 6620 5f5f 6765    ..    def __ge
-000024a0: 7469 7465 6d5f 5f28 7365 6c66 2c20 696e  titem__(self, in
-000024b0: 6465 7829 3a0d 0a20 2020 2020 2020 2072  dex):..        r
-000024c0: 6574 7572 6e20 7365 6c66 2e64 6174 615b  eturn self.data[
-000024d0: 696e 6465 785d 0d0a 2020 2020 0d0a 2020  index]..    ..  
-000024e0: 2020 6465 6620 5f5f 7365 7469 7465 6d5f    def __setitem_
-000024f0: 5f28 7365 6c66 2c20 696e 6465 782c 2076  _(self, index, v
-00002500: 616c 7565 293a 0d0a 2020 2020 2020 2020  alue):..        
-00002510: 7365 6c66 2e64 6174 615b 696e 6465 785d  self.data[index]
-00002520: 203d 2076 616c 7565 0d0a 2020 2020 2020   = value..      
-00002530: 2020 0d0a 2020 2020 4070 726f 7065 7274    ..    @propert
-00002540: 790d 0a20 2020 2064 6566 2073 6861 7065  y..    def shape
-00002550: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00002560: 2072 6574 7572 6e20 7365 6c66 2e64 6174   return self.dat
-00002570: 612e 7368 6170 650d 0a0d 0a20 2020 2040  a.shape....    @
-00002580: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
-00002590: 6620 7369 7a65 2873 656c 6629 3a0d 0a20  f size(self):.. 
-000025a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-000025b0: 6c66 2e64 6174 612e 7369 7a65 0d0a 0d0a  lf.data.size....
-000025c0: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-000025d0: 2020 2064 6566 206e 6469 6d28 7365 6c66     def ndim(self
-000025e0: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
-000025f0: 726e 2073 656c 662e 6461 7461 2e6e 6469  rn self.data.ndi
-00002600: 6d0d 0a0d 0a20 2020 2040 7072 6f70 6572  m....    @proper
-00002610: 7479 0d0a 2020 2020 6465 6620 6e6f 726d  ty..    def norm
-00002620: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00002630: 2061 7272 6179 5f66 6f72 6d20 3d20 7365   array_form = se
-00002640: 6c66 2e64 6174 610d 0a20 2020 2020 2020  lf.data..       
-00002650: 2072 6574 7572 6e20 6e70 2e6c 696e 616c   return np.linal
-00002660: 672e 6e6f 726d 2861 7272 6179 5f66 6f72  g.norm(array_for
-00002670: 6d29 0d0a 0d0a 2020 2020 4070 726f 7065  m)....    @prope
-00002680: 7274 790d 0a20 2020 2064 6566 206e 6e7a  rty..    def nnz
-00002690: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-000026a0: 2069 7465 7261 746f 7220 3d20 6e70 2e6e   iterator = np.n
-000026b0: 6469 7465 7228 7365 6c66 2c20 666c 6167  diter(self, flag
-000026c0: 733d 5b27 6d75 6c74 695f 696e 6465 7827  s=['multi_index'
-000026d0: 5d29 0d0a 2020 2020 2020 2020 6e20 3d20  ])..        n = 
-000026e0: 300d 0a20 2020 2020 2020 2066 6f72 2065  0..        for e
-000026f0: 6c65 6d65 6e74 2069 6e20 6974 6572 6174  lement in iterat
-00002700: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-00002710: 2063 6f6f 7264 7320 3d20 6974 6572 6174   coords = iterat
-00002720: 6f72 2e6d 756c 7469 5f69 6e64 6578 0d0a  or.multi_index..
-00002730: 2020 2020 2020 2020 2020 2020 6966 286e              if(n
-00002740: 702e 6162 7328 656c 656d 656e 742e 6974  p.abs(element.it
-00002750: 656d 2829 293e 6e75 6d65 725f 6469 7370  em())>numer_disp
-00002760: 6c61 795f 6375 746f 6666 293a 0d0a 2020  lay_cutoff):..  
-00002770: 2020 2020 2020 2020 2020 2020 2020 6e2b                n+
-00002780: 3d31 0d0a 2020 2020 2020 2020 7265 7475  =1..        retu
-00002790: 726e 206e 0d0a 0d0a 2020 2020 6465 6620  rn n....    def 
-000027a0: 6469 7370 6c61 7928 7365 6c66 2c6e 616d  display(self,nam
-000027b0: 653d 4e6f 6e65 2c69 6e64 656e 745f 7369  e=None,indent_si
-000027c0: 7a65 3d30 293a 0d0a 0d0a 2020 2020 2020  ze=0):....      
-000027d0: 2020 696e 6465 6e74 203d 2022 220d 0a20    indent = "".. 
-000027e0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-000027f0: 7261 6e67 6528 696e 6465 6e74 5f73 697a  range(indent_siz
-00002800: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00002810: 2069 6e64 656e 742b 3d22 2022 0d0a 0d0a   indent+=" "....
-00002820: 2020 2020 2020 2020 7072 696e 7428 290d          print().
-00002830: 0a20 2020 2020 2020 2069 6620 6e61 6d65  .        if name
-00002840: 2021 3d20 4e6f 6e65 3a0d 0a20 2020 2020   != None:..     
-00002850: 2020 2020 2020 2070 7269 6e74 2869 6e64         print(ind
-00002860: 656e 742b 2220 2020 2020 2020 206e 616d  ent+"        nam
-00002870: 653a 222c 6e61 6d65 290d 0a20 2020 2020  e:",name)..     
-00002880: 2020 2070 7269 6e74 2869 6e64 656e 742b     print(indent+
-00002890: 2220 2061 7272 6179 2074 7970 653a 2064  "  array type: d
-000028a0: 656e 7365 2229 0d0a 2020 2020 2020 2020  ense")..        
-000028b0: 7072 696e 7428 696e 6465 6e74 2b22 2020  print(indent+"  
-000028c0: 2020 2020 2073 6861 7065 3a22 2c73 656c       shape:",sel
-000028d0: 662e 7368 6170 6529 0d0a 2020 2020 2020  f.shape)..      
-000028e0: 2020 7072 696e 7428 696e 6465 6e74 2b22    print(indent+"
-000028f0: 2020 2020 2064 656e 7369 7479 3a22 2c73       density:",s
-00002900: 656c 662e 6e6e 7a2c 222f 222c 7365 6c66  elf.nnz,"/",self
-00002910: 2e73 697a 652c 227e 222c 7365 6c66 2e6e  .size,"~",self.n
-00002920: 6e7a 2f73 656c 662e 7369 7a65 2a31 3030  nz/self.size*100
-00002930: 2c22 2522 290d 0a20 2020 2020 2020 2070  ,"%")..        p
-00002940: 7269 6e74 2869 6e64 656e 742b 2220 2020  rint(indent+"   
-00002950: 7374 6174 6973 7469 633a 222c 7365 6c66  statistic:",self
-00002960: 2e73 7461 7469 7374 6963 290d 0a20 2020  .statistic)..   
-00002970: 2020 2020 2070 7269 6e74 2869 6e64 656e       print(inden
-00002980: 742b 2220 2020 2020 2066 6f72 6d61 743a  t+"      format:
-00002990: 222c 7365 6c66 2e66 6f72 6d61 7429 0d0a  ",self.format)..
-000029a0: 2020 2020 2020 2020 7072 696e 7428 696e          print(in
-000029b0: 6465 6e74 2b22 2020 2020 2065 6e63 6f64  dent+"     encod
-000029c0: 6572 3a22 2c73 656c 662e 656e 636f 6465  er:",self.encode
-000029d0: 7229 0d0a 2020 2020 2020 2020 7072 696e  r)..        prin
-000029e0: 7428 696e 6465 6e74 2b22 2020 2020 2020  t(indent+"      
-000029f0: 6d65 6d6f 7279 3a22 2c6d 656d 6f72 795f  memory:",memory_
-00002a00: 6469 7370 6c61 7928 7379 732e 6765 7473  display(sys.gets
-00002a10: 697a 656f 6628 7365 6c66 2e64 6174 6129  izeof(self.data)
-00002a20: 2b73 7973 2e67 6574 7369 7a65 6f66 2873  +sys.getsizeof(s
-00002a30: 656c 6629 2929 0d0a 2020 2020 2020 2020  elf)))..        
-00002a40: 7072 696e 7428 696e 6465 6e74 2b22 2020  print(indent+"  
-00002a50: 2020 2020 2020 6e6f 726d 3a22 2c73 656c        norm:",sel
-00002a60: 662e 6e6f 726d 290d 0a20 2020 2020 2020  f.norm)..       
-00002a70: 2070 7269 6e74 2869 6e64 656e 742b 2220   print(indent+" 
-00002a80: 2020 2020 656e 7472 6965 733a 2229 0d0a      entries:")..
-00002a90: 2020 2020 2020 2020 6974 6572 6174 6f72          iterator
-00002aa0: 203d 206e 702e 6e64 6974 6572 2873 656c   = np.nditer(sel
-00002ab0: 662c 2066 6c61 6773 3d5b 276d 756c 7469  f, flags=['multi
-00002ac0: 5f69 6e64 6578 275d 290d 0a20 2020 2020  _index'])..     
-00002ad0: 2020 2066 6f72 2065 6c65 6d65 6e74 2069     for element i
-00002ae0: 6e20 6974 6572 6174 6f72 3a0d 0a20 2020  n iterator:..   
-00002af0: 2020 2020 2020 2020 2063 6f6f 7264 7320           coords 
-00002b00: 3d20 6974 6572 6174 6f72 2e6d 756c 7469  = iterator.multi
-00002b10: 5f69 6e64 6578 0d0a 2020 2020 2020 2020  _index..        
-00002b20: 2020 2020 6966 286e 702e 6162 7328 656c      if(np.abs(el
-00002b30: 656d 656e 742e 6974 656d 2829 293e 6e75  ement.item())>nu
-00002b40: 6d65 725f 6469 7370 6c61 795f 6375 746f  mer_display_cuto
-00002b50: 6666 293a 0d0a 2020 2020 2020 2020 2020  ff):..          
-00002b60: 2020 2020 2020 7072 696e 7428 696e 6465        print(inde
-00002b70: 6e74 2b22 5c74 222c 636f 6f72 6473 2c63  nt+"\t",coords,c
-00002b80: 6c65 616e 5f66 6f72 6d61 7428 656c 656d  lean_format(elem
-00002b90: 656e 742e 6974 656d 2829 2929 0d0a 2020  ent.item()))..  
-00002ba0: 2020 2020 2020 7072 696e 7428 290d 0a0d        print()...
-00002bb0: 0a20 2020 2064 6566 2069 6e66 6f28 7365  .    def info(se
-00002bc0: 6c66 2c6e 616d 653d 4e6f 6e65 2c69 6e64  lf,name=None,ind
-00002bd0: 656e 745f 7369 7a65 3d30 293a 0d0a 0d0a  ent_size=0):....
-00002be0: 2020 2020 2020 2020 696e 6465 6e74 203d          indent =
-00002bf0: 2022 220d 0a20 2020 2020 2020 2066 6f72   ""..        for
-00002c00: 2069 2069 6e20 7261 6e67 6528 696e 6465   i in range(inde
-00002c10: 6e74 5f73 697a 6529 3a0d 0a20 2020 2020  nt_size):..     
-00002c20: 2020 2020 2020 2069 6e64 656e 742b 3d22         indent+="
-00002c30: 2022 0d0a 0d0a 2020 2020 2020 2020 7072   "....        pr
-00002c40: 696e 7428 290d 0a20 2020 2020 2020 2069  int()..        i
-00002c50: 6620 6e61 6d65 2021 3d20 4e6f 6e65 3a0d  f name != None:.
-00002c60: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00002c70: 6e74 2869 6e64 656e 742b 2220 2020 2020  nt(indent+"     
-00002c80: 2020 206e 616d 653a 222c 6e61 6d65 290d     name:",name).
-00002c90: 0a20 2020 2020 2020 2070 7269 6e74 2869  .        print(i
-00002ca0: 6e64 656e 742b 2220 2061 7272 6179 2074  ndent+"  array t
-00002cb0: 7970 653a 2064 656e 7365 2229 0d0a 2020  ype: dense")..  
-00002cc0: 2020 2020 2020 7072 696e 7428 696e 6465        print(inde
-00002cd0: 6e74 2b22 2020 2020 2020 2073 6861 7065  nt+"       shape
-00002ce0: 3a22 2c73 656c 662e 7368 6170 6529 0d0a  :",self.shape)..
-00002cf0: 2020 2020 2020 2020 7072 696e 7428 696e          print(in
-00002d00: 6465 6e74 2b22 2020 2020 2064 656e 7369  dent+"     densi
-00002d10: 7479 3a22 2c73 656c 662e 6e6e 7a2c 222f  ty:",self.nnz,"/
-00002d20: 222c 7365 6c66 2e73 697a 652c 227e 222c  ",self.size,"~",
-00002d30: 7365 6c66 2e6e 6e7a 2f73 656c 662e 7369  self.nnz/self.si
-00002d40: 7a65 2a31 3030 2c22 2522 290d 0a20 2020  ze*100,"%")..   
-00002d50: 2020 2020 2070 7269 6e74 2869 6e64 656e       print(inden
-00002d60: 742b 2220 2020 7374 6174 6973 7469 633a  t+"   statistic:
-00002d70: 222c 7365 6c66 2e73 7461 7469 7374 6963  ",self.statistic
-00002d80: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-00002d90: 2869 6e64 656e 742b 2220 2020 2020 2066  (indent+"      f
-00002da0: 6f72 6d61 743a 222c 7365 6c66 2e66 6f72  ormat:",self.for
-00002db0: 6d61 7429 0d0a 2020 2020 2020 2020 7072  mat)..        pr
-00002dc0: 696e 7428 696e 6465 6e74 2b22 2020 2020  int(indent+"    
-00002dd0: 2065 6e63 6f64 6572 3a22 2c73 656c 662e   encoder:",self.
-00002de0: 656e 636f 6465 7229 0d0a 2020 2020 2020  encoder)..      
-00002df0: 2020 7072 696e 7428 696e 6465 6e74 2b22    print(indent+"
-00002e00: 2020 2020 2020 6d65 6d6f 7279 3a22 2c6d        memory:",m
-00002e10: 656d 6f72 795f 6469 7370 6c61 7928 7379  emory_display(sy
-00002e20: 732e 6765 7473 697a 656f 6628 7365 6c66  s.getsizeof(self
-00002e30: 2e64 6174 6129 2b73 7973 2e67 6574 7369  .data)+sys.getsi
-00002e40: 7a65 6f66 2873 656c 6629 2929 0d0a 2020  zeof(self)))..  
-00002e50: 2020 2020 2020 7072 696e 7428 696e 6465        print(inde
-00002e60: 6e74 2b22 2020 2020 2020 2020 6e6f 726d  nt+"        norm
-00002e70: 3a22 2c73 656c 662e 6e6f 726d 290d 0a20  :",self.norm).. 
-00002e80: 2020 2020 2020 2070 7269 6e74 2829 0d0a         print()..
-00002e90: 0d0a 2020 2020 6465 6620 636f 7079 2873  ..    def copy(s
-00002ea0: 656c 6629 3a0d 0a20 2020 2020 2020 2023  elf):..        #
-00002eb0: 636f 7079 2064 656e 7365 2070 726f 7065  copy dense prope
-00002ec0: 7274 6965 730d 0a20 2020 2020 2020 2072  rties..        r
-00002ed0: 6574 203d 2064 656e 7365 2829 0d0a 2020  et = dense()..  
-00002ee0: 2020 2020 2020 7265 742e 6461 7461 203d        ret.data =
-00002ef0: 2073 656c 662e 6461 7461 2e63 6f70 7928   self.data.copy(
-00002f00: 290d 0a20 2020 2020 2020 2072 6574 2e73  )..        ret.s
-00002f10: 7461 7469 7374 6963 203d 2073 656c 662e  tatistic = self.
-00002f20: 7374 6174 6973 7469 630d 0a20 2020 2020  statistic..     
-00002f30: 2020 2072 6574 2e66 6f72 6d61 7420 3d20     ret.format = 
-00002f40: 7365 6c66 2e66 6f72 6d61 740d 0a20 2020  self.format..   
-00002f50: 2020 2020 2072 6574 2e65 6e63 6f64 6572       ret.encoder
-00002f60: 203d 2073 656c 662e 656e 636f 6465 720d   = self.encoder.
-00002f70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002f80: 7265 740d 0a20 2020 200d 0a20 2020 2064  ret..    ..    d
-00002f90: 6566 205f 5f61 6464 5f5f 2873 656c 662c  ef __add__(self,
-00002fa0: 206f 7468 6572 293a 0d0a 2020 2020 2020   other):..      
-00002fb0: 2020 6966 2873 656c 662e 7368 6170 6521    if(self.shape!
-00002fc0: 3d6f 7468 6572 2e73 6861 7065 0d0a 2020  =other.shape..  
-00002fd0: 2020 2020 2020 2020 2020 6f72 2073 656c            or sel
-00002fe0: 662e 7374 6174 6973 7469 6321 3d6f 7468  f.statistic!=oth
-00002ff0: 6572 2e73 7461 7469 7374 6963 0d0a 2020  er.statistic..  
-00003000: 2020 2020 2020 2020 2020 206f 7220 7365             or se
-00003010: 6c66 2e66 6f72 6d61 7421 3d6f 7468 6572  lf.format!=other
-00003020: 2e66 6f72 6d61 740d 0a20 2020 2020 2020  .format..       
-00003030: 2020 2020 2020 206f 7220 7365 6c66 2e65         or self.e
-00003040: 6e63 6f64 6572 213d 6f74 6865 722e 656e  ncoder!=other.en
-00003050: 636f 6465 7229 3a0d 0a20 2020 2020 2020  coder):..       
-00003060: 2020 2020 2065 7272 6f72 2822 4572 726f       error("Erro
-00003070: 725b 6465 6e73 652e 2b5d 3a20 496e 636f  r[dense.+]: Inco
-00003080: 6e73 6973 7465 6e74 206f 626a 6563 7420  nsistent object 
-00003090: 7072 6f70 6572 7469 6573 2229 0d0a 2020  properties")..  
-000030a0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000030b0: 2020 2020 7265 7420 3d20 7365 6c66 2e63      ret = self.c
-000030c0: 6f70 7928 290d 0a20 2020 2020 2020 2072  opy()..        r
-000030d0: 6574 2e64 6174 6120 3d20 7265 742e 6461  et.data = ret.da
-000030e0: 7461 2b6f 7468 6572 2e64 6174 610d 0a20  ta+other.data.. 
-000030f0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00003100: 740d 0a20 2020 2020 2020 200d 0a20 2020  t..        ..   
-00003110: 2064 6566 205f 5f73 7562 5f5f 2873 656c   def __sub__(sel
-00003120: 662c 206f 7468 6572 293a 0d0a 2020 2020  f, other):..    
-00003130: 2020 2020 6966 2873 656c 662e 7368 6170      if(self.shap
-00003140: 6521 3d6f 7468 6572 2e73 6861 7065 0d0a  e!=other.shape..
-00003150: 2020 2020 2020 2020 2020 2020 6f72 2073              or s
-00003160: 656c 662e 7374 6174 6973 7469 6321 3d6f  elf.statistic!=o
-00003170: 7468 6572 2e73 7461 7469 7374 6963 0d0a  ther.statistic..
-00003180: 2020 2020 2020 2020 2020 2020 206f 7220               or 
-00003190: 7365 6c66 2e66 6f72 6d61 7421 3d6f 7468  self.format!=oth
-000031a0: 6572 2e66 6f72 6d61 740d 0a20 2020 2020  er.format..     
-000031b0: 2020 2020 2020 2020 206f 7220 7365 6c66           or self
-000031c0: 2e65 6e63 6f64 6572 213d 6f74 6865 722e  .encoder!=other.
-000031d0: 656e 636f 6465 7229 3a0d 0a20 2020 2020  encoder):..     
-000031e0: 2020 2020 2020 2065 7272 6f72 2822 4572         error("Er
-000031f0: 726f 725b 6465 6e73 652e 2d5d 3a20 496e  ror[dense.-]: In
-00003200: 636f 6e73 6973 7465 6e74 206f 626a 6563  consistent objec
-00003210: 7420 7072 6f70 6572 7469 6573 2229 0d0a  t properties")..
-00003220: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00003230: 2020 2020 2020 7265 7420 3d20 7365 6c66        ret = self
-00003240: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
-00003250: 2072 6574 2e64 6174 6120 3d20 7265 742e   ret.data = ret.
-00003260: 6461 7461 2d6f 7468 6572 2e64 6174 610d  data-other.data.
-00003270: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00003280: 7265 740d 0a20 2020 2020 2020 200d 0a20  ret..        .. 
-00003290: 2020 2064 6566 205f 5f6d 756c 5f5f 2873     def __mul__(s
-000032a0: 656c 662c 206f 7468 6572 293a 0d0a 2020  elf, other):..  
-000032b0: 2020 2020 2020 7265 7420 3d20 7365 6c66        ret = self
-000032c0: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
-000032d0: 2072 6574 2e64 6174 6120 3d20 7265 742e   ret.data = ret.
-000032e0: 6461 7461 2a6f 7468 6572 0d0a 2020 2020  data*other..    
-000032f0: 2020 2020 7265 7475 726e 2072 6574 0d0a      return ret..
-00003300: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-00003310: 6620 5f5f 726d 756c 5f5f 2873 656c 662c  f __rmul__(self,
-00003320: 206f 7468 6572 293a 0d0a 2020 2020 2020   other):..      
-00003330: 2020 7265 7475 726e 2073 656c 662a 6f74    return self*ot
-00003340: 6865 720d 0a20 2020 2020 2020 200d 0a20  her..        .. 
-00003350: 2020 2064 6566 205f 5f6c 656e 5f5f 2873     def __len__(s
-00003360: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00003370: 6574 7572 6e20 6c65 6e28 7365 6c66 2e64  eturn len(self.d
-00003380: 6174 6129 0d0a 2020 2020 0d0a 2020 2020  ata)..    ..    
-00003390: 6465 6620 5f5f 7374 725f 5f28 7365 6c66  def __str__(self
-000033a0: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
-000033b0: 726e 2073 7472 2873 656c 662e 6461 7461  rn str(self.data
-000033c0: 290d 0a20 2020 200d 0a20 2020 2064 6566  )..    ..    def
-000033d0: 205f 5f72 6570 725f 5f28 7365 6c66 293a   __repr__(self):
-000033e0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000033f0: 2072 6570 7228 7365 6c66 2e64 6174 6129   repr(self.data)
-00003400: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00003410: 6465 6620 7377 6974 6368 5f66 6f72 6d61  def switch_forma
-00003420: 7428 7365 6c66 2c73 6176 655f 6d65 6d6f  t(self,save_memo
-00003430: 7279 3d46 616c 7365 293a 0d0a 2020 2020  ry=False):..    
-00003440: 2020 2020 2320 6d75 6c74 6970 6c79 2073      # multiply s
-00003450: 6967 6e20 6661 6374 6f72 2073 6967 6d61  ign factor sigma
-00003460: 5b69 5d20 746f 2065 7665 7279 2063 6f6e  [i] to every con
-00003470: 6a75 6761 7465 6420 696e 6469 6365 7320  jugated indices 
-00003480: 690d 0a0d 0a20 2020 2020 2020 2023 3a3a  i....        #::
+00001c50: 2323 2323 2323 2323 2323 0d0a 0d0a 636c  ##########....cl
+00001c60: 6173 7320 6465 6e73 653a 0d0a 2020 2020  ass dense:..    
+00001c70: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00001c80: 662c 2064 6174 613d 4e6f 6e65 2c20 656e  f, data=None, en
+00001c90: 636f 6465 7220 3d20 2263 616e 6f6e 6963  coder = "canonic
+00001ca0: 616c 222c 2066 6f72 6d61 7420 3d20 2273  al", format = "s
+00001cb0: 7461 6e64 6172 6422 2c20 7374 6174 6973  tandard", statis
+00001cc0: 7469 633d 4e6f 6e65 293a 0d0a 2020 2020  tic=None):..    
+00001cd0: 0d0a 2020 2020 2020 2020 2363 6f70 7920  ..        #copy 
+00001ce0: 6465 6e73 6520 7072 6f70 6572 7469 6573  dense properties
+00001cf0: 0d0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+00001d00: 6174 6120 3d20 4e6f 6e65 0d0a 2020 2020  ata = None..    
+00001d10: 2020 2020 7365 6c66 2e73 7461 7469 7374      self.statist
+00001d20: 6963 203d 204e 6f6e 650d 0a20 2020 2020  ic = None..     
+00001d30: 2020 2073 656c 662e 666f 726d 6174 203d     self.format =
+00001d40: 2066 6f72 6d61 740d 0a20 2020 2020 2020   format..       
+00001d50: 2073 656c 662e 656e 636f 6465 7220 3d20   self.encoder = 
+00001d60: 656e 636f 6465 720d 0a20 2020 200d 0a20  encoder..    .. 
+00001d70: 2020 2020 2020 2064 6566 6175 6c74 203d         default =
+00001d80: 2054 7275 650d 0a20 2020 200d 0a20 2020   True..    ..   
+00001d90: 2020 2020 2069 6628 656e 636f 6465 7220       if(encoder 
+00001da0: 6e6f 7420 696e 2065 6e63 6f64 6572 5f74  not in encoder_t
+00001db0: 7970 6529 3a0d 0a20 2020 2020 2020 2020  ype):..         
+00001dc0: 2020 2065 7272 6f72 2822 4572 726f 725b     error("Error[
+00001dd0: 6465 6e73 655d 3a20 556e 6b6e 6f77 6e20  dense]: Unknown 
+00001de0: 656e 636f 6465 722e 2229 0d0a 2020 2020  encoder.")..    
+00001df0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00001e00: 2020 6966 2866 6f72 6d61 7420 6e6f 7420    if(format not 
+00001e10: 696e 2066 6f72 6d61 745f 7479 7065 293a  in format_type):
+00001e20: 0d0a 2020 2020 2020 2020 2020 2020 6572  ..            er
+00001e30: 726f 7228 2245 7272 6f72 5b64 656e 7365  ror("Error[dense
+00001e40: 5d3a 2055 6e6b 6e6f 776e 2066 6f72 6d61  ]: Unknown forma
+00001e50: 742e 2229 0d0a 2020 2020 2020 2020 2020  t.")..          
+00001e60: 2020 0d0a 2020 2020 2020 2020 6966 2874    ..        if(t
+00001e70: 7970 6528 6461 7461 293d 3d6e 702e 6172  ype(data)==np.ar
+00001e80: 7261 7920 6f72 2074 7970 6528 6461 7461  ray or type(data
+00001e90: 293d 3d6e 702e 6e64 6172 7261 7920 6f72  )==np.ndarray or
+00001ea0: 2074 7970 6528 6461 7461 293d 3d6c 6973   type(data)==lis
+00001eb0: 7429 3a0d 0a20 2020 2020 2020 2020 2020  t):..           
+00001ec0: 2073 656c 662e 6461 7461 203d 206e 702e   self.data = np.
+00001ed0: 6172 7261 7928 6461 7461 290d 0a20 2020  array(data)..   
+00001ee0: 2020 2020 2020 2020 2064 6566 6175 6c74           default
+00001ef0: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
+00001f00: 2020 656c 6966 2874 7970 6528 6461 7461    elif(type(data
+00001f10: 293d 3d73 702e 434f 4f29 3a0d 0a20 2020  )==sp.COO):..   
+00001f20: 2020 2020 2020 2020 2073 656c 662e 6461           self.da
+00001f30: 7461 2020 3d20 6461 7461 2e74 6f64 656e  ta  = data.toden
+00001f40: 7365 2829 0d0a 2020 2020 2020 2020 2020  se()..          
+00001f50: 2020 6465 6661 756c 7420 3d20 4661 6c73    default = Fals
+00001f60: 650d 0a20 2020 2020 2020 2065 6c69 6628  e..        elif(
+00001f70: 7479 7065 2864 6174 6129 3d3d 7370 6172  type(data)==spar
+00001f80: 7365 293a 0d0a 2020 2020 2020 2020 2020  se):..          
+00001f90: 2020 2363 6f70 7920 6465 6e73 6520 7072    #copy dense pr
+00001fa0: 6f70 6572 7469 6573 0d0a 2020 2020 2020  operties..      
+00001fb0: 2020 2020 2020 7365 6c66 2e64 6174 6120        self.data 
+00001fc0: 3d20 6461 7461 2e64 6174 612e 746f 6465  = data.data.tode
+00001fd0: 6e73 6528 290d 0a20 2020 2020 2020 2020  nse()..         
+00001fe0: 2020 2073 656c 662e 7374 6174 6973 7469     self.statisti
+00001ff0: 6320 3d20 6461 7461 2e73 7461 7469 7374  c = data.statist
+00002000: 6963 0d0a 2020 2020 2020 2020 2020 2020  ic..            
+00002010: 7365 6c66 2e66 6f72 6d61 7420 3d20 6461  self.format = da
+00002020: 7461 2e66 6f72 6d61 740d 0a20 2020 2020  ta.format..     
+00002030: 2020 2020 2020 2073 656c 662e 656e 636f         self.enco
+00002040: 6465 7220 3d20 6461 7461 2e65 6e63 6f64  der = data.encod
+00002050: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
+00002060: 6465 6661 756c 7420 3d20 4661 6c73 650d  default = False.
+00002070: 0a20 2020 2020 2020 2065 6c69 6628 7479  .        elif(ty
+00002080: 7065 2864 6174 6129 3d3d 6465 6e73 6529  pe(data)==dense)
+00002090: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+000020a0: 636f 7079 2064 656e 7365 2070 726f 7065  copy dense prope
+000020b0: 7274 6965 730d 0a20 2020 2020 2020 2020  rties..         
+000020c0: 2020 2073 656c 662e 6461 7461 203d 2064     self.data = d
+000020d0: 6174 612e 6461 7461 2e63 6f70 7928 290d  ata.data.copy().
+000020e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000020f0: 662e 7374 6174 6973 7469 6320 3d20 6461  f.statistic = da
+00002100: 7461 2e73 7461 7469 7374 6963 0d0a 2020  ta.statistic..  
+00002110: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+00002120: 6f72 6d61 7420 3d20 6461 7461 2e66 6f72  ormat = data.for
+00002130: 6d61 740d 0a20 2020 2020 2020 2020 2020  mat..           
+00002140: 2073 656c 662e 656e 636f 6465 7220 3d20   self.encoder = 
+00002150: 6461 7461 2e65 6e63 6f64 6572 0d0a 2020  data.encoder..  
+00002160: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
+00002170: 7420 3d20 4661 6c73 650d 0a20 2020 2020  t = False..     
+00002180: 2020 2065 6c69 6628 6e70 2e69 7373 6361     elif(np.issca
+00002190: 6c61 7228 6461 7461 2929 3a0d 0a20 2020  lar(data)):..   
+000021a0: 2020 2020 2020 2020 2073 656c 662e 6461           self.da
+000021b0: 7461 203d 206e 702e 6172 7261 7928 6c69  ta = np.array(li
+000021c0: 7374 285b 6461 7461 5d29 290d 0a20 2020  st([data]))..   
+000021d0: 2020 2020 2020 2020 2064 6566 6175 6c74           default
+000021e0: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
+000021f0: 2020 656c 6966 2864 6174 613d 3d4e 6f6e    elif(data==Non
+00002200: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+00002210: 2022 6e6f 7468 696e 6720 746f 2073 6565   "nothing to see
+00002220: 2068 6572 6522 0d0a 2020 2020 2020 2020   here"..        
+00002230: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00002240: 2020 2065 7272 6f72 2822 4572 726f 725b     error("Error[
+00002250: 6465 6e73 655d 3a20 496e 7661 6c69 6420  dense]: Invalid 
+00002260: 696e 6974 6961 6c69 7a65 6420 6461 7461  initialized data
+00002270: 2e22 290d 0a20 2020 2020 2020 2020 2020  .")..           
+00002280: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
+00002290: 2020 2020 2069 6620 7374 6174 6973 7469       if statisti
+000022a0: 6320 213d 204e 6f6e 653a 0d0a 2020 2020  c != None:..    
+000022b0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+000022c0: 7469 7374 6963 203d 206d 616b 655f 7475  tistic = make_tu
+000022d0: 706c 6528 7374 6174 6973 7469 6329 0d0a  ple(statistic)..
+000022e0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000022f0: 2020 2020 2020 6966 206e 6f74 2064 6566        if not def
+00002300: 6175 6c74 2061 6e64 206e 6f74 2073 6b69  ault and not ski
+00002310: 705f 706f 7765 725f 6f66 5f74 776f 5f63  p_power_of_two_c
+00002320: 6865 636b 3a0d 0a20 2020 2020 2020 2020  heck:..         
+00002330: 2020 2066 6f72 2069 2c64 696d 2069 6e20     for i,dim in 
+00002340: 656e 756d 6572 6174 6528 7365 6c66 2e64  enumerate(self.d
+00002350: 6174 612e 7368 6170 6529 3a0d 0a20 2020  ata.shape):..   
+00002360: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00002370: 7365 6c66 2e73 7461 7469 7374 6963 5b69  self.statistic[i
+00002380: 5d20 696e 2066 6572 6d69 5f74 7970 6520  ] in fermi_type 
+00002390: 616e 6420 6469 6d20 213d 2069 6e74 2832  and dim != int(2
+000023a0: 2a2a 6d61 7468 2e66 6c6f 6f72 286e 702e  **math.floor(np.
+000023b0: 6c6f 6732 2864 696d 2929 293a 0d0a 2020  log2(dim))):..  
+000023c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023d0: 2020 6572 726f 7228 2245 7272 6f72 5b64    error("Error[d
+000023e0: 656e 7365 5d3a 2053 6f6d 6520 6f66 2074  ense]: Some of t
+000023f0: 6865 2066 6572 6d69 6f6e 6963 2074 656e  he fermionic ten
+00002400: 736f 7220 7368 6170 6573 2061 7265 206e  sor shapes are n
+00002410: 6f74 2061 2070 6f77 6572 206f 6620 7477  ot a power of tw
+00002420: 6f2e 5c6e 2020 2020 2020 2020 2020 2020  o.\n            
+00002430: 2020 4861 7665 2079 6f75 2061 6464 6564    Have you added
+00002440: 2074 6865 203c 7374 6174 6973 7469 633e   the <statistic>
+00002450: 2061 7267 756d 656e 7420 7768 656e 2063   argument when c
+00002460: 616c 6c69 6e67 2074 6869 7320 6675 6e63  alling this func
+00002470: 7469 6f6e 3f22 290d 0a20 2020 2020 2020  tion?")..       
+00002480: 2020 2020 2020 2020 200d 0a20 2020 2064           ..    d
+00002490: 6566 205f 5f67 6574 6974 656d 5f5f 2873  ef __getitem__(s
+000024a0: 656c 662c 2069 6e64 6578 293a 0d0a 2020  elf, index):..  
+000024b0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000024c0: 662e 6461 7461 5b69 6e64 6578 5d0d 0a20  f.data[index].. 
+000024d0: 2020 200d 0a20 2020 2064 6566 205f 5f73     ..    def __s
+000024e0: 6574 6974 656d 5f5f 2873 656c 662c 2069  etitem__(self, i
+000024f0: 6e64 6578 2c20 7661 6c75 6529 3a0d 0a20  ndex, value):.. 
+00002500: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
+00002510: 5b69 6e64 6578 5d20 3d20 7661 6c75 650d  [index] = value.
+00002520: 0a20 2020 2020 2020 200d 0a20 2020 2040  .        ..    @
+00002530: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
+00002540: 6620 7368 6170 6528 7365 6c66 293a 0d0a  f shape(self):..
+00002550: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00002560: 656c 662e 6461 7461 2e73 6861 7065 0d0a  elf.data.shape..
+00002570: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
+00002580: 0a20 2020 2064 6566 2073 697a 6528 7365  .    def size(se
+00002590: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
+000025a0: 7475 726e 2073 656c 662e 6461 7461 2e73  turn self.data.s
+000025b0: 697a 650d 0a0d 0a20 2020 2040 7072 6f70  ize....    @prop
+000025c0: 6572 7479 0d0a 2020 2020 6465 6620 6e64  erty..    def nd
+000025d0: 696d 2873 656c 6629 3a0d 0a20 2020 2020  im(self):..     
+000025e0: 2020 2072 6574 7572 6e20 7365 6c66 2e64     return self.d
+000025f0: 6174 612e 6e64 696d 0d0a 0d0a 2020 2020  ata.ndim....    
+00002600: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+00002610: 6566 206e 6f72 6d28 7365 6c66 293a 0d0a  ef norm(self):..
+00002620: 2020 2020 2020 2020 6172 7261 795f 666f          array_fo
+00002630: 726d 203d 2073 656c 662e 6461 7461 0d0a  rm = self.data..
+00002640: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00002650: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 6172  p.linalg.norm(ar
+00002660: 7261 795f 666f 726d 290d 0a0d 0a20 2020  ray_form)....   
+00002670: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
+00002680: 6465 6620 6e6e 7a28 7365 6c66 293a 0d0a  def nnz(self):..
+00002690: 2020 2020 2020 2020 6974 6572 6174 6f72          iterator
+000026a0: 203d 206e 702e 6e64 6974 6572 2873 656c   = np.nditer(sel
+000026b0: 662c 2066 6c61 6773 3d5b 276d 756c 7469  f, flags=['multi
+000026c0: 5f69 6e64 6578 275d 290d 0a20 2020 2020  _index'])..     
+000026d0: 2020 206e 203d 2030 0d0a 2020 2020 2020     n = 0..      
+000026e0: 2020 666f 7220 656c 656d 656e 7420 696e    for element in
+000026f0: 2069 7465 7261 746f 723a 0d0a 2020 2020   iterator:..    
+00002700: 2020 2020 2020 2020 636f 6f72 6473 203d          coords =
+00002710: 2069 7465 7261 746f 722e 6d75 6c74 695f   iterator.multi_
+00002720: 696e 6465 780d 0a20 2020 2020 2020 2020  index..         
+00002730: 2020 2069 6628 6e70 2e61 6273 2865 6c65     if(np.abs(ele
+00002740: 6d65 6e74 2e69 7465 6d28 2929 3e6e 756d  ment.item())>num
+00002750: 6572 5f64 6973 706c 6179 5f63 7574 6f66  er_display_cutof
+00002760: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
+00002770: 2020 2020 206e 2b3d 310d 0a20 2020 2020       n+=1..     
+00002780: 2020 2072 6574 7572 6e20 6e0d 0a0d 0a20     return n.... 
+00002790: 2020 2064 6566 2064 6973 706c 6179 2873     def display(s
+000027a0: 656c 662c 6e61 6d65 3d4e 6f6e 652c 696e  elf,name=None,in
+000027b0: 6465 6e74 5f73 697a 653d 3029 3a0d 0a0d  dent_size=0):...
+000027c0: 0a20 2020 2020 2020 2069 6e64 656e 7420  .        indent 
+000027d0: 3d20 2222 0d0a 2020 2020 2020 2020 666f  = ""..        fo
+000027e0: 7220 6920 696e 2072 616e 6765 2869 6e64  r i in range(ind
+000027f0: 656e 745f 7369 7a65 293a 0d0a 2020 2020  ent_size):..    
+00002800: 2020 2020 2020 2020 696e 6465 6e74 2b3d          indent+=
+00002810: 2220 220d 0a0d 0a20 2020 2020 2020 2070  " "....        p
+00002820: 7269 6e74 2829 0d0a 2020 2020 2020 2020  rint()..        
+00002830: 6966 206e 616d 6520 213d 204e 6f6e 653a  if name != None:
+00002840: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00002850: 696e 7428 696e 6465 6e74 2b22 2020 2020  int(indent+"    
+00002860: 2020 2020 6e61 6d65 3a22 2c6e 616d 6529      name:",name)
+00002870: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00002880: 696e 6465 6e74 2b22 2020 6172 7261 7920  indent+"  array 
+00002890: 7479 7065 3a20 6465 6e73 6522 290d 0a20  type: dense").. 
+000028a0: 2020 2020 2020 2070 7269 6e74 2869 6e64         print(ind
+000028b0: 656e 742b 2220 2020 2020 2020 7368 6170  ent+"       shap
+000028c0: 653a 222c 7365 6c66 2e73 6861 7065 290d  e:",self.shape).
+000028d0: 0a20 2020 2020 2020 2070 7269 6e74 2869  .        print(i
+000028e0: 6e64 656e 742b 2220 2020 2020 6465 6e73  ndent+"     dens
+000028f0: 6974 793a 222c 7365 6c66 2e6e 6e7a 2c22  ity:",self.nnz,"
+00002900: 2f22 2c73 656c 662e 7369 7a65 2c22 7e22  /",self.size,"~"
+00002910: 2c73 656c 662e 6e6e 7a2f 7365 6c66 2e73  ,self.nnz/self.s
+00002920: 697a 652a 3130 302c 2225 2229 0d0a 2020  ize*100,"%")..  
+00002930: 2020 2020 2020 7072 696e 7428 696e 6465        print(inde
+00002940: 6e74 2b22 2020 2073 7461 7469 7374 6963  nt+"   statistic
+00002950: 3a22 2c73 656c 662e 7374 6174 6973 7469  :",self.statisti
+00002960: 6329 0d0a 2020 2020 2020 2020 7072 696e  c)..        prin
+00002970: 7428 696e 6465 6e74 2b22 2020 2020 2020  t(indent+"      
+00002980: 666f 726d 6174 3a22 2c73 656c 662e 666f  format:",self.fo
+00002990: 726d 6174 290d 0a20 2020 2020 2020 2070  rmat)..        p
+000029a0: 7269 6e74 2869 6e64 656e 742b 2220 2020  rint(indent+"   
+000029b0: 2020 656e 636f 6465 723a 222c 7365 6c66    encoder:",self
+000029c0: 2e65 6e63 6f64 6572 290d 0a20 2020 2020  .encoder)..     
+000029d0: 2020 2070 7269 6e74 2869 6e64 656e 742b     print(indent+
+000029e0: 2220 2020 2020 206d 656d 6f72 793a 222c  "      memory:",
+000029f0: 6d65 6d6f 7279 5f64 6973 706c 6179 2873  memory_display(s
+00002a00: 7973 2e67 6574 7369 7a65 6f66 2873 656c  ys.getsizeof(sel
+00002a10: 662e 6461 7461 292b 7379 732e 6765 7473  f.data)+sys.gets
+00002a20: 697a 656f 6628 7365 6c66 2929 290d 0a20  izeof(self))).. 
+00002a30: 2020 2020 2020 2070 7269 6e74 2869 6e64         print(ind
+00002a40: 656e 742b 2220 2020 2020 2020 206e 6f72  ent+"        nor
+00002a50: 6d3a 222c 7365 6c66 2e6e 6f72 6d29 0d0a  m:",self.norm)..
+00002a60: 2020 2020 2020 2020 7072 696e 7428 696e          print(in
+00002a70: 6465 6e74 2b22 2020 2020 2065 6e74 7269  dent+"     entri
+00002a80: 6573 3a22 290d 0a20 2020 2020 2020 2069  es:")..        i
+00002a90: 7465 7261 746f 7220 3d20 6e70 2e6e 6469  terator = np.ndi
+00002aa0: 7465 7228 7365 6c66 2c20 666c 6167 733d  ter(self, flags=
+00002ab0: 5b27 6d75 6c74 695f 696e 6465 7827 5d29  ['multi_index'])
+00002ac0: 0d0a 2020 2020 2020 2020 666f 7220 656c  ..        for el
+00002ad0: 656d 656e 7420 696e 2069 7465 7261 746f  ement in iterato
+00002ae0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+00002af0: 636f 6f72 6473 203d 2069 7465 7261 746f  coords = iterato
+00002b00: 722e 6d75 6c74 695f 696e 6465 780d 0a20  r.multi_index.. 
+00002b10: 2020 2020 2020 2020 2020 2069 6628 6e70             if(np
+00002b20: 2e61 6273 2865 6c65 6d65 6e74 2e69 7465  .abs(element.ite
+00002b30: 6d28 2929 3e6e 756d 6572 5f64 6973 706c  m())>numer_displ
+00002b40: 6179 5f63 7574 6f66 6629 3a0d 0a20 2020  ay_cutoff):..   
+00002b50: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00002b60: 6e74 2869 6e64 656e 742b 225c 7422 2c63  nt(indent+"\t",c
+00002b70: 6f6f 7264 732c 636c 6561 6e5f 666f 726d  oords,clean_form
+00002b80: 6174 2865 6c65 6d65 6e74 2e69 7465 6d28  at(element.item(
+00002b90: 2929 290d 0a20 2020 2020 2020 2070 7269  )))..        pri
+00002ba0: 6e74 2829 0d0a 0d0a 2020 2020 6465 6620  nt()....    def 
+00002bb0: 696e 666f 2873 656c 662c 6e61 6d65 3d4e  info(self,name=N
+00002bc0: 6f6e 652c 696e 6465 6e74 5f73 697a 653d  one,indent_size=
+00002bd0: 3029 3a0d 0a0d 0a20 2020 2020 2020 2069  0):....        i
+00002be0: 6e64 656e 7420 3d20 2222 0d0a 2020 2020  ndent = ""..    
+00002bf0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00002c00: 6765 2869 6e64 656e 745f 7369 7a65 293a  ge(indent_size):
+00002c10: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+00002c20: 6465 6e74 2b3d 2220 220d 0a0d 0a20 2020  dent+=" "....   
+00002c30: 2020 2020 2070 7269 6e74 2829 0d0a 2020       print()..  
+00002c40: 2020 2020 2020 6966 206e 616d 6520 213d        if name !=
+00002c50: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00002c60: 2020 2020 7072 696e 7428 696e 6465 6e74      print(indent
+00002c70: 2b22 2020 2020 2020 2020 6e61 6d65 3a22  +"        name:"
+00002c80: 2c6e 616d 6529 0d0a 2020 2020 2020 2020  ,name)..        
+00002c90: 7072 696e 7428 696e 6465 6e74 2b22 2020  print(indent+"  
+00002ca0: 6172 7261 7920 7479 7065 3a20 6465 6e73  array type: dens
+00002cb0: 6522 290d 0a20 2020 2020 2020 2070 7269  e")..        pri
+00002cc0: 6e74 2869 6e64 656e 742b 2220 2020 2020  nt(indent+"     
+00002cd0: 2020 7368 6170 653a 222c 7365 6c66 2e73    shape:",self.s
+00002ce0: 6861 7065 290d 0a20 2020 2020 2020 2070  hape)..        p
+00002cf0: 7269 6e74 2869 6e64 656e 742b 2220 2020  rint(indent+"   
+00002d00: 2020 6465 6e73 6974 793a 222c 7365 6c66    density:",self
+00002d10: 2e6e 6e7a 2c22 2f22 2c73 656c 662e 7369  .nnz,"/",self.si
+00002d20: 7a65 2c22 7e22 2c73 656c 662e 6e6e 7a2f  ze,"~",self.nnz/
+00002d30: 7365 6c66 2e73 697a 652a 3130 302c 2225  self.size*100,"%
+00002d40: 2229 0d0a 2020 2020 2020 2020 7072 696e  ")..        prin
+00002d50: 7428 696e 6465 6e74 2b22 2020 2073 7461  t(indent+"   sta
+00002d60: 7469 7374 6963 3a22 2c73 656c 662e 7374  tistic:",self.st
+00002d70: 6174 6973 7469 6329 0d0a 2020 2020 2020  atistic)..      
+00002d80: 2020 7072 696e 7428 696e 6465 6e74 2b22    print(indent+"
+00002d90: 2020 2020 2020 666f 726d 6174 3a22 2c73        format:",s
+00002da0: 656c 662e 666f 726d 6174 290d 0a20 2020  elf.format)..   
+00002db0: 2020 2020 2070 7269 6e74 2869 6e64 656e       print(inden
+00002dc0: 742b 2220 2020 2020 656e 636f 6465 723a  t+"     encoder:
+00002dd0: 222c 7365 6c66 2e65 6e63 6f64 6572 290d  ",self.encoder).
+00002de0: 0a20 2020 2020 2020 2070 7269 6e74 2869  .        print(i
+00002df0: 6e64 656e 742b 2220 2020 2020 206d 656d  ndent+"      mem
+00002e00: 6f72 793a 222c 6d65 6d6f 7279 5f64 6973  ory:",memory_dis
+00002e10: 706c 6179 2873 7973 2e67 6574 7369 7a65  play(sys.getsize
+00002e20: 6f66 2873 656c 662e 6461 7461 292b 7379  of(self.data)+sy
+00002e30: 732e 6765 7473 697a 656f 6628 7365 6c66  s.getsizeof(self
+00002e40: 2929 290d 0a20 2020 2020 2020 2070 7269  )))..        pri
+00002e50: 6e74 2869 6e64 656e 742b 2220 2020 2020  nt(indent+"     
+00002e60: 2020 206e 6f72 6d3a 222c 7365 6c66 2e6e     norm:",self.n
+00002e70: 6f72 6d29 0d0a 2020 2020 2020 2020 7072  orm)..        pr
+00002e80: 696e 7428 290d 0a0d 0a20 2020 2064 6566  int()....    def
+00002e90: 2063 6f70 7928 7365 6c66 293a 0d0a 2020   copy(self):..  
+00002ea0: 2020 2020 2020 2363 6f70 7920 6465 6e73        #copy dens
+00002eb0: 6520 7072 6f70 6572 7469 6573 0d0a 2020  e properties..  
+00002ec0: 2020 2020 2020 7265 7420 3d20 6465 6e73        ret = dens
+00002ed0: 6528 290d 0a20 2020 2020 2020 2072 6574  e()..        ret
+00002ee0: 2e64 6174 6120 3d20 7365 6c66 2e64 6174  .data = self.dat
+00002ef0: 612e 636f 7079 2829 0d0a 2020 2020 2020  a.copy()..      
+00002f00: 2020 7265 742e 7374 6174 6973 7469 6320    ret.statistic 
+00002f10: 3d20 7365 6c66 2e73 7461 7469 7374 6963  = self.statistic
+00002f20: 0d0a 2020 2020 2020 2020 7265 742e 666f  ..        ret.fo
+00002f30: 726d 6174 203d 2073 656c 662e 666f 726d  rmat = self.form
+00002f40: 6174 0d0a 2020 2020 2020 2020 7265 742e  at..        ret.
+00002f50: 656e 636f 6465 7220 3d20 7365 6c66 2e65  encoder = self.e
+00002f60: 6e63 6f64 6572 0d0a 2020 2020 2020 2020  ncoder..        
+00002f70: 7265 7475 726e 2072 6574 0d0a 2020 2020  return ret..    
+00002f80: 0d0a 2020 2020 6465 6620 5f5f 6164 645f  ..    def __add_
+00002f90: 5f28 7365 6c66 2c20 6f74 6865 7229 3a0d  _(self, other):.
+00002fa0: 0a20 2020 2020 2020 2069 6628 7365 6c66  .        if(self
+00002fb0: 2e73 6861 7065 213d 6f74 6865 722e 7368  .shape!=other.sh
+00002fc0: 6170 650d 0a20 2020 2020 2020 2020 2020  ape..           
+00002fd0: 206f 7220 7365 6c66 2e73 7461 7469 7374   or self.statist
+00002fe0: 6963 213d 6f74 6865 722e 7374 6174 6973  ic!=other.statis
+00002ff0: 7469 630d 0a20 2020 2020 2020 2020 2020  tic..           
+00003000: 2020 6f72 2073 656c 662e 666f 726d 6174    or self.format
+00003010: 213d 6f74 6865 722e 666f 726d 6174 0d0a  !=other.format..
+00003020: 2020 2020 2020 2020 2020 2020 2020 6f72                or
+00003030: 2073 656c 662e 656e 636f 6465 7221 3d6f   self.encoder!=o
+00003040: 7468 6572 2e65 6e63 6f64 6572 293a 0d0a  ther.encoder):..
+00003050: 2020 2020 2020 2020 2020 2020 6572 726f              erro
+00003060: 7228 2245 7272 6f72 5b64 656e 7365 2e2b  r("Error[dense.+
+00003070: 5d3a 2049 6e63 6f6e 7369 7374 656e 7420  ]: Inconsistent 
+00003080: 6f62 6a65 6374 2070 726f 7065 7274 6965  object propertie
+00003090: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
+000030a0: 200d 0a20 2020 2020 2020 2072 6574 203d   ..        ret =
+000030b0: 2073 656c 662e 636f 7079 2829 0d0a 2020   self.copy()..  
+000030c0: 2020 2020 2020 7265 742e 6461 7461 203d        ret.data =
+000030d0: 2072 6574 2e64 6174 612b 6f74 6865 722e   ret.data+other.
+000030e0: 6461 7461 0d0a 2020 2020 2020 2020 7265  data..        re
+000030f0: 7475 726e 2072 6574 0d0a 2020 2020 2020  turn ret..      
+00003100: 2020 0d0a 2020 2020 6465 6620 5f5f 7375    ..    def __su
+00003110: 625f 5f28 7365 6c66 2c20 6f74 6865 7229  b__(self, other)
+00003120: 3a0d 0a20 2020 2020 2020 2069 6628 7365  :..        if(se
+00003130: 6c66 2e73 6861 7065 213d 6f74 6865 722e  lf.shape!=other.
+00003140: 7368 6170 650d 0a20 2020 2020 2020 2020  shape..         
+00003150: 2020 206f 7220 7365 6c66 2e73 7461 7469     or self.stati
+00003160: 7374 6963 213d 6f74 6865 722e 7374 6174  stic!=other.stat
+00003170: 6973 7469 630d 0a20 2020 2020 2020 2020  istic..         
+00003180: 2020 2020 6f72 2073 656c 662e 666f 726d      or self.form
+00003190: 6174 213d 6f74 6865 722e 666f 726d 6174  at!=other.format
+000031a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000031b0: 6f72 2073 656c 662e 656e 636f 6465 7221  or self.encoder!
+000031c0: 3d6f 7468 6572 2e65 6e63 6f64 6572 293a  =other.encoder):
+000031d0: 0d0a 2020 2020 2020 2020 2020 2020 6572  ..            er
+000031e0: 726f 7228 2245 7272 6f72 5b64 656e 7365  ror("Error[dense
+000031f0: 2e2d 5d3a 2049 6e63 6f6e 7369 7374 656e  .-]: Inconsisten
+00003200: 7420 6f62 6a65 6374 2070 726f 7065 7274  t object propert
+00003210: 6965 7322 290d 0a20 2020 2020 2020 2020  ies")..         
+00003220: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
+00003230: 203d 2073 656c 662e 636f 7079 2829 0d0a   = self.copy()..
+00003240: 2020 2020 2020 2020 7265 742e 6461 7461          ret.data
+00003250: 203d 2072 6574 2e64 6174 612d 6f74 6865   = ret.data-othe
+00003260: 722e 6461 7461 0d0a 2020 2020 2020 2020  r.data..        
+00003270: 7265 7475 726e 2072 6574 0d0a 2020 2020  return ret..    
+00003280: 2020 2020 0d0a 2020 2020 6465 6620 5f5f      ..    def __
+00003290: 6d75 6c5f 5f28 7365 6c66 2c20 6f74 6865  mul__(self, othe
+000032a0: 7229 3a0d 0a20 2020 2020 2020 2072 6574  r):..        ret
+000032b0: 203d 2073 656c 662e 636f 7079 2829 0d0a   = self.copy()..
+000032c0: 2020 2020 2020 2020 7265 742e 6461 7461          ret.data
+000032d0: 203d 2072 6574 2e64 6174 612a 6f74 6865   = ret.data*othe
+000032e0: 720d 0a20 2020 2020 2020 2072 6574 7572  r..        retur
+000032f0: 6e20 7265 740d 0a20 2020 2020 2020 200d  n ret..        .
+00003300: 0a20 2020 2064 6566 205f 5f72 6d75 6c5f  .    def __rmul_
+00003310: 5f28 7365 6c66 2c20 6f74 6865 7229 3a0d  _(self, other):.
+00003320: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00003330: 7365 6c66 2a6f 7468 6572 0d0a 2020 2020  self*other..    
+00003340: 2020 2020 0d0a 2020 2020 6465 6620 5f5f      ..    def __
+00003350: 6c65 6e5f 5f28 7365 6c66 293a 0d0a 2020  len__(self):..  
+00003360: 2020 2020 2020 7265 7475 726e 206c 656e        return len
+00003370: 2873 656c 662e 6461 7461 290d 0a20 2020  (self.data)..   
+00003380: 200d 0a20 2020 2064 6566 205f 5f73 7472   ..    def __str
+00003390: 5f5f 2873 656c 6629 3a0d 0a20 2020 2020  __(self):..     
+000033a0: 2020 2072 6574 7572 6e20 7374 7228 7365     return str(se
+000033b0: 6c66 2e64 6174 6129 0d0a 2020 2020 0d0a  lf.data)..    ..
+000033c0: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
+000033d0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+000033e0: 2072 6574 7572 6e20 7265 7072 2873 656c   return repr(sel
+000033f0: 662e 6461 7461 290d 0a20 2020 2020 2020  f.data)..       
+00003400: 200d 0a20 2020 2064 6566 2073 7769 7463   ..    def switc
+00003410: 685f 666f 726d 6174 2873 656c 662c 7361  h_format(self,sa
+00003420: 7665 5f6d 656d 6f72 793d 4661 6c73 6529  ve_memory=False)
+00003430: 3a0d 0a20 2020 2020 2020 2023 206d 756c  :..        # mul
+00003440: 7469 706c 7920 7369 676e 2066 6163 746f  tiply sign facto
+00003450: 7220 7369 676d 615b 695d 2074 6f20 6576  r sigma[i] to ev
+00003460: 6572 7920 636f 6e6a 7567 6174 6564 2069  ery conjugated i
+00003470: 6e64 6963 6573 2069 0d0a 0d0a 2020 2020  ndices i....    
+00003480: 2020 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a      #:::::::::::
 00003490: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 000034a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 000034b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 000034c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 000034d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000034e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000034f0: 3a3a 0d0a 2020 2020 2020 2020 2320 574f  ::..        # WO
-00003500: 524b 2049 4e20 5448 4520 464f 4c4c 4f57  RK IN THE FOLLOW
-00003510: 494e 4720 434f 4e44 4954 494f 4e53 2020  ING CONDITIONS  
-00003520: 2020 2020 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a      ::::::::::::
+000034e0: 3a3a 3a3a 3a3a 3a3a 3a0d 0a20 2020 2020  :::::::::..     
+000034f0: 2020 2023 2057 4f52 4b20 494e 2054 4845     # WORK IN THE
+00003500: 2046 4f4c 4c4f 5749 4e47 2043 4f4e 4449   FOLLOWING CONDI
+00003510: 5449 4f4e 5320 2020 2020 203a 3a3a 3a3a  TIONS      :::::
+00003520: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00003530: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00003540: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00003550: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00003560: 3a0d 0a20 2020 2020 2020 2023 2028 5749  :..        # (WI
-00003570: 4c4c 2043 4f4e 5645 5254 2041 5554 4f4d  LL CONVERT AUTOM
-00003580: 4154 4943 414c 4c59 2920 2020 2020 2020  ATICALLY)       
-00003590: 2020 203a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a     :::::::::::::
+00003550: 3a3a 3a3a 3a3a 3a3a 0d0a 2020 2020 2020  ::::::::..      
+00003560: 2020 2320 2857 494c 4c20 434f 4e56 4552    # (WILL CONVER
+00003570: 5420 4155 544f 4d41 5449 4341 4c4c 5929  T AUTOMATICALLY)
+00003580: 2020 2020 2020 2020 2020 3a3a 3a3a 3a3a            ::::::
+00003590: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 000035a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 000035b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000035c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000035d0: 0d0a 2020 2020 2020 2020 2320 2020 2d20  ..        #   - 
-000035e0: 6361 6e6f 6e69 6361 6c20 656e 636f 6465  canonical encode
-000035f0: 7220 2020 2020 2020 2020 2020 2020 2020  r               
-00003600: 2020 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a    ::::::::::::::
+000035c0: 3a3a 3a3a 3a3a 3a0d 0a20 2020 2020 2020  :::::::..       
+000035d0: 2023 2020 202d 2063 616e 6f6e 6963 616c   #   - canonical
+000035e0: 2065 6e63 6f64 6572 2020 2020 2020 2020   encoder        
+000035f0: 2020 2020 2020 2020 203a 3a3a 3a3a 3a3a           :::::::
+00003600: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00003610: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00003620: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00003630: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a0d  :::::::::::::::.
-00003640: 0a20 2020 2020 2020 2023 3a3a 3a3a 3a3a  .        #::::::
+00003630: 3a3a 3a3a 3a3a 0d0a 2020 2020 2020 2020  ::::::..        
+00003640: 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  #:::::::::::::::
 00003650: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00003660: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00003670: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00003680: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00003690: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000036a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a  ::::::::::::::..
-000036b0: 0d0a 2020 2020 2020 2020 6966 2073 6176  ..        if sav
-000036c0: 655f 6d65 6d6f 7279 203a 0d0a 2020 2020  e_memory :..    
-000036d0: 2020 2020 2020 2020 7265 7420 3d20 7365          ret = se
-000036e0: 6c66 0d0a 2020 2020 2020 2020 656c 7365  lf..        else
-000036f0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00003700: 6574 203d 2073 656c 662e 636f 7079 2829  et = self.copy()
-00003710: 0d0a 2020 2020 2020 2020 6966 2873 656c  ..        if(sel
-00003720: 662e 656e 636f 6465 723d 3d27 7061 7269  f.encoder=='pari
-00003730: 7479 2d70 7265 7365 7276 696e 6727 293a  ty-preserving'):
-00003740: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00003750: 7420 3d20 7265 742e 7377 6974 6368 5f65  t = ret.switch_e
-00003760: 6e63 6f64 6572 2873 6176 655f 6d65 6d6f  ncoder(save_memo
-00003770: 7279 3d54 7275 6529 0d0a 2020 2020 2020  ry=True)..      
-00003780: 2020 746f 5f63 616c 6320 3d20 5b5d 0d0a    to_calc = []..
-00003790: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-000037a0: 2072 616e 6765 2873 656c 662e 6e64 696d   range(self.ndim
-000037b0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000037c0: 746f 5f63 616c 6320 2b3d 2028 7265 742e  to_calc += (ret.
-000037d0: 7374 6174 6973 7469 635b 695d 3d3d 2d31  statistic[i]==-1
-000037e0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-000037f0: 6966 2872 6574 2e73 7461 7469 7374 6963  if(ret.statistic
-00003800: 5b69 5d3d 3d68 7962 7269 645f 7379 6d62  [i]==hybrid_symb
-00003810: 6f6c 293a 0d0a 2020 2020 2020 2020 2020  ol):..          
-00003820: 2020 2020 2020 6572 726f 7228 2245 7272        error("Err
-00003830: 6f72 5b73 7769 7463 685f 666f 726d 6174  or[switch_format
-00003840: 5d3a 2043 616e 6e6f 7420 7377 6974 6368  ]: Cannot switch
-00003850: 2066 6f72 6d61 7420 7769 7468 2061 2068   format with a h
-00003860: 7962 7269 6420 696e 6465 782e 5c6e 2020  ybrid index.\n  
-00003870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003880: 2020 2020 5370 6c69 7420 7468 656d 2069      Split them i
-00003890: 6e74 6f20 626f 736f 6e69 6320 616e 6420  nto bosonic and 
-000038a0: 6665 726d 696f 6e69 6320 6f6e 6573 2066  fermionic ones f
-000038b0: 6972 7374 2122 290d 0a20 2020 2020 2020  irst!")..       
-000038c0: 200d 0a20 2020 2020 2020 206b 3d30 0d0a   ..        k=0..
-000038d0: 2020 2020 2020 2020 6b6d 6178 203d 2072          kmax = r
-000038e0: 6574 2e6e 6469 6d0d 0a20 2020 2020 2020  et.ndim..       
-000038f0: 2073 3020 3d20 7469 6d65 2e74 696d 6528   s0 = time.time(
-00003900: 290d 0a20 2020 2020 2020 2073 3030 203d  )..        s00 =
-00003910: 2073 300d 0a20 2020 2020 2020 2070 7269   s0..        pri
-00003920: 6e74 2829 0d0a 0d0a 2020 2020 2020 2020  nt()....        
+000036a0: 3a3a 3a3a 3a0d 0a0d 0a20 2020 2020 2020  :::::....       
+000036b0: 2069 6620 7361 7665 5f6d 656d 6f72 7920   if save_memory 
+000036c0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+000036d0: 6574 203d 2073 656c 660d 0a20 2020 2020  et = self..     
+000036e0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+000036f0: 2020 2020 2020 7265 7420 3d20 7365 6c66        ret = self
+00003700: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
+00003710: 2069 6628 7365 6c66 2e65 6e63 6f64 6572   if(self.encoder
+00003720: 3d3d 2770 6172 6974 792d 7072 6573 6572  =='parity-preser
+00003730: 7669 6e67 2729 3a0d 0a20 2020 2020 2020  ving'):..       
+00003740: 2020 2020 2072 6574 203d 2072 6574 2e73       ret = ret.s
+00003750: 7769 7463 685f 656e 636f 6465 7228 7361  witch_encoder(sa
+00003760: 7665 5f6d 656d 6f72 793d 5472 7565 290d  ve_memory=True).
+00003770: 0a20 2020 2020 2020 2074 6f5f 6361 6c63  .        to_calc
+00003780: 203d 205b 5d0d 0a20 2020 2020 2020 2066   = []..        f
+00003790: 6f72 2069 2069 6e20 7261 6e67 6528 7365  or i in range(se
+000037a0: 6c66 2e6e 6469 6d29 3a0d 0a20 2020 2020  lf.ndim):..     
+000037b0: 2020 2020 2020 2074 6f5f 6361 6c63 202b         to_calc +
+000037c0: 3d20 2872 6574 2e73 7461 7469 7374 6963  = (ret.statistic
+000037d0: 5b69 5d3d 3d2d 3129 2c0d 0a20 2020 2020  [i]==-1),..     
+000037e0: 2020 2020 2020 2069 6628 7265 742e 7374         if(ret.st
+000037f0: 6174 6973 7469 635b 695d 3d3d 6879 6272  atistic[i]==hybr
+00003800: 6964 5f73 796d 626f 6c29 3a0d 0a20 2020  id_symbol):..   
+00003810: 2020 2020 2020 2020 2020 2020 2065 7272               err
+00003820: 6f72 2822 4572 726f 725b 7377 6974 6368  or("Error[switch
+00003830: 5f66 6f72 6d61 745d 3a20 4361 6e6e 6f74  _format]: Cannot
+00003840: 2073 7769 7463 6820 666f 726d 6174 2077   switch format w
+00003850: 6974 6820 6120 6879 6272 6964 2069 6e64  ith a hybrid ind
+00003860: 6578 2e5c 6e20 2020 2020 2020 2020 2020  ex.\n           
+00003870: 2020 2020 2020 2020 2020 2053 706c 6974             Split
+00003880: 2074 6865 6d20 696e 746f 2062 6f73 6f6e   them into boson
+00003890: 6963 2061 6e64 2066 6572 6d69 6f6e 6963  ic and fermionic
+000038a0: 206f 6e65 7320 6669 7273 7421 2229 0d0a   ones first!")..
+000038b0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000038c0: 2020 6b3d 300d 0a20 2020 2020 2020 206b    k=0..        k
+000038d0: 6d61 7820 3d20 7265 742e 6e64 696d 0d0a  max = ret.ndim..
+000038e0: 2020 2020 2020 2020 7330 203d 2074 696d          s0 = tim
+000038f0: 652e 7469 6d65 2829 0d0a 2020 2020 2020  e.time()..      
+00003900: 2020 7330 3020 3d20 7330 0d0a 2020 2020    s00 = s0..    
+00003910: 2020 2020 7072 6f67 7265 7373 5f73 7061      progress_spa
+00003920: 6365 2829 0d0a 0d0a 2020 2020 2020 2020  ce()....        
 00003930: 6461 7420 3d20 7265 742e 6461 7461 0d0a  dat = ret.data..
 00003940: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
 00003950: 2072 616e 6765 2872 6574 2e6e 6469 6d29   range(ret.ndim)
 00003960: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
 00003970: 6620 6e6f 7420 746f 5f63 616c 635b 695d  f not to_calc[i]
 00003980: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
 00003990: 2020 2020 636f 6e74 696e 7565 0d0a 0d0a      continue....
@@ -946,5908 +946,5884 @@
 00003b10: 222c 7261 7469 6f20 3d20 4661 6c73 652c  ",ratio = False,
 00003b20: 636f 6c6f 723d 2262 6c75 6522 2c74 696d  color="blue",tim
 00003b30: 653d 7469 6d65 2e74 696d 6528 292d 7330  e=time.time()-s0
 00003b40: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
 00003b50: 2020 2020 7330 203d 2074 696d 652e 7469      s0 = time.ti
 00003b60: 6d65 2829 0d0a 0d0a 2020 2020 2020 2020  me()....        
 00003b70: 636c 6561 725f 7072 6f67 7265 7373 2829  clear_progress()
-00003b80: 0d0a 2020 2020 2020 2020 7379 732e 7374  ..        sys.st
-00003b90: 646f 7574 2e77 7269 7465 2822 5c30 3333  dout.write("\033
-00003ba0: 5b46 2229 0d0a 0d0a 2020 2020 2020 2020  [F")....        
-00003bb0: 7265 742e 6461 7461 203d 2064 6174 0d0a  ret.data = dat..
-00003bc0: 0d0a 2020 2020 2020 2020 6966 2872 6574  ..        if(ret
-00003bd0: 2e66 6f72 6d61 743d 3d27 7374 616e 6461  .format=='standa
-00003be0: 7264 2729 3a0d 0a20 2020 2020 2020 2020  rd'):..         
-00003bf0: 2020 2072 6574 2e66 6f72 6d61 7420 3d20     ret.format = 
-00003c00: 276d 6174 7269 7827 0d0a 2020 2020 2020  'matrix'..      
-00003c10: 2020 656c 6966 2872 6574 2e66 6f72 6d61    elif(ret.forma
-00003c20: 743d 3d27 6d61 7472 6978 2729 3a0d 0a20  t=='matrix'):.. 
-00003c30: 2020 2020 2020 2020 2020 2072 6574 2e66             ret.f
-00003c40: 6f72 6d61 7420 3d20 2773 7461 6e64 6172  ormat = 'standar
-00003c50: 6427 0d0a 2020 2020 2020 2020 656c 7365  d'..        else
-00003c60: 3a0d 0a20 2020 2020 2020 2020 2020 2065  :..            e
-00003c70: 7272 6f72 2822 4572 726f 725b 7377 6974  rror("Error[swit
-00003c80: 6368 5f66 6f72 6d61 745d 3a20 756e 6b6e  ch_format]: unkn
-00003c90: 6f77 6e20 666f 726d 6174 2229 0d0a 2020  own format")..  
-00003ca0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00003cb0: 2020 2020 6966 2873 656c 662e 656e 636f      if(self.enco
-00003cc0: 6465 723d 3d27 7061 7269 7479 2d70 7265  der=='parity-pre
-00003cd0: 7365 7276 696e 6727 293a 0d0a 2020 2020  serving'):..    
-00003ce0: 2020 2020 2020 2020 7265 7420 3d20 7265          ret = re
-00003cf0: 742e 7377 6974 6368 5f65 6e63 6f64 6572  t.switch_encoder
-00003d00: 2873 6176 655f 6d65 6d6f 7279 3d54 7275  (save_memory=Tru
-00003d10: 6529 0d0a 2020 2020 2020 2020 7265 7475  e)..        retu
-00003d20: 726e 2072 6574 0d0a 0d0a 2020 2020 6465  rn ret....    de
-00003d30: 6620 7377 6974 6368 5f65 6e63 6f64 6572  f switch_encoder
-00003d40: 2873 656c 662c 7361 7665 5f6d 656d 6f72  (self,save_memor
-00003d50: 793d 4661 6c73 6529 3a0d 0a0d 0a20 2020  y=False):....   
-00003d60: 2020 2020 2069 6620 7361 7665 5f6d 656d       if save_mem
-00003d70: 6f72 7920 3a0d 0a20 2020 2020 2020 2020  ory :..         
-00003d80: 2020 2072 6574 203d 2073 656c 660d 0a20     ret = self.. 
-00003d90: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-00003da0: 2020 2020 2020 2020 2020 7265 7420 3d20            ret = 
-00003db0: 7365 6c66 2e63 6f70 7928 290d 0a0d 0a20  self.copy().... 
-00003dc0: 2020 2020 2020 206b 3d30 0d0a 2020 2020         k=0..    
-00003dd0: 2020 2020 6b6d 6178 203d 2072 6574 2e6e      kmax = ret.n
-00003de0: 6469 6d0d 0a20 2020 2020 2020 2073 3020  dim..        s0 
-00003df0: 3d20 7469 6d65 2e74 696d 6528 290d 0a20  = time.time().. 
-00003e00: 2020 2020 2020 2073 3030 203d 2073 300d         s00 = s0.
-00003e10: 0a20 2020 2020 2020 2070 7269 6e74 2829  .        print()
-00003e20: 0d0a 0d0a 2020 2020 2020 2020 6461 7420  ....        dat 
-00003e30: 3d20 7265 742e 6461 7461 0d0a 2020 2020  = ret.data..    
-00003e40: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00003e50: 6765 2872 6574 2e6e 6469 6d29 3a0d 0a20  ge(ret.ndim):.. 
-00003e60: 2020 2020 2020 2020 2020 2064 203d 2072             d = r
-00003e70: 6574 2e73 6861 7065 5b69 5d0d 0a20 2020  et.shape[i]..   
-00003e80: 2020 2020 2020 2020 2069 6620 7265 742e           if ret.
-00003e90: 7374 6174 6973 7469 635b 695d 2069 6e20  statistic[i] in 
-00003ea0: 6665 726d 695f 7479 7065 203a 0d0a 2020  fermi_type :..  
-00003eb0: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00003ec0: 7420 3d20 6461 742e 7461 6b65 2869 6e64  t = dat.take(ind
-00003ed0: 6963 6573 3d6e 702e 6172 7261 7928 5b70  ices=np.array([p
-00003ee0: 6172 616d 2e65 6e63 6f64 6572 2869 2920  aram.encoder(i) 
-00003ef0: 666f 7220 6920 696e 2072 616e 6765 2864  for i in range(d
-00003f00: 295d 292c 6178 6973 3d69 290d 0a0d 0a20  )]),axis=i).... 
-00003f10: 2020 2020 2020 2020 2020 2069 6620 7469             if ti
-00003f20: 6d65 2e74 696d 6528 292d 7330 203e 2032  me.time()-s0 > 2
-00003f30: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
-00003f40: 2020 2020 7368 6f77 5f70 726f 6772 6573      show_progres
-00003f50: 7328 692c 6b6d 6178 2c70 726f 6365 7373  s(i,kmax,process
-00003f60: 5f6e 616d 6520 3d20 2273 7769 7463 685f  _name = "switch_
-00003f70: 656e 636f 6465 7222 2c72 6174 696f 203d  encoder",ratio =
-00003f80: 2046 616c 7365 2c63 6f6c 6f72 3d22 6379   False,color="cy
-00003f90: 616e 222c 7469 6d65 3d74 696d 652e 7469  an",time=time.ti
-00003fa0: 6d65 2829 2d73 3030 290d 0a20 2020 2020  me()-s00)..     
-00003fb0: 2020 2020 2020 2020 2020 2073 3020 3d20             s0 = 
-00003fc0: 7469 6d65 2e74 696d 6528 290d 0a20 2020  time.time()..   
-00003fd0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00003fe0: 2020 2063 6c65 6172 5f70 726f 6772 6573     clear_progres
-00003ff0: 7328 290d 0a20 2020 2020 2020 2073 7973  s()..        sys
-00004000: 2e73 7464 6f75 742e 7772 6974 6528 225c  .stdout.write("\
-00004010: 3033 335b 4622 290d 0a0d 0a20 2020 2020  033[F")....     
-00004020: 2020 2072 6574 2e64 6174 6120 3d20 6461     ret.data = da
-00004030: 740d 0a0d 0a20 2020 2020 2020 2069 6628  t....        if(
-00004040: 7265 742e 656e 636f 6465 723d 3d27 6361  ret.encoder=='ca
-00004050: 6e6f 6e69 6361 6c27 293a 0d0a 2020 2020  nonical'):..    
-00004060: 2020 2020 2020 2020 7265 742e 656e 636f          ret.enco
-00004070: 6465 723d 2770 6172 6974 792d 7072 6573  der='parity-pres
-00004080: 6572 7669 6e67 270d 0a20 2020 2020 2020  erving'..       
-00004090: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-000040a0: 2020 2020 7265 742e 656e 636f 6465 723d      ret.encoder=
-000040b0: 2763 616e 6f6e 6963 616c 270d 0a20 2020  'canonical'..   
-000040c0: 2020 2020 2072 6574 7572 6e20 7265 740d       return ret.
-000040d0: 0a0d 0a20 2020 2064 6566 2066 6f72 6365  ...    def force
-000040e0: 5f65 6e63 6f64 6572 2873 656c 662c 7461  _encoder(self,ta
-000040f0: 7267 6574 3d22 6361 6e6f 6e69 6361 6c22  rget="canonical"
-00004100: 293a 0d0a 2020 2020 2020 2020 6966 2074  ):..        if t
-00004110: 6172 6765 7420 6e6f 7420 696e 2065 6e63  arget not in enc
-00004120: 6f64 6572 5f74 7970 653a 0d0a 2020 2020  oder_type:..    
-00004130: 2020 2020 2020 2020 6572 726f 7228 2245          error("E
-00004140: 7272 6f72 5b64 656e 7365 2e66 6f72 6365  rror[dense.force
-00004150: 5f65 6e63 6f64 6572 5d3a 2055 6e72 6563  _encoder]: Unrec
-00004160: 6f67 6e69 7a65 6420 7461 7267 6574 2065  ognized target e
-00004170: 6e63 6f64 6572 2e22 290d 0a20 2020 2020  ncoder.")..     
-00004180: 2020 2069 6620 7461 7267 6574 2021 3d20     if target != 
-00004190: 7365 6c66 2e65 6e63 6f64 6572 203a 0d0a  self.encoder :..
-000041a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000041b0: 726e 2073 656c 662e 7377 6974 6368 5f65  rn self.switch_e
-000041c0: 6e63 6f64 6572 2873 6176 655f 6d65 6d6f  ncoder(save_memo
-000041d0: 7279 3d54 7275 6529 0d0a 2020 2020 2020  ry=True)..      
-000041e0: 2020 656c 7365 203a 0d0a 2020 2020 2020    else :..      
-000041f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00004200: 662e 636f 7079 2829 0d0a 0d0a 2020 2020  f.copy()....    
-00004210: 6465 6620 666f 7263 655f 666f 726d 6174  def force_format
-00004220: 2873 656c 662c 7461 7267 6574 3d22 7374  (self,target="st
-00004230: 616e 6461 7264 2229 3a0d 0a20 2020 2020  andard"):..     
-00004240: 2020 2069 6620 7461 7267 6574 206e 6f74     if target not
-00004250: 2069 6e20 666f 726d 6174 5f74 7970 653a   in format_type:
-00004260: 0d0a 2020 2020 2020 2020 2020 2020 6572  ..            er
-00004270: 726f 7228 2245 7272 6f72 5b64 656e 7365  ror("Error[dense
-00004280: 2e66 6f72 6365 5f66 6f72 6d61 745d 3a20  .force_format]: 
-00004290: 556e 7265 636f 676e 697a 6564 2074 6172  Unrecognized tar
-000042a0: 6765 7420 666f 726d 6174 2e22 290d 0a20  get format.").. 
-000042b0: 2020 2020 2020 2069 6620 7461 7267 6574         if target
-000042c0: 2021 3d20 7365 6c66 2e66 6f72 6d61 7420   != self.format 
-000042d0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-000042e0: 6574 7572 6e20 7365 6c66 2e73 7769 7463  eturn self.switc
-000042f0: 685f 666f 726d 6174 2873 6176 655f 6d65  h_format(save_me
-00004300: 6d6f 7279 3d54 7275 6529 0d0a 2020 2020  mory=True)..    
-00004310: 2020 2020 656c 7365 203a 0d0a 2020 2020      else :..    
-00004320: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00004330: 656c 662e 636f 7079 2829 0d0a 0d0a 2020  elf.copy()....  
-00004340: 2020 6465 6620 6a6f 696e 5f6c 6567 7328    def join_legs(
-00004350: 7365 6c66 2c73 7472 696e 675f 696e 702c  self,string_inp,
-00004360: 6d61 6b65 5f66 6f72 6d61 743d 2773 7461  make_format='sta
-00004370: 6e64 6172 6427 2c69 6e74 6572 6d65 6469  ndard',intermedi
-00004380: 6174 655f 7374 6174 3d28 2d31 2c31 292c  ate_stat=(-1,1),
-00004390: 7361 7665 5f6d 656d 6f72 793d 4661 6c73  save_memory=Fals
-000043a0: 6529 3a0d 0a20 2020 2020 2020 2072 6574  e):..        ret
-000043b0: 7572 6e20 6a6f 696e 5f6c 6567 7328 7365  urn join_legs(se
-000043c0: 6c66 2c73 7472 696e 675f 696e 702c 6d61  lf,string_inp,ma
-000043d0: 6b65 5f66 6f72 6d61 742c 696e 7465 726d  ke_format,interm
-000043e0: 6564 6961 7465 5f73 7461 742c 7361 7665  ediate_stat,save
-000043f0: 5f6d 656d 6f72 7929 0d0a 0d0a 2020 2020  _memory)....    
-00004400: 6465 6620 7370 6c69 745f 6c65 6773 2873  def split_legs(s
-00004410: 656c 662c 7374 7269 6e67 5f69 6e70 2c66  elf,string_inp,f
-00004420: 696e 616c 5f73 7461 742c 6669 6e61 6c5f  inal_stat,final_
-00004430: 7368 6170 652c 696e 7465 726d 6564 6961  shape,intermedia
-00004440: 7465 5f73 7461 743d 282d 312c 3129 2c73  te_stat=(-1,1),s
-00004450: 6176 655f 6d65 6d6f 7279 3d46 616c 7365  ave_memory=False
-00004460: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
-00004470: 726e 2073 706c 6974 5f6c 6567 7328 7365  rn split_legs(se
-00004480: 6c66 2c73 7472 696e 675f 696e 702c 6669  lf,string_inp,fi
-00004490: 6e61 6c5f 7374 6174 2c66 696e 616c 5f73  nal_stat,final_s
-000044a0: 6861 7065 2c69 6e74 6572 6d65 6469 6174  hape,intermediat
-000044b0: 655f 7374 6174 2c73 6176 655f 6d65 6d6f  e_stat,save_memo
-000044c0: 7279 290d 0a0d 0a20 2020 2064 6566 2068  ry)....    def h
-000044d0: 636f 6e6a 7567 6174 6528 7365 6c66 2c69  conjugate(self,i
-000044e0: 6e70 7574 5f73 7472 696e 672c 7361 7665  nput_string,save
-000044f0: 5f6d 656d 6f72 793d 4661 6c73 6529 3a0d  _memory=False):.
-00004500: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00004510: 6863 6f6e 6a75 6761 7465 2873 656c 662c  hconjugate(self,
-00004520: 696e 7075 745f 7374 7269 6e67 2c73 6176  input_string,sav
-00004530: 655f 6d65 6d6f 7279 290d 0a0d 0a20 2020  e_memory)....   
-00004540: 2064 6566 2073 7664 2873 656c 662c 7374   def svd(self,st
-00004550: 7269 6e67 5f69 6e70 2c63 7574 6f66 663d  ring_inp,cutoff=
-00004560: 4e6f 6e65 2c73 6176 655f 6d65 6d6f 7279  None,save_memory
-00004570: 3d46 616c 7365 293a 0d0a 2020 2020 2020  =False):..      
-00004580: 2020 7265 7475 726e 2073 7664 2873 656c    return svd(sel
-00004590: 662c 7374 7269 6e67 5f69 6e70 2c63 7574  f,string_inp,cut
-000045a0: 6f66 662c 7361 7665 5f6d 656d 6f72 7929  off,save_memory)
-000045b0: 0d0a 0d0a 2020 2020 6465 6620 6569 6728  ....    def eig(
-000045c0: 7365 6c66 2c73 7472 696e 675f 696e 702c  self,string_inp,
-000045d0: 6375 746f 6666 3d4e 6f6e 652c 6465 6275  cutoff=None,debu
-000045e0: 675f 6d6f 6465 3d46 616c 7365 2c73 6176  g_mode=False,sav
-000045f0: 655f 6d65 6d6f 7279 3d46 616c 7365 293a  e_memory=False):
-00004600: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00004610: 2065 6967 2873 656c 662c 7374 7269 6e67   eig(self,string
-00004620: 5f69 6e70 2c63 7574 6f66 662c 6465 6275  _inp,cutoff,debu
-00004630: 675f 6d6f 6465 2c73 6176 655f 6d65 6d6f  g_mode,save_memo
-00004640: 7279 290d 0a0d 0a23 2323 2323 2323 2323  ry)....#########
+00003b80: 0d0a 2020 2020 2020 2020 7461 625f 7570  ..        tab_up
+00003b90: 2829 0d0a 0d0a 2020 2020 2020 2020 7265  ()....        re
+00003ba0: 742e 6461 7461 203d 2064 6174 0d0a 0d0a  t.data = dat....
+00003bb0: 2020 2020 2020 2020 6966 2872 6574 2e66          if(ret.f
+00003bc0: 6f72 6d61 743d 3d27 7374 616e 6461 7264  ormat=='standard
+00003bd0: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
+00003be0: 2072 6574 2e66 6f72 6d61 7420 3d20 276d   ret.format = 'm
+00003bf0: 6174 7269 7827 0d0a 2020 2020 2020 2020  atrix'..        
+00003c00: 656c 6966 2872 6574 2e66 6f72 6d61 743d  elif(ret.format=
+00003c10: 3d27 6d61 7472 6978 2729 3a0d 0a20 2020  ='matrix'):..   
+00003c20: 2020 2020 2020 2020 2072 6574 2e66 6f72           ret.for
+00003c30: 6d61 7420 3d20 2773 7461 6e64 6172 6427  mat = 'standard'
+00003c40: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00003c50: 0a20 2020 2020 2020 2020 2020 2065 7272  .            err
+00003c60: 6f72 2822 4572 726f 725b 7377 6974 6368  or("Error[switch
+00003c70: 5f66 6f72 6d61 745d 3a20 756e 6b6e 6f77  _format]: unknow
+00003c80: 6e20 666f 726d 6174 2229 0d0a 2020 2020  n format")..    
+00003c90: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00003ca0: 2020 6966 2873 656c 662e 656e 636f 6465    if(self.encode
+00003cb0: 723d 3d27 7061 7269 7479 2d70 7265 7365  r=='parity-prese
+00003cc0: 7276 696e 6727 293a 0d0a 2020 2020 2020  rving'):..      
+00003cd0: 2020 2020 2020 7265 7420 3d20 7265 742e        ret = ret.
+00003ce0: 7377 6974 6368 5f65 6e63 6f64 6572 2873  switch_encoder(s
+00003cf0: 6176 655f 6d65 6d6f 7279 3d54 7275 6529  ave_memory=True)
+00003d00: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00003d10: 2072 6574 0d0a 0d0a 2020 2020 6465 6620   ret....    def 
+00003d20: 7377 6974 6368 5f65 6e63 6f64 6572 2873  switch_encoder(s
+00003d30: 656c 662c 7361 7665 5f6d 656d 6f72 793d  elf,save_memory=
+00003d40: 4661 6c73 6529 3a0d 0a0d 0a20 2020 2020  False):....     
+00003d50: 2020 2069 6620 7361 7665 5f6d 656d 6f72     if save_memor
+00003d60: 7920 3a0d 0a20 2020 2020 2020 2020 2020  y :..           
+00003d70: 2072 6574 203d 2073 656c 660d 0a20 2020   ret = self..   
+00003d80: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00003d90: 2020 2020 2020 2020 7265 7420 3d20 7365          ret = se
+00003da0: 6c66 2e63 6f70 7928 290d 0a0d 0a20 2020  lf.copy()....   
+00003db0: 2020 2020 206b 3d30 0d0a 2020 2020 2020       k=0..      
+00003dc0: 2020 6b6d 6178 203d 2072 6574 2e6e 6469    kmax = ret.ndi
+00003dd0: 6d0d 0a20 2020 2020 2020 2073 3020 3d20  m..        s0 = 
+00003de0: 7469 6d65 2e74 696d 6528 290d 0a20 2020  time.time()..   
+00003df0: 2020 2020 2073 3030 203d 2073 300d 0a20       s00 = s0.. 
+00003e00: 2020 2020 2020 2070 726f 6772 6573 735f         progress_
+00003e10: 7370 6163 6528 290d 0a0d 0a20 2020 2020  space()....     
+00003e20: 2020 2064 6174 203d 2072 6574 2e64 6174     dat = ret.dat
+00003e30: 610d 0a20 2020 2020 2020 2066 6f72 2069  a..        for i
+00003e40: 2069 6e20 7261 6e67 6528 7265 742e 6e64   in range(ret.nd
+00003e50: 696d 293a 0d0a 2020 2020 2020 2020 2020  im):..          
+00003e60: 2020 6420 3d20 7265 742e 7368 6170 655b    d = ret.shape[
+00003e70: 695d 0d0a 2020 2020 2020 2020 2020 2020  i]..            
+00003e80: 6966 2072 6574 2e73 7461 7469 7374 6963  if ret.statistic
+00003e90: 5b69 5d20 696e 2066 6572 6d69 5f74 7970  [i] in fermi_typ
+00003ea0: 6520 3a0d 0a20 2020 2020 2020 2020 2020  e :..           
+00003eb0: 2020 2020 2064 6174 203d 2064 6174 2e74       dat = dat.t
+00003ec0: 616b 6528 696e 6469 6365 733d 6e70 2e61  ake(indices=np.a
+00003ed0: 7272 6179 285b 7061 7261 6d2e 656e 636f  rray([param.enco
+00003ee0: 6465 7228 6929 2066 6f72 2069 2069 6e20  der(i) for i in 
+00003ef0: 7261 6e67 6528 6429 5d29 2c61 7869 733d  range(d)]),axis=
+00003f00: 6929 0d0a 0d0a 2020 2020 2020 2020 2020  i)....          
+00003f10: 2020 6966 2074 696d 652e 7469 6d65 2829    if time.time()
+00003f20: 2d73 3020 3e20 3220 3a0d 0a20 2020 2020  -s0 > 2 :..     
+00003f30: 2020 2020 2020 2020 2020 2073 686f 775f             show_
+00003f40: 7072 6f67 7265 7373 2869 2c6b 6d61 782c  progress(i,kmax,
+00003f50: 7072 6f63 6573 735f 6e61 6d65 203d 2022  process_name = "
+00003f60: 7377 6974 6368 5f65 6e63 6f64 6572 222c  switch_encoder",
+00003f70: 7261 7469 6f20 3d20 4661 6c73 652c 636f  ratio = False,co
+00003f80: 6c6f 723d 2263 7961 6e22 2c74 696d 653d  lor="cyan",time=
+00003f90: 7469 6d65 2e74 696d 6528 292d 7330 3029  time.time()-s00)
+00003fa0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003fb0: 2020 7330 203d 2074 696d 652e 7469 6d65    s0 = time.time
+00003fc0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00003fd0: 0d0a 2020 2020 2020 2020 636c 6561 725f  ..        clear_
+00003fe0: 7072 6f67 7265 7373 2829 0d0a 2020 2020  progress()..    
+00003ff0: 2020 2020 7461 625f 7570 2829 0d0a 0d0a      tab_up()....
+00004000: 2020 2020 2020 2020 7265 742e 6461 7461          ret.data
+00004010: 203d 2064 6174 0d0a 0d0a 2020 2020 2020   = dat....      
+00004020: 2020 6966 2872 6574 2e65 6e63 6f64 6572    if(ret.encoder
+00004030: 3d3d 2763 616e 6f6e 6963 616c 2729 3a0d  =='canonical'):.
+00004040: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00004050: 2e65 6e63 6f64 6572 3d27 7061 7269 7479  .encoder='parity
+00004060: 2d70 7265 7365 7276 696e 6727 0d0a 2020  -preserving'..  
+00004070: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00004080: 2020 2020 2020 2020 2072 6574 2e65 6e63           ret.enc
+00004090: 6f64 6572 3d27 6361 6e6f 6e69 6361 6c27  oder='canonical'
+000040a0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000040b0: 2072 6574 0d0a 0d0a 2020 2020 6465 6620   ret....    def 
+000040c0: 666f 7263 655f 656e 636f 6465 7228 7365  force_encoder(se
+000040d0: 6c66 2c74 6172 6765 743d 2263 616e 6f6e  lf,target="canon
+000040e0: 6963 616c 2229 3a0d 0a20 2020 2020 2020  ical"):..       
+000040f0: 2069 6620 7461 7267 6574 206e 6f74 2069   if target not i
+00004100: 6e20 656e 636f 6465 725f 7479 7065 3a0d  n encoder_type:.
+00004110: 0a20 2020 2020 2020 2020 2020 2065 7272  .            err
+00004120: 6f72 2822 4572 726f 725b 6465 6e73 652e  or("Error[dense.
+00004130: 666f 7263 655f 656e 636f 6465 725d 3a20  force_encoder]: 
+00004140: 556e 7265 636f 676e 697a 6564 2074 6172  Unrecognized tar
+00004150: 6765 7420 656e 636f 6465 722e 2229 0d0a  get encoder.")..
+00004160: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
+00004170: 7420 213d 2073 656c 662e 656e 636f 6465  t != self.encode
+00004180: 7220 3a0d 0a20 2020 2020 2020 2020 2020  r :..           
+00004190: 2072 6574 7572 6e20 7365 6c66 2e73 7769   return self.swi
+000041a0: 7463 685f 656e 636f 6465 7228 7361 7665  tch_encoder(save
+000041b0: 5f6d 656d 6f72 793d 5472 7565 290d 0a20  _memory=True).. 
+000041c0: 2020 2020 2020 2065 6c73 6520 3a0d 0a20         else :.. 
+000041d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000041e0: 6e20 7365 6c66 2e63 6f70 7928 290d 0a0d  n self.copy()...
+000041f0: 0a20 2020 2064 6566 2066 6f72 6365 5f66  .    def force_f
+00004200: 6f72 6d61 7428 7365 6c66 2c74 6172 6765  ormat(self,targe
+00004210: 743d 2273 7461 6e64 6172 6422 293a 0d0a  t="standard"):..
+00004220: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
+00004230: 7420 6e6f 7420 696e 2066 6f72 6d61 745f  t not in format_
+00004240: 7479 7065 3a0d 0a20 2020 2020 2020 2020  type:..         
+00004250: 2020 2065 7272 6f72 2822 4572 726f 725b     error("Error[
+00004260: 6465 6e73 652e 666f 7263 655f 666f 726d  dense.force_form
+00004270: 6174 5d3a 2055 6e72 6563 6f67 6e69 7a65  at]: Unrecognize
+00004280: 6420 7461 7267 6574 2066 6f72 6d61 742e  d target format.
+00004290: 2229 0d0a 2020 2020 2020 2020 6966 2074  ")..        if t
+000042a0: 6172 6765 7420 213d 2073 656c 662e 666f  arget != self.fo
+000042b0: 726d 6174 203a 0d0a 2020 2020 2020 2020  rmat :..        
+000042c0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000042d0: 7377 6974 6368 5f66 6f72 6d61 7428 7361  switch_format(sa
+000042e0: 7665 5f6d 656d 6f72 793d 5472 7565 290d  ve_memory=True).
+000042f0: 0a20 2020 2020 2020 2065 6c73 6520 3a0d  .        else :.
+00004300: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00004310: 7572 6e20 7365 6c66 2e63 6f70 7928 290d  urn self.copy().
+00004320: 0a0d 0a20 2020 2064 6566 206a 6f69 6e5f  ...    def join_
+00004330: 6c65 6773 2873 656c 662c 7374 7269 6e67  legs(self,string
+00004340: 5f69 6e70 2c6d 616b 655f 666f 726d 6174  _inp,make_format
+00004350: 3d27 7374 616e 6461 7264 272c 696e 7465  ='standard',inte
+00004360: 726d 6564 6961 7465 5f73 7461 743d 282d  rmediate_stat=(-
+00004370: 312c 3129 2c73 6176 655f 6d65 6d6f 7279  1,1),save_memory
+00004380: 3d46 616c 7365 293a 0d0a 2020 2020 2020  =False):..      
+00004390: 2020 7265 7475 726e 206a 6f69 6e5f 6c65    return join_le
+000043a0: 6773 2873 656c 662c 7374 7269 6e67 5f69  gs(self,string_i
+000043b0: 6e70 2c6d 616b 655f 666f 726d 6174 2c69  np,make_format,i
+000043c0: 6e74 6572 6d65 6469 6174 655f 7374 6174  ntermediate_stat
+000043d0: 2c73 6176 655f 6d65 6d6f 7279 290d 0a0d  ,save_memory)...
+000043e0: 0a20 2020 2064 6566 2073 706c 6974 5f6c  .    def split_l
+000043f0: 6567 7328 7365 6c66 2c73 7472 696e 675f  egs(self,string_
+00004400: 696e 702c 6669 6e61 6c5f 7374 6174 2c66  inp,final_stat,f
+00004410: 696e 616c 5f73 6861 7065 2c69 6e74 6572  inal_shape,inter
+00004420: 6d65 6469 6174 655f 7374 6174 3d28 2d31  mediate_stat=(-1
+00004430: 2c31 292c 7361 7665 5f6d 656d 6f72 793d  ,1),save_memory=
+00004440: 4661 6c73 6529 3a0d 0a20 2020 2020 2020  False):..       
+00004450: 2072 6574 7572 6e20 7370 6c69 745f 6c65   return split_le
+00004460: 6773 2873 656c 662c 7374 7269 6e67 5f69  gs(self,string_i
+00004470: 6e70 2c66 696e 616c 5f73 7461 742c 6669  np,final_stat,fi
+00004480: 6e61 6c5f 7368 6170 652c 696e 7465 726d  nal_shape,interm
+00004490: 6564 6961 7465 5f73 7461 742c 7361 7665  ediate_stat,save
+000044a0: 5f6d 656d 6f72 7929 0d0a 0d0a 2020 2020  _memory)....    
+000044b0: 6465 6620 6863 6f6e 6a75 6761 7465 2873  def hconjugate(s
+000044c0: 656c 662c 696e 7075 745f 7374 7269 6e67  elf,input_string
+000044d0: 2c73 6176 655f 6d65 6d6f 7279 3d46 616c  ,save_memory=Fal
+000044e0: 7365 293a 0d0a 2020 2020 2020 2020 7265  se):..        re
+000044f0: 7475 726e 2068 636f 6e6a 7567 6174 6528  turn hconjugate(
+00004500: 7365 6c66 2c69 6e70 7574 5f73 7472 696e  self,input_strin
+00004510: 672c 7361 7665 5f6d 656d 6f72 7929 0d0a  g,save_memory)..
+00004520: 0d0a 2020 2020 6465 6620 7376 6428 7365  ..    def svd(se
+00004530: 6c66 2c73 7472 696e 675f 696e 702c 6375  lf,string_inp,cu
+00004540: 746f 6666 3d4e 6f6e 652c 7361 7665 5f6d  toff=None,save_m
+00004550: 656d 6f72 793d 4661 6c73 6529 3a0d 0a20  emory=False):.. 
+00004560: 2020 2020 2020 2072 6574 7572 6e20 7376         return sv
+00004570: 6428 7365 6c66 2c73 7472 696e 675f 696e  d(self,string_in
+00004580: 702c 6375 746f 6666 2c73 6176 655f 6d65  p,cutoff,save_me
+00004590: 6d6f 7279 290d 0a0d 0a20 2020 2064 6566  mory)....    def
+000045a0: 2065 6967 2873 656c 662c 7374 7269 6e67   eig(self,string
+000045b0: 5f69 6e70 2c63 7574 6f66 663d 4e6f 6e65  _inp,cutoff=None
+000045c0: 2c64 6562 7567 5f6d 6f64 653d 4661 6c73  ,debug_mode=Fals
+000045d0: 652c 7361 7665 5f6d 656d 6f72 793d 4661  e,save_memory=Fa
+000045e0: 6c73 6529 3a0d 0a20 2020 2020 2020 2072  lse):..        r
+000045f0: 6574 7572 6e20 6569 6728 7365 6c66 2c73  eturn eig(self,s
+00004600: 7472 696e 675f 696e 702c 6375 746f 6666  tring_inp,cutoff
+00004610: 2c64 6562 7567 5f6d 6f64 652c 7361 7665  ,debug_mode,save
+00004620: 5f6d 656d 6f72 7929 0d0a 0d0a 2323 2323  _memory)....####
+00004630: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004640: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00004650: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004660: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004670: 2323 2323 2323 2323 2323 230d 0a23 2320  ###########..## 
-00004680: 2020 2020 2020 2020 2020 2053 7061 7273             Spars
-00004690: 6520 4772 6173 736d 616e 6e20 6172 7261  e Grassmann arra
-000046a0: 7973 2020 2020 2020 2020 2020 2020 2023  ys             #
-000046b0: 230d 0a23 2323 2323 2323 2323 2323 2323  #..#############
-000046c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000046d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000046e0: 2323 2323 2323 230d 0a0d 0a63 6c61 7373  #######....class
-000046f0: 2073 7061 7273 653a 0d0a 2020 2020 6465   sparse:..    de
-00004700: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00004710: 2064 6174 613d 4e6f 6e65 2c20 656e 636f   data=None, enco
-00004720: 6465 7220 3d20 2263 616e 6f6e 6963 616c  der = "canonical
-00004730: 222c 2066 6f72 6d61 7420 3d20 2273 7461  ", format = "sta
-00004740: 6e64 6172 6422 2c20 7374 6174 6973 7469  ndard", statisti
-00004750: 6320 3d20 4e6f 6e65 293a 0d0a 2020 2020  c = None):..    
-00004760: 0d0a 2020 2020 2020 2020 2363 6f70 7920  ..        #copy 
-00004770: 7370 6172 7365 2070 726f 7065 7274 6965  sparse propertie
-00004780: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-00004790: 6461 7461 203d 204e 6f6e 650d 0a20 2020  data = None..   
-000047a0: 2020 2020 2073 656c 662e 7374 6174 6973       self.statis
-000047b0: 7469 6320 3d20 4e6f 6e65 0d0a 2020 2020  tic = None..    
-000047c0: 2020 2020 7365 6c66 2e66 6f72 6d61 7420      self.format 
-000047d0: 3d20 666f 726d 6174 0d0a 2020 2020 2020  = format..      
-000047e0: 2020 7365 6c66 2e65 6e63 6f64 6572 203d    self.encoder =
-000047f0: 2065 6e63 6f64 6572 0d0a 0d0a 2020 2020   encoder....    
-00004800: 2020 2020 6465 6661 756c 7420 3d20 5472      default = Tr
-00004810: 7565 0d0a 2020 2020 0d0a 2020 2020 2020  ue..    ..      
-00004820: 2020 6966 2865 6e63 6f64 6572 206e 6f74    if(encoder not
-00004830: 2069 6e20 656e 636f 6465 725f 7479 7065   in encoder_type
-00004840: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00004850: 6572 726f 7228 2245 7272 6f72 5b73 7061  error("Error[spa
-00004860: 7273 655d 3a20 556e 6b6e 6f77 6e20 656e  rse]: Unknown en
-00004870: 636f 6465 722e 2229 0d0a 2020 2020 2020  coder.")..      
-00004880: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00004890: 6966 2866 6f72 6d61 7420 6e6f 7420 696e  if(format not in
-000048a0: 2066 6f72 6d61 745f 7479 7065 293a 0d0a   format_type):..
-000048b0: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-000048c0: 7228 2245 7272 6f72 5b73 7061 7273 655d  r("Error[sparse]
-000048d0: 3a20 556e 6b6e 6f77 6e20 666f 726d 6174  : Unknown format
-000048e0: 2e22 290d 0a20 2020 2020 2020 2020 2020  .")..           
-000048f0: 200d 0a20 2020 2020 2020 2069 6628 7479   ..        if(ty
-00004900: 7065 2864 6174 6129 3d3d 6e70 2e61 7272  pe(data)==np.arr
-00004910: 6179 206f 7220 7479 7065 2864 6174 6129  ay or type(data)
-00004920: 3d3d 6e70 2e6e 6461 7272 6179 206f 7220  ==np.ndarray or 
-00004930: 7479 7065 2864 6174 6129 3d3d 6c69 7374  type(data)==list
-00004940: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00004950: 7365 6c66 2e64 6174 6120 203d 2073 702e  self.data  = sp.
-00004960: 434f 4f2e 6672 6f6d 5f6e 756d 7079 286e  COO.from_numpy(n
-00004970: 702e 6172 7261 7928 6461 7461 2929 0d0a  p.array(data))..
-00004980: 2020 2020 2020 2020 2020 2020 6465 6661              defa
-00004990: 756c 7420 3d20 4661 6c73 650d 0a20 2020  ult = False..   
-000049a0: 2020 2020 2065 6c69 6628 7479 7065 2864       elif(type(d
-000049b0: 6174 6129 3d3d 7370 2e43 4f4f 293a 0d0a  ata)==sp.COO):..
-000049c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000049d0: 2e64 6174 6120 203d 2064 6174 612e 636f  .data  = data.co
-000049e0: 7079 2829 0d0a 2020 2020 2020 2020 2020  py()..          
-000049f0: 2020 6465 6661 756c 7420 3d20 4661 6c73    default = Fals
-00004a00: 650d 0a20 2020 2020 2020 2065 6c69 6628  e..        elif(
-00004a10: 7479 7065 2864 6174 6129 3d3d 6465 6e73  type(data)==dens
-00004a20: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00004a30: 2023 636f 7079 2073 7061 7273 6520 7072   #copy sparse pr
-00004a40: 6f70 6572 7469 6573 0d0a 2020 2020 2020  operties..      
-00004a50: 2020 2020 2020 7365 6c66 2e64 6174 6120        self.data 
-00004a60: 203d 2073 702e 434f 4f2e 6672 6f6d 5f6e   = sp.COO.from_n
-00004a70: 756d 7079 2864 6174 612e 6461 7461 290d  umpy(data.data).
-00004a80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00004a90: 662e 7374 6174 6973 7469 6320 3d20 6461  f.statistic = da
-00004aa0: 7461 2e73 7461 7469 7374 6963 0d0a 2020  ta.statistic..  
-00004ab0: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-00004ac0: 6f72 6d61 7420 3d20 6461 7461 2e66 6f72  ormat = data.for
-00004ad0: 6d61 740d 0a20 2020 2020 2020 2020 2020  mat..           
-00004ae0: 2073 656c 662e 656e 636f 6465 7220 3d20   self.encoder = 
-00004af0: 6461 7461 2e65 6e63 6f64 6572 0d0a 2020  data.encoder..  
-00004b00: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
-00004b10: 7420 3d20 4661 6c73 650d 0a20 2020 2020  t = False..     
-00004b20: 2020 2065 6c69 6628 7479 7065 2864 6174     elif(type(dat
-00004b30: 6129 3d3d 7370 6172 7365 293a 0d0a 2020  a)==sparse):..  
-00004b40: 2020 2020 2020 2020 2020 2363 6f70 7920            #copy 
-00004b50: 7370 6172 7365 2070 726f 7065 7274 6965  sparse propertie
-00004b60: 730d 0a20 2020 2020 2020 2020 2020 2073  s..            s
-00004b70: 656c 662e 6461 7461 203d 2064 6174 612e  elf.data = data.
-00004b80: 6461 7461 2e63 6f70 7928 290d 0a20 2020  data.copy()..   
-00004b90: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-00004ba0: 6174 6973 7469 6320 3d20 6461 7461 2e73  atistic = data.s
-00004bb0: 7461 7469 7374 6963 0d0a 2020 2020 2020  tatistic..      
-00004bc0: 2020 2020 2020 7365 6c66 2e66 6f72 6d61        self.forma
-00004bd0: 7420 3d20 6461 7461 2e66 6f72 6d61 740d  t = data.format.
-00004be0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00004bf0: 662e 656e 636f 6465 7220 3d20 6461 7461  f.encoder = data
-00004c00: 2e65 6e63 6f64 6572 0d0a 2020 2020 2020  .encoder..      
-00004c10: 2020 2020 2020 6465 6661 756c 7420 3d20        default = 
-00004c20: 4661 6c73 650d 0a20 2020 2020 2020 2065  False..        e
-00004c30: 6c69 6620 6461 7461 3d3d 4e6f 6e65 3a0d  lif data==None:.
-00004c40: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
-00004c50: 7468 696e 6720 746f 2073 6565 2068 6572  thing to see her
-00004c60: 6522 0d0a 2020 2020 2020 2020 656c 7365  e"..        else
-00004c70: 3a0d 0a20 2020 2020 2020 2020 2020 2065  :..            e
-00004c80: 7272 6f72 2822 4572 726f 725b 7370 6172  rror("Error[spar
-00004c90: 7365 5d3a 2049 6e76 616c 6964 2069 6e69  se]: Invalid ini
-00004ca0: 7469 616c 697a 6564 2064 6174 6122 290d  tialized data").
-00004cb0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-00004cc0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00004cd0: 2069 6620 7374 6174 6973 7469 6320 213d   if statistic !=
-00004ce0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00004cf0: 2020 2020 7365 6c66 2e73 7461 7469 7374      self.statist
-00004d00: 6963 203d 206d 616b 655f 7475 706c 6528  ic = make_tuple(
-00004d10: 7374 6174 6973 7469 6329 0d0a 2020 2020  statistic)..    
-00004d20: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
-00004d30: 206e 6f74 2064 6566 6175 6c74 2061 6e64   not default and
-00004d40: 206e 6f74 2073 6b69 705f 706f 7765 725f   not skip_power_
-00004d50: 6f66 5f74 776f 5f63 6865 636b 3a0d 0a20  of_two_check:.. 
-00004d60: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00004d70: 2c64 696d 2069 6e20 656e 756d 6572 6174  ,dim in enumerat
-00004d80: 6528 7365 6c66 2e64 6174 612e 7368 6170  e(self.data.shap
-00004d90: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-00004da0: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-00004db0: 7469 7374 6963 5b69 5d20 696e 2066 6572  tistic[i] in fer
-00004dc0: 6d69 5f74 7970 6520 616e 6420 6469 6d20  mi_type and dim 
-00004dd0: 213d 2069 6e74 2832 2a2a 6d61 7468 2e66  != int(2**math.f
-00004de0: 6c6f 6f72 286e 702e 6c6f 6732 2864 696d  loor(np.log2(dim
-00004df0: 2929 293a 0d0a 2020 2020 2020 2020 2020  ))):..          
-00004e00: 2020 2020 2020 2020 2020 6572 726f 7228            error(
-00004e10: 2245 7272 6f72 5b73 7061 7273 655d 3a20  "Error[sparse]: 
-00004e20: 536f 6d65 206f 6620 7468 6520 6665 726d  Some of the ferm
-00004e30: 696f 6e69 6320 7465 6e73 6f72 2073 6861  ionic tensor sha
-00004e40: 7065 7320 6172 6520 6e6f 7420 6120 706f  pes are not a po
-00004e50: 7765 7220 6f66 2074 776f 2e5c 6e20 2020  wer of two.\n   
-00004e60: 2020 2020 2020 2020 2020 2020 4861 7665              Have
-00004e70: 2079 6f75 2061 6464 6564 2074 6865 203c   you added the <
-00004e80: 7374 6174 6973 7469 633e 2061 7267 756d  statistic> argum
-00004e90: 656e 7420 7768 656e 2063 616c 6c69 6e67  ent when calling
-00004ea0: 2074 6869 7320 6675 6e63 7469 6f6e 3f22   this function?"
-00004eb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004ec0: 2020 0d0a 2020 2020 4070 726f 7065 7274    ..    @propert
-00004ed0: 790d 0a20 2020 2064 6566 206e 6e7a 2873  y..    def nnz(s
-00004ee0: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00004ef0: 6574 7572 6e20 7365 6c66 2e64 6174 612e  eturn self.data.
-00004f00: 6e6e 7a0d 0a0d 0a20 2020 2040 7072 6f70  nnz....    @prop
-00004f10: 6572 7479 0d0a 2020 2020 6465 6620 7368  erty..    def sh
-00004f20: 6170 6528 7365 6c66 293a 0d0a 2020 2020  ape(self):..    
-00004f30: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00004f40: 6461 7461 2e73 6861 7065 0d0a 0d0a 2020  data.shape....  
-00004f50: 2020 4070 726f 7065 7274 790d 0a20 2020    @property..   
-00004f60: 2064 6566 2073 697a 6528 7365 6c66 293a   def size(self):
-00004f70: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00004f80: 2073 656c 662e 6461 7461 2e73 697a 650d   self.data.size.
-00004f90: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
-00004fa0: 0d0a 2020 2020 6465 6620 6e64 696d 2873  ..    def ndim(s
-00004fb0: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00004fc0: 6574 7572 6e20 7365 6c66 2e64 6174 612e  eturn self.data.
-00004fd0: 6e64 696d 0d0a 0d0a 2020 2020 4070 726f  ndim....    @pro
-00004fe0: 7065 7274 790d 0a20 2020 2064 6566 2063  perty..    def c
-00004ff0: 6f6f 7264 7328 7365 6c66 293a 0d0a 2020  oords(self):..  
-00005000: 2020 2020 2020 636f 6f72 6473 5f6c 6973        coords_lis
-00005010: 7420 3d20 5b5d 0d0a 2020 2020 2020 2020  t = []..        
-00005020: 666f 7220 656e 7472 7920 696e 2072 616e  for entry in ran
-00005030: 6765 2873 656c 662e 6461 7461 2e6e 6e7a  ge(self.data.nnz
-00005040: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00005050: 636f 6f72 6473 203d 205b 5d0d 0a20 2020  coords = []..   
-00005060: 2020 2020 2020 2020 2066 6f72 2061 7869           for axi
-00005070: 7320 696e 2072 616e 6765 2873 656c 662e  s in range(self.
-00005080: 6461 7461 2e6e 6469 6d29 3a0d 0a20 2020  data.ndim):..   
-00005090: 2020 2020 2020 2020 2020 2020 2063 6f6f               coo
-000050a0: 7264 7320 3d20 636f 6f72 6473 202b 205b  rds = coords + [
-000050b0: 7365 6c66 2e64 6174 612e 636f 6f72 6473  self.data.coords
-000050c0: 5b61 7869 735d 5b65 6e74 7279 5d5d 0d0a  [axis][entry]]..
-000050d0: 2020 2020 2020 2020 2020 2020 636f 6f72              coor
-000050e0: 6473 5f6c 6973 7420 3d20 636f 6f72 6473  ds_list = coords
-000050f0: 5f6c 6973 7420 2b20 5b74 7570 6c65 2863  _list + [tuple(c
-00005100: 6f6f 7264 7329 5d0d 0a20 2020 2020 2020  oords)]..       
-00005110: 2072 6574 7572 6e20 636f 6f72 6473 5f6c   return coords_l
-00005120: 6973 740d 0a0d 0a20 2020 2040 7072 6f70  ist....    @prop
-00005130: 6572 7479 0d0a 2020 2020 6465 6620 7661  erty..    def va
-00005140: 6c75 6528 7365 6c66 293a 0d0a 2020 2020  lue(self):..    
-00005150: 2020 2020 7661 6c75 655f 6c69 7374 203d      value_list =
-00005160: 205b 5d0d 0a20 2020 2020 2020 2066 6f72   []..        for
-00005170: 2065 6e74 7279 2069 6e20 7261 6e67 6528   entry in range(
-00005180: 7365 6c66 2e64 6174 612e 6e6e 7a29 3a0d  self.data.nnz):.
-00005190: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-000051a0: 7565 5f6c 6973 7420 3d20 7661 6c75 655f  ue_list = value_
-000051b0: 6c69 7374 202b 205b 7365 6c66 2e64 6174  list + [self.dat
-000051c0: 612e 6461 7461 5b65 6e74 7279 5d5d 0d0a  a.data[entry]]..
-000051d0: 2020 2020 2020 2020 7265 7475 726e 2076          return v
-000051e0: 616c 7565 5f6c 6973 740d 0a0d 0a20 2020  alue_list....   
-000051f0: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
-00005200: 6465 6620 6e6f 726d 2873 656c 6629 3a0d  def norm(self):.
-00005210: 0a20 2020 2020 2020 2061 7272 6179 5f66  .        array_f
-00005220: 6f72 6d20 3d20 7365 6c66 2e64 6174 612e  orm = self.data.
-00005230: 746f 6465 6e73 6528 290d 0a20 2020 2020  todense()..     
-00005240: 2020 2072 6574 7572 6e20 6e70 2e6c 696e     return np.lin
-00005250: 616c 672e 6e6f 726d 2861 7272 6179 5f66  alg.norm(array_f
-00005260: 6f72 6d29 0d0a 0d0a 2020 2020 6465 6620  orm)....    def 
-00005270: 6469 7370 6c61 7928 7365 6c66 2c20 6e61  display(self, na
-00005280: 6d65 3d4e 6f6e 652c 696e 6465 6e74 5f73  me=None,indent_s
-00005290: 697a 653d 3029 3a0d 0a0d 0a20 2020 2020  ize=0):....     
-000052a0: 2020 2069 6e64 656e 7420 3d20 2222 0d0a     indent = ""..
-000052b0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-000052c0: 2072 616e 6765 2869 6e64 656e 745f 7369   range(indent_si
-000052d0: 7a65 293a 0d0a 2020 2020 2020 2020 2020  ze):..          
-000052e0: 2020 696e 6465 6e74 2b3d 2220 220d 0a0d    indent+=" "...
-000052f0: 0a20 2020 2020 2020 2070 7269 6e74 2829  .        print()
-00005300: 0d0a 2020 2020 2020 2020 6966 206e 616d  ..        if nam
-00005310: 6520 213d 204e 6f6e 653a 0d0a 2020 2020  e != None:..    
-00005320: 2020 2020 2020 2020 7072 696e 7428 696e          print(in
-00005330: 6465 6e74 2b22 2020 2020 2020 2020 6e61  dent+"        na
-00005340: 6d65 3a22 2c6e 616d 6529 0d0a 2020 2020  me:",name)..    
-00005350: 2020 2020 7072 696e 7428 696e 6465 6e74      print(indent
-00005360: 2b22 2020 6172 7261 7920 7479 7065 3a20  +"  array type: 
-00005370: 7370 6172 7365 2229 0d0a 2020 2020 2020  sparse")..      
-00005380: 2020 7072 696e 7428 696e 6465 6e74 2b22    print(indent+"
-00005390: 2020 2020 2020 2073 6861 7065 3a22 2c73         shape:",s
-000053a0: 656c 662e 7368 6170 6529 0d0a 2020 2020  elf.shape)..    
-000053b0: 2020 2020 7072 696e 7428 696e 6465 6e74      print(indent
-000053c0: 2b22 2020 2020 2064 656e 7369 7479 3a22  +"     density:"
-000053d0: 2c73 656c 662e 6e6e 7a2c 222f 222c 7365  ,self.nnz,"/",se
-000053e0: 6c66 2e73 697a 652c 227e 222c 7365 6c66  lf.size,"~",self
-000053f0: 2e6e 6e7a 2f73 656c 662e 7369 7a65 2a31  .nnz/self.size*1
-00005400: 3030 2c22 2522 290d 0a20 2020 2020 2020  00,"%")..       
-00005410: 2070 7269 6e74 2869 6e64 656e 742b 2220   print(indent+" 
-00005420: 2020 7374 6174 6973 7469 633a 222c 7365    statistic:",se
-00005430: 6c66 2e73 7461 7469 7374 6963 290d 0a20  lf.statistic).. 
-00005440: 2020 2020 2020 2070 7269 6e74 2869 6e64         print(ind
-00005450: 656e 742b 2220 2020 2020 2066 6f72 6d61  ent+"      forma
-00005460: 743a 222c 7365 6c66 2e66 6f72 6d61 7429  t:",self.format)
-00005470: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00005480: 696e 6465 6e74 2b22 2020 2020 2065 6e63  indent+"     enc
-00005490: 6f64 6572 3a22 2c73 656c 662e 656e 636f  oder:",self.enco
-000054a0: 6465 7229 0d0a 2020 2020 2020 2020 7072  der)..        pr
-000054b0: 696e 7428 696e 6465 6e74 2b22 2020 2020  int(indent+"    
-000054c0: 2020 6d65 6d6f 7279 3a22 2c6d 656d 6f72    memory:",memor
-000054d0: 795f 6469 7370 6c61 7928 7379 732e 6765  y_display(sys.ge
-000054e0: 7473 697a 656f 6628 7365 6c66 2e64 6174  tsizeof(self.dat
-000054f0: 6129 2b73 7973 2e67 6574 7369 7a65 6f66  a)+sys.getsizeof
-00005500: 2873 656c 6629 2929 0d0a 2020 2020 2020  (self)))..      
-00005510: 2020 7072 696e 7428 696e 6465 6e74 2b22    print(indent+"
-00005520: 2020 2020 2020 2020 6e6f 726d 3a22 2c73          norm:",s
-00005530: 656c 662e 6e6f 726d 290d 0a20 2020 2020  elf.norm)..     
-00005540: 2020 2070 7269 6e74 2869 6e64 656e 742b     print(indent+
-00005550: 2220 2020 2020 656e 7472 6965 733a 2229  "     entries:")
-00005560: 0d0a 0d0a 2020 2020 2020 2020 4320 3d20  ....        C = 
-00005570: 7365 6c66 2e63 6f6f 7264 730d 0a20 2020  self.coords..   
-00005580: 2020 2020 2056 203d 2073 656c 662e 7661       V = self.va
-00005590: 6c75 650d 0a20 2020 2020 2020 2066 6f72  lue..        for
-000055a0: 2065 6c65 6d20 696e 2072 616e 6765 2873   elem in range(s
-000055b0: 656c 662e 6e6e 7a29 3a0d 0a20 2020 2020  elf.nnz):..     
-000055c0: 2020 2020 2020 2069 6628 6e70 2e61 6273         if(np.abs
-000055d0: 2856 5b65 6c65 6d5d 293e 6e75 6d65 725f  (V[elem])>numer_
-000055e0: 6469 7370 6c61 795f 6375 746f 6666 293a  display_cutoff):
-000055f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005600: 2020 7072 696e 7428 696e 6465 6e74 2b22    print(indent+"
-00005610: 5c74 222c 435b 656c 656d 5d2c 636c 6561  \t",C[elem],clea
-00005620: 6e5f 666f 726d 6174 2856 5b65 6c65 6d5d  n_format(V[elem]
-00005630: 2929 0d0a 2020 2020 2020 2020 7072 696e  ))..        prin
-00005640: 7428 290d 0a0d 0a20 2020 2064 6566 2069  t()....    def i
-00005650: 6e66 6f28 7365 6c66 2c6e 616d 653d 4e6f  nfo(self,name=No
-00005660: 6e65 2c69 6e64 656e 745f 7369 7a65 3d30  ne,indent_size=0
-00005670: 293a 0d0a 0d0a 2020 2020 2020 2020 696e  ):....        in
-00005680: 6465 6e74 203d 2022 220d 0a20 2020 2020  dent = ""..     
-00005690: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-000056a0: 6528 696e 6465 6e74 5f73 697a 6529 3a0d  e(indent_size):.
-000056b0: 0a20 2020 2020 2020 2020 2020 2069 6e64  .            ind
-000056c0: 656e 742b 3d22 2022 0d0a 0d0a 2020 2020  ent+=" "....    
-000056d0: 2020 2020 7072 696e 7428 290d 0a20 2020      print()..   
-000056e0: 2020 2020 2069 6620 6e61 6d65 2021 3d20       if name != 
-000056f0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00005700: 2020 2070 7269 6e74 2869 6e64 656e 742b     print(indent+
-00005710: 2220 2020 2020 2020 206e 616d 653a 222c  "        name:",
-00005720: 6e61 6d65 290d 0a20 2020 2020 2020 2070  name)..        p
-00005730: 7269 6e74 2869 6e64 656e 742b 2220 2061  rint(indent+"  a
-00005740: 7272 6179 2074 7970 653a 2073 7061 7273  rray type: spars
-00005750: 6522 290d 0a20 2020 2020 2020 2070 7269  e")..        pri
-00005760: 6e74 2869 6e64 656e 742b 2220 2020 2020  nt(indent+"     
-00005770: 2020 7368 6170 653a 222c 7365 6c66 2e73    shape:",self.s
-00005780: 6861 7065 290d 0a20 2020 2020 2020 2070  hape)..        p
-00005790: 7269 6e74 2869 6e64 656e 742b 2220 2020  rint(indent+"   
-000057a0: 2020 6465 6e73 6974 793a 222c 7365 6c66    density:",self
-000057b0: 2e6e 6e7a 2c22 2f22 2c73 656c 662e 7369  .nnz,"/",self.si
-000057c0: 7a65 2c22 7e22 2c73 656c 662e 6e6e 7a2f  ze,"~",self.nnz/
-000057d0: 7365 6c66 2e73 697a 652a 3130 302c 2225  self.size*100,"%
-000057e0: 2229 0d0a 2020 2020 2020 2020 7072 696e  ")..        prin
-000057f0: 7428 696e 6465 6e74 2b22 2020 2073 7461  t(indent+"   sta
-00005800: 7469 7374 6963 3a22 2c73 656c 662e 7374  tistic:",self.st
-00005810: 6174 6973 7469 6329 0d0a 2020 2020 2020  atistic)..      
-00005820: 2020 7072 696e 7428 696e 6465 6e74 2b22    print(indent+"
-00005830: 2020 2020 2020 666f 726d 6174 3a22 2c73        format:",s
-00005840: 656c 662e 666f 726d 6174 290d 0a20 2020  elf.format)..   
-00005850: 2020 2020 2070 7269 6e74 2869 6e64 656e       print(inden
-00005860: 742b 2220 2020 2020 656e 636f 6465 723a  t+"     encoder:
-00005870: 222c 7365 6c66 2e65 6e63 6f64 6572 290d  ",self.encoder).
-00005880: 0a20 2020 2020 2020 2070 7269 6e74 2869  .        print(i
-00005890: 6e64 656e 742b 2220 2020 2020 206d 656d  ndent+"      mem
-000058a0: 6f72 793a 222c 6d65 6d6f 7279 5f64 6973  ory:",memory_dis
-000058b0: 706c 6179 2873 7973 2e67 6574 7369 7a65  play(sys.getsize
-000058c0: 6f66 2873 656c 662e 6461 7461 292b 7379  of(self.data)+sy
-000058d0: 732e 6765 7473 697a 656f 6628 7365 6c66  s.getsizeof(self
-000058e0: 2929 290d 0a20 2020 2020 2020 2070 7269  )))..        pri
-000058f0: 6e74 2869 6e64 656e 742b 2220 2020 2020  nt(indent+"     
-00005900: 2020 206e 6f72 6d3a 222c 7365 6c66 2e6e     norm:",self.n
-00005910: 6f72 6d29 0d0a 2020 2020 2020 2020 7072  orm)..        pr
-00005920: 696e 7428 290d 0a0d 0a20 2020 2064 6566  int()....    def
-00005930: 2073 6574 5f76 616c 7565 2873 656c 662c   set_value(self,
-00005940: 656e 7472 792c 7661 6c75 6529 3a0d 0a20  entry,value):.. 
-00005950: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
-00005960: 2e64 6174 615b 656e 7472 795d 203d 2076  .data[entry] = v
-00005970: 616c 7565 0d0a 0d0a 2020 2020 6465 6620  alue....    def 
-00005980: 7265 6d6f 7665 5f65 6e74 7279 2873 656c  remove_entry(sel
-00005990: 662c 656e 7472 7929 3a0d 0a20 2020 2020  f,entry):..     
-000059a0: 2020 2070 6f70 7065 645f 636f 6f72 6473     popped_coords
-000059b0: 203d 205b 5d0d 0a20 2020 2020 2020 2066   = []..        f
-000059c0: 6f72 2061 7869 7320 696e 2072 616e 6765  or axis in range
-000059d0: 2873 656c 662e 6461 7461 2e6e 6469 6d29  (self.data.ndim)
-000059e0: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-000059f0: 6f70 7065 645f 636f 6f72 6473 203d 2070  opped_coords = p
-00005a00: 6f70 7065 645f 636f 6f72 6473 202b 205b  opped_coords + [
-00005a10: 6e70 2e64 656c 6574 6528 7365 6c66 2e64  np.delete(self.d
-00005a20: 6174 612e 636f 6f72 6473 5b61 7869 735d  ata.coords[axis]
-00005a30: 2c65 6e74 7279 295d 0d0a 2020 2020 2020  ,entry)]..      
-00005a40: 2020 706f 7070 6564 5f63 6f6f 7264 7320    popped_coords 
-00005a50: 3d20 6e70 2e61 7272 6179 2870 6f70 7065  = np.array(poppe
-00005a60: 645f 636f 6f72 6473 290d 0a20 2020 2020  d_coords)..     
-00005a70: 2020 2070 6f70 7065 645f 7661 6c75 6520     popped_value 
-00005a80: 3d20 6e70 2e64 656c 6574 6528 7365 6c66  = np.delete(self
-00005a90: 2e64 6174 612e 6461 7461 2c65 6e74 7279  .data.data,entry
-00005aa0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-00005ab0: 2020 2020 2073 656c 662e 6461 7461 2e63       self.data.c
-00005ac0: 6f6f 7264 7320 3d20 706f 7070 6564 5f63  oords = popped_c
-00005ad0: 6f6f 7264 730d 0a20 2020 2020 2020 2073  oords..        s
-00005ae0: 656c 662e 6461 7461 2e64 6174 6120 3d20  elf.data.data = 
-00005af0: 706f 7070 6564 5f76 616c 7565 0d0a 0d0a  popped_value....
-00005b00: 2020 2020 6465 6620 6170 7065 6e64 5f65      def append_e
-00005b10: 6e74 7279 2873 656c 662c 636f 6f72 6473  ntry(self,coords
-00005b20: 2c76 616c 7565 293a 0d0a 2020 2020 2020  ,value):..      
-00005b30: 2020 6170 7065 6e64 6564 5f63 6f6f 7264    appended_coord
-00005b40: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00005b50: 666f 7220 6178 6973 2069 6e20 7261 6e67  for axis in rang
-00005b60: 6528 7365 6c66 2e64 6174 612e 6e64 696d  e(self.data.ndim
-00005b70: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00005b80: 6170 7065 6e64 6564 5f63 6f6f 7264 7320  appended_coords 
-00005b90: 3d20 6170 7065 6e64 6564 5f63 6f6f 7264  = appended_coord
-00005ba0: 7320 2b20 5b6e 702e 6170 7065 6e64 2873  s + [np.append(s
-00005bb0: 656c 662e 6461 7461 2e63 6f6f 7264 735b  elf.data.coords[
-00005bc0: 6178 6973 5d2c 636f 6f72 6473 5b61 7869  axis],coords[axi
-00005bd0: 735d 295d 0d0a 2020 2020 2020 2020 6170  s])]..        ap
-00005be0: 7065 6e64 6564 5f63 6f6f 7264 7320 3d20  pended_coords = 
-00005bf0: 6e70 2e61 7272 6179 2861 7070 656e 6465  np.array(appende
-00005c00: 645f 636f 6f72 6473 290d 0a20 2020 2020  d_coords)..     
-00005c10: 2020 2061 7070 656e 6465 645f 7661 6c75     appended_valu
-00005c20: 6520 3d20 6e70 2e61 7070 656e 6428 7365  e = np.append(se
-00005c30: 6c66 2e64 6174 612e 6461 7461 2c76 616c  lf.data.data,val
-00005c40: 7565 290d 0a20 2020 2020 2020 200d 0a20  ue)..        .. 
-00005c50: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
-00005c60: 2e63 6f6f 7264 7320 3d20 6170 7065 6e64  .coords = append
-00005c70: 6564 5f63 6f6f 7264 730d 0a20 2020 2020  ed_coords..     
-00005c80: 2020 2073 656c 662e 6461 7461 2e64 6174     self.data.dat
-00005c90: 6120 3d20 6170 7065 6e64 6564 5f76 616c  a = appended_val
-00005ca0: 7565 0d0a 0d0a 2020 2020 6465 6620 7265  ue....    def re
-00005cb0: 6d6f 7665 5f7a 6572 6f73 2873 656c 6629  move_zeros(self)
-00005cc0: 3a0d 0a20 2020 2020 2020 2072 6574 203d  :..        ret =
-00005cd0: 2073 656c 662e 636f 7079 2829 0d0a 2020   self.copy()..  
-00005ce0: 2020 2020 2020 7a65 726f 5f65 6e74 7279        zero_entry
-00005cf0: 5f6c 6973 7420 3d20 5b5d 0d0a 2020 2020  _list = []..    
-00005d00: 2020 2020 666f 7220 656e 7472 7920 696e      for entry in
-00005d10: 2072 616e 6765 2872 6574 2e64 6174 612e   range(ret.data.
-00005d20: 6e6e 7a29 3a0d 0a20 2020 2020 2020 2020  nnz):..         
-00005d30: 2020 2069 6620 6e70 2e61 6273 2872 6574     if np.abs(ret
-00005d40: 2e64 6174 612e 6461 7461 5b65 6e74 7279  .data.data[entry
-00005d50: 5d29 203c 206e 756d 6572 5f63 7574 6f66  ]) < numer_cutof
-00005d60: 663a 0d0a 2020 2020 2020 2020 2020 2020  f:..            
-00005d70: 2020 2020 7a65 726f 5f65 6e74 7279 5f6c      zero_entry_l
-00005d80: 6973 7420 3d20 7a65 726f 5f65 6e74 7279  ist = zero_entry
-00005d90: 5f6c 6973 7420 2b20 5b65 6e74 7279 5d0d  _list + [entry].
-00005da0: 0a0d 0a20 2020 2020 2020 2066 6f72 2069  ...        for i
-00005db0: 2c7a 6572 6f5f 656e 7472 7920 696e 2065  ,zero_entry in e
-00005dc0: 6e75 6d65 7261 7465 287a 6572 6f5f 656e  numerate(zero_en
-00005dd0: 7472 795f 6c69 7374 293a 0d0a 2020 2020  try_list):..    
-00005de0: 2020 2020 2020 2020 7265 742e 7265 6d6f          ret.remo
-00005df0: 7665 5f65 6e74 7279 287a 6572 6f5f 656e  ve_entry(zero_en
-00005e00: 7472 792d 6929 0d0a 2020 2020 2020 2020  try-i)..        
-00005e10: 7265 7475 726e 2072 6574 0d0a 0d0a 2020  return ret....  
-00005e20: 2020 6465 6620 636f 7079 2873 656c 6629    def copy(self)
-00005e30: 3a0d 0a20 2020 2020 2020 2023 636f 7079  :..        #copy
-00005e40: 2073 7061 7273 6520 7072 6f70 6572 7469   sparse properti
-00005e50: 6573 0d0a 2020 2020 2020 2020 7265 7420  es..        ret 
-00005e60: 3d20 7370 6172 7365 2829 0d0a 2020 2020  = sparse()..    
-00005e70: 2020 2020 7265 742e 6461 7461 203d 2073      ret.data = s
-00005e80: 656c 662e 6461 7461 2e63 6f70 7928 290d  elf.data.copy().
-00005e90: 0a20 2020 2020 2020 2072 6574 2e73 7461  .        ret.sta
-00005ea0: 7469 7374 6963 203d 2073 656c 662e 7374  tistic = self.st
-00005eb0: 6174 6973 7469 630d 0a20 2020 2020 2020  atistic..       
-00005ec0: 2072 6574 2e66 6f72 6d61 7420 3d20 7365   ret.format = se
-00005ed0: 6c66 2e66 6f72 6d61 740d 0a20 2020 2020  lf.format..     
-00005ee0: 2020 2072 6574 2e65 6e63 6f64 6572 203d     ret.encoder =
-00005ef0: 2073 656c 662e 656e 636f 6465 720d 0a20   self.encoder.. 
-00005f00: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00005f10: 740d 0a20 2020 200d 0a20 2020 2064 6566  t..    ..    def
-00005f20: 205f 5f61 6464 5f5f 2873 656c 662c 206f   __add__(self, o
-00005f30: 7468 6572 293a 0d0a 2020 2020 2020 2020  ther):..        
-00005f40: 6966 2873 656c 662e 7368 6170 6521 3d6f  if(self.shape!=o
-00005f50: 7468 6572 2e73 6861 7065 0d0a 2020 2020  ther.shape..    
-00005f60: 2020 2020 2020 2020 6f72 2073 656c 662e          or self.
-00005f70: 7374 6174 6973 7469 6321 3d6f 7468 6572  statistic!=other
-00005f80: 2e73 7461 7469 7374 6963 0d0a 2020 2020  .statistic..    
-00005f90: 2020 2020 2020 2020 206f 7220 7365 6c66           or self
-00005fa0: 2e66 6f72 6d61 7421 3d6f 7468 6572 2e66  .format!=other.f
-00005fb0: 6f72 6d61 740d 0a20 2020 2020 2020 2020  ormat..         
-00005fc0: 2020 2020 206f 7220 7365 6c66 2e65 6e63       or self.enc
-00005fd0: 6f64 6572 213d 6f74 6865 722e 656e 636f  oder!=other.enco
-00005fe0: 6465 7229 3a0d 0a20 2020 2020 2020 2020  der):..         
-00005ff0: 2020 2065 7272 6f72 2822 4572 726f 725b     error("Error[
-00006000: 7370 6172 7365 2e2b 5d3a 2049 6e63 6f6e  sparse.+]: Incon
-00006010: 7369 7374 656e 7420 6f62 6a65 6374 2070  sistent object p
-00006020: 726f 7065 7274 6965 7322 290d 0a20 2020  roperties")..   
-00006030: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00006040: 2020 2072 6574 203d 2073 656c 662e 636f     ret = self.co
-00006050: 7079 2829 0d0a 2020 2020 2020 2020 7265  py()..        re
-00006060: 742e 6461 7461 203d 2072 6574 2e64 6174  t.data = ret.dat
-00006070: 612b 6f74 6865 722e 6461 7461 0d0a 2020  a+other.data..  
-00006080: 2020 2020 2020 7265 7475 726e 2072 6574        return ret
-00006090: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-000060a0: 6465 6620 5f5f 7375 625f 5f28 7365 6c66  def __sub__(self
-000060b0: 2c20 6f74 6865 7229 3a0d 0a20 2020 2020  , other):..     
-000060c0: 2020 2069 6628 7365 6c66 2e73 6861 7065     if(self.shape
-000060d0: 213d 6f74 6865 722e 7368 6170 650d 0a20  !=other.shape.. 
-000060e0: 2020 2020 2020 2020 2020 206f 7220 7365             or se
-000060f0: 6c66 2e73 7461 7469 7374 6963 213d 6f74  lf.statistic!=ot
-00006100: 6865 722e 7374 6174 6973 7469 630d 0a20  her.statistic.. 
-00006110: 2020 2020 2020 2020 2020 2020 6f72 2073              or s
-00006120: 656c 662e 666f 726d 6174 213d 6f74 6865  elf.format!=othe
-00006130: 722e 666f 726d 6174 0d0a 2020 2020 2020  r.format..      
-00006140: 2020 2020 2020 2020 6f72 2073 656c 662e          or self.
-00006150: 656e 636f 6465 7221 3d6f 7468 6572 2e65  encoder!=other.e
-00006160: 6e63 6f64 6572 293a 0d0a 2020 2020 2020  ncoder):..      
-00006170: 2020 2020 2020 6572 726f 7228 2245 7272        error("Err
-00006180: 6f72 5b73 7061 7273 652e 2d5d 3a20 496e  or[sparse.-]: In
-00006190: 636f 6e73 6973 7465 6e74 206f 626a 6563  consistent objec
-000061a0: 7420 7072 6f70 6572 7469 6573 2229 0d0a  t properties")..
-000061b0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000061c0: 2020 2020 2020 7265 7420 3d20 7365 6c66        ret = self
-000061d0: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
-000061e0: 2072 6574 2e64 6174 6120 3d20 7265 742e   ret.data = ret.
-000061f0: 6461 7461 2d6f 7468 6572 2e64 6174 610d  data-other.data.
-00006200: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00006210: 7265 740d 0a20 2020 2020 2020 200d 0a20  ret..        .. 
-00006220: 2020 2064 6566 205f 5f6d 756c 5f5f 2873     def __mul__(s
-00006230: 656c 662c 206f 7468 6572 293a 0d0a 2020  elf, other):..  
-00006240: 2020 2020 2020 7265 7420 3d20 7365 6c66        ret = self
-00006250: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
-00006260: 2072 6574 2e64 6174 6120 3d20 7265 742e   ret.data = ret.
-00006270: 6461 7461 2a6f 7468 6572 0d0a 2020 2020  data*other..    
-00006280: 2020 2020 7265 7475 726e 2072 6574 0d0a      return ret..
-00006290: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-000062a0: 6620 5f5f 726d 756c 5f5f 2873 656c 662c  f __rmul__(self,
-000062b0: 206f 7468 6572 293a 0d0a 2020 2020 2020   other):..      
-000062c0: 2020 7265 7475 726e 2073 656c 662a 6f74    return self*ot
-000062d0: 6865 720d 0a20 2020 2020 2020 200d 0a20  her..        .. 
-000062e0: 2020 2023 6465 6620 5f5f 6c65 6e5f 5f28     #def __len__(
-000062f0: 7365 6c66 293a 0d0a 2020 2020 2320 2020  self):..    #   
-00006300: 2072 6574 7572 6e20 6c65 6e28 7365 6c66   return len(self
-00006310: 2e64 6174 6129 0d0a 2020 2020 0d0a 2020  .data)..    ..  
-00006320: 2020 6465 6620 5f5f 7374 725f 5f28 7365    def __str__(se
-00006330: 6c66 293a 0d0a 2020 2020 2020 2020 7265  lf):..        re
-00006340: 7475 726e 2073 7472 2873 656c 662e 6461  turn str(self.da
-00006350: 7461 290d 0a20 2020 200d 0a20 2020 2064  ta)..    ..    d
-00006360: 6566 205f 5f72 6570 725f 5f28 7365 6c66  ef __repr__(self
-00006370: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
-00006380: 726e 2072 6570 7228 7365 6c66 2e64 6174  rn repr(self.dat
-00006390: 6129 0d0a 0d0a 2020 2020 6465 6620 7377  a)....    def sw
-000063a0: 6974 6368 5f66 6f72 6d61 7428 7365 6c66  itch_format(self
-000063b0: 2c73 6176 655f 6d65 6d6f 7279 3d46 616c  ,save_memory=Fal
-000063c0: 7365 293a 0d0a 2020 2020 2020 2020 7265  se):..        re
-000063d0: 7475 726e 2073 7061 7273 6528 6465 6e73  turn sparse(dens
-000063e0: 6528 7365 6c66 292e 7377 6974 6368 5f66  e(self).switch_f
-000063f0: 6f72 6d61 7428 7361 7665 5f6d 656d 6f72  ormat(save_memor
-00006400: 793d 7361 7665 5f6d 656d 6f72 7929 290d  y=save_memory)).
-00006410: 0a0d 0a20 2020 2064 6566 2073 7769 7463  ...    def switc
-00006420: 685f 656e 636f 6465 7228 7365 6c66 2c73  h_encoder(self,s
-00006430: 6176 655f 6d65 6d6f 7279 3d46 616c 7365  ave_memory=False
-00006440: 293a 0d0a 2020 2020 2020 2020 7265 7475  ):..        retu
-00006450: 726e 2073 7061 7273 6528 6465 6e73 6528  rn sparse(dense(
-00006460: 7365 6c66 292e 7377 6974 6368 5f65 6e63  self).switch_enc
-00006470: 6f64 6572 2873 6176 655f 6d65 6d6f 7279  oder(save_memory
-00006480: 3d73 6176 655f 6d65 6d6f 7279 2929 0d0a  =save_memory))..
-00006490: 0d0a 2020 2020 6465 6620 666f 7263 655f  ..    def force_
-000064a0: 656e 636f 6465 7228 7365 6c66 2c74 6172  encoder(self,tar
-000064b0: 6765 743d 2263 616e 6f6e 6963 616c 2229  get="canonical")
-000064c0: 3a0d 0a20 2020 2020 2020 2069 6620 7461  :..        if ta
-000064d0: 7267 6574 206e 6f74 2069 6e20 656e 636f  rget not in enco
-000064e0: 6465 725f 7479 7065 3a0d 0a20 2020 2020  der_type:..     
-000064f0: 2020 2020 2020 2065 7272 6f72 2822 4572         error("Er
-00006500: 726f 725b 7370 6172 7365 2e66 6f72 6365  ror[sparse.force
-00006510: 5f65 6e63 6f64 6572 5d3a 2055 6e72 6563  _encoder]: Unrec
-00006520: 6f67 6e69 7a65 6420 7461 7267 6574 2065  ognized target e
-00006530: 6e63 6f64 6572 2e22 290d 0a20 2020 2020  ncoder.")..     
-00006540: 2020 2069 6620 7461 7267 6574 2021 3d20     if target != 
-00006550: 7365 6c66 2e65 6e63 6f64 6572 203a 0d0a  self.encoder :..
-00006560: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00006570: 726e 2073 656c 662e 7377 6974 6368 5f65  rn self.switch_e
-00006580: 6e63 6f64 6572 2829 0d0a 2020 2020 2020  ncoder()..      
-00006590: 2020 656c 7365 203a 0d0a 2020 2020 2020    else :..      
-000065a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-000065b0: 662e 636f 7079 2829 0d0a 0d0a 2020 2020  f.copy()....    
-000065c0: 6465 6620 666f 7263 655f 666f 726d 6174  def force_format
-000065d0: 2873 656c 662c 7461 7267 6574 3d22 7374  (self,target="st
-000065e0: 616e 6461 7264 2229 3a0d 0a20 2020 2020  andard"):..     
-000065f0: 2020 2069 6620 7461 7267 6574 206e 6f74     if target not
-00006600: 2069 6e20 666f 726d 6174 5f74 7970 653a   in format_type:
-00006610: 0d0a 2020 2020 2020 2020 2020 2020 6572  ..            er
-00006620: 726f 7228 2245 7272 6f72 5b73 7061 7273  ror("Error[spars
-00006630: 652e 666f 7263 655f 666f 726d 6174 5d3a  e.force_format]:
-00006640: 2055 6e72 6563 6f67 6e69 7a65 6420 7461   Unrecognized ta
-00006650: 7267 6574 2066 6f72 6d61 742e 2229 0d0a  rget format.")..
-00006660: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
-00006670: 7420 213d 2073 656c 662e 666f 726d 6174  t != self.format
-00006680: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
-00006690: 7265 7475 726e 2073 656c 662e 7377 6974  return self.swit
-000066a0: 6368 5f66 6f72 6d61 7428 290d 0a20 2020  ch_format()..   
-000066b0: 2020 2020 2065 6c73 6520 3a0d 0a20 2020       else :..   
-000066c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000066d0: 7365 6c66 2e63 6f70 7928 290d 0a0d 0a20  self.copy().... 
-000066e0: 2020 2064 6566 206a 6f69 6e5f 6c65 6773     def join_legs
-000066f0: 2873 656c 662c 7374 7269 6e67 5f69 6e70  (self,string_inp
-00006700: 2c6d 616b 655f 666f 726d 6174 3d27 7374  ,make_format='st
-00006710: 616e 6461 7264 272c 696e 7465 726d 6564  andard',intermed
-00006720: 6961 7465 5f73 7461 743d 282d 312c 3129  iate_stat=(-1,1)
-00006730: 2c73 6176 655f 6d65 6d6f 7279 3d46 616c  ,save_memory=Fal
-00006740: 7365 293a 0d0a 2020 2020 2020 2020 7265  se):..        re
-00006750: 7475 726e 206a 6f69 6e5f 6c65 6773 2873  turn join_legs(s
-00006760: 656c 662c 7374 7269 6e67 5f69 6e70 2c6d  elf,string_inp,m
-00006770: 616b 655f 666f 726d 6174 2c69 6e74 6572  ake_format,inter
-00006780: 6d65 6469 6174 655f 7374 6174 2c73 6176  mediate_stat,sav
-00006790: 655f 6d65 6d6f 7279 290d 0a0d 0a20 2020  e_memory)....   
-000067a0: 2064 6566 2073 706c 6974 5f6c 6567 7328   def split_legs(
-000067b0: 7365 6c66 2c73 7472 696e 675f 696e 702c  self,string_inp,
-000067c0: 6669 6e61 6c5f 7374 6174 2c66 696e 616c  final_stat,final
-000067d0: 5f73 6861 7065 2c69 6e74 6572 6d65 6469  _shape,intermedi
-000067e0: 6174 655f 7374 6174 3d28 2d31 2c31 292c  ate_stat=(-1,1),
-000067f0: 7361 7665 5f6d 656d 6f72 793d 4661 6c73  save_memory=Fals
-00006800: 6529 3a0d 0a20 2020 2020 2020 2072 6574  e):..        ret
-00006810: 7572 6e20 7370 6c69 745f 6c65 6773 2873  urn split_legs(s
-00006820: 656c 662c 7374 7269 6e67 5f69 6e70 2c66  elf,string_inp,f
-00006830: 696e 616c 5f73 7461 742c 6669 6e61 6c5f  inal_stat,final_
-00006840: 7368 6170 652c 696e 7465 726d 6564 6961  shape,intermedia
-00006850: 7465 5f73 7461 742c 7361 7665 5f6d 656d  te_stat,save_mem
-00006860: 6f72 7929 0d0a 0d0a 2020 2020 6465 6620  ory)....    def 
-00006870: 6863 6f6e 6a75 6761 7465 2873 656c 662c  hconjugate(self,
-00006880: 696e 7075 745f 7374 7269 6e67 2c73 6176  input_string,sav
-00006890: 655f 6d65 6d6f 7279 3d46 616c 7365 293a  e_memory=False):
-000068a0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000068b0: 2068 636f 6e6a 7567 6174 6528 7365 6c66   hconjugate(self
-000068c0: 2c69 6e70 7574 5f73 7472 696e 672c 7361  ,input_string,sa
-000068d0: 7665 5f6d 656d 6f72 7929 0d0a 0d0a 2020  ve_memory)....  
-000068e0: 2020 6465 6620 7376 6428 7365 6c66 2c73    def svd(self,s
-000068f0: 7472 696e 675f 696e 702c 6375 746f 6666  tring_inp,cutoff
-00006900: 3d4e 6f6e 652c 7361 7665 5f6d 656d 6f72  =None,save_memor
-00006910: 793d 4661 6c73 6529 3a0d 0a20 2020 2020  y=False):..     
-00006920: 2020 2072 6574 7572 6e20 7376 6428 7365     return svd(se
-00006930: 6c66 2c73 7472 696e 675f 696e 702c 6375  lf,string_inp,cu
-00006940: 746f 6666 2c73 6176 655f 6d65 6d6f 7279  toff,save_memory
-00006950: 290d 0a0d 0a20 2020 2064 6566 2065 6967  )....    def eig
-00006960: 2873 656c 662c 7374 7269 6e67 5f69 6e70  (self,string_inp
-00006970: 2c63 7574 6f66 663d 4e6f 6e65 2c64 6562  ,cutoff=None,deb
-00006980: 7567 5f6d 6f64 653d 4661 6c73 652c 7361  ug_mode=False,sa
-00006990: 7665 5f6d 656d 6f72 793d 4661 6c73 6529  ve_memory=False)
-000069a0: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-000069b0: 6e20 6569 6728 7365 6c66 2c73 7472 696e  n eig(self,strin
-000069c0: 675f 696e 702c 6375 746f 6666 2c64 6562  g_inp,cutoff,deb
-000069d0: 7567 5f6d 6f64 652c 7361 7665 5f6d 656d  ug_mode,save_mem
-000069e0: 6f72 7929 0d0a 0d0a 2323 2323 2323 2323  ory)....########
+00004660: 0d0a 2323 2020 2020 2020 2020 2020 2020  ..##            
+00004670: 5370 6172 7365 2047 7261 7373 6d61 6e6e  Sparse Grassmann
+00004680: 2061 7272 6179 7320 2020 2020 2020 2020   arrays         
+00004690: 2020 2020 2323 0d0a 2323 2323 2323 2323      ##..########
+000046a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000046b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000046c0: 2323 2323 2323 2323 2323 2323 0d0a 0d0a  ############....
+000046d0: 636c 6173 7320 7370 6172 7365 3a0d 0a20  class sparse:.. 
+000046e0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000046f0: 7365 6c66 2c20 6461 7461 3d4e 6f6e 652c  self, data=None,
+00004700: 2065 6e63 6f64 6572 203d 2022 6361 6e6f   encoder = "cano
+00004710: 6e69 6361 6c22 2c20 666f 726d 6174 203d  nical", format =
+00004720: 2022 7374 616e 6461 7264 222c 2073 7461   "standard", sta
+00004730: 7469 7374 6963 203d 204e 6f6e 6529 3a0d  tistic = None):.
+00004740: 0a20 2020 200d 0a20 2020 2020 2020 2023  .    ..        #
+00004750: 636f 7079 2073 7061 7273 6520 7072 6f70  copy sparse prop
+00004760: 6572 7469 6573 0d0a 2020 2020 2020 2020  erties..        
+00004770: 7365 6c66 2e64 6174 6120 3d20 4e6f 6e65  self.data = None
+00004780: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
+00004790: 7461 7469 7374 6963 203d 204e 6f6e 650d  tatistic = None.
+000047a0: 0a20 2020 2020 2020 2073 656c 662e 666f  .        self.fo
+000047b0: 726d 6174 203d 2066 6f72 6d61 740d 0a20  rmat = format.. 
+000047c0: 2020 2020 2020 2073 656c 662e 656e 636f         self.enco
+000047d0: 6465 7220 3d20 656e 636f 6465 720d 0a0d  der = encoder...
+000047e0: 0a20 2020 2020 2020 2064 6566 6175 6c74  .        default
+000047f0: 203d 2054 7275 650d 0a20 2020 200d 0a20   = True..    .. 
+00004800: 2020 2020 2020 2069 6628 656e 636f 6465         if(encode
+00004810: 7220 6e6f 7420 696e 2065 6e63 6f64 6572  r not in encoder
+00004820: 5f74 7970 6529 3a0d 0a20 2020 2020 2020  _type):..       
+00004830: 2020 2020 2065 7272 6f72 2822 4572 726f       error("Erro
+00004840: 725b 7370 6172 7365 5d3a 2055 6e6b 6e6f  r[sparse]: Unkno
+00004850: 776e 2065 6e63 6f64 6572 2e22 290d 0a20  wn encoder.").. 
+00004860: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00004870: 2020 2020 2069 6628 666f 726d 6174 206e       if(format n
+00004880: 6f74 2069 6e20 666f 726d 6174 5f74 7970  ot in format_typ
+00004890: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+000048a0: 2065 7272 6f72 2822 4572 726f 725b 7370   error("Error[sp
+000048b0: 6172 7365 5d3a 2055 6e6b 6e6f 776e 2066  arse]: Unknown f
+000048c0: 6f72 6d61 742e 2229 0d0a 2020 2020 2020  ormat.")..      
+000048d0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000048e0: 6966 2874 7970 6528 6461 7461 293d 3d6e  if(type(data)==n
+000048f0: 702e 6172 7261 7920 6f72 2074 7970 6528  p.array or type(
+00004900: 6461 7461 293d 3d6e 702e 6e64 6172 7261  data)==np.ndarra
+00004910: 7920 6f72 2074 7970 6528 6461 7461 293d  y or type(data)=
+00004920: 3d6c 6973 7429 3a0d 0a20 2020 2020 2020  =list):..       
+00004930: 2020 2020 2073 656c 662e 6461 7461 2020       self.data  
+00004940: 3d20 7370 2e43 4f4f 2e66 726f 6d5f 6e75  = sp.COO.from_nu
+00004950: 6d70 7928 6e70 2e61 7272 6179 2864 6174  mpy(np.array(dat
+00004960: 6129 290d 0a20 2020 2020 2020 2020 2020  a))..           
+00004970: 2064 6566 6175 6c74 203d 2046 616c 7365   default = False
+00004980: 0d0a 2020 2020 2020 2020 656c 6966 2874  ..        elif(t
+00004990: 7970 6528 6461 7461 293d 3d73 702e 434f  ype(data)==sp.CO
+000049a0: 4f29 3a0d 0a20 2020 2020 2020 2020 2020  O):..           
+000049b0: 2073 656c 662e 6461 7461 2020 3d20 6461   self.data  = da
+000049c0: 7461 2e63 6f70 7928 290d 0a20 2020 2020  ta.copy()..     
+000049d0: 2020 2020 2020 2064 6566 6175 6c74 203d         default =
+000049e0: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
+000049f0: 656c 6966 2874 7970 6528 6461 7461 293d  elif(type(data)=
+00004a00: 3d64 656e 7365 293a 0d0a 2020 2020 2020  =dense):..      
+00004a10: 2020 2020 2020 2363 6f70 7920 7370 6172        #copy spar
+00004a20: 7365 2070 726f 7065 7274 6965 730d 0a20  se properties.. 
+00004a30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004a40: 6461 7461 2020 3d20 7370 2e43 4f4f 2e66  data  = sp.COO.f
+00004a50: 726f 6d5f 6e75 6d70 7928 6461 7461 2e64  rom_numpy(data.d
+00004a60: 6174 6129 0d0a 2020 2020 2020 2020 2020  ata)..          
+00004a70: 2020 7365 6c66 2e73 7461 7469 7374 6963    self.statistic
+00004a80: 203d 2064 6174 612e 7374 6174 6973 7469   = data.statisti
+00004a90: 630d 0a20 2020 2020 2020 2020 2020 2073  c..            s
+00004aa0: 656c 662e 666f 726d 6174 203d 2064 6174  elf.format = dat
+00004ab0: 612e 666f 726d 6174 0d0a 2020 2020 2020  a.format..      
+00004ac0: 2020 2020 2020 7365 6c66 2e65 6e63 6f64        self.encod
+00004ad0: 6572 203d 2064 6174 612e 656e 636f 6465  er = data.encode
+00004ae0: 720d 0a20 2020 2020 2020 2020 2020 2064  r..            d
+00004af0: 6566 6175 6c74 203d 2046 616c 7365 0d0a  efault = False..
+00004b00: 2020 2020 2020 2020 656c 6966 2874 7970          elif(typ
+00004b10: 6528 6461 7461 293d 3d73 7061 7273 6529  e(data)==sparse)
+00004b20: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
+00004b30: 636f 7079 2073 7061 7273 6520 7072 6f70  copy sparse prop
+00004b40: 6572 7469 6573 0d0a 2020 2020 2020 2020  erties..        
+00004b50: 2020 2020 7365 6c66 2e64 6174 6120 3d20      self.data = 
+00004b60: 6461 7461 2e64 6174 612e 636f 7079 2829  data.data.copy()
+00004b70: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00004b80: 6c66 2e73 7461 7469 7374 6963 203d 2064  lf.statistic = d
+00004b90: 6174 612e 7374 6174 6973 7469 630d 0a20  ata.statistic.. 
+00004ba0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00004bb0: 666f 726d 6174 203d 2064 6174 612e 666f  format = data.fo
+00004bc0: 726d 6174 0d0a 2020 2020 2020 2020 2020  rmat..          
+00004bd0: 2020 7365 6c66 2e65 6e63 6f64 6572 203d    self.encoder =
+00004be0: 2064 6174 612e 656e 636f 6465 720d 0a20   data.encoder.. 
+00004bf0: 2020 2020 2020 2020 2020 2064 6566 6175             defau
+00004c00: 6c74 203d 2046 616c 7365 0d0a 2020 2020  lt = False..    
+00004c10: 2020 2020 656c 6966 2064 6174 613d 3d4e      elif data==N
+00004c20: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00004c30: 2020 226e 6f74 6869 6e67 2074 6f20 7365    "nothing to se
+00004c40: 6520 6865 7265 220d 0a20 2020 2020 2020  e here"..       
+00004c50: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00004c60: 2020 2020 6572 726f 7228 2245 7272 6f72      error("Error
+00004c70: 5b73 7061 7273 655d 3a20 496e 7661 6c69  [sparse]: Invali
+00004c80: 6420 696e 6974 6961 6c69 7a65 6420 6461  d initialized da
+00004c90: 7461 2229 0d0a 2020 2020 2020 2020 2020  ta")..          
+00004ca0: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
+00004cb0: 2020 2020 2020 6966 2073 7461 7469 7374        if statist
+00004cc0: 6963 2021 3d20 4e6f 6e65 3a0d 0a20 2020  ic != None:..   
+00004cd0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00004ce0: 6174 6973 7469 6320 3d20 6d61 6b65 5f74  atistic = make_t
+00004cf0: 7570 6c65 2873 7461 7469 7374 6963 290d  uple(statistic).
+00004d00: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00004d10: 2020 2069 6620 6e6f 7420 6465 6661 756c     if not defaul
+00004d20: 7420 616e 6420 6e6f 7420 736b 6970 5f70  t and not skip_p
+00004d30: 6f77 6572 5f6f 665f 7477 6f5f 6368 6563  ower_of_two_chec
+00004d40: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
+00004d50: 666f 7220 692c 6469 6d20 696e 2065 6e75  for i,dim in enu
+00004d60: 6d65 7261 7465 2873 656c 662e 6461 7461  merate(self.data
+00004d70: 2e73 6861 7065 293a 0d0a 2020 2020 2020  .shape):..      
+00004d80: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00004d90: 662e 7374 6174 6973 7469 635b 695d 2069  f.statistic[i] i
+00004da0: 6e20 6665 726d 695f 7479 7065 2061 6e64  n fermi_type and
+00004db0: 2064 696d 2021 3d20 696e 7428 322a 2a6d   dim != int(2**m
+00004dc0: 6174 682e 666c 6f6f 7228 6e70 2e6c 6f67  ath.floor(np.log
+00004dd0: 3228 6469 6d29 2929 3a0d 0a20 2020 2020  2(dim))):..     
+00004de0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00004df0: 7272 6f72 2822 4572 726f 725b 7370 6172  rror("Error[spar
+00004e00: 7365 5d3a 2053 6f6d 6520 6f66 2074 6865  se]: Some of the
+00004e10: 2066 6572 6d69 6f6e 6963 2074 656e 736f   fermionic tenso
+00004e20: 7220 7368 6170 6573 2061 7265 206e 6f74  r shapes are not
+00004e30: 2061 2070 6f77 6572 206f 6620 7477 6f2e   a power of two.
+00004e40: 5c6e 2020 2020 2020 2020 2020 2020 2020  \n              
+00004e50: 2048 6176 6520 796f 7520 6164 6465 6420   Have you added 
+00004e60: 7468 6520 3c73 7461 7469 7374 6963 3e20  the <statistic> 
+00004e70: 6172 6775 6d65 6e74 2077 6865 6e20 6361  argument when ca
+00004e80: 6c6c 696e 6720 7468 6973 2066 756e 6374  lling this funct
+00004e90: 696f 6e3f 2229 0d0a 2020 2020 2020 2020  ion?")..        
+00004ea0: 2020 2020 2020 200d 0a20 2020 2040 7072         ..    @pr
+00004eb0: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
+00004ec0: 6e6e 7a28 7365 6c66 293a 0d0a 2020 2020  nnz(self):..    
+00004ed0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00004ee0: 6461 7461 2e6e 6e7a 0d0a 0d0a 2020 2020  data.nnz....    
+00004ef0: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+00004f00: 6566 2073 6861 7065 2873 656c 6629 3a0d  ef shape(self):.
+00004f10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00004f20: 7365 6c66 2e64 6174 612e 7368 6170 650d  self.data.shape.
+00004f30: 0a0d 0a20 2020 2040 7072 6f70 6572 7479  ...    @property
+00004f40: 0d0a 2020 2020 6465 6620 7369 7a65 2873  ..    def size(s
+00004f50: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
+00004f60: 6574 7572 6e20 7365 6c66 2e64 6174 612e  eturn self.data.
+00004f70: 7369 7a65 0d0a 0d0a 2020 2020 4070 726f  size....    @pro
+00004f80: 7065 7274 790d 0a20 2020 2064 6566 206e  perty..    def n
+00004f90: 6469 6d28 7365 6c66 293a 0d0a 2020 2020  dim(self):..    
+00004fa0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00004fb0: 6461 7461 2e6e 6469 6d0d 0a0d 0a20 2020  data.ndim....   
+00004fc0: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
+00004fd0: 6465 6620 636f 6f72 6473 2873 656c 6629  def coords(self)
+00004fe0: 3a0d 0a20 2020 2020 2020 2063 6f6f 7264  :..        coord
+00004ff0: 735f 6c69 7374 203d 205b 5d0d 0a20 2020  s_list = []..   
+00005000: 2020 2020 2066 6f72 2065 6e74 7279 2069       for entry i
+00005010: 6e20 7261 6e67 6528 7365 6c66 2e64 6174  n range(self.dat
+00005020: 612e 6e6e 7a29 3a0d 0a20 2020 2020 2020  a.nnz):..       
+00005030: 2020 2020 2063 6f6f 7264 7320 3d20 5b5d       coords = []
+00005040: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+00005050: 7220 6178 6973 2069 6e20 7261 6e67 6528  r axis in range(
+00005060: 7365 6c66 2e64 6174 612e 6e64 696d 293a  self.data.ndim):
+00005070: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005080: 2020 636f 6f72 6473 203d 2063 6f6f 7264    coords = coord
+00005090: 7320 2b20 5b73 656c 662e 6461 7461 2e63  s + [self.data.c
+000050a0: 6f6f 7264 735b 6178 6973 5d5b 656e 7472  oords[axis][entr
+000050b0: 795d 5d0d 0a20 2020 2020 2020 2020 2020  y]]..           
+000050c0: 2063 6f6f 7264 735f 6c69 7374 203d 2063   coords_list = c
+000050d0: 6f6f 7264 735f 6c69 7374 202b 205b 7475  oords_list + [tu
+000050e0: 706c 6528 636f 6f72 6473 295d 0d0a 2020  ple(coords)]..  
+000050f0: 2020 2020 2020 7265 7475 726e 2063 6f6f        return coo
+00005100: 7264 735f 6c69 7374 0d0a 0d0a 2020 2020  rds_list....    
+00005110: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+00005120: 6566 2076 616c 7565 2873 656c 6629 3a0d  ef value(self):.
+00005130: 0a20 2020 2020 2020 2076 616c 7565 5f6c  .        value_l
+00005140: 6973 7420 3d20 5b5d 0d0a 2020 2020 2020  ist = []..      
+00005150: 2020 666f 7220 656e 7472 7920 696e 2072    for entry in r
+00005160: 616e 6765 2873 656c 662e 6461 7461 2e6e  ange(self.data.n
+00005170: 6e7a 293a 0d0a 2020 2020 2020 2020 2020  nz):..          
+00005180: 2020 7661 6c75 655f 6c69 7374 203d 2076    value_list = v
+00005190: 616c 7565 5f6c 6973 7420 2b20 5b73 656c  alue_list + [sel
+000051a0: 662e 6461 7461 2e64 6174 615b 656e 7472  f.data.data[entr
+000051b0: 795d 5d0d 0a20 2020 2020 2020 2072 6574  y]]..        ret
+000051c0: 7572 6e20 7661 6c75 655f 6c69 7374 0d0a  urn value_list..
+000051d0: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
+000051e0: 0a20 2020 2064 6566 206e 6f72 6d28 7365  .    def norm(se
+000051f0: 6c66 293a 0d0a 2020 2020 2020 2020 6172  lf):..        ar
+00005200: 7261 795f 666f 726d 203d 2073 656c 662e  ray_form = self.
+00005210: 6461 7461 2e74 6f64 656e 7365 2829 0d0a  data.todense()..
+00005220: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00005230: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 6172  p.linalg.norm(ar
+00005240: 7261 795f 666f 726d 290d 0a0d 0a20 2020  ray_form)....   
+00005250: 2064 6566 2064 6973 706c 6179 2873 656c   def display(sel
+00005260: 662c 206e 616d 653d 4e6f 6e65 2c69 6e64  f, name=None,ind
+00005270: 656e 745f 7369 7a65 3d30 293a 0d0a 0d0a  ent_size=0):....
+00005280: 2020 2020 2020 2020 696e 6465 6e74 203d          indent =
+00005290: 2022 220d 0a20 2020 2020 2020 2066 6f72   ""..        for
+000052a0: 2069 2069 6e20 7261 6e67 6528 696e 6465   i in range(inde
+000052b0: 6e74 5f73 697a 6529 3a0d 0a20 2020 2020  nt_size):..     
+000052c0: 2020 2020 2020 2069 6e64 656e 742b 3d22         indent+="
+000052d0: 2022 0d0a 0d0a 2020 2020 2020 2020 7072   "....        pr
+000052e0: 696e 7428 290d 0a20 2020 2020 2020 2069  int()..        i
+000052f0: 6620 6e61 6d65 2021 3d20 4e6f 6e65 3a0d  f name != None:.
+00005300: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00005310: 6e74 2869 6e64 656e 742b 2220 2020 2020  nt(indent+"     
+00005320: 2020 206e 616d 653a 222c 6e61 6d65 290d     name:",name).
+00005330: 0a20 2020 2020 2020 2070 7269 6e74 2869  .        print(i
+00005340: 6e64 656e 742b 2220 2061 7272 6179 2074  ndent+"  array t
+00005350: 7970 653a 2073 7061 7273 6522 290d 0a20  ype: sparse").. 
+00005360: 2020 2020 2020 2070 7269 6e74 2869 6e64         print(ind
+00005370: 656e 742b 2220 2020 2020 2020 7368 6170  ent+"       shap
+00005380: 653a 222c 7365 6c66 2e73 6861 7065 290d  e:",self.shape).
+00005390: 0a20 2020 2020 2020 2070 7269 6e74 2869  .        print(i
+000053a0: 6e64 656e 742b 2220 2020 2020 6465 6e73  ndent+"     dens
+000053b0: 6974 793a 222c 7365 6c66 2e6e 6e7a 2c22  ity:",self.nnz,"
+000053c0: 2f22 2c73 656c 662e 7369 7a65 2c22 7e22  /",self.size,"~"
+000053d0: 2c73 656c 662e 6e6e 7a2f 7365 6c66 2e73  ,self.nnz/self.s
+000053e0: 697a 652a 3130 302c 2225 2229 0d0a 2020  ize*100,"%")..  
+000053f0: 2020 2020 2020 7072 696e 7428 696e 6465        print(inde
+00005400: 6e74 2b22 2020 2073 7461 7469 7374 6963  nt+"   statistic
+00005410: 3a22 2c73 656c 662e 7374 6174 6973 7469  :",self.statisti
+00005420: 6329 0d0a 2020 2020 2020 2020 7072 696e  c)..        prin
+00005430: 7428 696e 6465 6e74 2b22 2020 2020 2020  t(indent+"      
+00005440: 666f 726d 6174 3a22 2c73 656c 662e 666f  format:",self.fo
+00005450: 726d 6174 290d 0a20 2020 2020 2020 2070  rmat)..        p
+00005460: 7269 6e74 2869 6e64 656e 742b 2220 2020  rint(indent+"   
+00005470: 2020 656e 636f 6465 723a 222c 7365 6c66    encoder:",self
+00005480: 2e65 6e63 6f64 6572 290d 0a20 2020 2020  .encoder)..     
+00005490: 2020 2070 7269 6e74 2869 6e64 656e 742b     print(indent+
+000054a0: 2220 2020 2020 206d 656d 6f72 793a 222c  "      memory:",
+000054b0: 6d65 6d6f 7279 5f64 6973 706c 6179 2873  memory_display(s
+000054c0: 7973 2e67 6574 7369 7a65 6f66 2873 656c  ys.getsizeof(sel
+000054d0: 662e 6461 7461 292b 7379 732e 6765 7473  f.data)+sys.gets
+000054e0: 697a 656f 6628 7365 6c66 2929 290d 0a20  izeof(self))).. 
+000054f0: 2020 2020 2020 2070 7269 6e74 2869 6e64         print(ind
+00005500: 656e 742b 2220 2020 2020 2020 206e 6f72  ent+"        nor
+00005510: 6d3a 222c 7365 6c66 2e6e 6f72 6d29 0d0a  m:",self.norm)..
+00005520: 2020 2020 2020 2020 7072 696e 7428 696e          print(in
+00005530: 6465 6e74 2b22 2020 2020 2065 6e74 7269  dent+"     entri
+00005540: 6573 3a22 290d 0a0d 0a20 2020 2020 2020  es:")....       
+00005550: 2043 203d 2073 656c 662e 636f 6f72 6473   C = self.coords
+00005560: 0d0a 2020 2020 2020 2020 5620 3d20 7365  ..        V = se
+00005570: 6c66 2e76 616c 7565 0d0a 2020 2020 2020  lf.value..      
+00005580: 2020 666f 7220 656c 656d 2069 6e20 7261    for elem in ra
+00005590: 6e67 6528 7365 6c66 2e6e 6e7a 293a 0d0a  nge(self.nnz):..
+000055a0: 2020 2020 2020 2020 2020 2020 6966 286e              if(n
+000055b0: 702e 6162 7328 565b 656c 656d 5d29 3e6e  p.abs(V[elem])>n
+000055c0: 756d 6572 5f64 6973 706c 6179 5f63 7574  umer_display_cut
+000055d0: 6f66 6629 3a0d 0a20 2020 2020 2020 2020  off):..         
+000055e0: 2020 2020 2020 2070 7269 6e74 2869 6e64         print(ind
+000055f0: 656e 742b 225c 7422 2c43 5b65 6c65 6d5d  ent+"\t",C[elem]
+00005600: 2c63 6c65 616e 5f66 6f72 6d61 7428 565b  ,clean_format(V[
+00005610: 656c 656d 5d29 290d 0a20 2020 2020 2020  elem]))..       
+00005620: 2070 7269 6e74 2829 0d0a 0d0a 2020 2020   print()....    
+00005630: 6465 6620 696e 666f 2873 656c 662c 6e61  def info(self,na
+00005640: 6d65 3d4e 6f6e 652c 696e 6465 6e74 5f73  me=None,indent_s
+00005650: 697a 653d 3029 3a0d 0a0d 0a20 2020 2020  ize=0):....     
+00005660: 2020 2069 6e64 656e 7420 3d20 2222 0d0a     indent = ""..
+00005670: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00005680: 2072 616e 6765 2869 6e64 656e 745f 7369   range(indent_si
+00005690: 7a65 293a 0d0a 2020 2020 2020 2020 2020  ze):..          
+000056a0: 2020 696e 6465 6e74 2b3d 2220 220d 0a0d    indent+=" "...
+000056b0: 0a20 2020 2020 2020 2070 7269 6e74 2829  .        print()
+000056c0: 0d0a 2020 2020 2020 2020 6966 206e 616d  ..        if nam
+000056d0: 6520 213d 204e 6f6e 653a 0d0a 2020 2020  e != None:..    
+000056e0: 2020 2020 2020 2020 7072 696e 7428 696e          print(in
+000056f0: 6465 6e74 2b22 2020 2020 2020 2020 6e61  dent+"        na
+00005700: 6d65 3a22 2c6e 616d 6529 0d0a 2020 2020  me:",name)..    
+00005710: 2020 2020 7072 696e 7428 696e 6465 6e74      print(indent
+00005720: 2b22 2020 6172 7261 7920 7479 7065 3a20  +"  array type: 
+00005730: 7370 6172 7365 2229 0d0a 2020 2020 2020  sparse")..      
+00005740: 2020 7072 696e 7428 696e 6465 6e74 2b22    print(indent+"
+00005750: 2020 2020 2020 2073 6861 7065 3a22 2c73         shape:",s
+00005760: 656c 662e 7368 6170 6529 0d0a 2020 2020  elf.shape)..    
+00005770: 2020 2020 7072 696e 7428 696e 6465 6e74      print(indent
+00005780: 2b22 2020 2020 2064 656e 7369 7479 3a22  +"     density:"
+00005790: 2c73 656c 662e 6e6e 7a2c 222f 222c 7365  ,self.nnz,"/",se
+000057a0: 6c66 2e73 697a 652c 227e 222c 7365 6c66  lf.size,"~",self
+000057b0: 2e6e 6e7a 2f73 656c 662e 7369 7a65 2a31  .nnz/self.size*1
+000057c0: 3030 2c22 2522 290d 0a20 2020 2020 2020  00,"%")..       
+000057d0: 2070 7269 6e74 2869 6e64 656e 742b 2220   print(indent+" 
+000057e0: 2020 7374 6174 6973 7469 633a 222c 7365    statistic:",se
+000057f0: 6c66 2e73 7461 7469 7374 6963 290d 0a20  lf.statistic).. 
+00005800: 2020 2020 2020 2070 7269 6e74 2869 6e64         print(ind
+00005810: 656e 742b 2220 2020 2020 2066 6f72 6d61  ent+"      forma
+00005820: 743a 222c 7365 6c66 2e66 6f72 6d61 7429  t:",self.format)
+00005830: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00005840: 696e 6465 6e74 2b22 2020 2020 2065 6e63  indent+"     enc
+00005850: 6f64 6572 3a22 2c73 656c 662e 656e 636f  oder:",self.enco
+00005860: 6465 7229 0d0a 2020 2020 2020 2020 7072  der)..        pr
+00005870: 696e 7428 696e 6465 6e74 2b22 2020 2020  int(indent+"    
+00005880: 2020 6d65 6d6f 7279 3a22 2c6d 656d 6f72    memory:",memor
+00005890: 795f 6469 7370 6c61 7928 7379 732e 6765  y_display(sys.ge
+000058a0: 7473 697a 656f 6628 7365 6c66 2e64 6174  tsizeof(self.dat
+000058b0: 6129 2b73 7973 2e67 6574 7369 7a65 6f66  a)+sys.getsizeof
+000058c0: 2873 656c 6629 2929 0d0a 2020 2020 2020  (self)))..      
+000058d0: 2020 7072 696e 7428 696e 6465 6e74 2b22    print(indent+"
+000058e0: 2020 2020 2020 2020 6e6f 726d 3a22 2c73          norm:",s
+000058f0: 656c 662e 6e6f 726d 290d 0a20 2020 2020  elf.norm)..     
+00005900: 2020 2070 7269 6e74 2829 0d0a 0d0a 2020     print()....  
+00005910: 2020 6465 6620 7365 745f 7661 6c75 6528    def set_value(
+00005920: 7365 6c66 2c65 6e74 7279 2c76 616c 7565  self,entry,value
+00005930: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
+00005940: 2e64 6174 612e 6461 7461 5b65 6e74 7279  .data.data[entry
+00005950: 5d20 3d20 7661 6c75 650d 0a0d 0a20 2020  ] = value....   
+00005960: 2064 6566 2072 656d 6f76 655f 656e 7472   def remove_entr
+00005970: 7928 7365 6c66 2c65 6e74 7279 293a 0d0a  y(self,entry):..
+00005980: 2020 2020 2020 2020 706f 7070 6564 5f63          popped_c
+00005990: 6f6f 7264 7320 3d20 5b5d 0d0a 2020 2020  oords = []..    
+000059a0: 2020 2020 666f 7220 6178 6973 2069 6e20      for axis in 
+000059b0: 7261 6e67 6528 7365 6c66 2e64 6174 612e  range(self.data.
+000059c0: 6e64 696d 293a 0d0a 2020 2020 2020 2020  ndim):..        
+000059d0: 2020 2020 706f 7070 6564 5f63 6f6f 7264      popped_coord
+000059e0: 7320 3d20 706f 7070 6564 5f63 6f6f 7264  s = popped_coord
+000059f0: 7320 2b20 5b6e 702e 6465 6c65 7465 2873  s + [np.delete(s
+00005a00: 656c 662e 6461 7461 2e63 6f6f 7264 735b  elf.data.coords[
+00005a10: 6178 6973 5d2c 656e 7472 7929 5d0d 0a20  axis],entry)].. 
+00005a20: 2020 2020 2020 2070 6f70 7065 645f 636f         popped_co
+00005a30: 6f72 6473 203d 206e 702e 6172 7261 7928  ords = np.array(
+00005a40: 706f 7070 6564 5f63 6f6f 7264 7329 0d0a  popped_coords)..
+00005a50: 2020 2020 2020 2020 706f 7070 6564 5f76          popped_v
+00005a60: 616c 7565 203d 206e 702e 6465 6c65 7465  alue = np.delete
+00005a70: 2873 656c 662e 6461 7461 2e64 6174 612c  (self.data.data,
+00005a80: 656e 7472 7929 0d0a 2020 2020 2020 2020  entry)..        
+00005a90: 0d0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+00005aa0: 6174 612e 636f 6f72 6473 203d 2070 6f70  ata.coords = pop
+00005ab0: 7065 645f 636f 6f72 6473 0d0a 2020 2020  ped_coords..    
+00005ac0: 2020 2020 7365 6c66 2e64 6174 612e 6461      self.data.da
+00005ad0: 7461 203d 2070 6f70 7065 645f 7661 6c75  ta = popped_valu
+00005ae0: 650d 0a0d 0a20 2020 2064 6566 2061 7070  e....    def app
+00005af0: 656e 645f 656e 7472 7928 7365 6c66 2c63  end_entry(self,c
+00005b00: 6f6f 7264 732c 7661 6c75 6529 3a0d 0a20  oords,value):.. 
+00005b10: 2020 2020 2020 2061 7070 656e 6465 645f         appended_
+00005b20: 636f 6f72 6473 203d 205b 5d0d 0a20 2020  coords = []..   
+00005b30: 2020 2020 2066 6f72 2061 7869 7320 696e       for axis in
+00005b40: 2072 616e 6765 2873 656c 662e 6461 7461   range(self.data
+00005b50: 2e6e 6469 6d29 3a0d 0a20 2020 2020 2020  .ndim):..       
+00005b60: 2020 2020 2061 7070 656e 6465 645f 636f       appended_co
+00005b70: 6f72 6473 203d 2061 7070 656e 6465 645f  ords = appended_
+00005b80: 636f 6f72 6473 202b 205b 6e70 2e61 7070  coords + [np.app
+00005b90: 656e 6428 7365 6c66 2e64 6174 612e 636f  end(self.data.co
+00005ba0: 6f72 6473 5b61 7869 735d 2c63 6f6f 7264  ords[axis],coord
+00005bb0: 735b 6178 6973 5d29 5d0d 0a20 2020 2020  s[axis])]..     
+00005bc0: 2020 2061 7070 656e 6465 645f 636f 6f72     appended_coor
+00005bd0: 6473 203d 206e 702e 6172 7261 7928 6170  ds = np.array(ap
+00005be0: 7065 6e64 6564 5f63 6f6f 7264 7329 0d0a  pended_coords)..
+00005bf0: 2020 2020 2020 2020 6170 7065 6e64 6564          appended
+00005c00: 5f76 616c 7565 203d 206e 702e 6170 7065  _value = np.appe
+00005c10: 6e64 2873 656c 662e 6461 7461 2e64 6174  nd(self.data.dat
+00005c20: 612c 7661 6c75 6529 0d0a 2020 2020 2020  a,value)..      
+00005c30: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
+00005c40: 2e64 6174 612e 636f 6f72 6473 203d 2061  .data.coords = a
+00005c50: 7070 656e 6465 645f 636f 6f72 6473 0d0a  ppended_coords..
+00005c60: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
+00005c70: 612e 6461 7461 203d 2061 7070 656e 6465  a.data = appende
+00005c80: 645f 7661 6c75 650d 0a0d 0a20 2020 2064  d_value....    d
+00005c90: 6566 2072 656d 6f76 655f 7a65 726f 7328  ef remove_zeros(
+00005ca0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00005cb0: 7265 7420 3d20 7365 6c66 2e63 6f70 7928  ret = self.copy(
+00005cc0: 290d 0a20 2020 2020 2020 207a 6572 6f5f  )..        zero_
+00005cd0: 656e 7472 795f 6c69 7374 203d 205b 5d0d  entry_list = [].
+00005ce0: 0a20 2020 2020 2020 2066 6f72 2065 6e74  .        for ent
+00005cf0: 7279 2069 6e20 7261 6e67 6528 7265 742e  ry in range(ret.
+00005d00: 6461 7461 2e6e 6e7a 293a 0d0a 2020 2020  data.nnz):..    
+00005d10: 2020 2020 2020 2020 6966 206e 702e 6162          if np.ab
+00005d20: 7328 7265 742e 6461 7461 2e64 6174 615b  s(ret.data.data[
+00005d30: 656e 7472 795d 2920 3c20 6e75 6d65 725f  entry]) < numer_
+00005d40: 6375 746f 6666 3a0d 0a20 2020 2020 2020  cutoff:..       
+00005d50: 2020 2020 2020 2020 207a 6572 6f5f 656e           zero_en
+00005d60: 7472 795f 6c69 7374 203d 207a 6572 6f5f  try_list = zero_
+00005d70: 656e 7472 795f 6c69 7374 202b 205b 656e  entry_list + [en
+00005d80: 7472 795d 0d0a 0d0a 2020 2020 2020 2020  try]....        
+00005d90: 666f 7220 692c 7a65 726f 5f65 6e74 7279  for i,zero_entry
+00005da0: 2069 6e20 656e 756d 6572 6174 6528 7a65   in enumerate(ze
+00005db0: 726f 5f65 6e74 7279 5f6c 6973 7429 3a0d  ro_entry_list):.
+00005dc0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00005dd0: 2e72 656d 6f76 655f 656e 7472 7928 7a65  .remove_entry(ze
+00005de0: 726f 5f65 6e74 7279 2d69 290d 0a20 2020  ro_entry-i)..   
+00005df0: 2020 2020 2072 6574 7572 6e20 7265 740d       return ret.
+00005e00: 0a0d 0a20 2020 2064 6566 2063 6f70 7928  ...    def copy(
+00005e10: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00005e20: 2363 6f70 7920 7370 6172 7365 2070 726f  #copy sparse pro
+00005e30: 7065 7274 6965 730d 0a20 2020 2020 2020  perties..       
+00005e40: 2072 6574 203d 2073 7061 7273 6528 290d   ret = sparse().
+00005e50: 0a20 2020 2020 2020 2072 6574 2e64 6174  .        ret.dat
+00005e60: 6120 3d20 7365 6c66 2e64 6174 612e 636f  a = self.data.co
+00005e70: 7079 2829 0d0a 2020 2020 2020 2020 7265  py()..        re
+00005e80: 742e 7374 6174 6973 7469 6320 3d20 7365  t.statistic = se
+00005e90: 6c66 2e73 7461 7469 7374 6963 0d0a 2020  lf.statistic..  
+00005ea0: 2020 2020 2020 7265 742e 666f 726d 6174        ret.format
+00005eb0: 203d 2073 656c 662e 666f 726d 6174 0d0a   = self.format..
+00005ec0: 2020 2020 2020 2020 7265 742e 656e 636f          ret.enco
+00005ed0: 6465 7220 3d20 7365 6c66 2e65 6e63 6f64  der = self.encod
+00005ee0: 6572 0d0a 2020 2020 2020 2020 7265 7475  er..        retu
+00005ef0: 726e 2072 6574 0d0a 2020 2020 0d0a 2020  rn ret..    ..  
+00005f00: 2020 6465 6620 5f5f 6164 645f 5f28 7365    def __add__(se
+00005f10: 6c66 2c20 6f74 6865 7229 3a0d 0a20 2020  lf, other):..   
+00005f20: 2020 2020 2069 6628 7365 6c66 2e73 6861       if(self.sha
+00005f30: 7065 213d 6f74 6865 722e 7368 6170 650d  pe!=other.shape.
+00005f40: 0a20 2020 2020 2020 2020 2020 206f 7220  .            or 
+00005f50: 7365 6c66 2e73 7461 7469 7374 6963 213d  self.statistic!=
+00005f60: 6f74 6865 722e 7374 6174 6973 7469 630d  other.statistic.
+00005f70: 0a20 2020 2020 2020 2020 2020 2020 6f72  .             or
+00005f80: 2073 656c 662e 666f 726d 6174 213d 6f74   self.format!=ot
+00005f90: 6865 722e 666f 726d 6174 0d0a 2020 2020  her.format..    
+00005fa0: 2020 2020 2020 2020 2020 6f72 2073 656c            or sel
+00005fb0: 662e 656e 636f 6465 7221 3d6f 7468 6572  f.encoder!=other
+00005fc0: 2e65 6e63 6f64 6572 293a 0d0a 2020 2020  .encoder):..    
+00005fd0: 2020 2020 2020 2020 6572 726f 7228 2245          error("E
+00005fe0: 7272 6f72 5b73 7061 7273 652e 2b5d 3a20  rror[sparse.+]: 
+00005ff0: 496e 636f 6e73 6973 7465 6e74 206f 626a  Inconsistent obj
+00006000: 6563 7420 7072 6f70 6572 7469 6573 2229  ect properties")
+00006010: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+00006020: 2020 2020 2020 2020 7265 7420 3d20 7365          ret = se
+00006030: 6c66 2e63 6f70 7928 290d 0a20 2020 2020  lf.copy()..     
+00006040: 2020 2072 6574 2e64 6174 6120 3d20 7265     ret.data = re
+00006050: 742e 6461 7461 2b6f 7468 6572 2e64 6174  t.data+other.dat
+00006060: 610d 0a20 2020 2020 2020 2072 6574 7572  a..        retur
+00006070: 6e20 7265 740d 0a20 2020 2020 2020 200d  n ret..        .
+00006080: 0a20 2020 2064 6566 205f 5f73 7562 5f5f  .    def __sub__
+00006090: 2873 656c 662c 206f 7468 6572 293a 0d0a  (self, other):..
+000060a0: 2020 2020 2020 2020 6966 2873 656c 662e          if(self.
+000060b0: 7368 6170 6521 3d6f 7468 6572 2e73 6861  shape!=other.sha
+000060c0: 7065 0d0a 2020 2020 2020 2020 2020 2020  pe..            
+000060d0: 6f72 2073 656c 662e 7374 6174 6973 7469  or self.statisti
+000060e0: 6321 3d6f 7468 6572 2e73 7461 7469 7374  c!=other.statist
+000060f0: 6963 0d0a 2020 2020 2020 2020 2020 2020  ic..            
+00006100: 206f 7220 7365 6c66 2e66 6f72 6d61 7421   or self.format!
+00006110: 3d6f 7468 6572 2e66 6f72 6d61 740d 0a20  =other.format.. 
+00006120: 2020 2020 2020 2020 2020 2020 206f 7220               or 
+00006130: 7365 6c66 2e65 6e63 6f64 6572 213d 6f74  self.encoder!=ot
+00006140: 6865 722e 656e 636f 6465 7229 3a0d 0a20  her.encoder):.. 
+00006150: 2020 2020 2020 2020 2020 2065 7272 6f72             error
+00006160: 2822 4572 726f 725b 7370 6172 7365 2e2d  ("Error[sparse.-
+00006170: 5d3a 2049 6e63 6f6e 7369 7374 656e 7420  ]: Inconsistent 
+00006180: 6f62 6a65 6374 2070 726f 7065 7274 6965  object propertie
+00006190: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
+000061a0: 200d 0a20 2020 2020 2020 2072 6574 203d   ..        ret =
+000061b0: 2073 656c 662e 636f 7079 2829 0d0a 2020   self.copy()..  
+000061c0: 2020 2020 2020 7265 742e 6461 7461 203d        ret.data =
+000061d0: 2072 6574 2e64 6174 612d 6f74 6865 722e   ret.data-other.
+000061e0: 6461 7461 0d0a 2020 2020 2020 2020 7265  data..        re
+000061f0: 7475 726e 2072 6574 0d0a 2020 2020 2020  turn ret..      
+00006200: 2020 0d0a 2020 2020 6465 6620 5f5f 6d75    ..    def __mu
+00006210: 6c5f 5f28 7365 6c66 2c20 6f74 6865 7229  l__(self, other)
+00006220: 3a0d 0a20 2020 2020 2020 2072 6574 203d  :..        ret =
+00006230: 2073 656c 662e 636f 7079 2829 0d0a 2020   self.copy()..  
+00006240: 2020 2020 2020 7265 742e 6461 7461 203d        ret.data =
+00006250: 2072 6574 2e64 6174 612a 6f74 6865 720d   ret.data*other.
+00006260: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00006270: 7265 740d 0a20 2020 2020 2020 200d 0a20  ret..        .. 
+00006280: 2020 2064 6566 205f 5f72 6d75 6c5f 5f28     def __rmul__(
+00006290: 7365 6c66 2c20 6f74 6865 7229 3a0d 0a20  self, other):.. 
+000062a0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000062b0: 6c66 2a6f 7468 6572 0d0a 2020 2020 2020  lf*other..      
+000062c0: 2020 0d0a 2020 2020 2364 6566 205f 5f6c    ..    #def __l
+000062d0: 656e 5f5f 2873 656c 6629 3a0d 0a20 2020  en__(self):..   
+000062e0: 2023 2020 2020 7265 7475 726e 206c 656e   #    return len
+000062f0: 2873 656c 662e 6461 7461 290d 0a20 2020  (self.data)..   
+00006300: 200d 0a20 2020 2064 6566 205f 5f73 7472   ..    def __str
+00006310: 5f5f 2873 656c 6629 3a0d 0a20 2020 2020  __(self):..     
+00006320: 2020 2072 6574 7572 6e20 7374 7228 7365     return str(se
+00006330: 6c66 2e64 6174 6129 0d0a 2020 2020 0d0a  lf.data)..    ..
+00006340: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
+00006350: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00006360: 2072 6574 7572 6e20 7265 7072 2873 656c   return repr(sel
+00006370: 662e 6461 7461 290d 0a0d 0a20 2020 2064  f.data)....    d
+00006380: 6566 2073 7769 7463 685f 666f 726d 6174  ef switch_format
+00006390: 2873 656c 662c 7361 7665 5f6d 656d 6f72  (self,save_memor
+000063a0: 793d 4661 6c73 6529 3a0d 0a20 2020 2020  y=False):..     
+000063b0: 2020 2072 6574 7572 6e20 7370 6172 7365     return sparse
+000063c0: 2864 656e 7365 2873 656c 6629 2e73 7769  (dense(self).swi
+000063d0: 7463 685f 666f 726d 6174 2873 6176 655f  tch_format(save_
+000063e0: 6d65 6d6f 7279 3d73 6176 655f 6d65 6d6f  memory=save_memo
+000063f0: 7279 2929 0d0a 0d0a 2020 2020 6465 6620  ry))....    def 
+00006400: 7377 6974 6368 5f65 6e63 6f64 6572 2873  switch_encoder(s
+00006410: 656c 662c 7361 7665 5f6d 656d 6f72 793d  elf,save_memory=
+00006420: 4661 6c73 6529 3a0d 0a20 2020 2020 2020  False):..       
+00006430: 2072 6574 7572 6e20 7370 6172 7365 2864   return sparse(d
+00006440: 656e 7365 2873 656c 6629 2e73 7769 7463  ense(self).switc
+00006450: 685f 656e 636f 6465 7228 7361 7665 5f6d  h_encoder(save_m
+00006460: 656d 6f72 793d 7361 7665 5f6d 656d 6f72  emory=save_memor
+00006470: 7929 290d 0a0d 0a20 2020 2064 6566 2066  y))....    def f
+00006480: 6f72 6365 5f65 6e63 6f64 6572 2873 656c  orce_encoder(sel
+00006490: 662c 7461 7267 6574 3d22 6361 6e6f 6e69  f,target="canoni
+000064a0: 6361 6c22 293a 0d0a 2020 2020 2020 2020  cal"):..        
+000064b0: 6966 2074 6172 6765 7420 6e6f 7420 696e  if target not in
+000064c0: 2065 6e63 6f64 6572 5f74 7970 653a 0d0a   encoder_type:..
+000064d0: 2020 2020 2020 2020 2020 2020 6572 726f              erro
+000064e0: 7228 2245 7272 6f72 5b73 7061 7273 652e  r("Error[sparse.
+000064f0: 666f 7263 655f 656e 636f 6465 725d 3a20  force_encoder]: 
+00006500: 556e 7265 636f 676e 697a 6564 2074 6172  Unrecognized tar
+00006510: 6765 7420 656e 636f 6465 722e 2229 0d0a  get encoder.")..
+00006520: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
+00006530: 7420 213d 2073 656c 662e 656e 636f 6465  t != self.encode
+00006540: 7220 3a0d 0a20 2020 2020 2020 2020 2020  r :..           
+00006550: 2072 6574 7572 6e20 7365 6c66 2e73 7769   return self.swi
+00006560: 7463 685f 656e 636f 6465 7228 290d 0a20  tch_encoder().. 
+00006570: 2020 2020 2020 2065 6c73 6520 3a0d 0a20         else :.. 
+00006580: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00006590: 6e20 7365 6c66 2e63 6f70 7928 290d 0a0d  n self.copy()...
+000065a0: 0a20 2020 2064 6566 2066 6f72 6365 5f66  .    def force_f
+000065b0: 6f72 6d61 7428 7365 6c66 2c74 6172 6765  ormat(self,targe
+000065c0: 743d 2273 7461 6e64 6172 6422 293a 0d0a  t="standard"):..
+000065d0: 2020 2020 2020 2020 6966 2074 6172 6765          if targe
+000065e0: 7420 6e6f 7420 696e 2066 6f72 6d61 745f  t not in format_
+000065f0: 7479 7065 3a0d 0a20 2020 2020 2020 2020  type:..         
+00006600: 2020 2065 7272 6f72 2822 4572 726f 725b     error("Error[
+00006610: 7370 6172 7365 2e66 6f72 6365 5f66 6f72  sparse.force_for
+00006620: 6d61 745d 3a20 556e 7265 636f 676e 697a  mat]: Unrecogniz
+00006630: 6564 2074 6172 6765 7420 666f 726d 6174  ed target format
+00006640: 2e22 290d 0a20 2020 2020 2020 2069 6620  .")..        if 
+00006650: 7461 7267 6574 2021 3d20 7365 6c66 2e66  target != self.f
+00006660: 6f72 6d61 7420 3a0d 0a20 2020 2020 2020  ormat :..       
+00006670: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00006680: 2e73 7769 7463 685f 666f 726d 6174 2829  .switch_format()
+00006690: 0d0a 2020 2020 2020 2020 656c 7365 203a  ..        else :
+000066a0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000066b0: 7475 726e 2073 656c 662e 636f 7079 2829  turn self.copy()
+000066c0: 0d0a 0d0a 2020 2020 6465 6620 6a6f 696e  ....    def join
+000066d0: 5f6c 6567 7328 7365 6c66 2c73 7472 696e  _legs(self,strin
+000066e0: 675f 696e 702c 6d61 6b65 5f66 6f72 6d61  g_inp,make_forma
+000066f0: 743d 2773 7461 6e64 6172 6427 2c69 6e74  t='standard',int
+00006700: 6572 6d65 6469 6174 655f 7374 6174 3d28  ermediate_stat=(
+00006710: 2d31 2c31 292c 7361 7665 5f6d 656d 6f72  -1,1),save_memor
+00006720: 793d 4661 6c73 6529 3a0d 0a20 2020 2020  y=False):..     
+00006730: 2020 2072 6574 7572 6e20 6a6f 696e 5f6c     return join_l
+00006740: 6567 7328 7365 6c66 2c73 7472 696e 675f  egs(self,string_
+00006750: 696e 702c 6d61 6b65 5f66 6f72 6d61 742c  inp,make_format,
+00006760: 696e 7465 726d 6564 6961 7465 5f73 7461  intermediate_sta
+00006770: 742c 7361 7665 5f6d 656d 6f72 7929 0d0a  t,save_memory)..
+00006780: 0d0a 2020 2020 6465 6620 7370 6c69 745f  ..    def split_
+00006790: 6c65 6773 2873 656c 662c 7374 7269 6e67  legs(self,string
+000067a0: 5f69 6e70 2c66 696e 616c 5f73 7461 742c  _inp,final_stat,
+000067b0: 6669 6e61 6c5f 7368 6170 652c 696e 7465  final_shape,inte
+000067c0: 726d 6564 6961 7465 5f73 7461 743d 282d  rmediate_stat=(-
+000067d0: 312c 3129 2c73 6176 655f 6d65 6d6f 7279  1,1),save_memory
+000067e0: 3d46 616c 7365 293a 0d0a 2020 2020 2020  =False):..      
+000067f0: 2020 7265 7475 726e 2073 706c 6974 5f6c    return split_l
+00006800: 6567 7328 7365 6c66 2c73 7472 696e 675f  egs(self,string_
+00006810: 696e 702c 6669 6e61 6c5f 7374 6174 2c66  inp,final_stat,f
+00006820: 696e 616c 5f73 6861 7065 2c69 6e74 6572  inal_shape,inter
+00006830: 6d65 6469 6174 655f 7374 6174 2c73 6176  mediate_stat,sav
+00006840: 655f 6d65 6d6f 7279 290d 0a0d 0a20 2020  e_memory)....   
+00006850: 2064 6566 2068 636f 6e6a 7567 6174 6528   def hconjugate(
+00006860: 7365 6c66 2c69 6e70 7574 5f73 7472 696e  self,input_strin
+00006870: 672c 7361 7665 5f6d 656d 6f72 793d 4661  g,save_memory=Fa
+00006880: 6c73 6529 3a0d 0a20 2020 2020 2020 2072  lse):..        r
+00006890: 6574 7572 6e20 6863 6f6e 6a75 6761 7465  eturn hconjugate
+000068a0: 2873 656c 662c 696e 7075 745f 7374 7269  (self,input_stri
+000068b0: 6e67 2c73 6176 655f 6d65 6d6f 7279 290d  ng,save_memory).
+000068c0: 0a0d 0a20 2020 2064 6566 2073 7664 2873  ...    def svd(s
+000068d0: 656c 662c 7374 7269 6e67 5f69 6e70 2c63  elf,string_inp,c
+000068e0: 7574 6f66 663d 4e6f 6e65 2c73 6176 655f  utoff=None,save_
+000068f0: 6d65 6d6f 7279 3d46 616c 7365 293a 0d0a  memory=False):..
+00006900: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00006910: 7664 2873 656c 662c 7374 7269 6e67 5f69  vd(self,string_i
+00006920: 6e70 2c63 7574 6f66 662c 7361 7665 5f6d  np,cutoff,save_m
+00006930: 656d 6f72 7929 0d0a 0d0a 2020 2020 6465  emory)....    de
+00006940: 6620 6569 6728 7365 6c66 2c73 7472 696e  f eig(self,strin
+00006950: 675f 696e 702c 6375 746f 6666 3d4e 6f6e  g_inp,cutoff=Non
+00006960: 652c 6465 6275 675f 6d6f 6465 3d46 616c  e,debug_mode=Fal
+00006970: 7365 2c73 6176 655f 6d65 6d6f 7279 3d46  se,save_memory=F
+00006980: 616c 7365 293a 0d0a 2020 2020 2020 2020  alse):..        
+00006990: 7265 7475 726e 2065 6967 2873 656c 662c  return eig(self,
+000069a0: 7374 7269 6e67 5f69 6e70 2c63 7574 6f66  string_inp,cutof
+000069b0: 662c 6465 6275 675f 6d6f 6465 2c73 6176  f,debug_mode,sav
+000069c0: 655f 6d65 6d6f 7279 290d 0a0d 0a23 2323  e_memory)....###
+000069d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000069e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000069f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006a00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006a10: 2323 2323 2323 2323 2323 2323 0d0a 2323  ############..##
-00006a20: 2020 2020 2020 2050 6172 6974 7920 4361         Parity Ca
-00006a30: 6c63 756c 6174 696f 6e20 2869 6e74 6572  lculation (inter
-00006a40: 6e61 6c20 746f 6f6c 7329 2020 2020 2020  nal tools)      
-00006a50: 2323 0d0a 2323 2323 2323 2323 2323 2323  ##..############
-00006a60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006a70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006a80: 2323 2323 2323 2323 0d0a 0d0a 6465 6620  ########....def 
-00006a90: 6162 736f 6c75 7465 5f70 6172 6974 7928  absolute_parity(
-00006aa0: 7065 726d 7574 6174 696f 6e2c 2069 6e64  permutation, ind
-00006ab0: 6976 6964 7561 6c5f 7061 7269 7479 293a  ividual_parity):
-00006ac0: 0d0a 2020 2020 2222 220d 0a20 2020 2043  ..    """..    C
-00006ad0: 6f6d 7075 7465 2074 6865 2061 6273 6f6c  ompute the absol
-00006ae0: 7574 655f 7061 7269 7479 206f 6620 6120  ute_parity of a 
-00006af0: 7065 726d 7574 6174 696f 6e2c 2061 7373  permutation, ass
-00006b00: 756d 696e 6720 7468 6174 2073 6f6d 6520  uming that some 
-00006b10: 656c 656d 656e 7473 2061 6c77 6179 7320  elements always 
-00006b20: 636f 6d6d 7574 650d 0a20 2020 2077 6974  commute..    wit
-00006b30: 6820 6576 6572 7920 6f74 6865 7220 656c  h every other el
-00006b40: 656d 656e 742e 0d0a 2020 2020 0d0a 2020  ement...    ..  
-00006b50: 2020 5061 7261 6d65 7465 7273 3a0d 0a20    Parameters:.. 
-00006b60: 2020 2070 6572 6d75 7461 7469 6f6e 2028     permutation (
-00006b70: 6c69 7374 5b69 6e74 5d29 3a20 4120 6c69  list[int]): A li
-00006b80: 7374 206f 626a 6563 742e 0d0a 2020 2020  st object...    
-00006b90: 696e 6469 7669 6475 616c 5f70 6172 6974  individual_parit
-00006ba0: 7920 286c 6973 745b 696e 745d 293a 2041  y (list[int]): A
-00006bb0: 206c 6973 7420 6f66 206f 626a 6563 7427   list of object'
-00006bc0: 7320 6772 6173 736d 616e 6e20 7061 7269  s grassmann pari
-00006bd0: 7479 2e0d 0a20 2020 200d 0a20 2020 2052  ty...    ..    R
-00006be0: 6574 7572 6e73 3a0d 0a20 2020 2069 6e74  eturns:..    int
-00006bf0: 3a20 3120 6966 2074 6865 2070 6572 6d75  : 1 if the permu
-00006c00: 7461 7469 6f6e 2069 7320 6576 656e 2c20  tation is even, 
-00006c10: 2d31 2069 6620 7468 6520 7065 726d 7574  -1 if the permut
-00006c20: 6174 696f 6e20 6973 206f 6464 2e0d 0a20  ation is odd... 
-00006c30: 2020 2022 2222 0d0a 2020 2020 0d0a 2020     """..    ..  
-00006c40: 2020 6465 6620 6765 745f 636f 6d6d 7574    def get_commut
-00006c50: 6174 6976 655f 656c 656d 656e 7473 2870  ative_elements(p
-00006c60: 6572 6d75 7461 7469 6f6e 2c20 696e 6469  ermutation, indi
-00006c70: 7669 6475 616c 5f70 6172 6974 7929 3a0d  vidual_parity):.
-00006c80: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00006c90: 2020 2020 2020 5265 7475 726e 2061 2073        Return a s
-00006ca0: 6574 206f 6620 636f 6d6d 7574 696e 6520  et of commutine 
-00006cb0: 656c 656d 656e 7473 2028 696e 6469 7669  elements (indivi
-00006cc0: 6475 616c 5f70 6172 6974 7920 3d20 6576  dual_parity = ev
-00006cd0: 656e 290d 0a20 2020 2020 2020 2022 2222  en)..        """
-00006ce0: 0d0a 2020 2020 2020 2020 6966 286c 656e  ..        if(len
-00006cf0: 2870 6572 6d75 7461 7469 6f6e 2921 3d6c  (permutation)!=l
-00006d00: 656e 2869 6e64 6976 6964 7561 6c5f 7061  en(individual_pa
-00006d10: 7269 7479 2929 3a0d 0a20 2020 2020 2020  rity)):..       
-00006d20: 2020 2020 2065 7272 6f72 2822 4572 726f       error("Erro
-00006d30: 725b 6162 736f 6c75 7465 5f70 6172 6974  r[absolute_parit
-00006d40: 792e 6765 745f 636f 6d6d 7574 6174 6976  y.get_commutativ
-00006d50: 655f 656c 656d 656e 7473 5d3a 2049 6e63  e_elements]: Inc
-00006d60: 6f6e 7369 7374 656e 7420 6172 7261 7920  onsistent array 
-00006d70: 7369 7a65 7321 2229 0d0a 2020 2020 2020  sizes!")..      
-00006d80: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00006d90: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00006da0: 2020 2063 6f6d 6d75 7461 7469 7665 5f65     commutative_e
-00006db0: 6c65 6d65 6e74 7320 3d20 5b78 2066 6f72  lements = [x for
-00006dc0: 2069 2c78 2069 6e20 656e 756d 6572 6174   i,x in enumerat
-00006dd0: 6528 7065 726d 7574 6174 696f 6e29 2069  e(permutation) i
-00006de0: 6620 282d 3129 2a2a 696e 6469 7669 6475  f (-1)**individu
-00006df0: 616c 5f70 6172 6974 795b 695d 3d3d 315d  al_parity[i]==1]
-00006e00: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00006e10: 7475 726e 2073 6574 2863 6f6d 6d75 7461  turn set(commuta
-00006e20: 7469 7665 5f65 6c65 6d65 6e74 7329 0d0a  tive_elements)..
-00006e30: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00006e40: 2020 0d0a 2020 2020 636f 6d6d 7574 6174    ..    commutat
-00006e50: 6976 655f 656c 656d 656e 7473 203d 2067  ive_elements = g
-00006e60: 6574 5f63 6f6d 6d75 7461 7469 7665 5f65  et_commutative_e
-00006e70: 6c65 6d65 6e74 7328 7065 726d 7574 6174  lements(permutat
-00006e80: 696f 6e2c 2069 6e64 6976 6964 7561 6c5f  ion, individual_
-00006e90: 7061 7269 7479 290d 0a20 2020 206e 203d  parity)..    n =
-00006ea0: 206c 656e 2870 6572 6d75 7461 7469 6f6e   len(permutation
-00006eb0: 290d 0a20 2020 206e 6f6e 636f 6d6d 7574  )..    noncommut
-00006ec0: 6174 6976 655f 656c 656d 656e 7473 203d  ative_elements =
-00006ed0: 205b 7820 666f 7220 7820 696e 2070 6572   [x for x in per
-00006ee0: 6d75 7461 7469 6f6e 2069 6620 7820 6e6f  mutation if x no
-00006ef0: 7420 696e 2063 6f6d 6d75 7461 7469 7665  t in commutative
-00006f00: 5f65 6c65 6d65 6e74 735d 0d0a 2020 2020  _elements]..    
-00006f10: 696e 7665 7273 696f 6e73 203d 2030 0d0a  inversions = 0..
-00006f20: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00006f30: 6765 286c 656e 286e 6f6e 636f 6d6d 7574  ge(len(noncommut
-00006f40: 6174 6976 655f 656c 656d 656e 7473 2929  ative_elements))
-00006f50: 3a0d 0a20 2020 2020 2020 2066 6f72 206a  :..        for j
-00006f60: 2069 6e20 7261 6e67 6528 692b 312c 206c   in range(i+1, l
-00006f70: 656e 286e 6f6e 636f 6d6d 7574 6174 6976  en(noncommutativ
-00006f80: 655f 656c 656d 656e 7473 2929 3a0d 0a20  e_elements)):.. 
-00006f90: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00006fa0: 6e63 6f6d 6d75 7461 7469 7665 5f65 6c65  ncommutative_ele
-00006fb0: 6d65 6e74 735b 695d 203e 206e 6f6e 636f  ments[i] > nonco
-00006fc0: 6d6d 7574 6174 6976 655f 656c 656d 656e  mmutative_elemen
-00006fd0: 7473 5b6a 5d3a 0d0a 2020 2020 2020 2020  ts[j]:..        
-00006fe0: 2020 2020 2020 2020 696e 7665 7273 696f          inversio
-00006ff0: 6e73 202b 3d20 310d 0a20 2020 2072 6574  ns += 1..    ret
-00007000: 7572 6e20 282d 3129 2a2a 696e 7665 7273  urn (-1)**invers
-00007010: 696f 6e73 0d0a 0d0a 6465 6620 7265 6c61  ions....def rela
-00007020: 7469 7665 5f70 6172 6974 795f 696e 7428  tive_parity_int(
-00007030: 7065 726d 7574 6174 696f 6e31 2c20 7065  permutation1, pe
-00007040: 726d 7574 6174 696f 6e32 2c20 696e 6469  rmutation2, indi
-00007050: 7669 6475 616c 5f70 6172 6974 7931 293a  vidual_parity1):
-00007060: 0d0a 2020 2020 2222 220d 0a20 2020 2043  ..    """..    C
-00007070: 6f6d 7075 7465 2074 6865 2072 656c 6174  ompute the relat
-00007080: 6976 655f 7061 7269 7479 2066 726f 6d20  ive_parity from 
-00007090: 7065 726d 7574 696e 6720 7065 726d 7574  permuting permut
-000070a0: 6174 696f 6e31 2074 6f20 7065 726d 7574  ation1 to permut
-000070b0: 6174 696f 6e32 2077 6974 6820 7468 6520  ation2 with the 
-000070c0: 696e 6469 7669 6475 616c 2070 6172 6974  individual parit
-000070d0: 7920 6769 7665 6e20 6279 2069 6e64 6976  y given by indiv
-000070e0: 6964 7561 6c5f 7061 7269 7479 3120 6f66  idual_parity1 of
-000070f0: 2074 6865 206c 6973 7420 7065 726d 7574   the list permut
-00007100: 6174 696f 6e31 0d0a 2020 2020 0d0a 2020  ation1..    ..  
-00007110: 2020 5061 7261 6d65 7465 7273 3a0d 0a20    Parameters:.. 
-00007120: 2020 2070 6572 6d75 7461 7469 6f6e 3120     permutation1 
-00007130: 286c 6973 7429 3a20 6669 7273 7420 6c69  (list): first li
-00007140: 7374 0d0a 2020 2020 7065 726d 7574 6174  st..    permutat
-00007150: 696f 6e32 2028 6c69 7374 293a 2074 6172  ion2 (list): tar
-00007160: 6765 7420 6c69 7374 0d0a 2020 2020 696e  get list..    in
-00007170: 6469 7669 6475 616c 5f70 6172 6974 7931  dividual_parity1
-00007180: 2028 6c69 7374 293a 2067 7261 7373 6d61   (list): grassma
-00007190: 6e6e 2070 6172 6974 7920 6f66 2074 6865  nn parity of the
-000071a0: 2066 6972 7374 206c 6973 740d 0a20 2020   first list..   
-000071b0: 200d 0a20 2020 2052 6574 7572 6e73 3a0d   ..    Returns:.
-000071c0: 0a20 2020 2069 6e74 3a20 7265 6c61 7469  .    int: relati
-000071d0: 7665 2070 6172 6974 7920 6f66 2074 6865  ve parity of the
-000071e0: 2070 6572 6d75 7461 7469 6f6e 0d0a 2020   permutation..  
-000071f0: 2020 2222 220d 0a20 2020 200d 0a20 2020    """..    ..   
-00007200: 2064 6566 2070 6572 6d75 7465 5f63 2861   def permute_c(a
-00007210: 2c20 622c 2063 293a 0d0a 2020 2020 2020  , b, c):..      
-00007220: 2020 2222 220d 0a20 2020 2020 2020 2050    """..        P
-00007230: 6572 6d75 7465 2074 6865 2065 6c65 6d65  ermute the eleme
-00007240: 6e74 7320 6f66 2063 2061 6363 6f72 6469  nts of c accordi
-00007250: 6e67 2074 6f20 7468 6520 7065 726d 7574  ng to the permut
-00007260: 6174 696f 6e20 7468 6174 206d 6170 7320  ation that maps 
-00007270: 6120 746f 2062 2e0d 0a20 2020 2020 2020  a to b...       
-00007280: 2022 2222 0d0a 2020 2020 2020 2020 7820   """..        x 
-00007290: 3d20 6c69 7374 286e 702e 6172 6773 6f72  = list(np.argsor
-000072a0: 7428 6129 290d 0a20 2020 2020 2020 2078  t(a))..        x
-000072b0: 6320 3d20 5b20 635b 695d 2066 6f72 2069  c = [ c[i] for i
-000072c0: 2069 6e20 7820 5d0d 0a20 2020 2020 2020   in x ]..       
-000072d0: 2062 7863 203d 205b 2078 635b 695d 2066   bxc = [ xc[i] f
-000072e0: 6f72 2069 2069 6e20 6220 5d0d 0a20 2020  or i in b ]..   
-000072f0: 2020 2020 2072 6574 7572 6e20 6278 630d       return bxc.
-00007300: 0a0d 0a20 2020 2064 6566 2067 6574 5f6e  ...    def get_n
-00007310: 6f6e 636f 6d6d 7574 6174 6976 655f 656c  oncommutative_el
-00007320: 656d 656e 7473 2870 6572 6d75 7461 7469  ements(permutati
-00007330: 6f6e 2c20 696e 6469 7669 6475 616c 5f70  on, individual_p
-00007340: 6172 6974 7929 3a0d 0a20 2020 2020 2020  arity):..       
-00007350: 2022 2222 0d0a 2020 2020 2020 2020 5265   """..        Re
-00007360: 7475 726e 2061 204c 4953 5420 6f66 2063  turn a LIST of c
-00007370: 6f6d 6d75 7469 6e65 2065 6c65 6d65 6e74  ommutine element
-00007380: 7320 2869 6e64 6976 6964 7561 6c5f 7061  s (individual_pa
-00007390: 7269 7479 203d 2065 7665 6e29 0d0a 2020  rity = even)..  
-000073a0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-000073b0: 2020 2069 6628 6c65 6e28 7065 726d 7574     if(len(permut
-000073c0: 6174 696f 6e29 213d 6c65 6e28 696e 6469  ation)!=len(indi
-000073d0: 7669 6475 616c 5f70 6172 6974 7929 293a  vidual_parity)):
-000073e0: 0d0a 2020 2020 2020 2020 2020 2020 6572  ..            er
-000073f0: 726f 7228 2245 7272 6f72 5b72 656c 6174  ror("Error[relat
-00007400: 6976 655f 7061 7269 7479 5f69 6e74 2e67  ive_parity_int.g
-00007410: 6574 5f6e 6f6e 636f 6d6d 7574 6174 6976  et_noncommutativ
-00007420: 655f 656c 656d 656e 7473 5d3a 2049 6e63  e_elements]: Inc
-00007430: 6f6e 7369 7374 656e 7420 6172 7261 7920  onsistent array 
-00007440: 7369 7a65 7321 2229 0d0a 2020 2020 2020  sizes!")..      
-00007450: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00007460: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00007470: 2020 206e 6f6e 636f 6d6d 7574 6174 6976     noncommutativ
-00007480: 655f 656c 656d 656e 7473 203d 205b 7820  e_elements = [x 
-00007490: 666f 7220 692c 7820 696e 2065 6e75 6d65  for i,x in enume
-000074a0: 7261 7465 2870 6572 6d75 7461 7469 6f6e  rate(permutation
-000074b0: 2920 6966 2028 2d31 292a 2a69 6e64 6976  ) if (-1)**indiv
-000074c0: 6964 7561 6c5f 7061 7269 7479 5b69 5d3d  idual_parity[i]=
-000074d0: 3d2d 315d 0d0a 2020 2020 2020 2020 2020  =-1]..          
-000074e0: 2020 7265 7475 726e 206e 6f6e 636f 6d6d    return noncomm
-000074f0: 7574 6174 6976 655f 656c 656d 656e 7473  utative_elements
-00007500: 0d0a 0d0a 2020 2020 696e 6469 7669 6475  ....    individu
-00007510: 616c 5f70 6172 6974 7932 203d 2070 6572  al_parity2 = per
-00007520: 6d75 7465 5f63 2870 6572 6d75 7461 7469  mute_c(permutati
-00007530: 6f6e 312c 2070 6572 6d75 7461 7469 6f6e  on1, permutation
-00007540: 322c 2069 6e64 6976 6964 7561 6c5f 7061  2, individual_pa
-00007550: 7269 7479 3129 0d0a 2020 2020 0d0a 2020  rity1)..    ..  
-00007560: 2020 6e6f 6e63 6f6d 6d75 7461 7469 7665    noncommutative
-00007570: 5f65 6c65 6d65 6e74 7331 203d 2067 6574  _elements1 = get
-00007580: 5f6e 6f6e 636f 6d6d 7574 6174 6976 655f  _noncommutative_
-00007590: 656c 656d 656e 7473 2870 6572 6d75 7461  elements(permuta
-000075a0: 7469 6f6e 312c 696e 6469 7669 6475 616c  tion1,individual
-000075b0: 5f70 6172 6974 7931 290d 0a20 2020 206e  _parity1)..    n
-000075c0: 6f6e 636f 6d6d 7574 6174 6976 655f 656c  oncommutative_el
-000075d0: 656d 656e 7473 3220 3d20 6765 745f 6e6f  ements2 = get_no
-000075e0: 6e63 6f6d 6d75 7461 7469 7665 5f65 6c65  ncommutative_ele
-000075f0: 6d65 6e74 7328 7065 726d 7574 6174 696f  ments(permutatio
-00007600: 6e32 2c69 6e64 6976 6964 7561 6c5f 7061  n2,individual_pa
-00007610: 7269 7479 3229 0d0a 2020 2020 0d0a 2020  rity2)..    ..  
-00007620: 2020 6966 2873 6f72 7465 6428 6e6f 6e63    if(sorted(nonc
-00007630: 6f6d 6d75 7461 7469 7665 5f65 6c65 6d65  ommutative_eleme
-00007640: 6e74 7331 2920 213d 2073 6f72 7465 6428  nts1) != sorted(
-00007650: 6e6f 6e63 6f6d 6d75 7461 7469 7665 5f65  noncommutative_e
-00007660: 6c65 6d65 6e74 7332 2929 3a0d 0a20 2020  lements2)):..   
-00007670: 2020 2020 2065 7272 6f72 2822 4572 726f       error("Erro
-00007680: 725b 7265 6c61 7469 7665 5f70 6172 6974  r[relative_parit
-00007690: 795f 696e 745d 3a20 496e 636f 6e73 6973  y_int]: Inconsis
-000076a0: 7465 6e74 2067 7261 7373 6d61 6e6e 2d6f  tent grassmann-o
-000076b0: 6464 2069 6e64 6963 6573 2122 290d 0a20  dd indices!").. 
-000076c0: 2020 2020 2020 200d 0a20 2020 200d 0a20         ..    .. 
-000076d0: 2020 2061 6273 6f6c 7574 655f 7061 7269     absolute_pari
-000076e0: 7479 3120 3d20 6162 736f 6c75 7465 5f70  ty1 = absolute_p
-000076f0: 6172 6974 7928 7065 726d 7574 6174 696f  arity(permutatio
-00007700: 6e31 2c20 696e 6469 7669 6475 616c 5f70  n1, individual_p
-00007710: 6172 6974 7931 290d 0a20 2020 2061 6273  arity1)..    abs
-00007720: 6f6c 7574 655f 7061 7269 7479 3220 3d20  olute_parity2 = 
-00007730: 6162 736f 6c75 7465 5f70 6172 6974 7928  absolute_parity(
-00007740: 7065 726d 7574 6174 696f 6e32 2c20 696e  permutation2, in
-00007750: 6469 7669 6475 616c 5f70 6172 6974 7932  dividual_parity2
-00007760: 290d 0a20 2020 2072 6574 7572 6e20 6162  )..    return ab
-00007770: 736f 6c75 7465 5f70 6172 6974 7931 2a61  solute_parity1*a
-00007780: 6273 6f6c 7574 655f 7061 7269 7479 320d  bsolute_parity2.
-00007790: 0a20 2020 200d 0a64 6566 2072 656c 6174  .    ..def relat
-000077a0: 6976 655f 7061 7269 7479 5f73 696e 676c  ive_parity_singl
-000077b0: 655f 696e 7075 7428 7374 7269 6e67 2c20  e_input(string, 
-000077c0: 696e 6469 7669 6475 616c 5f70 6172 6974  individual_parit
-000077d0: 7931 293a 0d0a 2020 2020 2222 220d 0a20  y1):..    """.. 
-000077e0: 2020 2074 6865 2073 7472 696e 6720 7665     the string ve
-000077f0: 7273 696f 6e20 6f66 2072 656c 6174 6976  rsion of relativ
-00007800: 655f 7061 7269 7479 5f69 6e74 0d0a 2020  e_parity_int..  
-00007810: 2020 7468 6520 7369 676e 2066 6163 746f    the sign facto
-00007820: 7220 7665 7273 696f 6e20 6f66 2073 696e  r version of sin
-00007830: 676c 6520 696e 7075 7420 6569 6e73 756d  gle input einsum
-00007840: 0d0a 2020 2020 2222 220d 0a20 2020 205b  ..    """..    [
-00007850: 7374 7269 6e67 312c 7374 7269 6e67 325d  string1,string2]
-00007860: 203d 206c 6973 7428 7374 7269 6e67 2e73   = list(string.s
-00007870: 706c 6974 2822 2d3e 2229 290d 0a20 2020  plit("->"))..   
-00007880: 2075 6e69 7175 655f 6368 6172 7320 3d20   unique_chars = 
-00007890: 6c69 7374 2873 6574 2873 7472 696e 6731  list(set(string1
-000078a0: 2b73 7472 696e 6732 2929 0d0a 2020 2020  +string2))..    
-000078b0: 6368 6172 5f74 6f5f 696e 7420 3d20 7b63  char_to_int = {c
-000078c0: 6861 723a 2069 2066 6f72 2069 2c20 6368  har: i for i, ch
-000078d0: 6172 2069 6e20 656e 756d 6572 6174 6528  ar in enumerate(
-000078e0: 756e 6971 7565 5f63 6861 7273 297d 0d0a  unique_chars)}..
-000078f0: 2020 2020 7065 726d 7574 6174 696f 6e31      permutation1
-00007900: 203d 205b 6368 6172 5f74 6f5f 696e 745b   = [char_to_int[
-00007910: 6368 6172 5d20 666f 7220 6368 6172 2069  char] for char i
-00007920: 6e20 7374 7269 6e67 315d 0d0a 2020 2020  n string1]..    
-00007930: 7065 726d 7574 6174 696f 6e32 203d 205b  permutation2 = [
-00007940: 6368 6172 5f74 6f5f 696e 745b 6368 6172  char_to_int[char
-00007950: 5d20 666f 7220 6368 6172 2069 6e20 7374  ] for char in st
-00007960: 7269 6e67 325d 0d0a 2020 2020 7265 7475  ring2]..    retu
-00007970: 726e 2072 656c 6174 6976 655f 7061 7269  rn relative_pari
-00007980: 7479 5f69 6e74 2870 6572 6d75 7461 7469  ty_int(permutati
-00007990: 6f6e 312c 2070 6572 6d75 7461 7469 6f6e  on1, permutation
-000079a0: 322c 2069 6e64 6976 6964 7561 6c5f 7061  2, individual_pa
-000079b0: 7269 7479 3129 0d0a 0d0a 6465 6620 7265  rity1)....def re
-000079c0: 6c61 7469 7665 5f70 6172 6974 7928 7374  lative_parity(st
-000079d0: 7269 6e67 2c20 696e 6469 7669 6475 616c  ring, individual
-000079e0: 5f70 6172 6974 7929 3a0d 0a20 2020 2022  _parity):..    "
-000079f0: 2222 0d0a 2020 2020 496d 6167 696e 6520  ""..    Imagine 
-00007a00: 646f 696e 6720 4772 6173 736d 616e 6e20  doing Grassmann 
-00007a10: 7665 7273 696f 6e20 6f66 2045 696e 7375  version of Einsu
-00007a20: 6d2e 0d0a 2020 2020 5468 6973 2066 756e  m...    This fun
-00007a30: 6374 696f 6e20 7265 7475 726e 7320 7468  ction returns th
-00007a40: 6520 7369 676e 2066 6163 746f 7220 6f66  e sign factor of
-00007a50: 2074 6861 7420 7375 6d2e 0d0a 2020 2020   that sum...    
-00007a60: 596f 7520 6861 7665 2074 6f20 656e 7465  You have to ente
-00007a70: 7220 7468 6520 7061 7269 7479 206f 6620  r the parity of 
-00007a80: 7468 6520 696e 7075 7420 696e 6469 6365  the input indice
-00007a90: 7320 696e 205b 696e 6469 7669 6475 616c  s in [individual
-00007aa0: 5f70 6172 6974 795d 0d0a 2020 2020 5468  _parity]..    Th
-00007ab0: 6520 6772 6173 736d 616e 6e20 696e 6469  e grassmann indi
-00007ac0: 6365 7320 6d75 7374 206e 6f74 2062 6520  ces must not be 
-00007ad0: 6164 6465 6420 6f72 2072 656d 6f76 6564  added or removed
-00007ae0: 210d 0a20 2020 2055 7365 2061 2064 6966  !..    Use a dif
-00007af0: 6665 7265 6e74 2066 756e 6374 696f 6e20  ferent function 
-00007b00: 746f 2069 6e74 6567 7261 7465 2074 6865  to integrate the
-00007b10: 6d20 6f75 7421 0d0a 2020 2020 4578 616d  m out!..    Exam
-00007b20: 706c 6573 3a0d 0a20 2020 203e 3e20 7265  ples:..    >> re
-00007b30: 6c61 7469 7665 5f70 6172 6974 7928 2022  lative_parity( "
-00007b40: 6162 4364 452c 6158 6459 622d 3e58 4345  abCdE,aXdYb->XCE
-00007b50: 5922 2c20 5b30 2c30 2c31 2c30 2c31 2c30  Y", [0,0,1,0,1,0
-00007b60: 2c31 2c30 2c31 2c30 5d20 290d 0a20 2020  ,1,0,1,0] )..   
-00007b70: 203e 3e20 310d 0a20 2020 200d 0a20 2020   >> 1..    ..   
-00007b80: 203e 3e20 7265 6c61 7469 7665 5f70 6172   >> relative_par
-00007b90: 6974 7928 2022 6162 4364 452c 6158 5962  ity( "abCdE,aXYb
-00007ba0: 2d3e 4358 4559 222c 205b 302c 302c 312c  ->CXEY", [0,0,1,
-00007bb0: 302c 312c 302c 312c 312c 305d 2029 0d0a  0,1,0,1,1,0] )..
-00007bc0: 2020 2020 3e3e 202d 310d 0a20 2020 200d      >> -1..    .
-00007bd0: 0a20 2020 2022 2222 0d0a 2020 2020 5b73  .    """..    [s
-00007be0: 7472 696e 675f 696e 7075 742c 7374 7269  tring_input,stri
-00007bf0: 6e67 5f6f 7574 7075 745d 203d 206c 6973  ng_output] = lis
-00007c00: 7428 7374 7269 6e67 2e73 706c 6974 2822  t(string.split("
-00007c10: 2d3e 2229 290d 0a20 2020 2073 7472 696e  ->"))..    strin
-00007c20: 675f 6c69 7374 203d 206c 6973 7428 7374  g_list = list(st
-00007c30: 7269 6e67 5f69 6e70 7574 2e73 706c 6974  ring_input.split
-00007c40: 2822 2c22 2929 0d0a 2020 2020 0d0a 2020  (","))..    ..  
-00007c50: 2020 6a6f 696e 5f73 7472 696e 6720 3d20    join_string = 
-00007c60: 2222 0d0a 2020 2020 666f 7220 6920 696e  ""..    for i in
-00007c70: 2072 616e 6765 286c 656e 2873 7472 696e   range(len(strin
-00007c80: 675f 6c69 7374 2929 3a0d 0a20 2020 2020  g_list)):..     
-00007c90: 2020 206a 6f69 6e5f 7374 7269 6e67 203d     join_string =
-00007ca0: 206a 6f69 6e5f 7374 7269 6e67 202b 2073   join_string + s
-00007cb0: 7472 696e 675f 6c69 7374 5b69 5d0d 0a20  tring_list[i].. 
-00007cc0: 2020 2020 2020 200d 0a20 2020 2069 6628         ..    if(
-00007cd0: 6c65 6e28 6a6f 696e 5f73 7472 696e 6729  len(join_string)
-00007ce0: 213d 6c65 6e28 696e 6469 7669 6475 616c  !=len(individual
-00007cf0: 5f70 6172 6974 7929 293a 0d0a 2020 2020  _parity)):..    
-00007d00: 2020 2020 6572 726f 7228 2245 7272 6f72      error("Error
-00007d10: 5b72 656c 6174 6976 655f 7061 7269 7479  [relative_parity
-00007d20: 5d3a 2054 6865 206e 756d 6265 7220 6f66  ]: The number of
-00007d30: 2069 6e70 7574 206c 6973 7420 616e 6420   input list and 
-00007d40: 7061 7269 7479 206c 6973 7420 6172 6520  parity list are 
-00007d50: 6e6f 7420 636f 6e73 6973 7465 6e74 2122  not consistent!"
-00007d60: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-00007d70: 2020 2020 200d 0a20 2020 2023 7265 6d6f       ..    #remo
-00007d80: 7665 2074 6865 2073 756d 6d65 6420 696e  ve the summed in
-00007d90: 6469 6365 730d 0a20 2020 2064 6566 2072  dices..    def r
-00007da0: 656d 6f76 655f 6475 706c 6963 6174 6573  emove_duplicates
-00007db0: 286c 6973 7431 2c20 6c69 7374 3229 3a0d  (list1, list2):.
-00007dc0: 0a20 2020 2020 2020 206e 6577 5f6c 6973  .        new_lis
-00007dd0: 7431 203d 205b 5d0d 0a20 2020 2020 2020  t1 = []..       
-00007de0: 206e 6577 5f6c 6973 7432 203d 205b 5d0d   new_list2 = [].
-00007df0: 0a20 2020 2020 2020 2066 6f72 2069 2c20  .        for i, 
-00007e00: 7661 6c20 696e 2065 6e75 6d65 7261 7465  val in enumerate
-00007e10: 286c 6973 7431 293a 0d0a 2020 2020 2020  (list1):..      
-00007e20: 2020 2020 2020 6966 206c 6973 7431 2e63        if list1.c
-00007e30: 6f75 6e74 2876 616c 293d 3d31 203a 0d0a  ount(val)==1 :..
-00007e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e50: 6e65 775f 6c69 7374 312e 6170 7065 6e64  new_list1.append
-00007e60: 2876 616c 290d 0a20 2020 2020 2020 2020  (val)..         
-00007e70: 2020 2020 2020 206e 6577 5f6c 6973 7432         new_list2
-00007e80: 2e61 7070 656e 6428 6c69 7374 325b 695d  .append(list2[i]
-00007e90: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00007ea0: 6e20 6e65 775f 6c69 7374 312c 206e 6577  n new_list1, new
-00007eb0: 5f6c 6973 7432 0d0a 2020 2020 2020 2020  _list2..        
-00007ec0: 0d0a 2020 2020 6a6f 696e 5f73 7472 696e  ..    join_strin
-00007ed0: 675f 6c69 7374 2c69 6e64 6976 6964 7561  g_list,individua
-00007ee0: 6c5f 7061 7269 7479 203d 2072 656d 6f76  l_parity = remov
-00007ef0: 655f 6475 706c 6963 6174 6573 286c 6973  e_duplicates(lis
-00007f00: 7428 6a6f 696e 5f73 7472 696e 6729 2c20  t(join_string), 
-00007f10: 696e 6469 7669 6475 616c 5f70 6172 6974  individual_parit
-00007f20: 7929 0d0a 2020 2020 6a6f 696e 5f73 7472  y)..    join_str
-00007f30: 696e 6720 3d20 2727 2e6a 6f69 6e28 6a6f  ing = ''.join(jo
-00007f40: 696e 5f73 7472 696e 675f 6c69 7374 292b  in_string_list)+
-00007f50: 222d 3e22 2b73 7472 696e 675f 6f75 7470  "->"+string_outp
-00007f60: 7574 0d0a 2020 2020 7265 7475 726e 2072  ut..    return r
-00007f70: 656c 6174 6976 655f 7061 7269 7479 5f73  elative_parity_s
-00007f80: 696e 676c 655f 696e 7075 7428 6a6f 696e  ingle_input(join
-00007f90: 5f73 7472 696e 672c 2069 6e64 6976 6964  _string, individ
-00007fa0: 7561 6c5f 7061 7269 7479 290d 0a0d 0a64  ual_parity)....d
-00007fb0: 6566 2072 656f 7264 6572 696e 6728 7374  ef reordering(st
-00007fc0: 7269 6e67 612c 7374 7269 6e67 622c 6d79  ringa,stringb,my
-00007fd0: 6c69 7374 293a 0d0a 0d0a 2020 2020 7243  list):....    rC
-00007fe0: 203d 205b 5d0d 0a20 2020 2066 6f72 2062   = []..    for b
-00007ff0: 2069 6e20 7374 7269 6e67 623a 0d0a 2020   in stringb:..  
-00008000: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00008010: 2320 6c6f 6361 7465 2074 6865 206c 6f63  # locate the loc
-00008020: 6174 696f 6e20 6f66 2062 2069 6e20 7468  ation of b in th
-00008030: 6520 6f72 6967 696e 616c 2073 7472 696e  e original strin
-00008040: 670d 0a20 2020 2020 2020 2069 6e64 6578  g..        index
-00008050: 203d 2073 7472 696e 6761 2e69 6e64 6578   = stringa.index
-00008060: 2862 290d 0a0d 0a20 2020 2020 2020 2023  (b)....        #
-00008070: 2061 6464 206d 796c 6973 7427 7320 656c   add mylist's el
-00008080: 656d 656e 7420 6174 2074 6869 7320 696e  ement at this in
-00008090: 6465 7820 746f 2074 6865 206c 6973 740d  dex to the list.
-000080a0: 0a20 2020 2020 2020 2072 4320 2b3d 205b  .        rC += [
-000080b0: 6d79 6c69 7374 5b69 6e64 6578 5d5d 0d0a  mylist[index]]..
-000080c0: 0d0a 2020 2020 7265 7475 726e 2072 430d  ..    return rC.
-000080d0: 0a0d 0a23 2323 2323 2323 2323 2323 2323  ...#############
-000080e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000080f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008100: 2323 2323 2323 230d 0a23 2320 2020 2020  #######..##     
+00006a00: 230d 0a23 2320 2020 2020 2020 5061 7269  #..##       Pari
+00006a10: 7479 2043 616c 6375 6c61 7469 6f6e 2028  ty Calculation (
+00006a20: 696e 7465 726e 616c 2074 6f6f 6c73 2920  internal tools) 
+00006a30: 2020 2020 2023 230d 0a23 2323 2323 2323       ##..#######
+00006a40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006a60: 2323 2323 2323 2323 2323 2323 230d 0a0d  #############...
+00006a70: 0a64 6566 2061 6273 6f6c 7574 655f 7061  .def absolute_pa
+00006a80: 7269 7479 2870 6572 6d75 7461 7469 6f6e  rity(permutation
+00006a90: 2c20 696e 6469 7669 6475 616c 5f70 6172  , individual_par
+00006aa0: 6974 7929 3a0d 0a20 2020 2022 2222 0d0a  ity):..    """..
+00006ab0: 2020 2020 436f 6d70 7574 6520 7468 6520      Compute the 
+00006ac0: 6162 736f 6c75 7465 5f70 6172 6974 7920  absolute_parity 
+00006ad0: 6f66 2061 2070 6572 6d75 7461 7469 6f6e  of a permutation
+00006ae0: 2c20 6173 7375 6d69 6e67 2074 6861 7420  , assuming that 
+00006af0: 736f 6d65 2065 6c65 6d65 6e74 7320 616c  some elements al
+00006b00: 7761 7973 2063 6f6d 6d75 7465 0d0a 2020  ways commute..  
+00006b10: 2020 7769 7468 2065 7665 7279 206f 7468    with every oth
+00006b20: 6572 2065 6c65 6d65 6e74 2e0d 0a20 2020  er element...   
+00006b30: 200d 0a20 2020 2050 6172 616d 6574 6572   ..    Parameter
+00006b40: 733a 0d0a 2020 2020 7065 726d 7574 6174  s:..    permutat
+00006b50: 696f 6e20 286c 6973 745b 696e 745d 293a  ion (list[int]):
+00006b60: 2041 206c 6973 7420 6f62 6a65 6374 2e0d   A list object..
+00006b70: 0a20 2020 2069 6e64 6976 6964 7561 6c5f  .    individual_
+00006b80: 7061 7269 7479 2028 6c69 7374 5b69 6e74  parity (list[int
+00006b90: 5d29 3a20 4120 6c69 7374 206f 6620 6f62  ]): A list of ob
+00006ba0: 6a65 6374 2773 2067 7261 7373 6d61 6e6e  ject's grassmann
+00006bb0: 2070 6172 6974 792e 0d0a 2020 2020 0d0a   parity...    ..
+00006bc0: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
+00006bd0: 2020 696e 743a 2031 2069 6620 7468 6520    int: 1 if the 
+00006be0: 7065 726d 7574 6174 696f 6e20 6973 2065  permutation is e
+00006bf0: 7665 6e2c 202d 3120 6966 2074 6865 2070  ven, -1 if the p
+00006c00: 6572 6d75 7461 7469 6f6e 2069 7320 6f64  ermutation is od
+00006c10: 642e 0d0a 2020 2020 2222 220d 0a20 2020  d...    """..   
+00006c20: 200d 0a20 2020 2064 6566 2067 6574 5f63   ..    def get_c
+00006c30: 6f6d 6d75 7461 7469 7665 5f65 6c65 6d65  ommutative_eleme
+00006c40: 6e74 7328 7065 726d 7574 6174 696f 6e2c  nts(permutation,
+00006c50: 2069 6e64 6976 6964 7561 6c5f 7061 7269   individual_pari
+00006c60: 7479 293a 0d0a 2020 2020 2020 2020 2222  ty):..        ""
+00006c70: 220d 0a20 2020 2020 2020 2052 6574 7572  "..        Retur
+00006c80: 6e20 6120 7365 7420 6f66 2063 6f6d 6d75  n a set of commu
+00006c90: 7469 6e65 2065 6c65 6d65 6e74 7320 2869  tine elements (i
+00006ca0: 6e64 6976 6964 7561 6c5f 7061 7269 7479  ndividual_parity
+00006cb0: 203d 2065 7665 6e29 0d0a 2020 2020 2020   = even)..      
+00006cc0: 2020 2222 220d 0a20 2020 2020 2020 2069    """..        i
+00006cd0: 6628 6c65 6e28 7065 726d 7574 6174 696f  f(len(permutatio
+00006ce0: 6e29 213d 6c65 6e28 696e 6469 7669 6475  n)!=len(individu
+00006cf0: 616c 5f70 6172 6974 7929 293a 0d0a 2020  al_parity)):..  
+00006d00: 2020 2020 2020 2020 2020 6572 726f 7228            error(
+00006d10: 2245 7272 6f72 5b61 6273 6f6c 7574 655f  "Error[absolute_
+00006d20: 7061 7269 7479 2e67 6574 5f63 6f6d 6d75  parity.get_commu
+00006d30: 7461 7469 7665 5f65 6c65 6d65 6e74 735d  tative_elements]
+00006d40: 3a20 496e 636f 6e73 6973 7465 6e74 2061  : Inconsistent a
+00006d50: 7272 6179 2073 697a 6573 2122 290d 0a20  rray sizes!").. 
+00006d60: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00006d70: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00006d80: 2020 2020 2020 2020 636f 6d6d 7574 6174          commutat
+00006d90: 6976 655f 656c 656d 656e 7473 203d 205b  ive_elements = [
+00006da0: 7820 666f 7220 692c 7820 696e 2065 6e75  x for i,x in enu
+00006db0: 6d65 7261 7465 2870 6572 6d75 7461 7469  merate(permutati
+00006dc0: 6f6e 2920 6966 2028 2d31 292a 2a69 6e64  on) if (-1)**ind
+00006dd0: 6976 6964 7561 6c5f 7061 7269 7479 5b69  ividual_parity[i
+00006de0: 5d3d 3d31 5d0d 0a20 2020 2020 2020 2020  ]==1]..         
+00006df0: 2020 2072 6574 7572 6e20 7365 7428 636f     return set(co
+00006e00: 6d6d 7574 6174 6976 655f 656c 656d 656e  mmutative_elemen
+00006e10: 7473 290d 0a20 2020 2020 2020 2020 2020  ts)..           
+00006e20: 200d 0a20 2020 200d 0a20 2020 2063 6f6d   ..    ..    com
+00006e30: 6d75 7461 7469 7665 5f65 6c65 6d65 6e74  mutative_element
+00006e40: 7320 3d20 6765 745f 636f 6d6d 7574 6174  s = get_commutat
+00006e50: 6976 655f 656c 656d 656e 7473 2870 6572  ive_elements(per
+00006e60: 6d75 7461 7469 6f6e 2c20 696e 6469 7669  mutation, indivi
+00006e70: 6475 616c 5f70 6172 6974 7929 0d0a 2020  dual_parity)..  
+00006e80: 2020 6e20 3d20 6c65 6e28 7065 726d 7574    n = len(permut
+00006e90: 6174 696f 6e29 0d0a 2020 2020 6e6f 6e63  ation)..    nonc
+00006ea0: 6f6d 6d75 7461 7469 7665 5f65 6c65 6d65  ommutative_eleme
+00006eb0: 6e74 7320 3d20 5b78 2066 6f72 2078 2069  nts = [x for x i
+00006ec0: 6e20 7065 726d 7574 6174 696f 6e20 6966  n permutation if
+00006ed0: 2078 206e 6f74 2069 6e20 636f 6d6d 7574   x not in commut
+00006ee0: 6174 6976 655f 656c 656d 656e 7473 5d0d  ative_elements].
+00006ef0: 0a20 2020 2069 6e76 6572 7369 6f6e 7320  .    inversions 
+00006f00: 3d20 300d 0a20 2020 2066 6f72 2069 2069  = 0..    for i i
+00006f10: 6e20 7261 6e67 6528 6c65 6e28 6e6f 6e63  n range(len(nonc
+00006f20: 6f6d 6d75 7461 7469 7665 5f65 6c65 6d65  ommutative_eleme
+00006f30: 6e74 7329 293a 0d0a 2020 2020 2020 2020  nts)):..        
+00006f40: 666f 7220 6a20 696e 2072 616e 6765 2869  for j in range(i
+00006f50: 2b31 2c20 6c65 6e28 6e6f 6e63 6f6d 6d75  +1, len(noncommu
+00006f60: 7461 7469 7665 5f65 6c65 6d65 6e74 7329  tative_elements)
+00006f70: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00006f80: 6966 206e 6f6e 636f 6d6d 7574 6174 6976  if noncommutativ
+00006f90: 655f 656c 656d 656e 7473 5b69 5d20 3e20  e_elements[i] > 
+00006fa0: 6e6f 6e63 6f6d 6d75 7461 7469 7665 5f65  noncommutative_e
+00006fb0: 6c65 6d65 6e74 735b 6a5d 3a0d 0a20 2020  lements[j]:..   
+00006fc0: 2020 2020 2020 2020 2020 2020 2069 6e76               inv
+00006fd0: 6572 7369 6f6e 7320 2b3d 2031 0d0a 2020  ersions += 1..  
+00006fe0: 2020 7265 7475 726e 2028 2d31 292a 2a69    return (-1)**i
+00006ff0: 6e76 6572 7369 6f6e 730d 0a0d 0a64 6566  nversions....def
+00007000: 2072 656c 6174 6976 655f 7061 7269 7479   relative_parity
+00007010: 5f69 6e74 2870 6572 6d75 7461 7469 6f6e  _int(permutation
+00007020: 312c 2070 6572 6d75 7461 7469 6f6e 322c  1, permutation2,
+00007030: 2069 6e64 6976 6964 7561 6c5f 7061 7269   individual_pari
+00007040: 7479 3129 3a0d 0a20 2020 2022 2222 0d0a  ty1):..    """..
+00007050: 2020 2020 436f 6d70 7574 6520 7468 6520      Compute the 
+00007060: 7265 6c61 7469 7665 5f70 6172 6974 7920  relative_parity 
+00007070: 6672 6f6d 2070 6572 6d75 7469 6e67 2070  from permuting p
+00007080: 6572 6d75 7461 7469 6f6e 3120 746f 2070  ermutation1 to p
+00007090: 6572 6d75 7461 7469 6f6e 3220 7769 7468  ermutation2 with
+000070a0: 2074 6865 2069 6e64 6976 6964 7561 6c20   the individual 
+000070b0: 7061 7269 7479 2067 6976 656e 2062 7920  parity given by 
+000070c0: 696e 6469 7669 6475 616c 5f70 6172 6974  individual_parit
+000070d0: 7931 206f 6620 7468 6520 6c69 7374 2070  y1 of the list p
+000070e0: 6572 6d75 7461 7469 6f6e 310d 0a20 2020  ermutation1..   
+000070f0: 200d 0a20 2020 2050 6172 616d 6574 6572   ..    Parameter
+00007100: 733a 0d0a 2020 2020 7065 726d 7574 6174  s:..    permutat
+00007110: 696f 6e31 2028 6c69 7374 293a 2066 6972  ion1 (list): fir
+00007120: 7374 206c 6973 740d 0a20 2020 2070 6572  st list..    per
+00007130: 6d75 7461 7469 6f6e 3220 286c 6973 7429  mutation2 (list)
+00007140: 3a20 7461 7267 6574 206c 6973 740d 0a20  : target list.. 
+00007150: 2020 2069 6e64 6976 6964 7561 6c5f 7061     individual_pa
+00007160: 7269 7479 3120 286c 6973 7429 3a20 6772  rity1 (list): gr
+00007170: 6173 736d 616e 6e20 7061 7269 7479 206f  assmann parity o
+00007180: 6620 7468 6520 6669 7273 7420 6c69 7374  f the first list
+00007190: 0d0a 2020 2020 0d0a 2020 2020 5265 7475  ..    ..    Retu
+000071a0: 726e 733a 0d0a 2020 2020 696e 743a 2072  rns:..    int: r
+000071b0: 656c 6174 6976 6520 7061 7269 7479 206f  elative parity o
+000071c0: 6620 7468 6520 7065 726d 7574 6174 696f  f the permutatio
+000071d0: 6e0d 0a20 2020 2022 2222 0d0a 2020 2020  n..    """..    
+000071e0: 0d0a 2020 2020 6465 6620 7065 726d 7574  ..    def permut
+000071f0: 655f 6328 612c 2062 2c20 6329 3a0d 0a20  e_c(a, b, c):.. 
+00007200: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00007210: 2020 2020 5065 726d 7574 6520 7468 6520      Permute the 
+00007220: 656c 656d 656e 7473 206f 6620 6320 6163  elements of c ac
+00007230: 636f 7264 696e 6720 746f 2074 6865 2070  cording to the p
+00007240: 6572 6d75 7461 7469 6f6e 2074 6861 7420  ermutation that 
+00007250: 6d61 7073 2061 2074 6f20 622e 0d0a 2020  maps a to b...  
+00007260: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00007270: 2020 2078 203d 206c 6973 7428 6e70 2e61     x = list(np.a
+00007280: 7267 736f 7274 2861 2929 0d0a 2020 2020  rgsort(a))..    
+00007290: 2020 2020 7863 203d 205b 2063 5b69 5d20      xc = [ c[i] 
+000072a0: 666f 7220 6920 696e 2078 205d 0d0a 2020  for i in x ]..  
+000072b0: 2020 2020 2020 6278 6320 3d20 5b20 7863        bxc = [ xc
+000072c0: 5b69 5d20 666f 7220 6920 696e 2062 205d  [i] for i in b ]
+000072d0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000072e0: 2062 7863 0d0a 0d0a 2020 2020 6465 6620   bxc....    def 
+000072f0: 6765 745f 6e6f 6e63 6f6d 6d75 7461 7469  get_noncommutati
+00007300: 7665 5f65 6c65 6d65 6e74 7328 7065 726d  ve_elements(perm
+00007310: 7574 6174 696f 6e2c 2069 6e64 6976 6964  utation, individ
+00007320: 7561 6c5f 7061 7269 7479 293a 0d0a 2020  ual_parity):..  
+00007330: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00007340: 2020 2052 6574 7572 6e20 6120 4c49 5354     Return a LIST
+00007350: 206f 6620 636f 6d6d 7574 696e 6520 656c   of commutine el
+00007360: 656d 656e 7473 2028 696e 6469 7669 6475  ements (individu
+00007370: 616c 5f70 6172 6974 7920 3d20 6576 656e  al_parity = even
+00007380: 290d 0a20 2020 2020 2020 2022 2222 0d0a  )..        """..
+00007390: 2020 2020 2020 2020 6966 286c 656e 2870          if(len(p
+000073a0: 6572 6d75 7461 7469 6f6e 2921 3d6c 656e  ermutation)!=len
+000073b0: 2869 6e64 6976 6964 7561 6c5f 7061 7269  (individual_pari
+000073c0: 7479 2929 3a0d 0a20 2020 2020 2020 2020  ty)):..         
+000073d0: 2020 2065 7272 6f72 2822 4572 726f 725b     error("Error[
+000073e0: 7265 6c61 7469 7665 5f70 6172 6974 795f  relative_parity_
+000073f0: 696e 742e 6765 745f 6e6f 6e63 6f6d 6d75  int.get_noncommu
+00007400: 7461 7469 7665 5f65 6c65 6d65 6e74 735d  tative_elements]
+00007410: 3a20 496e 636f 6e73 6973 7465 6e74 2061  : Inconsistent a
+00007420: 7272 6179 2073 697a 6573 2122 290d 0a20  rray sizes!").. 
+00007430: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00007440: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00007450: 2020 2020 2020 2020 6e6f 6e63 6f6d 6d75          noncommu
+00007460: 7461 7469 7665 5f65 6c65 6d65 6e74 7320  tative_elements 
+00007470: 3d20 5b78 2066 6f72 2069 2c78 2069 6e20  = [x for i,x in 
+00007480: 656e 756d 6572 6174 6528 7065 726d 7574  enumerate(permut
+00007490: 6174 696f 6e29 2069 6620 282d 3129 2a2a  ation) if (-1)**
+000074a0: 696e 6469 7669 6475 616c 5f70 6172 6974  individual_parit
+000074b0: 795b 695d 3d3d 2d31 5d0d 0a20 2020 2020  y[i]==-1]..     
+000074c0: 2020 2020 2020 2072 6574 7572 6e20 6e6f         return no
+000074d0: 6e63 6f6d 6d75 7461 7469 7665 5f65 6c65  ncommutative_ele
+000074e0: 6d65 6e74 730d 0a0d 0a20 2020 2069 6e64  ments....    ind
+000074f0: 6976 6964 7561 6c5f 7061 7269 7479 3220  ividual_parity2 
+00007500: 3d20 7065 726d 7574 655f 6328 7065 726d  = permute_c(perm
+00007510: 7574 6174 696f 6e31 2c20 7065 726d 7574  utation1, permut
+00007520: 6174 696f 6e32 2c20 696e 6469 7669 6475  ation2, individu
+00007530: 616c 5f70 6172 6974 7931 290d 0a20 2020  al_parity1)..   
+00007540: 200d 0a20 2020 206e 6f6e 636f 6d6d 7574   ..    noncommut
+00007550: 6174 6976 655f 656c 656d 656e 7473 3120  ative_elements1 
+00007560: 3d20 6765 745f 6e6f 6e63 6f6d 6d75 7461  = get_noncommuta
+00007570: 7469 7665 5f65 6c65 6d65 6e74 7328 7065  tive_elements(pe
+00007580: 726d 7574 6174 696f 6e31 2c69 6e64 6976  rmutation1,indiv
+00007590: 6964 7561 6c5f 7061 7269 7479 3129 0d0a  idual_parity1)..
+000075a0: 2020 2020 6e6f 6e63 6f6d 6d75 7461 7469      noncommutati
+000075b0: 7665 5f65 6c65 6d65 6e74 7332 203d 2067  ve_elements2 = g
+000075c0: 6574 5f6e 6f6e 636f 6d6d 7574 6174 6976  et_noncommutativ
+000075d0: 655f 656c 656d 656e 7473 2870 6572 6d75  e_elements(permu
+000075e0: 7461 7469 6f6e 322c 696e 6469 7669 6475  tation2,individu
+000075f0: 616c 5f70 6172 6974 7932 290d 0a20 2020  al_parity2)..   
+00007600: 200d 0a20 2020 2069 6628 736f 7274 6564   ..    if(sorted
+00007610: 286e 6f6e 636f 6d6d 7574 6174 6976 655f  (noncommutative_
+00007620: 656c 656d 656e 7473 3129 2021 3d20 736f  elements1) != so
+00007630: 7274 6564 286e 6f6e 636f 6d6d 7574 6174  rted(noncommutat
+00007640: 6976 655f 656c 656d 656e 7473 3229 293a  ive_elements2)):
+00007650: 0d0a 2020 2020 2020 2020 6572 726f 7228  ..        error(
+00007660: 2245 7272 6f72 5b72 656c 6174 6976 655f  "Error[relative_
+00007670: 7061 7269 7479 5f69 6e74 5d3a 2049 6e63  parity_int]: Inc
+00007680: 6f6e 7369 7374 656e 7420 6772 6173 736d  onsistent grassm
+00007690: 616e 6e2d 6f64 6420 696e 6469 6365 7321  ann-odd indices!
+000076a0: 2229 0d0a 2020 2020 2020 2020 0d0a 2020  ")..        ..  
+000076b0: 2020 0d0a 2020 2020 6162 736f 6c75 7465    ..    absolute
+000076c0: 5f70 6172 6974 7931 203d 2061 6273 6f6c  _parity1 = absol
+000076d0: 7574 655f 7061 7269 7479 2870 6572 6d75  ute_parity(permu
+000076e0: 7461 7469 6f6e 312c 2069 6e64 6976 6964  tation1, individ
+000076f0: 7561 6c5f 7061 7269 7479 3129 0d0a 2020  ual_parity1)..  
+00007700: 2020 6162 736f 6c75 7465 5f70 6172 6974    absolute_parit
+00007710: 7932 203d 2061 6273 6f6c 7574 655f 7061  y2 = absolute_pa
+00007720: 7269 7479 2870 6572 6d75 7461 7469 6f6e  rity(permutation
+00007730: 322c 2069 6e64 6976 6964 7561 6c5f 7061  2, individual_pa
+00007740: 7269 7479 3229 0d0a 2020 2020 7265 7475  rity2)..    retu
+00007750: 726e 2061 6273 6f6c 7574 655f 7061 7269  rn absolute_pari
+00007760: 7479 312a 6162 736f 6c75 7465 5f70 6172  ty1*absolute_par
+00007770: 6974 7932 0d0a 2020 2020 0d0a 6465 6620  ity2..    ..def 
+00007780: 7265 6c61 7469 7665 5f70 6172 6974 795f  relative_parity_
+00007790: 7369 6e67 6c65 5f69 6e70 7574 2873 7472  single_input(str
+000077a0: 696e 672c 2069 6e64 6976 6964 7561 6c5f  ing, individual_
+000077b0: 7061 7269 7479 3129 3a0d 0a20 2020 2022  parity1):..    "
+000077c0: 2222 0d0a 2020 2020 7468 6520 7374 7269  ""..    the stri
+000077d0: 6e67 2076 6572 7369 6f6e 206f 6620 7265  ng version of re
+000077e0: 6c61 7469 7665 5f70 6172 6974 795f 696e  lative_parity_in
+000077f0: 740d 0a20 2020 2074 6865 2073 6967 6e20  t..    the sign 
+00007800: 6661 6374 6f72 2076 6572 7369 6f6e 206f  factor version o
+00007810: 6620 7369 6e67 6c65 2069 6e70 7574 2065  f single input e
+00007820: 696e 7375 6d0d 0a20 2020 2022 2222 0d0a  insum..    """..
+00007830: 2020 2020 5b73 7472 696e 6731 2c73 7472      [string1,str
+00007840: 696e 6732 5d20 3d20 6c69 7374 2873 7472  ing2] = list(str
+00007850: 696e 672e 7370 6c69 7428 222d 3e22 2929  ing.split("->"))
+00007860: 0d0a 2020 2020 756e 6971 7565 5f63 6861  ..    unique_cha
+00007870: 7273 203d 206c 6973 7428 7365 7428 7374  rs = list(set(st
+00007880: 7269 6e67 312b 7374 7269 6e67 3229 290d  ring1+string2)).
+00007890: 0a20 2020 2063 6861 725f 746f 5f69 6e74  .    char_to_int
+000078a0: 203d 207b 6368 6172 3a20 6920 666f 7220   = {char: i for 
+000078b0: 692c 2063 6861 7220 696e 2065 6e75 6d65  i, char in enume
+000078c0: 7261 7465 2875 6e69 7175 655f 6368 6172  rate(unique_char
+000078d0: 7329 7d0d 0a20 2020 2070 6572 6d75 7461  s)}..    permuta
+000078e0: 7469 6f6e 3120 3d20 5b63 6861 725f 746f  tion1 = [char_to
+000078f0: 5f69 6e74 5b63 6861 725d 2066 6f72 2063  _int[char] for c
+00007900: 6861 7220 696e 2073 7472 696e 6731 5d0d  har in string1].
+00007910: 0a20 2020 2070 6572 6d75 7461 7469 6f6e  .    permutation
+00007920: 3220 3d20 5b63 6861 725f 746f 5f69 6e74  2 = [char_to_int
+00007930: 5b63 6861 725d 2066 6f72 2063 6861 7220  [char] for char 
+00007940: 696e 2073 7472 696e 6732 5d0d 0a20 2020  in string2]..   
+00007950: 2072 6574 7572 6e20 7265 6c61 7469 7665   return relative
+00007960: 5f70 6172 6974 795f 696e 7428 7065 726d  _parity_int(perm
+00007970: 7574 6174 696f 6e31 2c20 7065 726d 7574  utation1, permut
+00007980: 6174 696f 6e32 2c20 696e 6469 7669 6475  ation2, individu
+00007990: 616c 5f70 6172 6974 7931 290d 0a0d 0a64  al_parity1)....d
+000079a0: 6566 2072 656c 6174 6976 655f 7061 7269  ef relative_pari
+000079b0: 7479 2873 7472 696e 672c 2069 6e64 6976  ty(string, indiv
+000079c0: 6964 7561 6c5f 7061 7269 7479 293a 0d0a  idual_parity):..
+000079d0: 2020 2020 2222 220d 0a20 2020 2049 6d61      """..    Ima
+000079e0: 6769 6e65 2064 6f69 6e67 2047 7261 7373  gine doing Grass
+000079f0: 6d61 6e6e 2076 6572 7369 6f6e 206f 6620  mann version of 
+00007a00: 4569 6e73 756d 2e0d 0a20 2020 2054 6869  Einsum...    Thi
+00007a10: 7320 6675 6e63 7469 6f6e 2072 6574 7572  s function retur
+00007a20: 6e73 2074 6865 2073 6967 6e20 6661 6374  ns the sign fact
+00007a30: 6f72 206f 6620 7468 6174 2073 756d 2e0d  or of that sum..
+00007a40: 0a20 2020 2059 6f75 2068 6176 6520 746f  .    You have to
+00007a50: 2065 6e74 6572 2074 6865 2070 6172 6974   enter the parit
+00007a60: 7920 6f66 2074 6865 2069 6e70 7574 2069  y of the input i
+00007a70: 6e64 6963 6573 2069 6e20 5b69 6e64 6976  ndices in [indiv
+00007a80: 6964 7561 6c5f 7061 7269 7479 5d0d 0a20  idual_parity].. 
+00007a90: 2020 2054 6865 2067 7261 7373 6d61 6e6e     The grassmann
+00007aa0: 2069 6e64 6963 6573 206d 7573 7420 6e6f   indices must no
+00007ab0: 7420 6265 2061 6464 6564 206f 7220 7265  t be added or re
+00007ac0: 6d6f 7665 6421 0d0a 2020 2020 5573 6520  moved!..    Use 
+00007ad0: 6120 6469 6666 6572 656e 7420 6675 6e63  a different func
+00007ae0: 7469 6f6e 2074 6f20 696e 7465 6772 6174  tion to integrat
+00007af0: 6520 7468 656d 206f 7574 210d 0a20 2020  e them out!..   
+00007b00: 2045 7861 6d70 6c65 733a 0d0a 2020 2020   Examples:..    
+00007b10: 3e3e 2072 656c 6174 6976 655f 7061 7269  >> relative_pari
+00007b20: 7479 2820 2261 6243 6445 2c61 5864 5962  ty( "abCdE,aXdYb
+00007b30: 2d3e 5843 4559 222c 205b 302c 302c 312c  ->XCEY", [0,0,1,
+00007b40: 302c 312c 302c 312c 302c 312c 305d 2029  0,1,0,1,0,1,0] )
+00007b50: 0d0a 2020 2020 3e3e 2031 0d0a 2020 2020  ..    >> 1..    
+00007b60: 0d0a 2020 2020 3e3e 2072 656c 6174 6976  ..    >> relativ
+00007b70: 655f 7061 7269 7479 2820 2261 6243 6445  e_parity( "abCdE
+00007b80: 2c61 5859 622d 3e43 5845 5922 2c20 5b30  ,aXYb->CXEY", [0
+00007b90: 2c30 2c31 2c30 2c31 2c30 2c31 2c31 2c30  ,0,1,0,1,0,1,1,0
+00007ba0: 5d20 290d 0a20 2020 203e 3e20 2d31 0d0a  ] )..    >> -1..
+00007bb0: 2020 2020 0d0a 2020 2020 2222 220d 0a20      ..    """.. 
+00007bc0: 2020 205b 7374 7269 6e67 5f69 6e70 7574     [string_input
+00007bd0: 2c73 7472 696e 675f 6f75 7470 7574 5d20  ,string_output] 
+00007be0: 3d20 6c69 7374 2873 7472 696e 672e 7370  = list(string.sp
+00007bf0: 6c69 7428 222d 3e22 2929 0d0a 2020 2020  lit("->"))..    
+00007c00: 7374 7269 6e67 5f6c 6973 7420 3d20 6c69  string_list = li
+00007c10: 7374 2873 7472 696e 675f 696e 7075 742e  st(string_input.
+00007c20: 7370 6c69 7428 222c 2229 290d 0a20 2020  split(","))..   
+00007c30: 200d 0a20 2020 206a 6f69 6e5f 7374 7269   ..    join_stri
+00007c40: 6e67 203d 2022 220d 0a20 2020 2066 6f72  ng = ""..    for
+00007c50: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00007c60: 7374 7269 6e67 5f6c 6973 7429 293a 0d0a  string_list)):..
+00007c70: 2020 2020 2020 2020 6a6f 696e 5f73 7472          join_str
+00007c80: 696e 6720 3d20 6a6f 696e 5f73 7472 696e  ing = join_strin
+00007c90: 6720 2b20 7374 7269 6e67 5f6c 6973 745b  g + string_list[
+00007ca0: 695d 0d0a 2020 2020 2020 2020 0d0a 2020  i]..        ..  
+00007cb0: 2020 6966 286c 656e 286a 6f69 6e5f 7374    if(len(join_st
+00007cc0: 7269 6e67 2921 3d6c 656e 2869 6e64 6976  ring)!=len(indiv
+00007cd0: 6964 7561 6c5f 7061 7269 7479 2929 3a0d  idual_parity)):.
+00007ce0: 0a20 2020 2020 2020 2065 7272 6f72 2822  .        error("
+00007cf0: 4572 726f 725b 7265 6c61 7469 7665 5f70  Error[relative_p
+00007d00: 6172 6974 795d 3a20 5468 6520 6e75 6d62  arity]: The numb
+00007d10: 6572 206f 6620 696e 7075 7420 6c69 7374  er of input list
+00007d20: 2061 6e64 2070 6172 6974 7920 6c69 7374   and parity list
+00007d30: 2061 7265 206e 6f74 2063 6f6e 7369 7374   are not consist
+00007d40: 656e 7421 2229 0d0a 2020 2020 2020 2020  ent!")..        
+00007d50: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00007d60: 2372 656d 6f76 6520 7468 6520 7375 6d6d  #remove the summ
+00007d70: 6564 2069 6e64 6963 6573 0d0a 2020 2020  ed indices..    
+00007d80: 6465 6620 7265 6d6f 7665 5f64 7570 6c69  def remove_dupli
+00007d90: 6361 7465 7328 6c69 7374 312c 206c 6973  cates(list1, lis
+00007da0: 7432 293a 0d0a 2020 2020 2020 2020 6e65  t2):..        ne
+00007db0: 775f 6c69 7374 3120 3d20 5b5d 0d0a 2020  w_list1 = []..  
+00007dc0: 2020 2020 2020 6e65 775f 6c69 7374 3220        new_list2 
+00007dd0: 3d20 5b5d 0d0a 2020 2020 2020 2020 666f  = []..        fo
+00007de0: 7220 692c 2076 616c 2069 6e20 656e 756d  r i, val in enum
+00007df0: 6572 6174 6528 6c69 7374 3129 3a0d 0a20  erate(list1):.. 
+00007e00: 2020 2020 2020 2020 2020 2069 6620 6c69             if li
+00007e10: 7374 312e 636f 756e 7428 7661 6c29 3d3d  st1.count(val)==
+00007e20: 3120 3a0d 0a20 2020 2020 2020 2020 2020  1 :..           
+00007e30: 2020 2020 206e 6577 5f6c 6973 7431 2e61       new_list1.a
+00007e40: 7070 656e 6428 7661 6c29 0d0a 2020 2020  ppend(val)..    
+00007e50: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00007e60: 6c69 7374 322e 6170 7065 6e64 286c 6973  list2.append(lis
+00007e70: 7432 5b69 5d29 0d0a 2020 2020 2020 2020  t2[i])..        
+00007e80: 7265 7475 726e 206e 6577 5f6c 6973 7431  return new_list1
+00007e90: 2c20 6e65 775f 6c69 7374 320d 0a20 2020  , new_list2..   
+00007ea0: 2020 2020 200d 0a20 2020 206a 6f69 6e5f       ..    join_
+00007eb0: 7374 7269 6e67 5f6c 6973 742c 696e 6469  string_list,indi
+00007ec0: 7669 6475 616c 5f70 6172 6974 7920 3d20  vidual_parity = 
+00007ed0: 7265 6d6f 7665 5f64 7570 6c69 6361 7465  remove_duplicate
+00007ee0: 7328 6c69 7374 286a 6f69 6e5f 7374 7269  s(list(join_stri
+00007ef0: 6e67 292c 2069 6e64 6976 6964 7561 6c5f  ng), individual_
+00007f00: 7061 7269 7479 290d 0a20 2020 206a 6f69  parity)..    joi
+00007f10: 6e5f 7374 7269 6e67 203d 2027 272e 6a6f  n_string = ''.jo
+00007f20: 696e 286a 6f69 6e5f 7374 7269 6e67 5f6c  in(join_string_l
+00007f30: 6973 7429 2b22 2d3e 222b 7374 7269 6e67  ist)+"->"+string
+00007f40: 5f6f 7574 7075 740d 0a20 2020 2072 6574  _output..    ret
+00007f50: 7572 6e20 7265 6c61 7469 7665 5f70 6172  urn relative_par
+00007f60: 6974 795f 7369 6e67 6c65 5f69 6e70 7574  ity_single_input
+00007f70: 286a 6f69 6e5f 7374 7269 6e67 2c20 696e  (join_string, in
+00007f80: 6469 7669 6475 616c 5f70 6172 6974 7929  dividual_parity)
+00007f90: 0d0a 0d0a 6465 6620 7265 6f72 6465 7269  ....def reorderi
+00007fa0: 6e67 2873 7472 696e 6761 2c73 7472 696e  ng(stringa,strin
+00007fb0: 6762 2c6d 796c 6973 7429 3a0d 0a0d 0a20  gb,mylist):.... 
+00007fc0: 2020 2072 4320 3d20 5b5d 0d0a 2020 2020     rC = []..    
+00007fd0: 666f 7220 6220 696e 2073 7472 696e 6762  for b in stringb
+00007fe0: 3a0d 0a20 2020 2020 2020 200d 0a20 2020  :..        ..   
+00007ff0: 2020 2020 2023 206c 6f63 6174 6520 7468       # locate th
+00008000: 6520 6c6f 6361 7469 6f6e 206f 6620 6220  e location of b 
+00008010: 696e 2074 6865 206f 7269 6769 6e61 6c20  in the original 
+00008020: 7374 7269 6e67 0d0a 2020 2020 2020 2020  string..        
+00008030: 696e 6465 7820 3d20 7374 7269 6e67 612e  index = stringa.
+00008040: 696e 6465 7828 6229 0d0a 0d0a 2020 2020  index(b)....    
+00008050: 2020 2020 2320 6164 6420 6d79 6c69 7374      # add mylist
+00008060: 2773 2065 6c65 6d65 6e74 2061 7420 7468  's element at th
+00008070: 6973 2069 6e64 6578 2074 6f20 7468 6520  is index to the 
+00008080: 6c69 7374 0d0a 2020 2020 2020 2020 7243  list..        rC
+00008090: 202b 3d20 5b6d 796c 6973 745b 696e 6465   += [mylist[inde
+000080a0: 785d 5d0d 0a0d 0a20 2020 2072 6574 7572  x]]....    retur
+000080b0: 6e20 7243 0d0a 0d0a 2323 2323 2323 2323  n rC....########
+000080c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000080d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000080e0: 2323 2323 2323 2323 2323 2323 0d0a 2323  ############..##
+000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008100: 2020 2020 2045 696e 7375 6d73 2020 2020       Einsums    
 00008110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008120: 4569 6e73 756d 7320 2020 2020 2020 2020  Einsums         
-00008130: 2020 2020 2020 2020 2020 2023 230d 0a23             ##..#
+00008120: 2323 0d0a 2323 2323 2323 2323 2323 2323  ##..############
+00008130: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00008140: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008150: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008160: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008170: 2323 230d 0a0d 0a64 6566 2064 656e 756d  ###....def denum
-00008180: 6572 6174 6528 7374 7269 6e67 293a 0d0a  erate(string):..
-00008190: 2020 2020 2320 7475 726e 206e 756d 6265      # turn numbe
-000081a0: 7265 6420 696e 6469 6365 7320 746f 206a  red indices to j
-000081b0: 7573 7420 7369 6e67 6c65 2069 6e64 6963  ust single indic
-000081c0: 6573 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  es -------------
-000081d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000081e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000081f0: 2d2d 2d2d 2d0d 0a20 2020 2069 6e64 6578  -----..    index
-00008200: 5f63 6861 7220 3d20 5b5d 0d0a 2020 2020  _char = []..    
-00008210: 666f 7220 6320 696e 2073 7472 696e 6720  for c in string 
-00008220: 3a0d 0a20 2020 2020 2020 2069 6620 6320  :..        if c 
-00008230: 6e6f 7420 696e 206e 756d 6265 725f 6368  not in number_ch
-00008240: 6172 6163 7465 723a 0d0a 2020 2020 2020  aracter:..      
-00008250: 2020 2020 2020 696e 6465 785f 6368 6172        index_char
-00008260: 202b 3d20 632c 0d0a 2020 2020 2020 2020   += c,..        
-00008270: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00008280: 2020 2069 6e64 6578 5f63 6861 725b 6c65     index_char[le
-00008290: 6e28 696e 6465 785f 6368 6172 292d 315d  n(index_char)-1]
-000082a0: 202b 3d20 630d 0a20 2020 2075 6e69 7175   += c..    uniqu
-000082b0: 655f 746f 6b65 6e73 203d 206c 6973 7428  e_tokens = list(
-000082c0: 6469 6374 2e66 726f 6d6b 6579 7328 696e  dict.fromkeys(in
-000082d0: 6465 785f 6368 6172 2929 0d0a 2020 2020  dex_char))..    
-000082e0: 746f 5f62 655f 7265 706c 6163 6564 203d  to_be_replaced =
-000082f0: 205b 5d0d 0a20 2020 2066 6f72 2069 7465   []..    for ite
-00008300: 6d20 696e 2075 6e69 7175 655f 746f 6b65  m in unique_toke
-00008310: 6e73 3a0d 0a20 2020 2020 2020 2069 6620  ns:..        if 
-00008320: 6c65 6e28 6974 656d 2920 3e20 3120 3a0d  len(item) > 1 :.
-00008330: 0a20 2020 2020 2020 2020 2020 2074 6f5f  .            to_
-00008340: 6265 5f72 6570 6c61 6365 6420 2b3d 2069  be_replaced += i
-00008350: 7465 6d2c 0d0a 2020 2020 746f 5f62 655f  tem,..    to_be_
-00008360: 7265 706c 6163 6564 203d 2073 6f72 7465  replaced = sorte
-00008370: 6428 746f 5f62 655f 7265 706c 6163 6564  d(to_be_replaced
-00008380: 2c20 6b65 793d 6c65 6e2c 2072 6576 6572  , key=len, rever
-00008390: 7365 3d54 7275 6529 0d0a 2020 2020 746f  se=True)..    to
-000083a0: 6b65 6e5f 6c69 7374 203d 2073 7472 696e  ken_list = strin
-000083b0: 670d 0a20 2020 2066 6f72 2069 2069 6e20  g..    for i in 
-000083c0: 7261 6e67 6528 6c65 6e28 746f 5f62 655f  range(len(to_be_
-000083d0: 7265 706c 6163 6564 2929 203a 0d0a 2020  replaced)) :..  
-000083e0: 2020 2020 2020 6e65 775f 6368 6172 203d        new_char =
-000083f0: 2067 6574 5f63 6861 7228 746f 6b65 6e5f   get_char(token_
-00008400: 6c69 7374 290d 0a20 2020 2020 2020 2074  list)..        t
-00008410: 6f6b 656e 5f6c 6973 7420 2b3d 206e 6577  oken_list += new
-00008420: 5f63 6861 720d 0a20 2020 2020 2020 2074  _char..        t
-00008430: 6f5f 6265 5f72 6570 6c61 6365 645b 695d  o_be_replaced[i]
-00008440: 203d 205b 746f 5f62 655f 7265 706c 6163   = [to_be_replac
-00008450: 6564 5b69 5d2c 6e65 775f 6368 6172 5d0d  ed[i],new_char].
-00008460: 0a20 2020 2066 6f72 205b 6331 2c63 325d  .    for [c1,c2]
-00008470: 2069 6e20 746f 5f62 655f 7265 706c 6163   in to_be_replac
-00008480: 6564 203a 0d0a 2020 2020 2020 2020 7374  ed :..        st
-00008490: 7269 6e67 203d 2073 7472 696e 672e 7265  ring = string.re
-000084a0: 706c 6163 6528 6331 2c63 3229 0d0a 2020  place(c1,c2)..  
-000084b0: 2020 7265 7475 726e 2073 7472 696e 670d    return string.
-000084c0: 0a0d 0a64 6566 2065 696e 7375 6d28 2a61  ...def einsum(*a
-000084d0: 7267 732c 666f 726d 6174 3d22 7374 616e  rgs,format="stan
-000084e0: 6461 7264 222c 656e 636f 6465 723d 2263  dard",encoder="c
-000084f0: 616e 6f6e 6963 616c 222c 6465 6275 675f  anonical",debug_
-00008500: 6d6f 6465 3d46 616c 7365 293a 0d0a 0d0a  mode=False):....
-00008510: 2020 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a      #:::::::::::
+00008150: 2323 2323 2323 2323 0d0a 0d0a 6465 6620  ########....def 
+00008160: 6465 6e75 6d65 7261 7465 2873 7472 696e  denumerate(strin
+00008170: 6729 3a0d 0a20 2020 2023 2074 7572 6e20  g):..    # turn 
+00008180: 6e75 6d62 6572 6564 2069 6e64 6963 6573  numbered indices
+00008190: 2074 6f20 6a75 7374 2073 696e 676c 6520   to just single 
+000081a0: 696e 6469 6365 7320 2d2d 2d2d 2d2d 2d2d  indices --------
+000081b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000081c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000081d0: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
+000081e0: 696e 6465 785f 6368 6172 203d 205b 5d0d  index_char = [].
+000081f0: 0a20 2020 2066 6f72 2063 2069 6e20 7374  .    for c in st
+00008200: 7269 6e67 203a 0d0a 2020 2020 2020 2020  ring :..        
+00008210: 6966 2063 206e 6f74 2069 6e20 6e75 6d62  if c not in numb
+00008220: 6572 5f63 6861 7261 6374 6572 3a0d 0a20  er_character:.. 
+00008230: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+00008240: 5f63 6861 7220 2b3d 2063 2c0d 0a20 2020  _char += c,..   
+00008250: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00008260: 2020 2020 2020 2020 696e 6465 785f 6368          index_ch
+00008270: 6172 5b6c 656e 2869 6e64 6578 5f63 6861  ar[len(index_cha
+00008280: 7229 2d31 5d20 2b3d 2063 0d0a 2020 2020  r)-1] += c..    
+00008290: 756e 6971 7565 5f74 6f6b 656e 7320 3d20  unique_tokens = 
+000082a0: 6c69 7374 2864 6963 742e 6672 6f6d 6b65  list(dict.fromke
+000082b0: 7973 2869 6e64 6578 5f63 6861 7229 290d  ys(index_char)).
+000082c0: 0a20 2020 2074 6f5f 6265 5f72 6570 6c61  .    to_be_repla
+000082d0: 6365 6420 3d20 5b5d 0d0a 2020 2020 666f  ced = []..    fo
+000082e0: 7220 6974 656d 2069 6e20 756e 6971 7565  r item in unique
+000082f0: 5f74 6f6b 656e 733a 0d0a 2020 2020 2020  _tokens:..      
+00008300: 2020 6966 206c 656e 2869 7465 6d29 203e    if len(item) >
+00008310: 2031 203a 0d0a 2020 2020 2020 2020 2020   1 :..          
+00008320: 2020 746f 5f62 655f 7265 706c 6163 6564    to_be_replaced
+00008330: 202b 3d20 6974 656d 2c0d 0a20 2020 2074   += item,..    t
+00008340: 6f5f 6265 5f72 6570 6c61 6365 6420 3d20  o_be_replaced = 
+00008350: 736f 7274 6564 2874 6f5f 6265 5f72 6570  sorted(to_be_rep
+00008360: 6c61 6365 642c 206b 6579 3d6c 656e 2c20  laced, key=len, 
+00008370: 7265 7665 7273 653d 5472 7565 290d 0a20  reverse=True).. 
+00008380: 2020 2074 6f6b 656e 5f6c 6973 7420 3d20     token_list = 
+00008390: 7374 7269 6e67 0d0a 2020 2020 666f 7220  string..    for 
+000083a0: 6920 696e 2072 616e 6765 286c 656e 2874  i in range(len(t
+000083b0: 6f5f 6265 5f72 6570 6c61 6365 6429 2920  o_be_replaced)) 
+000083c0: 3a0d 0a20 2020 2020 2020 206e 6577 5f63  :..        new_c
+000083d0: 6861 7220 3d20 6765 745f 6368 6172 2874  har = get_char(t
+000083e0: 6f6b 656e 5f6c 6973 7429 0d0a 2020 2020  oken_list)..    
+000083f0: 2020 2020 746f 6b65 6e5f 6c69 7374 202b      token_list +
+00008400: 3d20 6e65 775f 6368 6172 0d0a 2020 2020  = new_char..    
+00008410: 2020 2020 746f 5f62 655f 7265 706c 6163      to_be_replac
+00008420: 6564 5b69 5d20 3d20 5b74 6f5f 6265 5f72  ed[i] = [to_be_r
+00008430: 6570 6c61 6365 645b 695d 2c6e 6577 5f63  eplaced[i],new_c
+00008440: 6861 725d 0d0a 2020 2020 666f 7220 5b63  har]..    for [c
+00008450: 312c 6332 5d20 696e 2074 6f5f 6265 5f72  1,c2] in to_be_r
+00008460: 6570 6c61 6365 6420 3a0d 0a20 2020 2020  eplaced :..     
+00008470: 2020 2073 7472 696e 6720 3d20 7374 7269     string = stri
+00008480: 6e67 2e72 6570 6c61 6365 2863 312c 6332  ng.replace(c1,c2
+00008490: 290d 0a20 2020 2072 6574 7572 6e20 7374  )..    return st
+000084a0: 7269 6e67 0d0a 0d0a 6465 6620 6569 6e73  ring....def eins
+000084b0: 756d 282a 6172 6773 2c66 6f72 6d61 743d  um(*args,format=
+000084c0: 2273 7461 6e64 6172 6422 2c65 6e63 6f64  "standard",encod
+000084d0: 6572 3d22 6361 6e6f 6e69 6361 6c22 2c64  er="canonical",d
+000084e0: 6562 7567 5f6d 6f64 653d 4661 6c73 6529  ebug_mode=False)
+000084f0: 3a0d 0a0d 0a20 2020 2023 3a3a 3a3a 3a3a  :....    #::::::
+00008500: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00008510: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00008520: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00008530: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00008540: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00008550: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00008560: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00008570: 3a3a 3a3a 3a0d 0a20 2020 2023 2020 2020  :::::..    #    
-00008580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008590: 2049 6d70 6f72 7461 6e74 2076 6172 6961   Important varia
-000085a0: 626c 6573 2061 6e64 2069 7473 206d 6561  bles and its mea
-000085b0: 6e69 6e67 730d 0a20 2020 2023 3a3a 3a3a  nings..    #::::
+00008550: 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a 2020 2020  ::::::::::..    
+00008560: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+00008570: 2020 2020 2020 496d 706f 7274 616e 7420        Important 
+00008580: 7661 7269 6162 6c65 7320 616e 6420 6974  variables and it
+00008590: 7320 6d65 616e 696e 6773 0d0a 2020 2020  s meanings..    
+000085a0: 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  #:::::::::::::::
+000085b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 000085c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 000085d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 000085e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 000085f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00008600: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00008610: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a 2020  ::::::::::::..  
-00008620: 2020 230d 0a20 2020 2023 2020 2020 2020    #..    #      
-00008630: 2069 6e73 7472 7563 7469 6f6e 5f73 7472   instruction_str
-00008640: 696e 6720 3d20 7468 6520 7768 6f6c 6520  ing = the whole 
-00008650: 696e 7075 7420 7465 7874 2077 6974 6820  input text with 
-00008660: 7370 6163 6573 2072 656d 6f76 6564 0d0a  spaces removed..
-00008670: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-00008680: 2020 2020 6861 735f 6f75 7470 7574 203d      has_output =
-00008690: 2054 7275 6520 6966 2074 6865 203c 696e   True if the <in
-000086a0: 7075 745f 7374 7269 6e67 3e20 6861 7320  put_string> has 
-000086b0: 7468 6520 6f75 7470 7574 2073 6563 7469  the output secti
-000086c0: 6f6e 0d0a 2020 2020 2320 2020 2020 2020  on..    #       
-000086d0: 2020 2020 2020 696e 7075 745f 7374 7269        input_stri
-000086e0: 6e67 203d 2074 6865 206c 6566 7420 7369  ng = the left si
-000086f0: 6465 206f 6620 7468 6520 6172 726f 770d  de of the arrow.
-00008700: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
-00008710: 2020 6f75 7470 7574 5f73 7472 696e 6720    output_string 
-00008720: 3d20 7468 6520 7269 6768 7420 7369 6465  = the right side
-00008730: 206f 6620 7468 6520 6172 726f 770d 0a20   of the arrow.. 
-00008740: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-00008750: 2020 2020 2020 7375 6d6d 616e 6420 3d20        summand = 
-00008760: 3c69 6e70 7574 5f73 7472 696e 673e 2077  <input_string> w
-00008770: 6974 686f 7574 2063 6f6d 6d61 730d 0a20  ithout commas.. 
-00008780: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-00008790: 2020 2020 2020 2020 206e 6f62 6a20 3d20           nobj = 
-000087a0: 6e75 6d62 6572 206f 6620 696e 7075 7420  number of input 
-000087b0: 6f62 6a65 6374 730d 0a20 2020 2023 2020  objects..    #  
-000087c0: 2020 2020 2020 2020 206f 626a 5f69 6e64           obj_ind
-000087d0: 6578 5f6c 6973 7420 3d20 6c69 7374 206f  ex_list = list o
-000087e0: 6620 696e 6469 7669 6475 616c 2069 6e64  f individual ind
-000087f0: 6578 2073 7472 696e 6773 206f 6620 696e  ex strings of in
-00008800: 7075 7420 6f62 6a65 6374 730d 0a20 2020  put objects..   
-00008810: 2023 2020 2020 2020 2020 2020 2020 2020   #              
-00008820: 2020 206f 626a 5f6c 6973 7420 3d20 6c69     obj_list = li
-00008830: 7374 206f 6620 696e 7075 7420 6f62 6a65  st of input obje
-00008840: 6374 730d 0a20 2020 2023 2020 2020 2020  cts..    #      
-00008850: 2020 2020 2020 2020 2073 7461 7473 5f6c           stats_l
-00008860: 6973 7420 3d20 696e 7075 7420 6f62 6a65  ist = input obje
-00008870: 6374 2773 2073 7461 7473 206a 6f69 6e65  ct's stats joine
-00008880: 6420 696e 746f 2061 2073 696e 676c 6520  d into a single 
-00008890: 6c69 7374 0d0a 2020 2020 2320 2020 2020  list..    #     
-000088a0: 2020 2020 2020 2020 2020 7368 6170 655f            shape_
-000088b0: 6c69 7374 203d 2069 6e70 7574 206f 626a  list = input obj
-000088c0: 6563 7427 7320 7368 6170 6520 6a6f 696e  ect's shape join
-000088d0: 6564 2069 6e74 6f20 6120 7369 6e67 6c65  ed into a single
-000088e0: 206c 6973 740d 0a20 2020 2023 2020 2020   list..    #    
-000088f0: 2020 2020 7375 6d6d 6564 5f69 6e64 6578      summed_index
-00008900: 5f69 6e66 6f20 3d20 5b20 5b63 6861 722c  _info = [ [char,
-00008910: 2063 6f6e 6a75 6761 7465 645f 6368 6172   conjugated_char
-00008920: 5d2c 205b 696e 6465 7820 6c6f 6361 7469  ], [index locati
-00008930: 6f6e 7320 696e 203c 696e 7075 745f 7374  ons in <input_st
-00008940: 7269 6e67 3e5d 205d 0d0a 0d0a 0d0a 2020  ring>] ]......  
-00008950: 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a    #:::::::::::::
+00008600: 3a0d 0a20 2020 2023 0d0a 2020 2020 2320  :..    #..    # 
+00008610: 2020 2020 2020 696e 7374 7275 6374 696f        instructio
+00008620: 6e5f 7374 7269 6e67 203d 2074 6865 2077  n_string = the w
+00008630: 686f 6c65 2069 6e70 7574 2074 6578 7420  hole input text 
+00008640: 7769 7468 2073 7061 6365 7320 7265 6d6f  with spaces remo
+00008650: 7665 640d 0a20 2020 2023 2020 2020 2020  ved..    #      
+00008660: 2020 2020 2020 2020 2068 6173 5f6f 7574           has_out
+00008670: 7075 7420 3d20 5472 7565 2069 6620 7468  put = True if th
+00008680: 6520 3c69 6e70 7574 5f73 7472 696e 673e  e <input_string>
+00008690: 2068 6173 2074 6865 206f 7574 7075 7420   has the output 
+000086a0: 7365 6374 696f 6e0d 0a20 2020 2023 2020  section..    #  
+000086b0: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+000086c0: 5f73 7472 696e 6720 3d20 7468 6520 6c65  _string = the le
+000086d0: 6674 2073 6964 6520 6f66 2074 6865 2061  ft side of the a
+000086e0: 7272 6f77 0d0a 2020 2020 2320 2020 2020  rrow..    #     
+000086f0: 2020 2020 2020 206f 7574 7075 745f 7374         output_st
+00008700: 7269 6e67 203d 2074 6865 2072 6967 6874  ring = the right
+00008710: 2073 6964 6520 6f66 2074 6865 2061 7272   side of the arr
+00008720: 6f77 0d0a 2020 2020 2320 2020 2020 2020  ow..    #       
+00008730: 2020 2020 2020 2020 2020 2073 756d 6d61             summa
+00008740: 6e64 203d 203c 696e 7075 745f 7374 7269  nd = <input_stri
+00008750: 6e67 3e20 7769 7468 6f75 7420 636f 6d6d  ng> without comm
+00008760: 6173 0d0a 2020 2020 2320 2020 2020 2020  as..    #       
+00008770: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00008780: 626a 203d 206e 756d 6265 7220 6f66 2069  bj = number of i
+00008790: 6e70 7574 206f 626a 6563 7473 0d0a 2020  nput objects..  
+000087a0: 2020 2320 2020 2020 2020 2020 2020 6f62    #           ob
+000087b0: 6a5f 696e 6465 785f 6c69 7374 203d 206c  j_index_list = l
+000087c0: 6973 7420 6f66 2069 6e64 6976 6964 7561  ist of individua
+000087d0: 6c20 696e 6465 7820 7374 7269 6e67 7320  l index strings 
+000087e0: 6f66 2069 6e70 7574 206f 626a 6563 7473  of input objects
+000087f0: 0d0a 2020 2020 2320 2020 2020 2020 2020  ..    #         
+00008800: 2020 2020 2020 2020 6f62 6a5f 6c69 7374          obj_list
+00008810: 203d 206c 6973 7420 6f66 2069 6e70 7574   = list of input
+00008820: 206f 626a 6563 7473 0d0a 2020 2020 2320   objects..    # 
+00008830: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00008840: 6174 735f 6c69 7374 203d 2069 6e70 7574  ats_list = input
+00008850: 206f 626a 6563 7427 7320 7374 6174 7320   object's stats 
+00008860: 6a6f 696e 6564 2069 6e74 6f20 6120 7369  joined into a si
+00008870: 6e67 6c65 206c 6973 740d 0a20 2020 2023  ngle list..    #
+00008880: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00008890: 6861 7065 5f6c 6973 7420 3d20 696e 7075  hape_list = inpu
+000088a0: 7420 6f62 6a65 6374 2773 2073 6861 7065  t object's shape
+000088b0: 206a 6f69 6e65 6420 696e 746f 2061 2073   joined into a s
+000088c0: 696e 676c 6520 6c69 7374 0d0a 2020 2020  ingle list..    
+000088d0: 2320 2020 2020 2020 2073 756d 6d65 645f  #        summed_
+000088e0: 696e 6465 785f 696e 666f 203d 205b 205b  index_info = [ [
+000088f0: 6368 6172 2c20 636f 6e6a 7567 6174 6564  char, conjugated
+00008900: 5f63 6861 725d 2c20 5b69 6e64 6578 206c  _char], [index l
+00008910: 6f63 6174 696f 6e73 2069 6e20 3c69 6e70  ocations in <inp
+00008920: 7574 5f73 7472 696e 673e 5d20 5d0d 0a0d  ut_string>] ]...
+00008930: 0a0d 0a20 2020 2023 3a3a 3a3a 3a3a 3a3a  ...    #::::::::
+00008940: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00008950: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00008960: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00008970: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00008980: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00008990: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000089a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000089b0: 3a3a 3a0d 0a20 2020 2023 2020 2020 2020  :::..    #      
-000089c0: 2020 2020 2020 2020 5374 6570 2030 3a20          Step 0: 
-000089d0: 496e 7075 7420 7072 6f63 6573 7369 6e67  Input processing
-000089e0: 0d0a 2020 2020 233a 3a3a 3a3a 3a3a 3a3a  ..    #:::::::::
+00008990: 3a3a 3a3a 3a3a 3a3a 0d0a 2020 2020 2320  ::::::::..    # 
+000089a0: 2020 2020 2020 2020 2020 2020 2053 7465               Ste
+000089b0: 7020 303a 2049 6e70 7574 2070 726f 6365  p 0: Input proce
+000089c0: 7373 696e 670d 0a20 2020 2023 3a3a 3a3a  ssing..    #::::
+000089d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000089e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 000089f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00008a00: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00008a10: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00008a20: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00008a30: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00008a40: 3a3a 3a3a 3a3a 3a0d 0a0d 0a20 2020 2023  :::::::....    #
-00008a50: 2072 656d 6f76 6520 7370 6163 6573 202d   remove spaces -
+00008a20: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a 0d0a  ::::::::::::....
+00008a30: 2020 2020 2320 7265 6d6f 7665 2073 7061      # remove spa
+00008a40: 6365 7320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ces ------------
+00008a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00008a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00008a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00008a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008ab0: 0d0a 2020 2020 696e 7374 7275 6374 696f  ..    instructio
-00008ac0: 6e5f 7374 7269 6e67 203d 2061 7267 735b  n_string = args[
-00008ad0: 305d 2e72 6570 6c61 6365 2822 2022 2c22  0].replace(" ","
-00008ae0: 2229 0d0a 0d0a 2020 2020 696e 7374 7275  ")....    instru
-00008af0: 6374 696f 6e5f 7374 7269 6e67 203d 2064  ction_string = d
-00008b00: 656e 756d 6572 6174 6528 696e 7374 7275  enumerate(instru
-00008b10: 6374 696f 6e5f 7374 7269 6e67 290d 0a0d  ction_string)...
-00008b20: 0a20 2020 2068 6173 5f6f 7574 7075 7420  .    has_output 
-00008b30: 3d20 696e 7374 7275 6374 696f 6e5f 7374  = instruction_st
-00008b40: 7269 6e67 2e63 6f75 6e74 2822 2d3e 2229  ring.count("->")
-00008b50: 203e 2030 0d0a 2020 2020 6966 2069 6e73   > 0..    if ins
-00008b60: 7472 7563 7469 6f6e 5f73 7472 696e 672e  truction_string.
-00008b70: 636f 756e 7428 222d 3e22 2920 3e20 3120  count("->") > 1 
-00008b80: 3a0d 0a20 2020 2020 2020 2065 7272 6f72  :..        error
-00008b90: 2822 4572 726f 725b 6569 6e73 756d 5d3a  ("Error[einsum]:
-00008ba0: 204f 6e6c 7920 6f6e 6520 6172 726f 7720   Only one arrow 
-00008bb0: 6973 2061 6c6c 6f77 6564 2069 6e20 7468  is allowed in th
-00008bc0: 6520 696e 7075 7420 7374 7269 6e67 2122  e input string!"
-00008bd0: 290d 0a0d 0a20 2020 2069 6620 6861 735f  )....    if has_
-00008be0: 6f75 7470 7574 3a0d 0a20 2020 2020 2020  output:..       
-00008bf0: 2069 6e70 7574 5f73 7472 696e 672c 206f   input_string, o
-00008c00: 7574 7075 745f 7374 7269 6e67 203d 2069  utput_string = i
-00008c10: 6e73 7472 7563 7469 6f6e 5f73 7472 696e  nstruction_strin
-00008c20: 672e 7370 6c69 7428 222d 3e22 290d 0a20  g.split("->").. 
-00008c30: 2020 2020 2020 2069 6620 6f75 7470 7574         if output
-00008c40: 5f73 7472 696e 672e 636f 756e 7428 222c  _string.count(",
-00008c50: 2229 203e 2030 203a 0d0a 2020 2020 2020  ") > 0 :..      
-00008c60: 2020 2020 2020 6572 726f 7228 2245 7272        error("Err
-00008c70: 6f72 5b65 696e 7375 6d5d 3a20 4f75 7470  or[einsum]: Outp
-00008c80: 7574 2073 7472 696e 6720 6d75 7374 206e  ut string must n
-00008c90: 6f74 2063 6f6e 7461 696e 2063 6f6d 6d61  ot contain comma
-00008ca0: 7320 2827 2c27 2920 2122 290d 0a20 2020  s (',') !")..   
-00008cb0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00008cc0: 696e 7075 745f 7374 7269 6e67 203d 2069  input_string = i
-00008cd0: 6e73 7472 7563 7469 6f6e 5f73 7472 696e  nstruction_strin
-00008ce0: 670d 0a0d 0a20 2020 2073 756d 6d61 6e64  g....    summand
-00008cf0: 203d 2069 6e70 7574 5f73 7472 696e 672e   = input_string.
-00008d00: 7265 706c 6163 6528 222c 222c 2222 290d  replace(",","").
-00008d10: 0a0d 0a20 2020 206f 626a 5f69 6e64 6578  ...    obj_index
-00008d20: 5f6c 6973 7420 3d20 696e 7075 745f 7374  _list = input_st
-00008d30: 7269 6e67 2e73 706c 6974 2822 2c22 290d  ring.split(",").
-00008d40: 0a20 2020 206e 6f62 6a20 3d20 6c65 6e28  .    nobj = len(
-00008d50: 6f62 6a5f 696e 6465 785f 6c69 7374 290d  obj_index_list).
-00008d60: 0a0d 0a20 2020 206f 626a 5f6c 6973 7420  ...    obj_list 
-00008d70: 3d20 6d61 6b65 5f6c 6973 7428 6172 6773  = make_list(args
-00008d80: 5b31 3a31 2b6e 6f62 6a5d 290d 0a20 2020  [1:1+nobj])..   
-00008d90: 2073 7461 7473 5f6c 6973 7420 3d20 7375   stats_list = su
-00008da0: 6d28 5b20 6d61 6b65 5f6c 6973 7428 6f62  m([ make_list(ob
-00008db0: 6a2e 7374 6174 6973 7469 6329 2066 6f72  j.statistic) for
-00008dc0: 206f 626a 2069 6e20 6f62 6a5f 6c69 7374   obj in obj_list
-00008dd0: 205d 2c5b 5d29 0d0a 2020 2020 7368 6170   ],[])..    shap
-00008de0: 655f 6c69 7374 203d 2073 756d 285b 206d  e_list = sum([ m
-00008df0: 616b 655f 6c69 7374 286f 626a 2e73 6861  ake_list(obj.sha
-00008e00: 7065 2920 666f 7220 6f62 6a20 696e 206f  pe) for obj in o
-00008e10: 626a 5f6c 6973 7420 5d2c 5b5d 290d 0a0d  bj_list ],[])...
-00008e20: 0a20 2020 2023 2066 6f72 6365 2065 7665  .    # force eve
-00008e30: 7279 7468 696e 6720 746f 2062 6520 6361  rything to be ca
-00008e40: 6e6f 6e69 6361 6c20 616e 6420 7374 616e  nonical and stan
-00008e50: 6461 7264 202d 2d2d 2d2d 2d2d 2d2d 2d2d  dard -----------
-00008e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00008e80: 2d2d 2d2d 2d2d 0d0a 2020 2020 2320 616c  ------..    # al
-00008e90: 736f 2066 6f72 6365 2065 7665 7279 7468  so force everyth
-00008ea0: 696e 6720 746f 2062 6520 6f66 2074 6865  ing to be of the
-00008eb0: 2073 616d 6520 7479 7065 0d0a 0d0a 2020   same type....  
-00008ec0: 2020 7468 6973 5f74 7970 6520 3d20 7479    this_type = ty
-00008ed0: 7065 286f 626a 5f6c 6973 745b 305d 290d  pe(obj_list[0]).
-00008ee0: 0a20 2020 2074 6869 735f 656e 636f 6465  .    this_encode
-00008ef0: 7220 3d20 6f62 6a5f 6c69 7374 5b30 5d2e  r = obj_list[0].
-00008f00: 656e 636f 6465 720d 0a20 2020 2074 6869  encoder..    thi
-00008f10: 735f 666f 726d 6174 203d 206f 626a 5f6c  s_format = obj_l
-00008f20: 6973 745b 305d 2e66 6f72 6d61 740d 0a20  ist[0].format.. 
-00008f30: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00008f40: 6528 6c65 6e28 6f62 6a5f 6c69 7374 2929  e(len(obj_list))
-00008f50: 3a0d 0a20 2020 2020 2020 206f 626a 5f6c  :..        obj_l
-00008f60: 6973 745b 695d 203d 2074 6869 735f 7479  ist[i] = this_ty
-00008f70: 7065 286f 626a 5f6c 6973 745b 695d 2e66  pe(obj_list[i].f
-00008f80: 6f72 6365 5f65 6e63 6f64 6572 2827 6361  orce_encoder('ca
-00008f90: 6e6f 6e69 6361 6c27 292e 666f 7263 655f  nonical').force_
-00008fa0: 666f 726d 6174 2827 7374 616e 6461 7264  format('standard
-00008fb0: 2729 292e 6461 7461 0d0a 0d0a 2020 2020  ')).data....    
-00008fc0: 2320 6765 7420 736f 6d65 2069 6e66 6f72  # get some infor
-00008fd0: 6d61 7469 6f6e 2061 626f 7574 2074 6865  mation about the
-00008fe0: 2073 756d 6d65 6420 696e 6469 6365 7320   summed indices 
+00008a90: 2d2d 2d2d 2d0d 0a20 2020 2069 6e73 7472  -----..    instr
+00008aa0: 7563 7469 6f6e 5f73 7472 696e 6720 3d20  uction_string = 
+00008ab0: 6172 6773 5b30 5d2e 7265 706c 6163 6528  args[0].replace(
+00008ac0: 2220 222c 2222 290d 0a0d 0a20 2020 2069  " ","")....    i
+00008ad0: 6e73 7472 7563 7469 6f6e 5f73 7472 696e  nstruction_strin
+00008ae0: 6720 3d20 6465 6e75 6d65 7261 7465 2869  g = denumerate(i
+00008af0: 6e73 7472 7563 7469 6f6e 5f73 7472 696e  nstruction_strin
+00008b00: 6729 0d0a 0d0a 2020 2020 6861 735f 6f75  g)....    has_ou
+00008b10: 7470 7574 203d 2069 6e73 7472 7563 7469  tput = instructi
+00008b20: 6f6e 5f73 7472 696e 672e 636f 756e 7428  on_string.count(
+00008b30: 222d 3e22 2920 3e20 300d 0a20 2020 2069  "->") > 0..    i
+00008b40: 6620 696e 7374 7275 6374 696f 6e5f 7374  f instruction_st
+00008b50: 7269 6e67 2e63 6f75 6e74 2822 2d3e 2229  ring.count("->")
+00008b60: 203e 2031 203a 0d0a 2020 2020 2020 2020   > 1 :..        
+00008b70: 6572 726f 7228 2245 7272 6f72 5b65 696e  error("Error[ein
+00008b80: 7375 6d5d 3a20 4f6e 6c79 206f 6e65 2061  sum]: Only one a
+00008b90: 7272 6f77 2069 7320 616c 6c6f 7765 6420  rrow is allowed 
+00008ba0: 696e 2074 6865 2069 6e70 7574 2073 7472  in the input str
+00008bb0: 696e 6721 2229 0d0a 0d0a 2020 2020 6966  ing!")....    if
+00008bc0: 2068 6173 5f6f 7574 7075 743a 0d0a 2020   has_output:..  
+00008bd0: 2020 2020 2020 696e 7075 745f 7374 7269        input_stri
+00008be0: 6e67 2c20 6f75 7470 7574 5f73 7472 696e  ng, output_strin
+00008bf0: 6720 3d20 696e 7374 7275 6374 696f 6e5f  g = instruction_
+00008c00: 7374 7269 6e67 2e73 706c 6974 2822 2d3e  string.split("->
+00008c10: 2229 0d0a 2020 2020 2020 2020 6966 206f  ")..        if o
+00008c20: 7574 7075 745f 7374 7269 6e67 2e63 6f75  utput_string.cou
+00008c30: 6e74 2822 2c22 2920 3e20 3020 3a0d 0a20  nt(",") > 0 :.. 
+00008c40: 2020 2020 2020 2020 2020 2065 7272 6f72             error
+00008c50: 2822 4572 726f 725b 6569 6e73 756d 5d3a  ("Error[einsum]:
+00008c60: 204f 7574 7075 7420 7374 7269 6e67 206d   Output string m
+00008c70: 7573 7420 6e6f 7420 636f 6e74 6169 6e20  ust not contain 
+00008c80: 636f 6d6d 6173 2028 272c 2729 2021 2229  commas (',') !")
+00008c90: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
+00008ca0: 2020 2020 2069 6e70 7574 5f73 7472 696e       input_strin
+00008cb0: 6720 3d20 696e 7374 7275 6374 696f 6e5f  g = instruction_
+00008cc0: 7374 7269 6e67 0d0a 0d0a 2020 2020 7375  string....    su
+00008cd0: 6d6d 616e 6420 3d20 696e 7075 745f 7374  mmand = input_st
+00008ce0: 7269 6e67 2e72 6570 6c61 6365 2822 2c22  ring.replace(","
+00008cf0: 2c22 2229 0d0a 0d0a 2020 2020 6f62 6a5f  ,"")....    obj_
+00008d00: 696e 6465 785f 6c69 7374 203d 2069 6e70  index_list = inp
+00008d10: 7574 5f73 7472 696e 672e 7370 6c69 7428  ut_string.split(
+00008d20: 222c 2229 0d0a 2020 2020 6e6f 626a 203d  ",")..    nobj =
+00008d30: 206c 656e 286f 626a 5f69 6e64 6578 5f6c   len(obj_index_l
+00008d40: 6973 7429 0d0a 0d0a 2020 2020 6f62 6a5f  ist)....    obj_
+00008d50: 6c69 7374 203d 206d 616b 655f 6c69 7374  list = make_list
+00008d60: 2861 7267 735b 313a 312b 6e6f 626a 5d29  (args[1:1+nobj])
+00008d70: 0d0a 2020 2020 7374 6174 735f 6c69 7374  ..    stats_list
+00008d80: 203d 2073 756d 285b 206d 616b 655f 6c69   = sum([ make_li
+00008d90: 7374 286f 626a 2e73 7461 7469 7374 6963  st(obj.statistic
+00008da0: 2920 666f 7220 6f62 6a20 696e 206f 626a  ) for obj in obj
+00008db0: 5f6c 6973 7420 5d2c 5b5d 290d 0a20 2020  _list ],[])..   
+00008dc0: 2073 6861 7065 5f6c 6973 7420 3d20 7375   shape_list = su
+00008dd0: 6d28 5b20 6d61 6b65 5f6c 6973 7428 6f62  m([ make_list(ob
+00008de0: 6a2e 7368 6170 6529 2066 6f72 206f 626a  j.shape) for obj
+00008df0: 2069 6e20 6f62 6a5f 6c69 7374 205d 2c5b   in obj_list ],[
+00008e00: 5d29 0d0a 0d0a 2020 2020 2320 666f 7263  ])....    # forc
+00008e10: 6520 6576 6572 7974 6869 6e67 2074 6f20  e everything to 
+00008e20: 6265 2063 616e 6f6e 6963 616c 2061 6e64  be canonical and
+00008e30: 2073 7461 6e64 6172 6420 2d2d 2d2d 2d2d   standard ------
+00008e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020  -----------..   
+00008e70: 2023 2061 6c73 6f20 666f 7263 6520 6576   # also force ev
+00008e80: 6572 7974 6869 6e67 2074 6f20 6265 206f  erything to be o
+00008e90: 6620 7468 6520 7361 6d65 2074 7970 650d  f the same type.
+00008ea0: 0a0d 0a20 2020 2074 6869 735f 7479 7065  ...    this_type
+00008eb0: 203d 2074 7970 6528 6f62 6a5f 6c69 7374   = type(obj_list
+00008ec0: 5b30 5d29 0d0a 2020 2020 7468 6973 5f65  [0])..    this_e
+00008ed0: 6e63 6f64 6572 203d 206f 626a 5f6c 6973  ncoder = obj_lis
+00008ee0: 745b 305d 2e65 6e63 6f64 6572 0d0a 2020  t[0].encoder..  
+00008ef0: 2020 7468 6973 5f66 6f72 6d61 7420 3d20    this_format = 
+00008f00: 6f62 6a5f 6c69 7374 5b30 5d2e 666f 726d  obj_list[0].form
+00008f10: 6174 0d0a 2020 2020 666f 7220 6920 696e  at..    for i in
+00008f20: 2072 616e 6765 286c 656e 286f 626a 5f6c   range(len(obj_l
+00008f30: 6973 7429 293a 0d0a 2020 2020 2020 2020  ist)):..        
+00008f40: 6f62 6a5f 6c69 7374 5b69 5d20 3d20 7468  obj_list[i] = th
+00008f50: 6973 5f74 7970 6528 6f62 6a5f 6c69 7374  is_type(obj_list
+00008f60: 5b69 5d2e 666f 7263 655f 656e 636f 6465  [i].force_encode
+00008f70: 7228 2763 616e 6f6e 6963 616c 2729 2e66  r('canonical').f
+00008f80: 6f72 6365 5f66 6f72 6d61 7428 2773 7461  orce_format('sta
+00008f90: 6e64 6172 6427 2929 2e64 6174 610d 0a0d  ndard')).data...
+00008fa0: 0a20 2020 2023 2067 6574 2073 6f6d 6520  .    # get some 
+00008fb0: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
+00008fc0: 7420 7468 6520 7375 6d6d 6564 2069 6e64  t the summed ind
+00008fd0: 6963 6573 202d 2d2d 2d2d 2d2d 2d2d 2d2d  ices -----------
+00008fe0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00008ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009020: 2d0d 0a20 2020 2023 205b 2066 3d3c 6368  -..    # [ f=<ch
-00009030: 6172 3e2c 205b 696e 6465 7820 6c6f 6361  ar>, [index loca
-00009040: 7469 6f6e 7320 696e 206c 665d 2c20 5b73  tions in lf], [s
-00009050: 7461 7469 7374 6963 735d 205d 0d0a 2020  tatistics] ]..  
-00009060: 2020 7375 6d6d 6564 5f69 6e64 6578 5f69    summed_index_i
-00009070: 6e66 6f20 3d20 5b5d 0d0a 0d0a 2020 2020  nfo = []....    
-00009080: 666f 7220 692c 6368 6172 2069 6e20 656e  for i,char in en
-00009090: 756d 6572 6174 6528 7375 6d6d 616e 6429  umerate(summand)
-000090a0: 3a0d 0a0d 0a20 2020 2020 2020 2023 2073  :....        # s
-000090b0: 6b69 7020 6966 2062 6f73 6f6e 6963 0d0a  kip if bosonic..
-000090c0: 2020 2020 2020 2020 6966 2073 7461 7473          if stats
-000090d0: 5f6c 6973 745b 695d 2069 6e20 626f 7365  _list[i] in bose
-000090e0: 5f74 7970 653a 0d0a 2020 2020 2020 2020  _type:..        
-000090f0: 2020 2020 636f 6e74 696e 7565 0d0a 0d0a      continue....
-00009100: 2020 2020 2020 2020 6c66 203d 2020 696e          lf =  in
-00009110: 7075 745f 7374 7269 6e67 2e63 6f75 6e74  put_string.count
-00009120: 2863 6861 7229 0d0a 2020 2020 2020 2020  (char)..        
-00009130: 6966 2068 6173 5f6f 7574 7075 7420 3a0d  if has_output :.
-00009140: 0a20 2020 2020 2020 2020 2020 2072 6620  .            rf 
-00009150: 3d20 6f75 7470 7574 5f73 7472 696e 672e  = output_string.
-00009160: 636f 756e 7428 6368 6172 290d 0a20 2020  count(char)..   
-00009170: 2020 2020 2020 2020 2069 6620 6c66 3e32           if lf>2
-00009180: 206f 7220 7266 3e31 206f 7220 286c 662b   or rf>1 or (lf+
-00009190: 7266 2925 323d 3d31 203a 0d0a 2020 2020  rf)%2==1 :..    
-000091a0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-000091b0: 663e 3220 3a0d 0a20 2020 2020 2020 2020  f>2 :..         
-000091c0: 2020 2020 2020 2020 2020 2072 6561 736f             reaso
-000091d0: 6e20 3d20 226c 663e 3222 0d0a 2020 2020  n = "lf>2"..    
-000091e0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000091f0: 2072 663e 3120 3a0d 0a20 2020 2020 2020   rf>1 :..       
-00009200: 2020 2020 2020 2020 2020 2020 2072 6561               rea
-00009210: 736f 6e20 3d20 2272 663e 3122 0d0a 2020  son = "rf>1"..  
-00009220: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00009230: 7365 203a 0d0a 2020 2020 2020 2020 2020  se :..          
-00009240: 2020 2020 2020 2020 2020 7265 6173 6f6e            reason
-00009250: 203d 2022 286c 662b 7266 2925 323d 3d31   = "(lf+rf)%2==1
-00009260: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-00009270: 2020 2065 7272 6f72 2822 4572 726f 725b     error("Error[
-00009280: 6569 6e73 756d 5d3a 2049 6e63 6f6e 7369  einsum]: Inconsi
-00009290: 7374 656e 7420 696e 6465 7820 7374 6174  stent index stat
-000092a0: 6973 7469 6373 2e20 2872 6561 736f 6e3a  istics. (reason:
-000092b0: 222b 7265 6173 6f6e 2b22 2922 290d 0a20  "+reason+")").. 
-000092c0: 2020 2020 2020 2065 6c73 6520 3a0d 0a20         else :.. 
-000092d0: 2020 2020 2020 2020 2020 2069 6620 6c66             if lf
-000092e0: 3e32 3a0d 0a20 2020 2020 2020 2020 2020  >2:..           
-000092f0: 2020 2020 2072 6561 736f 6e20 3d20 226c       reason = "l
-00009300: 663e 3222 0d0a 2020 2020 2020 2020 2020  f>2"..          
-00009310: 2020 2020 2020 6572 726f 7228 2245 7272        error("Err
-00009320: 6f72 5b65 696e 7375 6d5d 3a20 496e 636f  or[einsum]: Inco
-00009330: 6e73 6973 7465 6e74 2069 6e64 6578 2073  nsistent index s
-00009340: 7461 7469 7374 6963 732e 2028 7265 6173  tatistics. (reas
-00009350: 6f6e 3a22 2b72 6561 736f 6e2b 2229 2229  on:"+reason+")")
-00009360: 0d0a 0d0a 2020 2020 2020 2020 6966 206c  ....        if l
-00009370: 663d 3d31 3a0d 0a20 2020 2020 2020 2020  f==1:..         
-00009380: 2020 2063 6f6e 7469 6e75 650d 0a0d 0a20     continue.... 
-00009390: 2020 2020 2020 2023 2061 6464 2061 206e         # add a n
-000093a0: 6577 2065 6e74 7279 2069 6620 6974 2069  ew entry if it i
-000093b0: 7320 6120 6e65 7720 6368 6172 6163 7465  s a new characte
-000093c0: 720d 0a20 2020 2020 2020 2069 6620 7375  r..        if su
-000093d0: 6d6d 616e 645b 3a69 5d2e 636f 756e 7428  mmand[:i].count(
-000093e0: 6368 6172 293d 3d30 203a 0d0a 2020 2020  char)==0 :..    
-000093f0: 2020 2020 2020 2020 7375 6d6d 6564 5f69          summed_i
-00009400: 6e64 6578 5f69 6e66 6f20 2b3d 205b 205b  ndex_info += [ [
-00009410: 2063 6861 722c 205b 695d 202c 205b 7374   char, [i] , [st
-00009420: 6174 735f 6c69 7374 5b69 5d5d 205d 205d  ats_list[i]] ] ]
-00009430: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00009440: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00009450: 206b 2069 6e20 7261 6e67 6528 6c65 6e28   k in range(len(
-00009460: 7375 6d6d 6564 5f69 6e64 6578 5f69 6e66  summed_index_inf
-00009470: 6f29 293a 0d0a 2020 2020 2020 2020 2020  o)):..          
-00009480: 2020 2020 2020 6966 2873 756d 6d65 645f        if(summed_
-00009490: 696e 6465 785f 696e 666f 5b6b 5d5b 305d  index_info[k][0]
-000094a0: 3d3d 6368 6172 293a 0d0a 2020 2020 2020  ==char):..      
-000094b0: 2020 2020 2020 2020 2020 2020 2020 7375                su
-000094c0: 6d6d 6564 5f69 6e64 6578 5f69 6e66 6f5b  mmed_index_info[
-000094d0: 6b5d 5b31 5d20 2b3d 205b 695d 0d0a 2020  k][1] += [i]..  
-000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094f0: 2020 7375 6d6d 6564 5f69 6e64 6578 5f69    summed_index_i
-00009500: 6e66 6f5b 6b5d 5b32 5d20 2b3d 205b 7374  nfo[k][2] += [st
-00009510: 6174 735f 6c69 7374 5b69 5d5d 0d0a 0d0a  ats_list[i]]....
-00009520: 2020 2020 6465 6620 6973 5f73 7461 7477      def is_statw
-00009530: 6973 655f 696e 636f 6e73 6973 7465 6e74  ise_inconsistent
-00009540: 2873 7461 7431 2c73 7461 7432 293a 0d0a  (stat1,stat2):..
-00009550: 2020 2020 2020 2020 6966 205b 7374 6174          if [stat
-00009560: 312c 7374 6174 325d 203d 3d20 5b30 2c30  1,stat2] == [0,0
-00009570: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
-00009580: 7265 7475 726e 2046 616c 7365 0d0a 2020  return False..  
-00009590: 2020 2020 2020 656c 6966 205b 7374 6174        elif [stat
-000095a0: 312c 7374 6174 325d 203d 3d20 5b31 2c2d  1,stat2] == [1,-
-000095b0: 315d 3a0d 0a20 2020 2020 2020 2020 2020  1]:..           
-000095c0: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
-000095d0: 2020 2020 2020 2065 6c69 6620 5b73 7461         elif [sta
-000095e0: 7431 2c73 7461 7432 5d20 3d3d 205b 2d31  t1,stat2] == [-1
-000095f0: 2c31 5d3a 0d0a 2020 2020 2020 2020 2020  ,1]:..          
-00009600: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
-00009610: 2020 2020 2020 2020 656c 6966 205b 7374          elif [st
-00009620: 6174 312c 7374 6174 325d 203d 3d20 5b68  at1,stat2] == [h
-00009630: 7962 7269 645f 7379 6d62 6f6c 2c68 7962  ybrid_symbol,hyb
-00009640: 7269 645f 7379 6d62 6f6c 5d3a 0d0a 2020  rid_symbol]:..  
-00009650: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009660: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00009670: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00009680: 2020 2072 6574 7572 6e20 5472 7565 0d0a     return True..
-00009690: 0d0a 2020 2020 666f 7220 5b63 6861 722c  ..    for [char,
-000096a0: 6c6f 6361 7469 6f6e 2c73 7461 7473 5d20  location,stats] 
-000096b0: 696e 2073 756d 6d65 645f 696e 6465 785f  in summed_index_
-000096c0: 696e 666f 3a0d 0a20 2020 2020 2020 2069  info:..        i
-000096d0: 6620 6c65 6e28 7374 6174 7329 3d3d 3220  f len(stats)==2 
-000096e0: 616e 6420 6973 5f73 7461 7477 6973 655f  and is_statwise_
-000096f0: 696e 636f 6e73 6973 7465 6e74 2873 7461  inconsistent(sta
-00009700: 7473 5b30 5d2c 7374 6174 735b 315d 293a  ts[0],stats[1]):
-00009710: 0d0a 2020 2020 2020 2020 2020 2020 6572  ..            er
-00009720: 726f 7228 2245 7272 6f72 5b65 696e 7375  ror("Error[einsu
-00009730: 6d5d 3a20 5468 6520 636f 6e74 7261 6374  m]: The contract
-00009740: 6564 2069 6e64 6963 6573 2068 6176 6520  ed indices have 
-00009750: 696e 636f 6e73 6973 7465 6e74 2073 7461  inconsistent sta
-00009760: 7469 7374 6963 2122 290d 0a20 2020 200d  tistic!")..    .
-00009770: 0a20 2020 2069 6620 6465 6275 675f 6d6f  .    if debug_mo
-00009780: 6465 203a 0d0a 2020 2020 2020 2020 7072  de :..        pr
-00009790: 696e 7428 290d 0a20 2020 2020 2020 2070  int()..        p
-000097a0: 7269 6e74 2822 696e 7075 743a 222c 696e  rint("input:",in
-000097b0: 7374 7275 6374 696f 6e5f 7374 7269 6e67  struction_string
-000097c0: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-000097d0: 2822 6f62 6a20 696e 6469 6365 733a 2229  ("obj indices:")
-000097e0: 0d0a 2020 2020 2020 2020 666f 7220 656c  ..        for el
-000097f0: 656d 2069 6e20 6f62 6a5f 696e 6465 785f  em in obj_index_
-00009800: 6c69 7374 3a0d 0a20 2020 2020 2020 2020  list:..         
-00009810: 2020 2070 7269 6e74 2822 2022 2c65 6c65     print(" ",ele
-00009820: 6d29 0d0a 2020 2020 0d0a 2020 2020 233a  m)..    ..    #:
+00009000: 2d2d 2d2d 2d2d 0d0a 2020 2020 2320 5b20  ------..    # [ 
+00009010: 663d 3c63 6861 723e 2c20 5b69 6e64 6578  f=<char>, [index
+00009020: 206c 6f63 6174 696f 6e73 2069 6e20 6c66   locations in lf
+00009030: 5d2c 205b 7374 6174 6973 7469 6373 5d20  ], [statistics] 
+00009040: 5d0d 0a20 2020 2073 756d 6d65 645f 696e  ]..    summed_in
+00009050: 6465 785f 696e 666f 203d 205b 5d0d 0a0d  dex_info = []...
+00009060: 0a20 2020 2066 6f72 2069 2c63 6861 7220  .    for i,char 
+00009070: 696e 2065 6e75 6d65 7261 7465 2873 756d  in enumerate(sum
+00009080: 6d61 6e64 293a 0d0a 0d0a 2020 2020 2020  mand):....      
+00009090: 2020 2320 736b 6970 2069 6620 626f 736f    # skip if boso
+000090a0: 6e69 630d 0a20 2020 2020 2020 2069 6620  nic..        if 
+000090b0: 7374 6174 735f 6c69 7374 5b69 5d20 696e  stats_list[i] in
+000090c0: 2062 6f73 655f 7479 7065 3a0d 0a20 2020   bose_type:..   
+000090d0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+000090e0: 650d 0a0d 0a20 2020 2020 2020 206c 6620  e....        lf 
+000090f0: 3d20 2069 6e70 7574 5f73 7472 696e 672e  =  input_string.
+00009100: 636f 756e 7428 6368 6172 290d 0a20 2020  count(char)..   
+00009110: 2020 2020 2069 6620 6861 735f 6f75 7470       if has_outp
+00009120: 7574 203a 0d0a 2020 2020 2020 2020 2020  ut :..          
+00009130: 2020 7266 203d 206f 7574 7075 745f 7374    rf = output_st
+00009140: 7269 6e67 2e63 6f75 6e74 2863 6861 7229  ring.count(char)
+00009150: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00009160: 206c 663e 3220 6f72 2072 663e 3120 6f72   lf>2 or rf>1 or
+00009170: 2028 6c66 2b72 6629 2532 3d3d 3120 3a0d   (lf+rf)%2==1 :.
+00009180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009190: 2069 6620 6c66 3e32 203a 0d0a 2020 2020   if lf>2 :..    
+000091a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091b0: 7265 6173 6f6e 203d 2022 6c66 3e32 220d  reason = "lf>2".
+000091c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000091d0: 2065 6c69 6620 7266 3e31 203a 0d0a 2020   elif rf>1 :..  
+000091e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091f0: 2020 7265 6173 6f6e 203d 2022 7266 3e31    reason = "rf>1
+00009200: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+00009210: 2020 2065 6c73 6520 3a0d 0a20 2020 2020     else :..     
+00009220: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00009230: 6561 736f 6e20 3d20 2228 6c66 2b72 6629  eason = "(lf+rf)
+00009240: 2532 3d3d 3122 0d0a 2020 2020 2020 2020  %2==1"..        
+00009250: 2020 2020 2020 2020 6572 726f 7228 2245          error("E
+00009260: 7272 6f72 5b65 696e 7375 6d5d 3a20 496e  rror[einsum]: In
+00009270: 636f 6e73 6973 7465 6e74 2069 6e64 6578  consistent index
+00009280: 2073 7461 7469 7374 6963 732e 2028 7265   statistics. (re
+00009290: 6173 6f6e 3a22 2b72 6561 736f 6e2b 2229  ason:"+reason+")
+000092a0: 2229 0d0a 2020 2020 2020 2020 656c 7365  ")..        else
+000092b0: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
+000092c0: 6966 206c 663e 323a 0d0a 2020 2020 2020  if lf>2:..      
+000092d0: 2020 2020 2020 2020 2020 7265 6173 6f6e            reason
+000092e0: 203d 2022 6c66 3e32 220d 0a20 2020 2020   = "lf>2"..     
+000092f0: 2020 2020 2020 2020 2020 2065 7272 6f72             error
+00009300: 2822 4572 726f 725b 6569 6e73 756d 5d3a  ("Error[einsum]:
+00009310: 2049 6e63 6f6e 7369 7374 656e 7420 696e   Inconsistent in
+00009320: 6465 7820 7374 6174 6973 7469 6373 2e20  dex statistics. 
+00009330: 2872 6561 736f 6e3a 222b 7265 6173 6f6e  (reason:"+reason
+00009340: 2b22 2922 290d 0a0d 0a20 2020 2020 2020  +")")....       
+00009350: 2069 6620 6c66 3d3d 313a 0d0a 2020 2020   if lf==1:..    
+00009360: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00009370: 0d0a 0d0a 2020 2020 2020 2020 2320 6164  ....        # ad
+00009380: 6420 6120 6e65 7720 656e 7472 7920 6966  d a new entry if
+00009390: 2069 7420 6973 2061 206e 6577 2063 6861   it is a new cha
+000093a0: 7261 6374 6572 0d0a 2020 2020 2020 2020  racter..        
+000093b0: 6966 2073 756d 6d61 6e64 5b3a 695d 2e63  if summand[:i].c
+000093c0: 6f75 6e74 2863 6861 7229 3d3d 3020 3a0d  ount(char)==0 :.
+000093d0: 0a20 2020 2020 2020 2020 2020 2073 756d  .            sum
+000093e0: 6d65 645f 696e 6465 785f 696e 666f 202b  med_index_info +
+000093f0: 3d20 5b20 5b20 6368 6172 2c20 5b69 5d20  = [ [ char, [i] 
+00009400: 2c20 5b73 7461 7473 5f6c 6973 745b 695d  , [stats_list[i]
+00009410: 5d20 5d20 5d0d 0a20 2020 2020 2020 2065  ] ] ]..        e
+00009420: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00009430: 2020 666f 7220 6b20 696e 2072 616e 6765    for k in range
+00009440: 286c 656e 2873 756d 6d65 645f 696e 6465  (len(summed_inde
+00009450: 785f 696e 666f 2929 3a0d 0a20 2020 2020  x_info)):..     
+00009460: 2020 2020 2020 2020 2020 2069 6628 7375             if(su
+00009470: 6d6d 6564 5f69 6e64 6578 5f69 6e66 6f5b  mmed_index_info[
+00009480: 6b5d 5b30 5d3d 3d63 6861 7229 3a0d 0a20  k][0]==char):.. 
+00009490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094a0: 2020 2073 756d 6d65 645f 696e 6465 785f     summed_index_
+000094b0: 696e 666f 5b6b 5d5b 315d 202b 3d20 5b69  info[k][1] += [i
+000094c0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+000094d0: 2020 2020 2020 2073 756d 6d65 645f 696e         summed_in
+000094e0: 6465 785f 696e 666f 5b6b 5d5b 325d 202b  dex_info[k][2] +
+000094f0: 3d20 5b73 7461 7473 5f6c 6973 745b 695d  = [stats_list[i]
+00009500: 5d0d 0a0d 0a20 2020 2064 6566 2069 735f  ]....    def is_
+00009510: 7374 6174 7769 7365 5f69 6e63 6f6e 7369  statwise_inconsi
+00009520: 7374 656e 7428 7374 6174 312c 7374 6174  stent(stat1,stat
+00009530: 3229 3a0d 0a20 2020 2020 2020 2069 6620  2):..        if 
+00009540: 5b73 7461 7431 2c73 7461 7432 5d20 3d3d  [stat1,stat2] ==
+00009550: 205b 302c 305d 3a0d 0a20 2020 2020 2020   [0,0]:..       
+00009560: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00009570: 650d 0a20 2020 2020 2020 2065 6c69 6620  e..        elif 
+00009580: 5b73 7461 7431 2c73 7461 7432 5d20 3d3d  [stat1,stat2] ==
+00009590: 205b 312c 2d31 5d3a 0d0a 2020 2020 2020   [1,-1]:..      
+000095a0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+000095b0: 7365 0d0a 2020 2020 2020 2020 656c 6966  se..        elif
+000095c0: 205b 7374 6174 312c 7374 6174 325d 203d   [stat1,stat2] =
+000095d0: 3d20 5b2d 312c 315d 3a0d 0a20 2020 2020  = [-1,1]:..     
+000095e0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+000095f0: 6c73 650d 0a20 2020 2020 2020 2065 6c69  lse..        eli
+00009600: 6620 5b73 7461 7431 2c73 7461 7432 5d20  f [stat1,stat2] 
+00009610: 3d3d 205b 6879 6272 6964 5f73 796d 626f  == [hybrid_symbo
+00009620: 6c2c 6879 6272 6964 5f73 796d 626f 6c5d  l,hybrid_symbol]
+00009630: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00009640: 6574 7572 6e20 4661 6c73 650d 0a20 2020  eturn False..   
+00009650: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00009660: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+00009670: 7275 650d 0a0d 0a20 2020 2066 6f72 205b  rue....    for [
+00009680: 6368 6172 2c6c 6f63 6174 696f 6e2c 7374  char,location,st
+00009690: 6174 735d 2069 6e20 7375 6d6d 6564 5f69  ats] in summed_i
+000096a0: 6e64 6578 5f69 6e66 6f3a 0d0a 2020 2020  ndex_info:..    
+000096b0: 2020 2020 6966 206c 656e 2873 7461 7473      if len(stats
+000096c0: 293d 3d32 2061 6e64 2069 735f 7374 6174  )==2 and is_stat
+000096d0: 7769 7365 5f69 6e63 6f6e 7369 7374 656e  wise_inconsisten
+000096e0: 7428 7374 6174 735b 305d 2c73 7461 7473  t(stats[0],stats
+000096f0: 5b31 5d29 3a0d 0a20 2020 2020 2020 2020  [1]):..         
+00009700: 2020 2065 7272 6f72 2822 4572 726f 725b     error("Error[
+00009710: 6569 6e73 756d 5d3a 2054 6865 2063 6f6e  einsum]: The con
+00009720: 7472 6163 7465 6420 696e 6469 6365 7320  tracted indices 
+00009730: 6861 7665 2069 6e63 6f6e 7369 7374 656e  have inconsisten
+00009740: 7420 7374 6174 6973 7469 6321 2229 0d0a  t statistic!")..
+00009750: 2020 2020 0d0a 2020 2020 6966 2064 6562      ..    if deb
+00009760: 7567 5f6d 6f64 6520 3a0d 0a20 2020 2020  ug_mode :..     
+00009770: 2020 2070 7269 6e74 2829 0d0a 2020 2020     print()..    
+00009780: 2020 2020 7072 696e 7428 2269 6e70 7574      print("input
+00009790: 3a22 2c69 6e73 7472 7563 7469 6f6e 5f73  :",instruction_s
+000097a0: 7472 696e 6729 0d0a 2020 2020 2020 2020  tring)..        
+000097b0: 7072 696e 7428 226f 626a 2069 6e64 6963  print("obj indic
+000097c0: 6573 3a22 290d 0a20 2020 2020 2020 2066  es:")..        f
+000097d0: 6f72 2065 6c65 6d20 696e 206f 626a 5f69  or elem in obj_i
+000097e0: 6e64 6578 5f6c 6973 743a 0d0a 2020 2020  ndex_list:..    
+000097f0: 2020 2020 2020 2020 7072 696e 7428 2220          print(" 
+00009800: 222c 656c 656d 290d 0a20 2020 200d 0a20  ",elem)..    .. 
+00009810: 2020 2023 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a     #::::::::::::
+00009820: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00009830: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00009840: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00009850: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00009860: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00009870: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00009880: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a0d  :::::::::::::::.
-00009890: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
-000098a0: 2020 2020 5374 6570 2031 3a20 7265 706c      Step 1: repl
-000098b0: 6163 6520 7468 6520 636f 6e6a 7567 6174  ace the conjugat
-000098c0: 6564 2076 6172 6961 626c 6527 7320 696e  ed variable's in
-000098d0: 6465 7820 7769 7468 2061 206e 6577 2063  dex with a new c
-000098e0: 6861 7261 6374 6572 0d0a 2020 2020 2320  haracter..    # 
-000098f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009900: 2020 2020 2061 6e64 2072 656d 6f76 6520       and remove 
-00009910: 626f 736f 6e69 6320 7374 7269 6e67 0d0a  bosonic string..
-00009920: 2020 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a      #:::::::::::
+00009870: 3a3a 3a3a 0d0a 2020 2020 2320 2020 2020  ::::..    #     
+00009880: 2020 2020 2020 2020 2053 7465 7020 313a           Step 1:
+00009890: 2072 6570 6c61 6365 2074 6865 2063 6f6e   replace the con
+000098a0: 6a75 6761 7465 6420 7661 7269 6162 6c65  jugated variable
+000098b0: 2773 2069 6e64 6578 2077 6974 6820 6120  's index with a 
+000098c0: 6e65 7720 6368 6172 6163 7465 720d 0a20  new character.. 
+000098d0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+000098e0: 2020 2020 2020 2020 2020 616e 6420 7265            and re
+000098f0: 6d6f 7665 2062 6f73 6f6e 6963 2073 7472  move bosonic str
+00009900: 696e 670d 0a20 2020 2023 3a3a 3a3a 3a3a  ing..    #::::::
+00009910: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00009920: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00009930: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00009940: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00009950: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00009960: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00009970: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00009980: 3a3a 3a3a 3a0d 0a0d 0a20 2020 2066 7375  :::::....    fsu
-00009990: 6d6d 616e 6420 2020 3d20 2222 0d0a 2020  mmand   = ""..  
-000099a0: 2020 6673 756d 6d61 6e64 5f75 203d 2022    fsummand_u = "
-000099b0: 220d 0a20 2020 2066 7374 6174 735f 6c69  "..    fstats_li
-000099c0: 7374 203d 205b 5d0d 0a20 2020 2066 7368  st = []..    fsh
-000099d0: 6170 655f 6c69 7374 203d 205b 5d0d 0a20  ape_list = [].. 
-000099e0: 2020 2063 6861 726c 6973 7420 3d20 7375     charlist = su
-000099f0: 6d6d 616e 640d 0a20 2020 2066 6f72 2069  mmand..    for i
-00009a00: 2c63 6861 7220 696e 2065 6e75 6d65 7261  ,char in enumera
-00009a10: 7465 2873 756d 6d61 6e64 293a 0d0a 2020  te(summand):..  
-00009a20: 2020 2020 2020 6966 2073 7461 7473 5f6c        if stats_l
-00009a30: 6973 745b 695d 203d 3d20 303a 0d0a 2020  ist[i] == 0:..  
-00009a40: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00009a50: 7565 0d0a 0d0a 2020 2020 2020 2020 6673  ue....        fs
-00009a60: 756d 6d61 6e64 2020 2020 2b3d 2063 6861  ummand    += cha
-00009a70: 720d 0a20 2020 2020 2020 2066 7374 6174  r..        fstat
-00009a80: 735f 6c69 7374 202b 3d20 7374 6174 735f  s_list += stats_
-00009a90: 6c69 7374 5b69 5d2c 0d0a 2020 2020 2020  list[i],..      
-00009aa0: 2020 6673 6861 7065 5f6c 6973 7420 2b3d    fshape_list +=
-00009ab0: 2073 6861 7065 5f6c 6973 745b 695d 2c0d   shape_list[i],.
-00009ac0: 0a0d 0a20 2020 2020 2020 2069 6620 7374  ...        if st
-00009ad0: 6174 735f 6c69 7374 5b69 5d20 3d3d 202d  ats_list[i] == -
-00009ae0: 3120 616e 6420 7375 6d6d 616e 642e 636f  1 and summand.co
-00009af0: 756e 7428 6368 6172 293e 313a 0d0a 2020  unt(char)>1:..  
-00009b00: 2020 2020 2020 2020 2020 6e65 775f 6368            new_ch
-00009b10: 6172 203d 2067 6574 5f63 6861 7228 6368  ar = get_char(ch
-00009b20: 6172 6c69 7374 290d 0a20 2020 2020 2020  arlist)..       
-00009b30: 2020 2020 2063 6861 726c 6973 7420 2b3d       charlist +=
-00009b40: 206e 6577 5f63 6861 720d 0a20 2020 2020   new_char..     
-00009b50: 2020 2020 2020 2066 7375 6d6d 616e 645f         fsummand_
-00009b60: 7520 2b3d 206e 6577 5f63 6861 720d 0a0d  u += new_char...
-00009b70: 0a20 2020 2020 2020 2020 2020 2023 2065  .            # e
-00009b80: 6469 7420 7468 6520 7375 6d6d 6564 5f69  dit the summed_i
-00009b90: 6e64 6578 5f69 6e66 6f2c 2077 6974 6820  ndex_info, with 
-00009ba0: 7468 6520 706f 7369 7469 6f6e 2073 7761  the position swa
-00009bb0: 7070 6564 2061 206c 6974 746c 6520 6269  pped a little bi
-00009bc0: 7420 6173 2077 656c 6c0d 0a20 2020 2020  t as well..     
-00009bd0: 2020 2020 2020 2066 6f72 206a 2c5b 6368         for j,[ch
-00009be0: 6172 322c 6c6f 6361 7469 6f6e 2c73 7461  ar2,location,sta
-00009bf0: 7473 5d20 696e 2065 6e75 6d65 7261 7465  ts] in enumerate
-00009c00: 2873 756d 6d65 645f 696e 6465 785f 696e  (summed_index_in
-00009c10: 666f 293a 0d0a 2020 2020 2020 2020 2020  fo):..          
-00009c20: 2020 2020 2020 6966 2063 6861 7232 3d3d        if char2==
-00009c30: 6368 6172 203a 0d0a 2020 2020 2020 2020  char :..        
-00009c40: 2020 2020 2020 2020 2020 2020 7375 6d6d              summ
-00009c50: 6564 5f69 6e64 6578 5f69 6e66 6f5b 6a5d  ed_index_info[j]
-00009c60: 5b30 5d20 3d20 5b63 6861 722c 6e65 775f  [0] = [char,new_
-00009c70: 6368 6172 5d0d 0a20 2020 2020 2020 2020  char]..         
-00009c80: 2020 2020 2020 2020 2020 2069 6620 7374             if st
-00009c90: 6174 7320 3d3d 205b 2d31 2c31 5d3a 0d0a  ats == [-1,1]:..
-00009ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cb0: 2020 2020 2020 2020 7375 6d6d 6564 5f69          summed_i
-00009cc0: 6e64 6578 5f69 6e66 6f5b 6a5d 5b31 5d20  ndex_info[j][1] 
-00009cd0: 3d20 5b20 7375 6d6d 6564 5f69 6e64 6578  = [ summed_index
-00009ce0: 5f69 6e66 6f5b 6a5d 5b31 5d5b 315d 2c20  _info[j][1][1], 
-00009cf0: 7375 6d6d 6564 5f69 6e64 6578 5f69 6e66  summed_index_inf
-00009d00: 6f5b 6a5d 5b31 5d5b 305d 205d 0d0a 2020  o[j][1][0] ]..  
-00009d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d20: 2020 2020 2020 7375 6d6d 6564 5f69 6e64        summed_ind
-00009d30: 6578 5f69 6e66 6f5b 6a5d 5b32 5d20 3d20  ex_info[j][2] = 
-00009d40: 5b20 7375 6d6d 6564 5f69 6e64 6578 5f69  [ summed_index_i
-00009d50: 6e66 6f5b 6a5d 5b32 5d5b 315d 2c20 7375  nfo[j][2][1], su
-00009d60: 6d6d 6564 5f69 6e64 6578 5f69 6e66 6f5b  mmed_index_info[
-00009d70: 6a5d 5b32 5d5b 305d 205d 0d0a 2020 2020  j][2][0] ]..    
-00009d80: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00009d90: 2020 2020 2020 2066 7375 6d6d 616e 645f         fsummand_
-00009da0: 7520 2b3d 2063 6861 720d 0a20 2020 2066  u += char..    f
-00009db0: 7374 6174 7320 3d20 6673 7461 7473 5f6c  stats = fstats_l
-00009dc0: 6973 742e 636f 7079 2829 0d0a 2020 2020  ist.copy()..    
-00009dd0: 6673 6861 7065 203d 2066 7368 6170 655f  fshape = fshape_
-00009de0: 6c69 7374 2e63 6f70 7928 290d 0a20 2020  list.copy()..   
-00009df0: 2066 7374 6174 735f 7520 3d20 6673 7461   fstats_u = fsta
-00009e00: 7473 5f6c 6973 742e 636f 7079 2829 0d0a  ts_list.copy()..
-00009e10: 2020 2020 6673 6861 7065 5f75 203d 2066      fshape_u = f
-00009e20: 7368 6170 655f 6c69 7374 2e63 6f70 7928  shape_list.copy(
-00009e30: 290d 0a0d 0a20 2020 2023 2072 656d 6f76  )....    # remov
-00009e40: 6520 7468 6520 7374 6174 2065 6e74 7279  e the stat entry
-00009e50: 2061 7320 6974 2069 7320 7265 6475 6e64   as it is redund
-00009e60: 616e 740d 0a20 2020 2066 6f72 2069 2c65  ant..    for i,e
-00009e70: 6c65 6d20 696e 2065 6e75 6d65 7261 7465  lem in enumerate
-00009e80: 2873 756d 6d65 645f 696e 6465 785f 696e  (summed_index_in
-00009e90: 666f 293a 0d0a 2020 2020 2020 2020 7375  fo):..        su
-00009ea0: 6d6d 6564 5f69 6e64 6578 5f69 6e66 6f5b  mmed_index_info[
-00009eb0: 695d 203d 2065 6c65 6d5b 3a32 5d0d 0a0d  i] = elem[:2]...
-00009ec0: 0a20 2020 2069 6620 6465 6275 675f 6d6f  .    if debug_mo
-00009ed0: 6465 203a 0d0a 2020 2020 2020 2020 7072  de :..        pr
-00009ee0: 696e 7428 290d 0a20 2020 2020 2020 2070  int()..        p
-00009ef0: 7269 6e74 2822 203a 3a3a 3a3a 3a3a 3a3a  rint(" :::::::::
-00009f00: 3a20 7265 706c 6163 6520 636f 6e6a 7567  : replace conjug
-00009f10: 6174 6564 2069 6e64 6963 6573 2062 7920  ated indices by 
-00009f20: 756e 6971 7565 2063 6861 7261 6374 6572  unique character
-00009f30: 7320 3a3a 3a3a 3a3a 3a3a 3a3a 2022 290d  s :::::::::: ").
-00009f40: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
-00009f50: 7375 6d6d 616e 642c 223c 2d2d 2d20 6673  summand,"<--- fs
-00009f60: 756d 6d61 6e64 203d 206f 7269 6769 6e61  ummand = origina
-00009f70: 6c20 696e 6469 6365 7322 290d 0a20 2020  l indices")..   
-00009f80: 2020 2020 2070 7269 6e74 2866 7375 6d6d       print(fsumm
-00009f90: 616e 645f 752c 223c 2d2d 2d20 6673 756d  and_u,"<--- fsum
-00009fa0: 6d61 6e64 5f75 203d 2072 6570 6c61 6365  mand_u = replace
-00009fb0: 2063 6f6e 6a75 6761 7465 6420 696e 6469   conjugated indi
-00009fc0: 6365 7320 6279 2075 6e69 7175 6520 6368  ces by unique ch
-00009fd0: 6172 6163 7465 7273 2229 0d0a 2020 2020  aracters")..    
-00009fe0: 2020 2020 7072 696e 7428 6673 7461 7473      print(fstats
-00009ff0: 5f75 2c22 3c2d 2d2d 2066 7374 6174 735f  _u,"<--- fstats_
-0000a000: 7522 290d 0a20 2020 2020 2020 2070 7269  u")..        pri
-0000a010: 6e74 2866 7368 6170 655f 752c 223c 2d2d  nt(fshape_u,"<--
-0000a020: 2d20 6673 6861 7065 5f75 2229 0d0a 2020  - fshape_u")..  
-0000a030: 2020 2020 2020 7072 696e 7428 2273 756d        print("sum
-0000a040: 6d65 6420 696e 6469 6365 7320 696e 666f  med indices info
-0000a050: 3a22 290d 0a20 2020 2020 2020 2066 6f72  :")..        for
-0000a060: 2065 6c65 6d20 696e 2073 756d 6d65 645f   elem in summed_
-0000a070: 696e 6465 785f 696e 666f 3a0d 0a20 2020  index_info:..   
-0000a080: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-0000a090: 2022 2c22 203d 2022 2e6a 6f69 6e28 656c   "," = ".join(el
-0000a0a0: 656d 5b30 5d29 2c22 2820 6c6f 6361 7469  em[0]),"( locati
-0000a0b0: 6f6e 203d 222c 656c 656d 5b31 5d2c 2229  on =",elem[1],")
-0000a0c0: 2229 0d0a 2020 2020 2020 2020 0d0a 2020  ")..        ..  
-0000a0d0: 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a    #:::::::::::::
+00009960: 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a 0d0a 2020  ::::::::::....  
+00009970: 2020 6673 756d 6d61 6e64 2020 203d 2022    fsummand   = "
+00009980: 220d 0a20 2020 2066 7375 6d6d 616e 645f  "..    fsummand_
+00009990: 7520 3d20 2222 0d0a 2020 2020 6673 7461  u = ""..    fsta
+000099a0: 7473 5f6c 6973 7420 3d20 5b5d 0d0a 2020  ts_list = []..  
+000099b0: 2020 6673 6861 7065 5f6c 6973 7420 3d20    fshape_list = 
+000099c0: 5b5d 0d0a 2020 2020 6368 6172 6c69 7374  []..    charlist
+000099d0: 203d 2073 756d 6d61 6e64 0d0a 2020 2020   = summand..    
+000099e0: 666f 7220 692c 6368 6172 2069 6e20 656e  for i,char in en
+000099f0: 756d 6572 6174 6528 7375 6d6d 616e 6429  umerate(summand)
+00009a00: 3a0d 0a20 2020 2020 2020 2069 6620 7374  :..        if st
+00009a10: 6174 735f 6c69 7374 5b69 5d20 3d3d 2030  ats_list[i] == 0
+00009a20: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
+00009a30: 6f6e 7469 6e75 650d 0a0d 0a20 2020 2020  ontinue....     
+00009a40: 2020 2066 7375 6d6d 616e 6420 2020 202b     fsummand    +
+00009a50: 3d20 6368 6172 0d0a 2020 2020 2020 2020  = char..        
+00009a60: 6673 7461 7473 5f6c 6973 7420 2b3d 2073  fstats_list += s
+00009a70: 7461 7473 5f6c 6973 745b 695d 2c0d 0a20  tats_list[i],.. 
+00009a80: 2020 2020 2020 2066 7368 6170 655f 6c69         fshape_li
+00009a90: 7374 202b 3d20 7368 6170 655f 6c69 7374  st += shape_list
+00009aa0: 5b69 5d2c 0d0a 0d0a 2020 2020 2020 2020  [i],....        
+00009ab0: 6966 2073 7461 7473 5f6c 6973 745b 695d  if stats_list[i]
+00009ac0: 203d 3d20 2d31 2061 6e64 2073 756d 6d61   == -1 and summa
+00009ad0: 6e64 2e63 6f75 6e74 2863 6861 7229 3e31  nd.count(char)>1
+00009ae0: 3a0d 0a20 2020 2020 2020 2020 2020 206e  :..            n
+00009af0: 6577 5f63 6861 7220 3d20 6765 745f 6368  ew_char = get_ch
+00009b00: 6172 2863 6861 726c 6973 7429 0d0a 2020  ar(charlist)..  
+00009b10: 2020 2020 2020 2020 2020 6368 6172 6c69            charli
+00009b20: 7374 202b 3d20 6e65 775f 6368 6172 0d0a  st += new_char..
+00009b30: 2020 2020 2020 2020 2020 2020 6673 756d              fsum
+00009b40: 6d61 6e64 5f75 202b 3d20 6e65 775f 6368  mand_u += new_ch
+00009b50: 6172 0d0a 0d0a 2020 2020 2020 2020 2020  ar....          
+00009b60: 2020 2320 6564 6974 2074 6865 2073 756d    # edit the sum
+00009b70: 6d65 645f 696e 6465 785f 696e 666f 2c20  med_index_info, 
+00009b80: 7769 7468 2074 6865 2070 6f73 6974 696f  with the positio
+00009b90: 6e20 7377 6170 7065 6420 6120 6c69 7474  n swapped a litt
+00009ba0: 6c65 2062 6974 2061 7320 7765 6c6c 0d0a  le bit as well..
+00009bb0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00009bc0: 6a2c 5b63 6861 7232 2c6c 6f63 6174 696f  j,[char2,locatio
+00009bd0: 6e2c 7374 6174 735d 2069 6e20 656e 756d  n,stats] in enum
+00009be0: 6572 6174 6528 7375 6d6d 6564 5f69 6e64  erate(summed_ind
+00009bf0: 6578 5f69 6e66 6f29 3a0d 0a20 2020 2020  ex_info):..     
+00009c00: 2020 2020 2020 2020 2020 2069 6620 6368             if ch
+00009c10: 6172 323d 3d63 6861 7220 3a0d 0a20 2020  ar2==char :..   
+00009c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c30: 2073 756d 6d65 645f 696e 6465 785f 696e   summed_index_in
+00009c40: 666f 5b6a 5d5b 305d 203d 205b 6368 6172  fo[j][0] = [char
+00009c50: 2c6e 6577 5f63 6861 725d 0d0a 2020 2020  ,new_char]..    
+00009c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c70: 6966 2073 7461 7473 203d 3d20 5b2d 312c  if stats == [-1,
+00009c80: 315d 3a0d 0a20 2020 2020 2020 2020 2020  1]:..           
+00009c90: 2020 2020 2020 2020 2020 2020 2073 756d               sum
+00009ca0: 6d65 645f 696e 6465 785f 696e 666f 5b6a  med_index_info[j
+00009cb0: 5d5b 315d 203d 205b 2073 756d 6d65 645f  ][1] = [ summed_
+00009cc0: 696e 6465 785f 696e 666f 5b6a 5d5b 315d  index_info[j][1]
+00009cd0: 5b31 5d2c 2073 756d 6d65 645f 696e 6465  [1], summed_inde
+00009ce0: 785f 696e 666f 5b6a 5d5b 315d 5b30 5d20  x_info[j][1][0] 
+00009cf0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00009d00: 2020 2020 2020 2020 2020 2073 756d 6d65             summe
+00009d10: 645f 696e 6465 785f 696e 666f 5b6a 5d5b  d_index_info[j][
+00009d20: 325d 203d 205b 2073 756d 6d65 645f 696e  2] = [ summed_in
+00009d30: 6465 785f 696e 666f 5b6a 5d5b 325d 5b31  dex_info[j][2][1
+00009d40: 5d2c 2073 756d 6d65 645f 696e 6465 785f  ], summed_index_
+00009d50: 696e 666f 5b6a 5d5b 325d 5b30 5d20 5d0d  info[j][2][0] ].
+00009d60: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
+00009d70: 2020 2020 2020 2020 2020 2020 6673 756d              fsum
+00009d80: 6d61 6e64 5f75 202b 3d20 6368 6172 0d0a  mand_u += char..
+00009d90: 2020 2020 6673 7461 7473 203d 2066 7374      fstats = fst
+00009da0: 6174 735f 6c69 7374 2e63 6f70 7928 290d  ats_list.copy().
+00009db0: 0a20 2020 2066 7368 6170 6520 3d20 6673  .    fshape = fs
+00009dc0: 6861 7065 5f6c 6973 742e 636f 7079 2829  hape_list.copy()
+00009dd0: 0d0a 2020 2020 6673 7461 7473 5f75 203d  ..    fstats_u =
+00009de0: 2066 7374 6174 735f 6c69 7374 2e63 6f70   fstats_list.cop
+00009df0: 7928 290d 0a20 2020 2066 7368 6170 655f  y()..    fshape_
+00009e00: 7520 3d20 6673 6861 7065 5f6c 6973 742e  u = fshape_list.
+00009e10: 636f 7079 2829 0d0a 0d0a 2020 2020 2320  copy()....    # 
+00009e20: 7265 6d6f 7665 2074 6865 2073 7461 7420  remove the stat 
+00009e30: 656e 7472 7920 6173 2069 7420 6973 2072  entry as it is r
+00009e40: 6564 756e 6461 6e74 0d0a 2020 2020 666f  edundant..    fo
+00009e50: 7220 692c 656c 656d 2069 6e20 656e 756d  r i,elem in enum
+00009e60: 6572 6174 6528 7375 6d6d 6564 5f69 6e64  erate(summed_ind
+00009e70: 6578 5f69 6e66 6f29 3a0d 0a20 2020 2020  ex_info):..     
+00009e80: 2020 2073 756d 6d65 645f 696e 6465 785f     summed_index_
+00009e90: 696e 666f 5b69 5d20 3d20 656c 656d 5b3a  info[i] = elem[:
+00009ea0: 325d 0d0a 0d0a 2020 2020 6966 2064 6562  2]....    if deb
+00009eb0: 7567 5f6d 6f64 6520 3a0d 0a20 2020 2020  ug_mode :..     
+00009ec0: 2020 2070 7269 6e74 2829 0d0a 2020 2020     print()..    
+00009ed0: 2020 2020 7072 696e 7428 2220 3a3a 3a3a      print(" ::::
+00009ee0: 3a3a 3a3a 3a3a 2072 6570 6c61 6365 2063  :::::: replace c
+00009ef0: 6f6e 6a75 6761 7465 6420 696e 6469 6365  onjugated indice
+00009f00: 7320 6279 2075 6e69 7175 6520 6368 6172  s by unique char
+00009f10: 6163 7465 7273 203a 3a3a 3a3a 3a3a 3a3a  acters :::::::::
+00009f20: 3a20 2229 0d0a 2020 2020 2020 2020 7072  : ")..        pr
+00009f30: 696e 7428 6673 756d 6d61 6e64 2c22 3c2d  int(fsummand,"<-
+00009f40: 2d2d 2066 7375 6d6d 616e 6420 3d20 6f72  -- fsummand = or
+00009f50: 6967 696e 616c 2069 6e64 6963 6573 2229  iginal indices")
+00009f60: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00009f70: 6673 756d 6d61 6e64 5f75 2c22 3c2d 2d2d  fsummand_u,"<---
+00009f80: 2066 7375 6d6d 616e 645f 7520 3d20 7265   fsummand_u = re
+00009f90: 706c 6163 6520 636f 6e6a 7567 6174 6564  place conjugated
+00009fa0: 2069 6e64 6963 6573 2062 7920 756e 6971   indices by uniq
+00009fb0: 7565 2063 6861 7261 6374 6572 7322 290d  ue characters").
+00009fc0: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
+00009fd0: 7374 6174 735f 752c 223c 2d2d 2d20 6673  stats_u,"<--- fs
+00009fe0: 7461 7473 5f75 2229 0d0a 2020 2020 2020  tats_u")..      
+00009ff0: 2020 7072 696e 7428 6673 6861 7065 5f75    print(fshape_u
+0000a000: 2c22 3c2d 2d2d 2066 7368 6170 655f 7522  ,"<--- fshape_u"
+0000a010: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
+0000a020: 2822 7375 6d6d 6564 2069 6e64 6963 6573  ("summed indices
+0000a030: 2069 6e66 6f3a 2229 0d0a 2020 2020 2020   info:")..      
+0000a040: 2020 666f 7220 656c 656d 2069 6e20 7375    for elem in su
+0000a050: 6d6d 6564 5f69 6e64 6578 5f69 6e66 6f3a  mmed_index_info:
+0000a060: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+0000a070: 696e 7428 2220 222c 2220 3d20 222e 6a6f  int(" "," = ".jo
+0000a080: 696e 2865 6c65 6d5b 305d 292c 2228 206c  in(elem[0]),"( l
+0000a090: 6f63 6174 696f 6e20 3d22 2c65 6c65 6d5b  ocation =",elem[
+0000a0a0: 315d 2c22 2922 290d 0a20 2020 2020 2020  1],")")..       
+0000a0b0: 200d 0a20 2020 2023 3a3a 3a3a 3a3a 3a3a   ..    #::::::::
+0000a0c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000a0d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000a0e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000a0f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000a100: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000a110: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000a120: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000a130: 3a3a 3a0d 0a20 2020 2023 2020 2020 2020  :::..    #      
-0000a140: 2020 2020 2020 2020 5374 6570 2032 3a20          Step 2: 
-0000a150: 4172 7261 6e67 6520 7468 6520 696e 6469  Arrange the indi
-0000a160: 6365 7320 2870 7265 7375 6d29 2061 6e64  ces (presum) and
-0000a170: 2063 6f6d 7075 7465 2074 6865 2073 6967   compute the sig
-0000a180: 6e20 6661 6374 6f72 0d0a 2020 2020 233a  n factor..    #:
+0000a110: 3a3a 3a3a 3a3a 3a3a 0d0a 2020 2020 2320  ::::::::..    # 
+0000a120: 2020 2020 2020 2020 2020 2020 2053 7465               Ste
+0000a130: 7020 323a 2041 7272 616e 6765 2074 6865  p 2: Arrange the
+0000a140: 2069 6e64 6963 6573 2028 7072 6573 756d   indices (presum
+0000a150: 2920 616e 6420 636f 6d70 7574 6520 7468  ) and compute th
+0000a160: 6520 7369 676e 2066 6163 746f 720d 0a20  e sign factor.. 
+0000a170: 2020 2023 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a     #::::::::::::
+0000a180: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000a190: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000a1a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000a1b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000a1c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000a1d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000a1e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a0d  :::::::::::::::.
-0000a1f0: 0a0d 0a20 2020 2023 2074 6865 2073 756d  ...    # the sum
-0000a200: 6d65 6420 696e 6469 6365 7320 6172 6520  med indices are 
-0000a210: 6e6f 7720 6e65 7874 2074 6f20 6561 6368  now next to each
-0000a220: 206f 7468 6572 2077 6974 6820 7468 6520   other with the 
-0000a230: 636f 6e6a 7567 6174 6564 206f 6e65 2074  conjugated one t
-0000a240: 6f20 7468 6520 7269 6768 740d 0a0d 0a20  o the right.... 
-0000a250: 2020 2066 7375 6d6d 616e 645f 7572 203d     fsummand_ur =
-0000a260: 2066 7375 6d6d 616e 645f 750d 0a20 2020   fsummand_u..   
-0000a270: 2066 6f72 205b 205b 6331 2c63 325d 2c20   for [ [c1,c2], 
-0000a280: 6c6f 6320 5d20 696e 2073 756d 6d65 645f  loc ] in summed_
-0000a290: 696e 6465 785f 696e 666f 3a0d 0a20 2020  index_info:..   
-0000a2a0: 2020 2020 2066 7375 6d6d 616e 645f 7572       fsummand_ur
-0000a2b0: 203d 2066 7375 6d6d 616e 645f 7572 2e72   = fsummand_ur.r
-0000a2c0: 6570 6c61 6365 2863 322c 2222 290d 0a20  eplace(c2,"").. 
-0000a2d0: 2020 2020 2020 2066 7375 6d6d 616e 645f         fsummand_
-0000a2e0: 7572 203d 2066 7375 6d6d 616e 645f 7572  ur = fsummand_ur
-0000a2f0: 2e72 6570 6c61 6365 2863 312c 6331 2b63  .replace(c1,c1+c
-0000a300: 3229 0d0a 0d0a 2020 2020 6673 7461 7473  2)....    fstats
-0000a310: 5f75 7220 3d20 7265 6f72 6465 7269 6e67  _ur = reordering
-0000a320: 2866 7375 6d6d 616e 645f 752c 6673 756d  (fsummand_u,fsum
-0000a330: 6d61 6e64 5f75 722c 6673 7461 7473 5f6c  mand_ur,fstats_l
-0000a340: 6973 7429 0d0a 2020 2020 6673 6861 7065  ist)..    fshape
-0000a350: 5f75 7220 3d20 7265 6f72 6465 7269 6e67  _ur = reordering
-0000a360: 2866 7375 6d6d 616e 645f 752c 6673 756d  (fsummand_u,fsum
-0000a370: 6d61 6e64 5f75 722c 6673 6861 7065 5f6c  mand_ur,fshape_l
-0000a380: 6973 7429 0d0a 0d0a 2020 2020 6966 2064  ist)....    if d
-0000a390: 6562 7567 5f6d 6f64 6520 3a0d 0a20 2020  ebug_mode :..   
-0000a3a0: 2020 2020 2070 7269 6e74 2829 0d0a 2020       print()..  
-0000a3b0: 2020 2020 2020 7072 696e 7428 2220 3a3a        print(" ::
-0000a3c0: 3a3a 3a3a 3a3a 3a3a 3a3a 206d 6f76 6520  :::::::::: move 
-0000a3d0: 7468 6520 636f 6e6a 7567 6174 6564 2074  the conjugated t
-0000a3e0: 6f20 7468 6520 7269 6768 7420 6f66 2069  o the right of i
-0000a3f0: 7473 2070 6169 7220 3a3a 3a3a 3a3a 3a3a  ts pair ::::::::
-0000a400: 3a3a 3a20 2229 0d0a 2020 2020 2020 2020  ::: ")..        
-0000a410: 7072 696e 7428 6673 756d 6d61 6e64 5f75  print(fsummand_u
-0000a420: 2c22 3c2d 2d2d 2066 7375 6d6d 616e 645f  ,"<--- fsummand_
-0000a430: 7522 290d 0a20 2020 2020 2020 2070 7269  u")..        pri
-0000a440: 6e74 2866 7375 6d6d 616e 645f 7572 2c22  nt(fsummand_ur,"
-0000a450: 3c2d 2d2d 2066 7375 6d6d 616e 645f 7572  <--- fsummand_ur
-0000a460: 203d 206d 6f76 6520 7468 6520 636f 6e6a   = move the conj
-0000a470: 7567 6174 6564 2074 6f20 7468 6520 7269  ugated to the ri
-0000a480: 6768 7420 6f66 2069 7473 2070 6169 7222  ght of its pair"
-0000a490: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-0000a4a0: 2866 7374 6174 735f 7572 2c22 3c2d 2d2d  (fstats_ur,"<---
-0000a4b0: 2066 7374 6174 735f 7572 2229 0d0a 2020   fstats_ur")..  
-0000a4c0: 2020 2020 2020 7072 696e 7428 6673 6861        print(fsha
-0000a4d0: 7065 5f75 722c 223c 2d2d 2d20 6673 6861  pe_ur,"<--- fsha
-0000a4e0: 7065 5f75 7222 290d 0a20 2020 2020 2020  pe_ur")..       
-0000a4f0: 200d 0a20 2020 2023 2072 656d 6f76 6520   ..    # remove 
-0000a500: 7468 6520 6c65 6164 696e 6720 616e 6420  the leading and 
-0000a510: 7472 6169 6c69 6e67 2063 6861 7273 2074  trailing chars t
-0000a520: 6861 7420 6973 2074 6865 2073 616d 6520  hat is the same 
-0000a530: 6173 2074 6865 2070 7265 2d72 6561 7272  as the pre-rearr
-0000a540: 616e 6765 6420 7374 7269 6e67 0d0a 0d0a  anged string....
-0000a550: 2020 2020 6e61 6c6c 5f75 203d 206c 656e      nall_u = len
-0000a560: 2866 7375 6d6d 616e 645f 7529 0d0a 0d0a  (fsummand_u)....
-0000a570: 2020 2020 6e6c 203d 2030 0d0a 2020 2020      nl = 0..    
-0000a580: 666f 7220 6920 696e 2072 616e 6765 286e  for i in range(n
-0000a590: 616c 6c5f 7529 3a0d 0a20 2020 2020 2020  all_u):..       
-0000a5a0: 2069 6620 6673 756d 6d61 6e64 5f75 5b69   if fsummand_u[i
-0000a5b0: 5d20 213d 2066 7375 6d6d 616e 645f 7572  ] != fsummand_ur
-0000a5c0: 5b69 5d3a 0d0a 2020 2020 2020 2020 2020  [i]:..          
-0000a5d0: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
-0000a5e0: 206e 6c2b 3d31 0d0a 2020 2020 6e72 203d   nl+=1..    nr =
-0000a5f0: 2030 0d0a 2020 2020 666f 7220 6920 696e   0..    for i in
-0000a600: 2072 616e 6765 286e 616c 6c5f 7529 3a0d   range(nall_u):.
-0000a610: 0a20 2020 2020 2020 2069 6620 6673 756d  .        if fsum
-0000a620: 6d61 6e64 5f75 5b6e 616c 6c5f 752d 312d  mand_u[nall_u-1-
-0000a630: 695d 2021 3d20 6673 756d 6d61 6e64 5f75  i] != fsummand_u
-0000a640: 725b 6e61 6c6c 5f75 2d31 2d69 5d3a 0d0a  r[nall_u-1-i]:..
-0000a650: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-0000a660: 6b0d 0a20 2020 2020 2020 206e 722b 3d31  k..        nr+=1
-0000a670: 0d0a 2020 2020 6e72 203d 206e 616c 6c5f  ..    nr = nall_
-0000a680: 752d 6e72 0d0a 0d0a 2020 2020 6673 756d  u-nr....    fsum
-0000a690: 6d61 6e64 5f75 7420 203d 2066 7375 6d6d  mand_ut  = fsumm
-0000a6a0: 616e 645f 755b 6e6c 3a6e 725d 0d0a 2020  and_u[nl:nr]..  
-0000a6b0: 2020 6673 7461 7473 5f75 7420 2020 3d20    fstats_ut   = 
-0000a6c0: 6673 7461 7473 5f75 5b6e 6c3a 6e72 5d0d  fstats_u[nl:nr].
-0000a6d0: 0a20 2020 2066 7368 6170 655f 7574 2020  .    fshape_ut  
-0000a6e0: 203d 2066 7368 6170 655f 755b 6e6c 3a6e   = fshape_u[nl:n
-0000a6f0: 725d 0d0a 2020 2020 6673 756d 6d61 6e64  r]..    fsummand
-0000a700: 5f75 7274 2020 3d20 6673 756d 6d61 6e64  _urt  = fsummand
-0000a710: 5f75 725b 6e6c 3a6e 725d 0d0a 2020 2020  _ur[nl:nr]..    
-0000a720: 6673 7461 7473 5f75 7274 2020 203d 2066  fstats_urt   = f
-0000a730: 7374 6174 735f 7572 5b6e 6c3a 6e72 5d0d  stats_ur[nl:nr].
-0000a740: 0a20 2020 2066 7368 6170 655f 7572 7420  .    fshape_urt 
-0000a750: 2020 3d20 6673 6861 7065 5f75 725b 6e6c    = fshape_ur[nl
-0000a760: 3a6e 725d 0d0a 0d0a 2020 2020 6966 206e  :nr]....    if n
-0000a770: 6c3e 6e72 203a 0d0a 2020 2020 2020 2020  l>nr :..        
-0000a780: 736b 6970 5f53 3120 3d20 5472 7565 0d0a  skip_S1 = True..
-0000a790: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0000a7a0: 2020 2073 6b69 705f 5331 203d 2046 616c     skip_S1 = Fal
-0000a7b0: 7365 0d0a 0d0a 2020 2020 6966 2064 6562  se....    if deb
-0000a7c0: 7567 5f6d 6f64 6520 3a0d 0a20 2020 2020  ug_mode :..     
-0000a7d0: 2020 2070 7269 6e74 2829 0d0a 2020 2020     print()..    
-0000a7e0: 2020 2020 7072 696e 7428 2220 3a3a 3a3a      print(" ::::
-0000a7f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000a800: 3a3a 3a3a 2074 7269 6d20 6c65 6674 2061  :::: trim left a
-0000a810: 6e64 2072 6967 6874 203a 3a3a 3a3a 3a3a  nd right :::::::
-0000a820: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000a830: 3a20 2229 0d0a 2020 2020 2020 2020 6966  : ")..        if
-0000a840: 2073 6b69 705f 5331 203a 0d0a 2020 2020   skip_S1 :..    
-0000a850: 2020 2020 2020 2020 7072 696e 7428 2266          print("f
-0000a860: 7375 6d6d 616e 645f 7520 616e 6420 6673  summand_u and fs
-0000a870: 756d 6d61 6e64 5f75 7220 6172 6520 6964  ummand_ur are id
-0000a880: 656e 7469 6361 6c2e 2229 0d0a 2020 2020  entical.")..    
-0000a890: 2020 2020 2020 2020 7072 696e 7428 2253          print("S
-0000a8a0: 3120 6361 6c63 756c 6174 696f 6e20 6973  1 calculation is
-0000a8b0: 2073 6b69 7070 6564 2e22 290d 0a20 2020   skipped.")..   
-0000a8c0: 2020 2020 2065 6c73 6520 3a0d 0a20 2020       else :..   
-0000a8d0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-0000a8e0: 7375 6d6d 616e 645f 752c 223c 2d2d 2d20  summand_u,"<--- 
-0000a8f0: 6673 756d 6d61 6e64 5f75 2229 0d0a 2020  fsummand_u")..  
-0000a900: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0000a910: 6673 756d 6d61 6e64 5f75 742c 223c 2d2d  fsummand_ut,"<--
-0000a920: 2d20 6673 756d 6d61 6e64 5f75 7420 3d20  - fsummand_ut = 
-0000a930: 7472 696d 2066 7375 6d6d 616e 645f 7520  trim fsummand_u 
-0000a940: 6c65 6674 2061 6e64 2072 6967 6874 2229  left and right")
-0000a950: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-0000a960: 696e 7428 6673 7461 7473 5f75 742c 223c  int(fstats_ut,"<
-0000a970: 2d2d 2d20 6673 7461 7473 5f75 7422 290d  --- fstats_ut").
-0000a980: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-0000a990: 6e74 2866 7368 6170 655f 7574 2c22 3c2d  nt(fshape_ut,"<-
-0000a9a0: 2d2d 2066 7368 6170 655f 7574 2229 0d0a  -- fshape_ut")..
-0000a9b0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000a9c0: 7428 290d 0a20 2020 2020 2020 2020 2020  t()..           
-0000a9d0: 2070 7269 6e74 2866 7375 6d6d 616e 645f   print(fsummand_
-0000a9e0: 7572 2c22 3c2d 2d2d 2066 7375 6d6d 616e  ur,"<--- fsumman
-0000a9f0: 645f 7572 2229 0d0a 2020 2020 2020 2020  d_ur")..        
-0000aa00: 2020 2020 7072 696e 7428 6673 756d 6d61      print(fsumma
-0000aa10: 6e64 5f75 7274 2c22 3c2d 2d2d 2066 7375  nd_urt,"<--- fsu
-0000aa20: 6d6d 616e 645f 7572 7420 3d20 7472 696d  mmand_urt = trim
-0000aa30: 2066 7375 6d6d 616e 645f 7572 206c 6566   fsummand_ur lef
-0000aa40: 7420 616e 6420 7269 6768 7422 290d 0a20  t and right").. 
-0000aa50: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000aa60: 2866 7374 6174 735f 7572 742c 223c 2d2d  (fstats_urt,"<--
-0000aa70: 2d20 6673 7461 7473 5f75 7274 2229 0d0a  - fstats_urt")..
-0000aa80: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000aa90: 7428 6673 6861 7065 5f75 7274 2c22 3c2d  t(fshape_urt,"<-
-0000aaa0: 2d2d 2066 7368 6170 655f 7572 7422 290d  -- fshape_urt").
-0000aab0: 0a20 2020 2020 2020 200d 0a20 2020 2053  .        ..    S
-0000aac0: 315f 7367 6e5f 636f 6d70 7574 6174 696f  1_sgn_computatio
-0000aad0: 6e5f 7374 7269 6e67 203d 2066 7375 6d6d  n_string = fsumm
-0000aae0: 616e 645f 7574 2b22 2d3e 222b 6673 756d  and_ut+"->"+fsum
-0000aaf0: 6d61 6e64 5f75 7274 0d0a 2020 2020 0d0a  mand_urt..    ..
-0000ab00: 2020 2020 6966 2064 6562 7567 5f6d 6f64      if debug_mod
-0000ab10: 6520 616e 6420 6e6f 7420 736b 6970 5f53  e and not skip_S
-0000ab20: 3120 3a0d 0a20 2020 2020 2020 2070 7269  1 :..        pri
-0000ab30: 6e74 2829 0d0a 2020 2020 2020 2020 7072  nt()..        pr
-0000ab40: 696e 7428 5331 5f73 676e 5f63 6f6d 7075  int(S1_sgn_compu
-0000ab50: 7461 7469 6f6e 5f73 7472 696e 672c 223c  tation_string,"<
-0000ab60: 2d2d 2d20 7374 7269 6e67 2075 7365 6420  --- string used 
-0000ab70: 696e 2053 3120 636f 6d70 7574 6174 696f  in S1 computatio
-0000ab80: 6e22 290d 0a20 2020 200d 0a20 2020 2023  n")..    ..    #
-0000ab90: 2072 656d 6f76 6520 7468 6520 636f 6e6a   remove the conj
-0000aba0: 7567 6174 6564 2063 6861 7261 6374 6572  ugated character
-0000abb0: 2069 6620 626f 7468 2074 6865 206e 6f6e   if both the non
-0000abc0: 6e63 6f6e 6a75 6761 7465 6420 616e 6420  nconjugated and 
-0000abd0: 636f 6e6a 7567 6174 6564 2061 7265 2070  conjugated are p
-0000abe0: 7265 7365 6e74 0d0a 2020 2020 0d0a 2020  resent..    ..  
-0000abf0: 2020 2320 646f 2074 6865 2075 7420 6f6e    # do the ut on
-0000ac00: 6c79 0d0a 2020 2020 6673 756d 6d61 6e64  ly..    fsummand
-0000ac10: 5f75 7478 203d 2022 220d 0a20 2020 2066  _utx = ""..    f
-0000ac20: 7374 6174 735f 7574 7820 2020 3d20 5b5d  stats_utx   = []
-0000ac30: 0d0a 2020 2020 6673 6861 7065 5f75 7478  ..    fshape_utx
-0000ac40: 2020 203d 205b 5d0d 0a20 2020 206e 616c     = []..    nal
-0000ac50: 6c5f 7574 203d 206c 656e 2866 7375 6d6d  l_ut = len(fsumm
-0000ac60: 616e 645f 7574 290d 0a20 2020 2066 6f72  and_ut)..    for
-0000ac70: 2069 2069 6e20 7261 6e67 6528 6e61 6c6c   i in range(nall
-0000ac80: 5f75 7429 3a0d 0a20 2020 2020 2020 2063  _ut):..        c
-0000ac90: 203d 2066 7375 6d6d 616e 645f 7574 5b69   = fsummand_ut[i
-0000aca0: 5d0d 0a20 2020 2020 2020 2074 6f5f 736b  ]..        to_sk
-0000acb0: 6970 203d 2046 616c 7365 0d0a 2020 2020  ip = False..    
-0000acc0: 2020 2020 6966 2066 7374 6174 735f 7574      if fstats_ut
-0000acd0: 5b69 5d3d 3d2d 3120 3a0d 0a20 2020 2020  [i]==-1 :..     
-0000ace0: 2020 2020 2020 2066 6f72 205b 205b 6331         for [ [c1
-0000acf0: 2c63 325d 2c20 6c6f 6320 5d20 696e 2073  ,c2], loc ] in s
-0000ad00: 756d 6d65 645f 696e 6465 785f 696e 666f  ummed_index_info
-0000ad10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000ad20: 2020 2069 6620 633d 3d63 3220 616e 6420     if c==c2 and 
-0000ad30: 6673 756d 6d61 6e64 5f75 742e 636f 756e  fsummand_ut.coun
-0000ad40: 7428 6331 293e 303a 0d0a 2020 2020 2020  t(c1)>0:..      
-0000ad50: 2020 2020 2020 2020 2020 2020 2020 746f                to
-0000ad60: 5f73 6b69 7020 3d20 5472 7565 0d0a 2020  _skip = True..  
-0000ad70: 2020 2020 2020 6966 2074 6f5f 736b 6970        if to_skip
-0000ad80: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
-0000ad90: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
-0000ada0: 2020 6673 756d 6d61 6e64 5f75 7478 202b    fsummand_utx +
-0000adb0: 3d20 6673 756d 6d61 6e64 5f75 745b 695d  = fsummand_ut[i]
-0000adc0: 0d0a 2020 2020 2020 2020 6673 7461 7473  ..        fstats
-0000add0: 5f75 7478 2020 202b 3d20 6673 7461 7473  _utx   += fstats
-0000ade0: 5f75 745b 695d 2c0d 0a20 2020 2020 2020  _ut[i],..       
-0000adf0: 2066 7368 6170 655f 7574 7820 2020 2b3d   fshape_utx   +=
-0000ae00: 2066 7368 6170 655f 7574 5b69 5d2c 0d0a   fshape_ut[i],..
-0000ae10: 2020 2020 5331 6469 6d20 3d20 6c65 6e28      S1dim = len(
-0000ae20: 6673 756d 6d61 6e64 5f75 7478 290d 0a0d  fsummand_utx)...
-0000ae30: 0a20 2020 2069 6620 6465 6275 675f 6d6f  .    if debug_mo
-0000ae40: 6465 2061 6e64 206e 6f74 2073 6b69 705f  de and not skip_
-0000ae50: 5331 203a 0d0a 2020 2020 2020 2020 7072  S1 :..        pr
-0000ae60: 696e 7428 290d 0a20 2020 2020 2020 2070  int()..        p
-0000ae70: 7269 6e74 2822 203a 3a3a 3a3a 3a3a 2072  rint(" ::::::: r
-0000ae80: 656d 6f76 6520 7468 6520 636f 6e6a 7567  emove the conjug
-0000ae90: 6174 6564 2069 6620 626f 7468 206f 6620  ated if both of 
-0000aea0: 7468 6520 7061 6972 2061 7265 2070 7265  the pair are pre
-0000aeb0: 7365 6e74 203a 3a3a 3a3a 3a3a 2022 290d  sent ::::::: ").
-0000aec0: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
-0000aed0: 7375 6d6d 616e 645f 7574 2c22 3c2d 2d2d  summand_ut,"<---
-0000aee0: 2066 7375 6d6d 616e 645f 7574 2229 0d0a   fsummand_ut")..
-0000aef0: 2020 2020 2020 2020 7072 696e 7428 6673          print(fs
-0000af00: 756d 6d61 6e64 5f75 7478 2c22 3c2d 2d2d  ummand_utx,"<---
-0000af10: 2066 7375 6d6d 616e 645f 7574 7820 3d20   fsummand_utx = 
-0000af20: 7265 6d6f 7665 206f 6e20 6f66 2074 6865  remove on of the
-0000af30: 2070 6169 7222 290d 0a20 2020 2020 2020   pair")..       
-0000af40: 2070 7269 6e74 2866 7374 6174 735f 7574   print(fstats_ut
-0000af50: 782c 223c 2d2d 2d20 6673 7461 7473 5f75  x,"<--- fstats_u
-0000af60: 7478 2229 0d0a 2020 2020 2020 2020 7072  tx")..        pr
-0000af70: 696e 7428 6673 6861 7065 5f75 7478 2c22  int(fshape_utx,"
-0000af80: 3c2d 2d2d 2066 7368 6170 655f 7574 7822  <--- fshape_utx"
-0000af90: 290d 0a20 2020 200d 0a20 2020 2023 206d  )..    ..    # m
-0000afa0: 616b 6520 7468 6520 636f 7079 206d 6170  ake the copy map
-0000afb0: 0d0a 2020 2020 636f 7079 5f6d 6170 203d  ..    copy_map =
-0000afc0: 205b 5d0d 0a20 2020 2066 7375 6d6d 616e   []..    fsumman
-0000afd0: 645f 7574 785f 7220 3d20 6c69 7374 2866  d_utx_r = list(f
-0000afe0: 7375 6d6d 616e 645f 7574 7829 2023 7468  summand_utx) #th
-0000aff0: 6973 2069 7320 7573 6564 2069 6e20 7468  is is used in th
-0000b000: 6520 6d6f 636b 2072 6563 6f6e 7374 7275  e mock reconstru
-0000b010: 6374 696f 6e0d 0a20 2020 2066 6f72 2069  ction..    for i
-0000b020: 5f75 742c 2063 2069 6e20 656e 756d 6572  _ut, c in enumer
-0000b030: 6174 6528 6673 756d 6d61 6e64 5f75 7429  ate(fsummand_ut)
-0000b040: 3a0d 0a20 2020 2020 2020 2069 6620 6320  :..        if c 
-0000b050: 6e6f 7420 696e 2066 7375 6d6d 616e 645f  not in fsummand_
-0000b060: 7574 783a 0d0a 2020 2020 2020 2020 2020  utx:..          
-0000b070: 2020 2366 696e 6420 7468 6520 6c6f 6361    #find the loca
-0000b080: 7469 6f6e 206f 6620 6974 7320 7061 6972  tion of its pair
-0000b090: 2066 6972 7374 0d0a 2020 2020 2020 2020   first..        
-0000b0a0: 2020 2020 635f 7061 6972 203d 2022 3f22      c_pair = "?"
-0000b0b0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-0000b0c0: 7220 5b5b 6331 2c63 325d 2c5f 5d20 696e  r [[c1,c2],_] in
-0000b0d0: 2073 756d 6d65 645f 696e 6465 785f 696e   summed_index_in
-0000b0e0: 666f 3a0d 0a20 2020 2020 2020 2020 2020  fo:..           
-0000b0f0: 2020 2020 2069 6620 633d 3d63 3220 3a0d       if c==c2 :.
-0000b100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b110: 2020 2020 2069 5f75 7478 203d 2066 7375       i_utx = fsu
-0000b120: 6d6d 616e 645f 7574 785f 722e 696e 6465  mmand_utx_r.inde
-0000b130: 7828 6331 290d 0a20 2020 2020 2020 2020  x(c1)..         
-0000b140: 2020 2020 2020 2020 2020 2063 5f70 6169             c_pai
-0000b150: 7220 3d20 6331 0d0a 2020 2020 2020 2020  r = c1..        
-0000b160: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-0000b170: 6b0d 0a20 2020 2020 2020 2020 2020 2063  k..            c
-0000b180: 6f70 795f 6d61 7020 2b3d 205b 695f 7574  opy_map += [i_ut
-0000b190: 2c69 5f75 7478 5d2c 0d0a 2020 2020 2020  ,i_utx],..      
-0000b1a0: 2020 2020 2020 6673 756d 6d61 6e64 5f75        fsummand_u
-0000b1b0: 7478 5f72 2e69 6e73 6572 7428 695f 7574  tx_r.insert(i_ut
-0000b1c0: 2c63 290d 0a20 2020 200d 0a20 2020 2064  ,c)..    ..    d
-0000b1d0: 6566 2075 7365 5f63 6f70 795f 6d61 7028  ef use_copy_map(
-0000b1e0: 7468 655f 6d61 702c 7468 655f 6c69 7374  the_map,the_list
-0000b1f0: 2c61 7070 6c79 5f6e 6567 6174 6976 653d  ,apply_negative=
-0000b200: 4661 6c73 6529 3a0d 0a20 2020 2020 2020  False):..       
-0000b210: 206e 6577 5f6c 6973 7420 3d20 6c69 7374   new_list = list
-0000b220: 2874 6865 5f6c 6973 7429 2e63 6f70 7928  (the_list).copy(
-0000b230: 290d 0a20 2020 2020 2020 2066 6f72 205b  )..        for [
-0000b240: 6932 2c69 315d 2069 6e20 7468 655f 6d61  i2,i1] in the_ma
-0000b250: 7020 3a0d 0a20 2020 2020 2020 2020 2020  p :..           
-0000b260: 2069 6620 6170 706c 795f 6e65 6761 7469   if apply_negati
-0000b270: 7665 203a 0d0a 2020 2020 2020 2020 2020  ve :..          
-0000b280: 2020 2020 2020 6e65 775f 6c69 7374 2e69        new_list.i
-0000b290: 6e73 6572 7428 6932 2c2d 6e65 775f 6c69  nsert(i2,-new_li
-0000b2a0: 7374 5b69 315d 290d 0a20 2020 2020 2020  st[i1])..       
-0000b2b0: 2020 2020 2065 6c73 6520 3a0d 0a20 2020       else :..   
-0000b2c0: 2020 2020 2020 2020 2020 2020 206e 6577               new
-0000b2d0: 5f6c 6973 742e 696e 7365 7274 2869 322c  _list.insert(i2,
-0000b2e0: 6e65 775f 6c69 7374 5b69 315d 290d 0a20  new_list[i1]).. 
-0000b2f0: 2020 2020 2020 2072 6574 7572 6e20 6e65         return ne
-0000b300: 775f 6c69 7374 0d0a 2020 2020 0d0a 2020  w_list..    ..  
-0000b310: 2020 6966 2064 6562 7567 5f6d 6f64 6520    if debug_mode 
-0000b320: 616e 6420 6e6f 7420 736b 6970 5f53 313a  and not skip_S1:
-0000b330: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-0000b340: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-0000b350: 2822 203a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  (" :::::::::::::
-0000b360: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a20 7465  ::::::::::::: te
-0000b370: 7374 696e 6720 636f 7079 5f6d 6170 203a  sting copy_map :
-0000b380: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000b390: 3a3a 3a3a 3a3a 3a3a 2022 290d 0a20 2020  :::::::: ")..   
-0000b3a0: 2020 2020 2066 7375 6d6d 616e 645f 7574       fsummand_ut
-0000b3b0: 3220 3d20 2727 2e6a 6f69 6e28 7573 655f  2 = ''.join(use_
-0000b3c0: 636f 7079 5f6d 6170 2863 6f70 795f 6d61  copy_map(copy_ma
-0000b3d0: 702c 6c69 7374 2866 7375 6d6d 616e 645f  p,list(fsummand_
-0000b3e0: 7574 7829 2929 0d0a 2020 2020 2020 2020  utx)))..        
-0000b3f0: 6673 7461 7473 5f75 7432 203d 2075 7365  fstats_ut2 = use
-0000b400: 5f63 6f70 795f 6d61 7028 636f 7079 5f6d  _copy_map(copy_m
-0000b410: 6170 2c66 7374 6174 735f 7574 782c 6170  ap,fstats_utx,ap
-0000b420: 706c 795f 6e65 6761 7469 7665 3d54 7275  ply_negative=Tru
-0000b430: 6529 0d0a 2020 2020 2020 2020 6673 6861  e)..        fsha
-0000b440: 7065 5f75 7432 203d 2075 7365 5f63 6f70  pe_ut2 = use_cop
-0000b450: 795f 6d61 7028 636f 7079 5f6d 6170 2c66  y_map(copy_map,f
-0000b460: 7368 6170 655f 7574 7829 0d0a 2020 2020  shape_utx)..    
-0000b470: 2020 2020 7072 696e 7428 2220 222c 6673      print(" ",fs
-0000b480: 756d 6d61 6e64 5f75 7432 2c22 7673 222c  ummand_ut2,"vs",
-0000b490: 6673 756d 6d61 6e64 5f75 7429 0d0a 2020  fsummand_ut)..  
-0000b4a0: 2020 2020 2020 7072 696e 7428 2220 222c        print(" ",
-0000b4b0: 6673 7461 7473 5f75 7432 2c22 7673 222c  fstats_ut2,"vs",
-0000b4c0: 6673 7461 7473 5f75 7429 0d0a 2020 2020  fstats_ut)..    
-0000b4d0: 2020 2020 7072 696e 7428 2220 222c 6673      print(" ",fs
-0000b4e0: 6861 7065 5f75 7432 2c22 7673 222c 6673  hape_ut2,"vs",fs
-0000b4f0: 6861 7065 5f75 7429 0d0a 2020 2020 2020  hape_ut)..      
-0000b500: 2020 0d0a 2020 2020 2320 6673 756d 6d61    ..    # fsumma
-0000b510: 6e64 5f75 7478 206e 6565 6473 2074 6f20  nd_utx needs to 
-0000b520: 6265 2072 6570 6c61 6365 6420 7769 7468  be replaced with
-0000b530: 2074 6865 206f 7269 6769 6e61 6c20 696e   the original in
-0000b540: 6469 6365 7320 746f 206f 6274 6169 6e20  dices to obtain 
-0000b550: 5331 5f69 6e64 6578 5f73 7472 696e 670d  S1_index_string.
-0000b560: 0a20 2020 2053 315f 696e 6465 785f 7374  .    S1_index_st
-0000b570: 7269 6e67 2020 3d20 2222 0d0a 2020 2020  ring  = ""..    
-0000b580: 666f 7220 6320 696e 2066 7375 6d6d 616e  for c in fsumman
-0000b590: 645f 7574 783a 0d0a 2020 2020 2020 2020  d_utx:..        
-0000b5a0: 6966 2063 2069 6e20 7375 6d6d 616e 643a  if c in summand:
-0000b5b0: 0d0a 2020 2020 2020 2020 2020 2020 5331  ..            S1
-0000b5c0: 5f69 6e64 6578 5f73 7472 696e 6720 2b3d  _index_string +=
-0000b5d0: 2063 0d0a 2020 2020 2020 2020 656c 7365   c..        else
-0000b5e0: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-0000b5f0: 6f72 205b 205b 6331 2c63 325d 2c20 6c6f  or [ [c1,c2], lo
-0000b600: 6320 5d20 696e 2073 756d 6d65 645f 696e  c ] in summed_in
-0000b610: 6465 785f 696e 666f 3a0d 0a20 2020 2020  dex_info:..     
-0000b620: 2020 2020 2020 2020 2020 2069 6620 633d             if c=
-0000b630: 3d63 3220 3a0d 0a20 2020 2020 2020 2020  =c2 :..         
-0000b640: 2020 2020 2020 2020 2020 2053 315f 696e             S1_in
-0000b650: 6465 785f 7374 7269 6e67 202b 3d20 6331  dex_string += c1
-0000b660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000b670: 2020 2020 2020 6272 6561 6b0d 0a20 2020        break..   
-0000b680: 2053 315f 7368 6170 6520 3d20 5b5d 0d0a   S1_shape = []..
-0000b690: 2020 2020 666f 7220 6320 696e 2053 315f      for c in S1_
-0000b6a0: 696e 6465 785f 7374 7269 6e67 3a0d 0a20  index_string:.. 
-0000b6b0: 2020 2020 2020 2069 6e64 203d 2066 7375         ind = fsu
-0000b6c0: 6d6d 616e 642e 696e 6465 7828 6329 0d0a  mmand.index(c)..
-0000b6d0: 2020 2020 2020 2020 5331 5f73 6861 7065          S1_shape
-0000b6e0: 202b 3d20 6673 6861 7065 5b69 6e64 5d2c   += fshape[ind],
-0000b6f0: 0d0a 2020 2020 5331 5f73 6861 7065 203d  ..    S1_shape =
-0000b700: 206d 616b 655f 7475 706c 6528 5331 5f73   make_tuple(S1_s
-0000b710: 6861 7065 290d 0a20 2020 200d 0a20 2020  hape)..    ..   
-0000b720: 2069 6620 6465 6275 675f 6d6f 6465 2061   if debug_mode a
-0000b730: 6e64 206e 6f74 2073 6b69 705f 5331 203a  nd not skip_S1 :
-0000b740: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-0000b750: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-0000b760: 2822 203a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  (" :::::::::::::
+0000a1d0: 3a3a 3a3a 0d0a 0d0a 2020 2020 2320 7468  ::::....    # th
+0000a1e0: 6520 7375 6d6d 6564 2069 6e64 6963 6573  e summed indices
+0000a1f0: 2061 7265 206e 6f77 206e 6578 7420 746f   are now next to
+0000a200: 2065 6163 6820 6f74 6865 7220 7769 7468   each other with
+0000a210: 2074 6865 2063 6f6e 6a75 6761 7465 6420   the conjugated 
+0000a220: 6f6e 6520 746f 2074 6865 2072 6967 6874  one to the right
+0000a230: 0d0a 0d0a 2020 2020 6673 756d 6d61 6e64  ....    fsummand
+0000a240: 5f75 7220 3d20 6673 756d 6d61 6e64 5f75  _ur = fsummand_u
+0000a250: 0d0a 2020 2020 666f 7220 5b20 5b63 312c  ..    for [ [c1,
+0000a260: 6332 5d2c 206c 6f63 205d 2069 6e20 7375  c2], loc ] in su
+0000a270: 6d6d 6564 5f69 6e64 6578 5f69 6e66 6f3a  mmed_index_info:
+0000a280: 0d0a 2020 2020 2020 2020 6673 756d 6d61  ..        fsumma
+0000a290: 6e64 5f75 7220 3d20 6673 756d 6d61 6e64  nd_ur = fsummand
+0000a2a0: 5f75 722e 7265 706c 6163 6528 6332 2c22  _ur.replace(c2,"
+0000a2b0: 2229 0d0a 2020 2020 2020 2020 6673 756d  ")..        fsum
+0000a2c0: 6d61 6e64 5f75 7220 3d20 6673 756d 6d61  mand_ur = fsumma
+0000a2d0: 6e64 5f75 722e 7265 706c 6163 6528 6331  nd_ur.replace(c1
+0000a2e0: 2c63 312b 6332 290d 0a0d 0a20 2020 2066  ,c1+c2)....    f
+0000a2f0: 7374 6174 735f 7572 203d 2072 656f 7264  stats_ur = reord
+0000a300: 6572 696e 6728 6673 756d 6d61 6e64 5f75  ering(fsummand_u
+0000a310: 2c66 7375 6d6d 616e 645f 7572 2c66 7374  ,fsummand_ur,fst
+0000a320: 6174 735f 6c69 7374 290d 0a20 2020 2066  ats_list)..    f
+0000a330: 7368 6170 655f 7572 203d 2072 656f 7264  shape_ur = reord
+0000a340: 6572 696e 6728 6673 756d 6d61 6e64 5f75  ering(fsummand_u
+0000a350: 2c66 7375 6d6d 616e 645f 7572 2c66 7368  ,fsummand_ur,fsh
+0000a360: 6170 655f 6c69 7374 290d 0a0d 0a20 2020  ape_list)....   
+0000a370: 2069 6620 6465 6275 675f 6d6f 6465 203a   if debug_mode :
+0000a380: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+0000a390: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
+0000a3a0: 2822 203a 3a3a 3a3a 3a3a 3a3a 3a3a 3a20  (" :::::::::::: 
+0000a3b0: 6d6f 7665 2074 6865 2063 6f6e 6a75 6761  move the conjuga
+0000a3c0: 7465 6420 746f 2074 6865 2072 6967 6874  ted to the right
+0000a3d0: 206f 6620 6974 7320 7061 6972 203a 3a3a   of its pair :::
+0000a3e0: 3a3a 3a3a 3a3a 3a3a 2022 290d 0a20 2020  :::::::: ")..   
+0000a3f0: 2020 2020 2070 7269 6e74 2866 7375 6d6d       print(fsumm
+0000a400: 616e 645f 752c 223c 2d2d 2d20 6673 756d  and_u,"<--- fsum
+0000a410: 6d61 6e64 5f75 2229 0d0a 2020 2020 2020  mand_u")..      
+0000a420: 2020 7072 696e 7428 6673 756d 6d61 6e64    print(fsummand
+0000a430: 5f75 722c 223c 2d2d 2d20 6673 756d 6d61  _ur,"<--- fsumma
+0000a440: 6e64 5f75 7220 3d20 6d6f 7665 2074 6865  nd_ur = move the
+0000a450: 2063 6f6e 6a75 6761 7465 6420 746f 2074   conjugated to t
+0000a460: 6865 2072 6967 6874 206f 6620 6974 7320  he right of its 
+0000a470: 7061 6972 2229 0d0a 2020 2020 2020 2020  pair")..        
+0000a480: 7072 696e 7428 6673 7461 7473 5f75 722c  print(fstats_ur,
+0000a490: 223c 2d2d 2d20 6673 7461 7473 5f75 7222  "<--- fstats_ur"
+0000a4a0: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
+0000a4b0: 2866 7368 6170 655f 7572 2c22 3c2d 2d2d  (fshape_ur,"<---
+0000a4c0: 2066 7368 6170 655f 7572 2229 0d0a 2020   fshape_ur")..  
+0000a4d0: 2020 2020 2020 0d0a 2020 2020 2320 7265        ..    # re
+0000a4e0: 6d6f 7665 2074 6865 206c 6561 6469 6e67  move the leading
+0000a4f0: 2061 6e64 2074 7261 696c 696e 6720 6368   and trailing ch
+0000a500: 6172 7320 7468 6174 2069 7320 7468 6520  ars that is the 
+0000a510: 7361 6d65 2061 7320 7468 6520 7072 652d  same as the pre-
+0000a520: 7265 6172 7261 6e67 6564 2073 7472 696e  rearranged strin
+0000a530: 670d 0a0d 0a20 2020 206e 616c 6c5f 7520  g....    nall_u 
+0000a540: 3d20 6c65 6e28 6673 756d 6d61 6e64 5f75  = len(fsummand_u
+0000a550: 290d 0a0d 0a20 2020 206e 6c20 3d20 300d  )....    nl = 0.
+0000a560: 0a20 2020 2066 6f72 2069 2069 6e20 7261  .    for i in ra
+0000a570: 6e67 6528 6e61 6c6c 5f75 293a 0d0a 2020  nge(nall_u):..  
+0000a580: 2020 2020 2020 6966 2066 7375 6d6d 616e        if fsumman
+0000a590: 645f 755b 695d 2021 3d20 6673 756d 6d61  d_u[i] != fsumma
+0000a5a0: 6e64 5f75 725b 695d 3a0d 0a20 2020 2020  nd_ur[i]:..     
+0000a5b0: 2020 2020 2020 2062 7265 616b 0d0a 2020         break..  
+0000a5c0: 2020 2020 2020 6e6c 2b3d 310d 0a20 2020        nl+=1..   
+0000a5d0: 206e 7220 3d20 300d 0a20 2020 2066 6f72   nr = 0..    for
+0000a5e0: 2069 2069 6e20 7261 6e67 6528 6e61 6c6c   i in range(nall
+0000a5f0: 5f75 293a 0d0a 2020 2020 2020 2020 6966  _u):..        if
+0000a600: 2066 7375 6d6d 616e 645f 755b 6e61 6c6c   fsummand_u[nall
+0000a610: 5f75 2d31 2d69 5d20 213d 2066 7375 6d6d  _u-1-i] != fsumm
+0000a620: 616e 645f 7572 5b6e 616c 6c5f 752d 312d  and_ur[nall_u-1-
+0000a630: 695d 3a0d 0a20 2020 2020 2020 2020 2020  i]:..           
+0000a640: 2062 7265 616b 0d0a 2020 2020 2020 2020   break..        
+0000a650: 6e72 2b3d 310d 0a20 2020 206e 7220 3d20  nr+=1..    nr = 
+0000a660: 6e61 6c6c 5f75 2d6e 720d 0a0d 0a20 2020  nall_u-nr....   
+0000a670: 2066 7375 6d6d 616e 645f 7574 2020 3d20   fsummand_ut  = 
+0000a680: 6673 756d 6d61 6e64 5f75 5b6e 6c3a 6e72  fsummand_u[nl:nr
+0000a690: 5d0d 0a20 2020 2066 7374 6174 735f 7574  ]..    fstats_ut
+0000a6a0: 2020 203d 2066 7374 6174 735f 755b 6e6c     = fstats_u[nl
+0000a6b0: 3a6e 725d 0d0a 2020 2020 6673 6861 7065  :nr]..    fshape
+0000a6c0: 5f75 7420 2020 3d20 6673 6861 7065 5f75  _ut   = fshape_u
+0000a6d0: 5b6e 6c3a 6e72 5d0d 0a20 2020 2066 7375  [nl:nr]..    fsu
+0000a6e0: 6d6d 616e 645f 7572 7420 203d 2066 7375  mmand_urt  = fsu
+0000a6f0: 6d6d 616e 645f 7572 5b6e 6c3a 6e72 5d0d  mmand_ur[nl:nr].
+0000a700: 0a20 2020 2066 7374 6174 735f 7572 7420  .    fstats_urt 
+0000a710: 2020 3d20 6673 7461 7473 5f75 725b 6e6c    = fstats_ur[nl
+0000a720: 3a6e 725d 0d0a 2020 2020 6673 6861 7065  :nr]..    fshape
+0000a730: 5f75 7274 2020 203d 2066 7368 6170 655f  _urt   = fshape_
+0000a740: 7572 5b6e 6c3a 6e72 5d0d 0a0d 0a20 2020  ur[nl:nr]....   
+0000a750: 2069 6620 6e6c 3e6e 7220 3a0d 0a20 2020   if nl>nr :..   
+0000a760: 2020 2020 2073 6b69 705f 5331 203d 2054       skip_S1 = T
+0000a770: 7275 650d 0a20 2020 2065 6c73 653a 0d0a  rue..    else:..
+0000a780: 2020 2020 2020 2020 736b 6970 5f53 3120          skip_S1 
+0000a790: 3d20 4661 6c73 650d 0a0d 0a20 2020 2069  = False....    i
+0000a7a0: 6620 6465 6275 675f 6d6f 6465 203a 0d0a  f debug_mode :..
+0000a7b0: 2020 2020 2020 2020 7072 696e 7428 290d          print().
+0000a7c0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+0000a7d0: 203a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a   :::::::::::::::
+0000a7e0: 3a3a 3a3a 3a3a 3a3a 3a20 7472 696d 206c  ::::::::: trim l
+0000a7f0: 6566 7420 616e 6420 7269 6768 7420 3a3a  eft and right ::
+0000a800: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000a810: 3a3a 3a3a 3a3a 2022 290d 0a20 2020 2020  :::::: ")..     
+0000a820: 2020 2069 6620 736b 6970 5f53 3120 3a0d     if skip_S1 :.
+0000a830: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+0000a840: 6e74 2822 6673 756d 6d61 6e64 5f75 2061  nt("fsummand_u a
+0000a850: 6e64 2066 7375 6d6d 616e 645f 7572 2061  nd fsummand_ur a
+0000a860: 7265 2069 6465 6e74 6963 616c 2e22 290d  re identical.").
+0000a870: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+0000a880: 6e74 2822 5331 2063 616c 6375 6c61 7469  nt("S1 calculati
+0000a890: 6f6e 2069 7320 736b 6970 7065 642e 2229  on is skipped.")
+0000a8a0: 0d0a 2020 2020 2020 2020 656c 7365 203a  ..        else :
+0000a8b0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+0000a8c0: 696e 7428 6673 756d 6d61 6e64 5f75 2c22  int(fsummand_u,"
+0000a8d0: 3c2d 2d2d 2066 7375 6d6d 616e 645f 7522  <--- fsummand_u"
+0000a8e0: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
+0000a8f0: 7269 6e74 2866 7375 6d6d 616e 645f 7574  rint(fsummand_ut
+0000a900: 2c22 3c2d 2d2d 2066 7375 6d6d 616e 645f  ,"<--- fsummand_
+0000a910: 7574 203d 2074 7269 6d20 6673 756d 6d61  ut = trim fsumma
+0000a920: 6e64 5f75 206c 6566 7420 616e 6420 7269  nd_u left and ri
+0000a930: 6768 7422 290d 0a20 2020 2020 2020 2020  ght")..         
+0000a940: 2020 2070 7269 6e74 2866 7374 6174 735f     print(fstats_
+0000a950: 7574 2c22 3c2d 2d2d 2066 7374 6174 735f  ut,"<--- fstats_
+0000a960: 7574 2229 0d0a 2020 2020 2020 2020 2020  ut")..          
+0000a970: 2020 7072 696e 7428 6673 6861 7065 5f75    print(fshape_u
+0000a980: 742c 223c 2d2d 2d20 6673 6861 7065 5f75  t,"<--- fshape_u
+0000a990: 7422 290d 0a20 2020 2020 2020 2020 2020  t")..           
+0000a9a0: 2070 7269 6e74 2829 0d0a 2020 2020 2020   print()..      
+0000a9b0: 2020 2020 2020 7072 696e 7428 6673 756d        print(fsum
+0000a9c0: 6d61 6e64 5f75 722c 223c 2d2d 2d20 6673  mand_ur,"<--- fs
+0000a9d0: 756d 6d61 6e64 5f75 7222 290d 0a20 2020  ummand_ur")..   
+0000a9e0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+0000a9f0: 7375 6d6d 616e 645f 7572 742c 223c 2d2d  summand_urt,"<--
+0000aa00: 2d20 6673 756d 6d61 6e64 5f75 7274 203d  - fsummand_urt =
+0000aa10: 2074 7269 6d20 6673 756d 6d61 6e64 5f75   trim fsummand_u
+0000aa20: 7220 6c65 6674 2061 6e64 2072 6967 6874  r left and right
+0000aa30: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+0000aa40: 7072 696e 7428 6673 7461 7473 5f75 7274  print(fstats_urt
+0000aa50: 2c22 3c2d 2d2d 2066 7374 6174 735f 7572  ,"<--- fstats_ur
+0000aa60: 7422 290d 0a20 2020 2020 2020 2020 2020  t")..           
+0000aa70: 2070 7269 6e74 2866 7368 6170 655f 7572   print(fshape_ur
+0000aa80: 742c 223c 2d2d 2d20 6673 6861 7065 5f75  t,"<--- fshape_u
+0000aa90: 7274 2229 0d0a 2020 2020 2020 2020 0d0a  rt")..        ..
+0000aaa0: 2020 2020 5331 5f73 676e 5f63 6f6d 7075      S1_sgn_compu
+0000aab0: 7461 7469 6f6e 5f73 7472 696e 6720 3d20  tation_string = 
+0000aac0: 6673 756d 6d61 6e64 5f75 742b 222d 3e22  fsummand_ut+"->"
+0000aad0: 2b66 7375 6d6d 616e 645f 7572 740d 0a20  +fsummand_urt.. 
+0000aae0: 2020 200d 0a20 2020 2069 6620 6465 6275     ..    if debu
+0000aaf0: 675f 6d6f 6465 2061 6e64 206e 6f74 2073  g_mode and not s
+0000ab00: 6b69 705f 5331 203a 0d0a 2020 2020 2020  kip_S1 :..      
+0000ab10: 2020 7072 696e 7428 290d 0a20 2020 2020    print()..     
+0000ab20: 2020 2070 7269 6e74 2853 315f 7367 6e5f     print(S1_sgn_
+0000ab30: 636f 6d70 7574 6174 696f 6e5f 7374 7269  computation_stri
+0000ab40: 6e67 2c22 3c2d 2d2d 2073 7472 696e 6720  ng,"<--- string 
+0000ab50: 7573 6564 2069 6e20 5331 2063 6f6d 7075  used in S1 compu
+0000ab60: 7461 7469 6f6e 2229 0d0a 2020 2020 0d0a  tation")..    ..
+0000ab70: 2020 2020 2320 7265 6d6f 7665 2074 6865      # remove the
+0000ab80: 2063 6f6e 6a75 6761 7465 6420 6368 6172   conjugated char
+0000ab90: 6163 7465 7220 6966 2062 6f74 6820 7468  acter if both th
+0000aba0: 6520 6e6f 6e6e 636f 6e6a 7567 6174 6564  e nonnconjugated
+0000abb0: 2061 6e64 2063 6f6e 6a75 6761 7465 6420   and conjugated 
+0000abc0: 6172 6520 7072 6573 656e 740d 0a20 2020  are present..   
+0000abd0: 200d 0a20 2020 2023 2064 6f20 7468 6520   ..    # do the 
+0000abe0: 7574 206f 6e6c 790d 0a20 2020 2066 7375  ut only..    fsu
+0000abf0: 6d6d 616e 645f 7574 7820 3d20 2222 0d0a  mmand_utx = ""..
+0000ac00: 2020 2020 6673 7461 7473 5f75 7478 2020      fstats_utx  
+0000ac10: 203d 205b 5d0d 0a20 2020 2066 7368 6170   = []..    fshap
+0000ac20: 655f 7574 7820 2020 3d20 5b5d 0d0a 2020  e_utx   = []..  
+0000ac30: 2020 6e61 6c6c 5f75 7420 3d20 6c65 6e28    nall_ut = len(
+0000ac40: 6673 756d 6d61 6e64 5f75 7429 0d0a 2020  fsummand_ut)..  
+0000ac50: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+0000ac60: 286e 616c 6c5f 7574 293a 0d0a 2020 2020  (nall_ut):..    
+0000ac70: 2020 2020 6320 3d20 6673 756d 6d61 6e64      c = fsummand
+0000ac80: 5f75 745b 695d 0d0a 2020 2020 2020 2020  _ut[i]..        
+0000ac90: 746f 5f73 6b69 7020 3d20 4661 6c73 650d  to_skip = False.
+0000aca0: 0a20 2020 2020 2020 2069 6620 6673 7461  .        if fsta
+0000acb0: 7473 5f75 745b 695d 3d3d 2d31 203a 0d0a  ts_ut[i]==-1 :..
+0000acc0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000acd0: 5b20 5b63 312c 6332 5d2c 206c 6f63 205d  [ [c1,c2], loc ]
+0000ace0: 2069 6e20 7375 6d6d 6564 5f69 6e64 6578   in summed_index
+0000acf0: 5f69 6e66 6f3a 0d0a 2020 2020 2020 2020  _info:..        
+0000ad00: 2020 2020 2020 2020 6966 2063 3d3d 6332          if c==c2
+0000ad10: 2061 6e64 2066 7375 6d6d 616e 645f 7574   and fsummand_ut
+0000ad20: 2e63 6f75 6e74 2863 3129 3e30 3a0d 0a20  .count(c1)>0:.. 
+0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad40: 2020 2074 6f5f 736b 6970 203d 2054 7275     to_skip = Tru
+0000ad50: 650d 0a20 2020 2020 2020 2069 6620 746f  e..        if to
+0000ad60: 5f73 6b69 7020 3a0d 0a20 2020 2020 2020  _skip :..       
+0000ad70: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
+0000ad80: 2020 2020 2020 2066 7375 6d6d 616e 645f         fsummand_
+0000ad90: 7574 7820 2b3d 2066 7375 6d6d 616e 645f  utx += fsummand_
+0000ada0: 7574 5b69 5d0d 0a20 2020 2020 2020 2066  ut[i]..        f
+0000adb0: 7374 6174 735f 7574 7820 2020 2b3d 2066  stats_utx   += f
+0000adc0: 7374 6174 735f 7574 5b69 5d2c 0d0a 2020  stats_ut[i],..  
+0000add0: 2020 2020 2020 6673 6861 7065 5f75 7478        fshape_utx
+0000ade0: 2020 202b 3d20 6673 6861 7065 5f75 745b     += fshape_ut[
+0000adf0: 695d 2c0d 0a20 2020 2053 3164 696d 203d  i],..    S1dim =
+0000ae00: 206c 656e 2866 7375 6d6d 616e 645f 7574   len(fsummand_ut
+0000ae10: 7829 0d0a 0d0a 2020 2020 6966 2064 6562  x)....    if deb
+0000ae20: 7567 5f6d 6f64 6520 616e 6420 6e6f 7420  ug_mode and not 
+0000ae30: 736b 6970 5f53 3120 3a0d 0a20 2020 2020  skip_S1 :..     
+0000ae40: 2020 2070 7269 6e74 2829 0d0a 2020 2020     print()..    
+0000ae50: 2020 2020 7072 696e 7428 2220 3a3a 3a3a      print(" ::::
+0000ae60: 3a3a 3a20 7265 6d6f 7665 2074 6865 2063  ::: remove the c
+0000ae70: 6f6e 6a75 6761 7465 6420 6966 2062 6f74  onjugated if bot
+0000ae80: 6820 6f66 2074 6865 2070 6169 7220 6172  h of the pair ar
+0000ae90: 6520 7072 6573 656e 7420 3a3a 3a3a 3a3a  e present ::::::
+0000aea0: 3a20 2229 0d0a 2020 2020 2020 2020 7072  : ")..        pr
+0000aeb0: 696e 7428 6673 756d 6d61 6e64 5f75 742c  int(fsummand_ut,
+0000aec0: 223c 2d2d 2d20 6673 756d 6d61 6e64 5f75  "<--- fsummand_u
+0000aed0: 7422 290d 0a20 2020 2020 2020 2070 7269  t")..        pri
+0000aee0: 6e74 2866 7375 6d6d 616e 645f 7574 782c  nt(fsummand_utx,
+0000aef0: 223c 2d2d 2d20 6673 756d 6d61 6e64 5f75  "<--- fsummand_u
+0000af00: 7478 203d 2072 656d 6f76 6520 6f6e 206f  tx = remove on o
+0000af10: 6620 7468 6520 7061 6972 2229 0d0a 2020  f the pair")..  
+0000af20: 2020 2020 2020 7072 696e 7428 6673 7461        print(fsta
+0000af30: 7473 5f75 7478 2c22 3c2d 2d2d 2066 7374  ts_utx,"<--- fst
+0000af40: 6174 735f 7574 7822 290d 0a20 2020 2020  ats_utx")..     
+0000af50: 2020 2070 7269 6e74 2866 7368 6170 655f     print(fshape_
+0000af60: 7574 782c 223c 2d2d 2d20 6673 6861 7065  utx,"<--- fshape
+0000af70: 5f75 7478 2229 0d0a 2020 2020 0d0a 2020  _utx")..    ..  
+0000af80: 2020 2320 6d61 6b65 2074 6865 2063 6f70    # make the cop
+0000af90: 7920 6d61 700d 0a20 2020 2063 6f70 795f  y map..    copy_
+0000afa0: 6d61 7020 3d20 5b5d 0d0a 2020 2020 6673  map = []..    fs
+0000afb0: 756d 6d61 6e64 5f75 7478 5f72 203d 206c  ummand_utx_r = l
+0000afc0: 6973 7428 6673 756d 6d61 6e64 5f75 7478  ist(fsummand_utx
+0000afd0: 2920 2374 6869 7320 6973 2075 7365 6420  ) #this is used 
+0000afe0: 696e 2074 6865 206d 6f63 6b20 7265 636f  in the mock reco
+0000aff0: 6e73 7472 7563 7469 6f6e 0d0a 2020 2020  nstruction..    
+0000b000: 666f 7220 695f 7574 2c20 6320 696e 2065  for i_ut, c in e
+0000b010: 6e75 6d65 7261 7465 2866 7375 6d6d 616e  numerate(fsumman
+0000b020: 645f 7574 293a 0d0a 2020 2020 2020 2020  d_ut):..        
+0000b030: 6966 2063 206e 6f74 2069 6e20 6673 756d  if c not in fsum
+0000b040: 6d61 6e64 5f75 7478 3a0d 0a20 2020 2020  mand_utx:..     
+0000b050: 2020 2020 2020 2023 6669 6e64 2074 6865         #find the
+0000b060: 206c 6f63 6174 696f 6e20 6f66 2069 7473   location of its
+0000b070: 2070 6169 7220 6669 7273 740d 0a20 2020   pair first..   
+0000b080: 2020 2020 2020 2020 2063 5f70 6169 7220           c_pair 
+0000b090: 3d20 223f 220d 0a20 2020 2020 2020 2020  = "?"..         
+0000b0a0: 2020 2066 6f72 205b 5b63 312c 6332 5d2c     for [[c1,c2],
+0000b0b0: 5f5d 2069 6e20 7375 6d6d 6564 5f69 6e64  _] in summed_ind
+0000b0c0: 6578 5f69 6e66 6f3a 0d0a 2020 2020 2020  ex_info:..      
+0000b0d0: 2020 2020 2020 2020 2020 6966 2063 3d3d            if c==
+0000b0e0: 6332 203a 0d0a 2020 2020 2020 2020 2020  c2 :..          
+0000b0f0: 2020 2020 2020 2020 2020 695f 7574 7820            i_utx 
+0000b100: 3d20 6673 756d 6d61 6e64 5f75 7478 5f72  = fsummand_utx_r
+0000b110: 2e69 6e64 6578 2863 3129 0d0a 2020 2020  .index(c1)..    
+0000b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b130: 635f 7061 6972 203d 2063 310d 0a20 2020  c_pair = c1..   
+0000b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b150: 2062 7265 616b 0d0a 2020 2020 2020 2020   break..        
+0000b160: 2020 2020 636f 7079 5f6d 6170 202b 3d20      copy_map += 
+0000b170: 5b69 5f75 742c 695f 7574 785d 2c0d 0a20  [i_ut,i_utx],.. 
+0000b180: 2020 2020 2020 2020 2020 2066 7375 6d6d             fsumm
+0000b190: 616e 645f 7574 785f 722e 696e 7365 7274  and_utx_r.insert
+0000b1a0: 2869 5f75 742c 6329 0d0a 2020 2020 0d0a  (i_ut,c)..    ..
+0000b1b0: 2020 2020 6465 6620 7573 655f 636f 7079      def use_copy
+0000b1c0: 5f6d 6170 2874 6865 5f6d 6170 2c74 6865  _map(the_map,the
+0000b1d0: 5f6c 6973 742c 6170 706c 795f 6e65 6761  _list,apply_nega
+0000b1e0: 7469 7665 3d46 616c 7365 293a 0d0a 2020  tive=False):..  
+0000b1f0: 2020 2020 2020 6e65 775f 6c69 7374 203d        new_list =
+0000b200: 206c 6973 7428 7468 655f 6c69 7374 292e   list(the_list).
+0000b210: 636f 7079 2829 0d0a 2020 2020 2020 2020  copy()..        
+0000b220: 666f 7220 5b69 322c 6931 5d20 696e 2074  for [i2,i1] in t
+0000b230: 6865 5f6d 6170 203a 0d0a 2020 2020 2020  he_map :..      
+0000b240: 2020 2020 2020 6966 2061 7070 6c79 5f6e        if apply_n
+0000b250: 6567 6174 6976 6520 3a0d 0a20 2020 2020  egative :..     
+0000b260: 2020 2020 2020 2020 2020 206e 6577 5f6c             new_l
+0000b270: 6973 742e 696e 7365 7274 2869 322c 2d6e  ist.insert(i2,-n
+0000b280: 6577 5f6c 6973 745b 6931 5d29 0d0a 2020  ew_list[i1])..  
+0000b290: 2020 2020 2020 2020 2020 656c 7365 203a            else :
+0000b2a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b2b0: 2020 6e65 775f 6c69 7374 2e69 6e73 6572    new_list.inser
+0000b2c0: 7428 6932 2c6e 6577 5f6c 6973 745b 6931  t(i2,new_list[i1
+0000b2d0: 5d29 0d0a 2020 2020 2020 2020 7265 7475  ])..        retu
+0000b2e0: 726e 206e 6577 5f6c 6973 740d 0a20 2020  rn new_list..   
+0000b2f0: 200d 0a20 2020 2069 6620 6465 6275 675f   ..    if debug_
+0000b300: 6d6f 6465 2061 6e64 206e 6f74 2073 6b69  mode and not ski
+0000b310: 705f 5331 3a0d 0a20 2020 2020 2020 2070  p_S1:..        p
+0000b320: 7269 6e74 2829 0d0a 2020 2020 2020 2020  rint()..        
+0000b330: 7072 696e 7428 2220 3a3a 3a3a 3a3a 3a3a  print(" ::::::::
+0000b340: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000b350: 3a3a 2074 6573 7469 6e67 2063 6f70 795f  :: testing copy_
+0000b360: 6d61 7020 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  map ::::::::::::
+0000b370: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a20 2229  ::::::::::::: ")
+0000b380: 0d0a 2020 2020 2020 2020 6673 756d 6d61  ..        fsumma
+0000b390: 6e64 5f75 7432 203d 2027 272e 6a6f 696e  nd_ut2 = ''.join
+0000b3a0: 2875 7365 5f63 6f70 795f 6d61 7028 636f  (use_copy_map(co
+0000b3b0: 7079 5f6d 6170 2c6c 6973 7428 6673 756d  py_map,list(fsum
+0000b3c0: 6d61 6e64 5f75 7478 2929 290d 0a20 2020  mand_utx)))..   
+0000b3d0: 2020 2020 2066 7374 6174 735f 7574 3220       fstats_ut2 
+0000b3e0: 3d20 7573 655f 636f 7079 5f6d 6170 2863  = use_copy_map(c
+0000b3f0: 6f70 795f 6d61 702c 6673 7461 7473 5f75  opy_map,fstats_u
+0000b400: 7478 2c61 7070 6c79 5f6e 6567 6174 6976  tx,apply_negativ
+0000b410: 653d 5472 7565 290d 0a20 2020 2020 2020  e=True)..       
+0000b420: 2066 7368 6170 655f 7574 3220 3d20 7573   fshape_ut2 = us
+0000b430: 655f 636f 7079 5f6d 6170 2863 6f70 795f  e_copy_map(copy_
+0000b440: 6d61 702c 6673 6861 7065 5f75 7478 290d  map,fshape_utx).
+0000b450: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+0000b460: 2022 2c66 7375 6d6d 616e 645f 7574 322c   ",fsummand_ut2,
+0000b470: 2276 7322 2c66 7375 6d6d 616e 645f 7574  "vs",fsummand_ut
+0000b480: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
+0000b490: 2822 2022 2c66 7374 6174 735f 7574 322c  (" ",fstats_ut2,
+0000b4a0: 2276 7322 2c66 7374 6174 735f 7574 290d  "vs",fstats_ut).
+0000b4b0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+0000b4c0: 2022 2c66 7368 6170 655f 7574 322c 2276   ",fshape_ut2,"v
+0000b4d0: 7322 2c66 7368 6170 655f 7574 290d 0a20  s",fshape_ut).. 
+0000b4e0: 2020 2020 2020 200d 0a20 2020 2023 2066         ..    # f
+0000b4f0: 7375 6d6d 616e 645f 7574 7820 6e65 6564  summand_utx need
+0000b500: 7320 746f 2062 6520 7265 706c 6163 6564  s to be replaced
+0000b510: 2077 6974 6820 7468 6520 6f72 6967 696e   with the origin
+0000b520: 616c 2069 6e64 6963 6573 2074 6f20 6f62  al indices to ob
+0000b530: 7461 696e 2053 315f 696e 6465 785f 7374  tain S1_index_st
+0000b540: 7269 6e67 0d0a 2020 2020 5331 5f69 6e64  ring..    S1_ind
+0000b550: 6578 5f73 7472 696e 6720 203d 2022 220d  ex_string  = "".
+0000b560: 0a20 2020 2066 6f72 2063 2069 6e20 6673  .    for c in fs
+0000b570: 756d 6d61 6e64 5f75 7478 3a0d 0a20 2020  ummand_utx:..   
+0000b580: 2020 2020 2069 6620 6320 696e 2073 756d       if c in sum
+0000b590: 6d61 6e64 3a0d 0a20 2020 2020 2020 2020  mand:..         
+0000b5a0: 2020 2053 315f 696e 6465 785f 7374 7269     S1_index_stri
+0000b5b0: 6e67 202b 3d20 630d 0a20 2020 2020 2020  ng += c..       
+0000b5c0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+0000b5d0: 2020 2020 666f 7220 5b20 5b63 312c 6332      for [ [c1,c2
+0000b5e0: 5d2c 206c 6f63 205d 2069 6e20 7375 6d6d  ], loc ] in summ
+0000b5f0: 6564 5f69 6e64 6578 5f69 6e66 6f3a 0d0a  ed_index_info:..
+0000b600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b610: 6966 2063 3d3d 6332 203a 0d0a 2020 2020  if c==c2 :..    
+0000b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b630: 5331 5f69 6e64 6578 5f73 7472 696e 6720  S1_index_string 
+0000b640: 2b3d 2063 310d 0a20 2020 2020 2020 2020  += c1..         
+0000b650: 2020 2020 2020 2020 2020 2062 7265 616b             break
+0000b660: 0d0a 2020 2020 5331 5f73 6861 7065 203d  ..    S1_shape =
+0000b670: 205b 5d0d 0a20 2020 2066 6f72 2063 2069   []..    for c i
+0000b680: 6e20 5331 5f69 6e64 6578 5f73 7472 696e  n S1_index_strin
+0000b690: 673a 0d0a 2020 2020 2020 2020 696e 6420  g:..        ind 
+0000b6a0: 3d20 6673 756d 6d61 6e64 2e69 6e64 6578  = fsummand.index
+0000b6b0: 2863 290d 0a20 2020 2020 2020 2053 315f  (c)..        S1_
+0000b6c0: 7368 6170 6520 2b3d 2066 7368 6170 655b  shape += fshape[
+0000b6d0: 696e 645d 2c0d 0a20 2020 2053 315f 7368  ind],..    S1_sh
+0000b6e0: 6170 6520 3d20 6d61 6b65 5f74 7570 6c65  ape = make_tuple
+0000b6f0: 2853 315f 7368 6170 6529 0d0a 2020 2020  (S1_shape)..    
+0000b700: 0d0a 2020 2020 6966 2064 6562 7567 5f6d  ..    if debug_m
+0000b710: 6f64 6520 616e 6420 6e6f 7420 736b 6970  ode and not skip
+0000b720: 5f53 3120 3a0d 0a20 2020 2020 2020 2070  _S1 :..        p
+0000b730: 7269 6e74 2829 0d0a 2020 2020 2020 2020  rint()..        
+0000b740: 7072 696e 7428 2220 3a3a 3a3a 3a3a 3a3a  print(" ::::::::
+0000b750: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000b760: 3a3a 3a3a 3a3a 2053 3120 7374 7566 6620  :::::: S1 stuff 
 0000b770: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000b780: 3a20 5331 2073 7475 6666 203a 3a3a 3a3a  : S1 stuff :::::
-0000b790: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000b7a0: 3a3a 3a3a 3a3a 3a3a 2022 290d 0a20 2020  :::::::: ")..   
-0000b7b0: 2020 2020 2070 7269 6e74 2853 315f 696e       print(S1_in
-0000b7c0: 6465 785f 7374 7269 6e67 2c22 3c2d 2d2d  dex_string,"<---
-0000b7d0: 2053 3127 7320 696e 6465 7820 7374 7269   S1's index stri
-0000b7e0: 6e67 2229 0d0a 2020 2020 2020 2020 7072  ng")..        pr
-0000b7f0: 696e 7428 5331 5f73 6861 7065 2c22 3c2d  int(S1_shape,"<-
-0000b800: 2d2d 2053 3127 7320 7368 6170 6522 290d  -- S1's shape").
-0000b810: 0a20 2020 2020 2020 200d 0a20 2020 2023  .        ..    #
-0000b820: 2073 6967 6e20 6661 6374 6f72 2063 6f6d   sign factor com
-0000b830: 7075 7461 7469 6f6e 202d 2d2d 2d2d 2d2d  putation -------
+0000b780: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a20 2229  ::::::::::::: ")
+0000b790: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+0000b7a0: 5331 5f69 6e64 6578 5f73 7472 696e 672c  S1_index_string,
+0000b7b0: 223c 2d2d 2d20 5331 2773 2069 6e64 6578  "<--- S1's index
+0000b7c0: 2073 7472 696e 6722 290d 0a20 2020 2020   string")..     
+0000b7d0: 2020 2070 7269 6e74 2853 315f 7368 6170     print(S1_shap
+0000b7e0: 652c 223c 2d2d 2d20 5331 2773 2073 6861  e,"<--- S1's sha
+0000b7f0: 7065 2229 0d0a 2020 2020 2020 2020 0d0a  pe")..        ..
+0000b800: 2020 2020 2320 7369 676e 2066 6163 746f      # sign facto
+0000b810: 7220 636f 6d70 7574 6174 696f 6e20 2d2d  r computation --
+0000b820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000b840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 0000b850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000b880: 2d2d 0d0a 2020 2020 0d0a 2020 2020 6966  --..    ..    if
-0000b890: 2053 3164 696d 3e30 2061 6e64 206e 6f74   S1dim>0 and not
-0000b8a0: 2073 6b69 705f 5331 3a0d 0a0d 0a20 2020   skip_S1:....   
-0000b8b0: 2020 2020 2053 3120 3d20 6e70 2e7a 6572       S1 = np.zer
-0000b8c0: 6f73 2853 315f 7368 6170 652c 6474 7970  os(S1_shape,dtyp
-0000b8d0: 653d 696e 7429 0d0a 2020 2020 2020 2020  e=int)..        
-0000b8e0: 6974 6572 6174 6f72 203d 206e 702e 6e64  iterator = np.nd
-0000b8f0: 6974 6572 2853 312c 2066 6c61 6773 3d5b  iter(S1, flags=[
-0000b900: 276d 756c 7469 5f69 6e64 6578 275d 290d  'multi_index']).
-0000b910: 0a20 2020 2020 2020 2069 6e64 6976 6964  .        individ
-0000b920: 7561 6c5f 7061 7269 7479 5f6c 6973 7420  ual_parity_list 
-0000b930: 3d20 5b5d 0d0a 2020 2020 2020 2020 7367  = []..        sg
-0000b940: 6e5f 6c69 7374 203d 205b 5d0d 0a0d 0a20  n_list = [].... 
-0000b950: 2020 2020 2020 206b 3d31 0d0a 2020 2020         k=1..    
-0000b960: 2020 2020 6b6d 6178 203d 2067 6574 7369      kmax = getsi
-0000b970: 7a65 2853 315f 7368 6170 6529 0d0a 0d0a  ze(S1_shape)....
-0000b980: 2020 2020 2020 2020 7330 203d 2074 696d          s0 = tim
-0000b990: 652e 7469 6d65 2829 0d0a 2020 2020 2020  e.time()..      
-0000b9a0: 2020 7330 3020 3d20 7330 0d0a 2020 2020    s00 = s0..    
-0000b9b0: 2020 2020 7072 696e 7428 2920 2320 3c3c      print() # <<
-0000b9c0: 2044 6f6e 2774 2072 656d 6f76 6520 7468   Don't remove th
-0000b9d0: 6973 2e20 5468 6973 2069 7320 666f 7220  is. This is for 
-0000b9e0: 7468 6520 7368 6f77 5f70 726f 6772 6573  the show_progres
-0000b9f0: 7321 0d0a 0d0a 2020 2020 2020 2020 666f  s!....        fo
-0000ba00: 7220 656c 656d 656e 7420 696e 2069 7465  r element in ite
-0000ba10: 7261 746f 723a 0d0a 2020 2020 2020 2020  rator:..        
-0000ba20: 2020 2020 636f 6f72 6473 203d 2069 7465      coords = ite
-0000ba30: 7261 746f 722e 6d75 6c74 695f 696e 6465  rator.multi_inde
-0000ba40: 780d 0a20 2020 2020 2020 2020 2020 2064  x..            d
-0000ba50: 7570 7065 645f 636f 6f72 6473 203d 2075  upped_coords = u
-0000ba60: 7365 5f63 6f70 795f 6d61 7028 636f 7079  se_copy_map(copy
-0000ba70: 5f6d 6170 2c63 6f6f 7264 7329 0d0a 2020  _map,coords)..  
-0000ba80: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000ba90: 2020 2020 2020 2020 696e 6469 7669 6475          individu
-0000baa0: 616c 5f70 6172 6974 7920 3d20 5b20 7061  al_parity = [ pa
-0000bab0: 7261 6d2e 6770 6172 6974 7928 6929 2532  ram.gparity(i)%2
-0000bac0: 2066 6f72 2069 2069 6e20 6475 7070 6564   for i in dupped
-0000bad0: 5f63 6f6f 7264 7320 5d0d 0a0d 0a20 2020  _coords ]....   
-0000bae0: 2020 2020 2020 2020 2069 6620 696e 6469           if indi
-0000baf0: 7669 6475 616c 5f70 6172 6974 7920 6e6f  vidual_parity no
-0000bb00: 7420 696e 2069 6e64 6976 6964 7561 6c5f  t in individual_
-0000bb10: 7061 7269 7479 5f6c 6973 743a 0d0a 2020  parity_list:..  
-0000bb20: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000bb30: 6469 7669 6475 616c 5f70 6172 6974 795f  dividual_parity_
-0000bb40: 6c69 7374 202b 3d20 696e 6469 7669 6475  list += individu
-0000bb50: 616c 5f70 6172 6974 792c 0d0a 2020 2020  al_parity,..    
-0000bb60: 2020 2020 2020 2020 2020 2020 7367 6e20              sgn 
-0000bb70: 3d20 7265 6c61 7469 7665 5f70 6172 6974  = relative_parit
-0000bb80: 7928 5331 5f73 676e 5f63 6f6d 7075 7461  y(S1_sgn_computa
-0000bb90: 7469 6f6e 5f73 7472 696e 672c 696e 6469  tion_string,indi
-0000bba0: 7669 6475 616c 5f70 6172 6974 7929 0d0a  vidual_parity)..
-0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbc0: 7367 6e5f 6c69 7374 202b 3d20 7367 6e2c  sgn_list += sgn,
-0000bbd0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-0000bbe0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0000bbf0: 2020 2020 2069 6e64 6578 203d 2069 6e64       index = ind
-0000bc00: 6976 6964 7561 6c5f 7061 7269 7479 5f6c  ividual_parity_l
-0000bc10: 6973 742e 696e 6465 7828 696e 6469 7669  ist.index(indivi
-0000bc20: 6475 616c 5f70 6172 6974 7929 0d0a 2020  dual_parity)..  
-0000bc30: 2020 2020 2020 2020 2020 2020 2020 7367                sg
-0000bc40: 6e20 3d20 7367 6e5f 6c69 7374 5b69 6e64  n = sgn_list[ind
-0000bc50: 6578 5d0d 0a0d 0a20 2020 2020 2020 2020  ex]....         
-0000bc60: 2020 2053 315b 636f 6f72 6473 5d20 3d20     S1[coords] = 
-0000bc70: 7367 6e0d 0a0d 0a20 2020 2020 2020 2020  sgn....         
-0000bc80: 2020 2069 6620 7469 6d65 2e74 696d 6528     if time.time(
-0000bc90: 292d 7330 203e 2032 203a 0d0a 2020 2020  )-s0 > 2 :..    
-0000bca0: 2020 2020 2020 2020 2020 2020 7368 6f77              show
-0000bcb0: 5f70 726f 6772 6573 7328 6b2c 6b6d 6178  _progress(k,kmax
-0000bcc0: 2b31 2c70 726f 6365 7373 5f6e 616d 6520  +1,process_name 
-0000bcd0: 3d20 2265 696e 7375 6d5f 7367 6e31 222c  = "einsum_sgn1",
-0000bce0: 7261 7469 6f20 3d20 4661 6c73 652c 636f  ratio = False,co
-0000bcf0: 6c6f 723d 2272 6564 222c 7469 6d65 3d74  lor="red",time=t
-0000bd00: 696d 652e 7469 6d65 2829 2d73 3030 290d  ime.time()-s00).
-0000bd10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bd20: 2073 3020 3d20 7469 6d65 2e74 696d 6528   s0 = time.time(
-0000bd30: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
-0000bd40: 0a20 2020 2020 2020 2020 2020 206b 2b3d  .            k+=
-0000bd50: 310d 0a0d 0a20 2020 2020 2020 2063 6c65  1....        cle
-0000bd60: 6172 5f70 726f 6772 6573 7328 290d 0a20  ar_progress().. 
-0000bd70: 2020 2020 2020 2073 7973 2e73 7464 6f75         sys.stdou
-0000bd80: 742e 7772 6974 6528 225c 3033 335b 4622  t.write("\033[F"
-0000bd90: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-0000bda0: 2023 2020 3a3a 3a20 5375 6d6d 6172 7920   #  ::: Summary 
-0000bdb0: 3a3a 3a0d 0a20 2020 2023 0d0a 2020 2020  :::..    #..    
-0000bdc0: 2320 2053 3120 6973 2074 6865 2073 6967  #  S1 is the sig
-0000bdd0: 6e20 6661 6374 6f72 2066 726f 6d20 7468  n factor from th
-0000bde0: 6520 696e 6974 6961 6c20 7265 6172 7261  e initial rearra
-0000bdf0: 6e67 656d 656e 740d 0a20 2020 2023 2020  ngement..    #  
-0000be00: 4974 7320 696e 6465 7820 7374 7269 6e67  Its index string
-0000be10: 2069 7320 5331 5f69 6e64 6578 5f73 7472   is S1_index_str
-0000be20: 696e 670d 0a0d 0a20 2020 2023 3a3a 3a3a  ing....    #::::
+0000b860: 2d2d 2d2d 2d2d 2d0d 0a20 2020 200d 0a20  -------..    .. 
+0000b870: 2020 2069 6620 5331 6469 6d3e 3020 616e     if S1dim>0 an
+0000b880: 6420 6e6f 7420 736b 6970 5f53 313a 0d0a  d not skip_S1:..
+0000b890: 0d0a 2020 2020 2020 2020 5331 203d 206e  ..        S1 = n
+0000b8a0: 702e 7a65 726f 7328 5331 5f73 6861 7065  p.zeros(S1_shape
+0000b8b0: 2c64 7479 7065 3d69 6e74 290d 0a20 2020  ,dtype=int)..   
+0000b8c0: 2020 2020 2069 7465 7261 746f 7220 3d20       iterator = 
+0000b8d0: 6e70 2e6e 6469 7465 7228 5331 2c20 666c  np.nditer(S1, fl
+0000b8e0: 6167 733d 5b27 6d75 6c74 695f 696e 6465  ags=['multi_inde
+0000b8f0: 7827 5d29 0d0a 2020 2020 2020 2020 696e  x'])..        in
+0000b900: 6469 7669 6475 616c 5f70 6172 6974 795f  dividual_parity_
+0000b910: 6c69 7374 203d 205b 5d0d 0a20 2020 2020  list = []..     
+0000b920: 2020 2073 676e 5f6c 6973 7420 3d20 5b5d     sgn_list = []
+0000b930: 0d0a 0d0a 2020 2020 2020 2020 6b3d 310d  ....        k=1.
+0000b940: 0a20 2020 2020 2020 206b 6d61 7820 3d20  .        kmax = 
+0000b950: 6765 7473 697a 6528 5331 5f73 6861 7065  getsize(S1_shape
+0000b960: 290d 0a0d 0a20 2020 2020 2020 2073 3020  )....        s0 
+0000b970: 3d20 7469 6d65 2e74 696d 6528 290d 0a20  = time.time().. 
+0000b980: 2020 2020 2020 2073 3030 203d 2073 300d         s00 = s0.
+0000b990: 0a20 2020 2020 2020 2070 726f 6772 6573  .        progres
+0000b9a0: 735f 7370 6163 6528 2920 2320 3c3c 2044  s_space() # << D
+0000b9b0: 6f6e 2774 2072 656d 6f76 6520 7468 6973  on't remove this
+0000b9c0: 2e20 5468 6973 2069 7320 666f 7220 7468  . This is for th
+0000b9d0: 6520 7368 6f77 5f70 726f 6772 6573 7321  e show_progress!
+0000b9e0: 0d0a 0d0a 2020 2020 2020 2020 666f 7220  ....        for 
+0000b9f0: 656c 656d 656e 7420 696e 2069 7465 7261  element in itera
+0000ba00: 746f 723a 0d0a 2020 2020 2020 2020 2020  tor:..          
+0000ba10: 2020 636f 6f72 6473 203d 2069 7465 7261    coords = itera
+0000ba20: 746f 722e 6d75 6c74 695f 696e 6465 780d  tor.multi_index.
+0000ba30: 0a20 2020 2020 2020 2020 2020 2064 7570  .            dup
+0000ba40: 7065 645f 636f 6f72 6473 203d 2075 7365  ped_coords = use
+0000ba50: 5f63 6f70 795f 6d61 7028 636f 7079 5f6d  _copy_map(copy_m
+0000ba60: 6170 2c63 6f6f 7264 7329 0d0a 2020 2020  ap,coords)..    
+0000ba70: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000ba80: 2020 2020 2020 696e 6469 7669 6475 616c        individual
+0000ba90: 5f70 6172 6974 7920 3d20 5b20 7061 7261  _parity = [ para
+0000baa0: 6d2e 6770 6172 6974 7928 6929 2532 2066  m.gparity(i)%2 f
+0000bab0: 6f72 2069 2069 6e20 6475 7070 6564 5f63  or i in dupped_c
+0000bac0: 6f6f 7264 7320 5d0d 0a0d 0a20 2020 2020  oords ]....     
+0000bad0: 2020 2020 2020 2069 6620 696e 6469 7669         if indivi
+0000bae0: 6475 616c 5f70 6172 6974 7920 6e6f 7420  dual_parity not 
+0000baf0: 696e 2069 6e64 6976 6964 7561 6c5f 7061  in individual_pa
+0000bb00: 7269 7479 5f6c 6973 743a 0d0a 2020 2020  rity_list:..    
+0000bb10: 2020 2020 2020 2020 2020 2020 696e 6469              indi
+0000bb20: 7669 6475 616c 5f70 6172 6974 795f 6c69  vidual_parity_li
+0000bb30: 7374 202b 3d20 696e 6469 7669 6475 616c  st += individual
+0000bb40: 5f70 6172 6974 792c 0d0a 2020 2020 2020  _parity,..      
+0000bb50: 2020 2020 2020 2020 2020 7367 6e20 3d20            sgn = 
+0000bb60: 7265 6c61 7469 7665 5f70 6172 6974 7928  relative_parity(
+0000bb70: 5331 5f73 676e 5f63 6f6d 7075 7461 7469  S1_sgn_computati
+0000bb80: 6f6e 5f73 7472 696e 672c 696e 6469 7669  on_string,indivi
+0000bb90: 6475 616c 5f70 6172 6974 7929 0d0a 2020  dual_parity)..  
+0000bba0: 2020 2020 2020 2020 2020 2020 2020 7367                sg
+0000bbb0: 6e5f 6c69 7374 202b 3d20 7367 6e2c 0d0a  n_list += sgn,..
+0000bbc0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000bbd0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000bbe0: 2020 2069 6e64 6578 203d 2069 6e64 6976     index = indiv
+0000bbf0: 6964 7561 6c5f 7061 7269 7479 5f6c 6973  idual_parity_lis
+0000bc00: 742e 696e 6465 7828 696e 6469 7669 6475  t.index(individu
+0000bc10: 616c 5f70 6172 6974 7929 0d0a 2020 2020  al_parity)..    
+0000bc20: 2020 2020 2020 2020 2020 2020 7367 6e20              sgn 
+0000bc30: 3d20 7367 6e5f 6c69 7374 5b69 6e64 6578  = sgn_list[index
+0000bc40: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+0000bc50: 2053 315b 636f 6f72 6473 5d20 3d20 7367   S1[coords] = sg
+0000bc60: 6e0d 0a0d 0a20 2020 2020 2020 2020 2020  n....           
+0000bc70: 2069 6620 7469 6d65 2e74 696d 6528 292d   if time.time()-
+0000bc80: 7330 203e 2032 203a 0d0a 2020 2020 2020  s0 > 2 :..      
+0000bc90: 2020 2020 2020 2020 2020 7368 6f77 5f70            show_p
+0000bca0: 726f 6772 6573 7328 6b2c 6b6d 6178 2b31  rogress(k,kmax+1
+0000bcb0: 2c70 726f 6365 7373 5f6e 616d 6520 3d20  ,process_name = 
+0000bcc0: 2265 696e 7375 6d5f 7367 6e31 222c 7261  "einsum_sgn1",ra
+0000bcd0: 7469 6f20 3d20 4661 6c73 652c 636f 6c6f  tio = False,colo
+0000bce0: 723d 2272 6564 222c 7469 6d65 3d74 696d  r="red",time=tim
+0000bcf0: 652e 7469 6d65 2829 2d73 3030 290d 0a20  e.time()-s00).. 
+0000bd00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000bd10: 3020 3d20 7469 6d65 2e74 696d 6528 290d  0 = time.time().
+0000bd20: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0000bd30: 2020 2020 2020 2020 2020 206b 2b3d 310d             k+=1.
+0000bd40: 0a0d 0a20 2020 2020 2020 2063 6c65 6172  ...        clear
+0000bd50: 5f70 726f 6772 6573 7328 290d 0a20 2020  _progress()..   
+0000bd60: 2020 2020 2074 6162 5f75 7028 290d 0a20       tab_up().. 
+0000bd70: 2020 2020 2020 200d 0a20 2020 2023 2020         ..    #  
+0000bd80: 3a3a 3a20 5375 6d6d 6172 7920 3a3a 3a0d  ::: Summary :::.
+0000bd90: 0a20 2020 2023 0d0a 2020 2020 2320 2053  .    #..    #  S
+0000bda0: 3120 6973 2074 6865 2073 6967 6e20 6661  1 is the sign fa
+0000bdb0: 6374 6f72 2066 726f 6d20 7468 6520 696e  ctor from the in
+0000bdc0: 6974 6961 6c20 7265 6172 7261 6e67 656d  itial rearrangem
+0000bdd0: 656e 740d 0a20 2020 2023 2020 4974 7320  ent..    #  Its 
+0000bde0: 696e 6465 7820 7374 7269 6e67 2069 7320  index string is 
+0000bdf0: 5331 5f69 6e64 6578 5f73 7472 696e 670d  S1_index_string.
+0000be00: 0a0d 0a20 2020 2023 3a3a 3a3a 3a3a 3a3a  ...    #::::::::
+0000be10: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000be20: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000be30: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000be40: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000be50: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000be60: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000be70: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000be80: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a 2020  ::::::::::::..  
-0000be90: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0000bea0: 2053 7465 7020 333a 2053 6967 6e20 6661   Step 3: Sign fa
-0000beb0: 6374 6f72 2066 726f 6d20 7468 6520 7375  ctor from the su
-0000bec0: 6d6d 6564 2070 6169 720d 0a20 2020 2023  mmed pair..    #
+0000be60: 3a3a 3a3a 3a3a 3a3a 0d0a 2020 2020 2320  ::::::::..    # 
+0000be70: 2020 2020 2020 2020 2020 2020 2053 7465               Ste
+0000be80: 7020 333a 2053 6967 6e20 6661 6374 6f72  p 3: Sign factor
+0000be90: 2066 726f 6d20 7468 6520 7375 6d6d 6564   from the summed
+0000bea0: 2070 6169 720d 0a20 2020 2023 3a3a 3a3a   pair..    #::::
+0000beb0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000bec0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000bed0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000bee0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000bef0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000bf00: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000bf10: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000bf20: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000bf30: 0d0a 0d0a 2020 2020 5332 5f64 696d 6c69  ....    S2_dimli
-0000bf40: 7374 203d 205b 5d0d 0a20 2020 2053 325f  st = []..    S2_
-0000bf50: 696e 6465 785f 7374 7269 6e67 203d 2022  index_string = "
-0000bf60: 220d 0a20 2020 2073 756d 6d65 645f 696e  "..    summed_in
-0000bf70: 6469 6365 7320 3d20 6673 756d 6d61 6e64  dices = fsummand
-0000bf80: 5f75 720d 0a20 2020 2066 6f72 205b 205b  _ur..    for [ [
-0000bf90: 6331 2c63 325d 2c20 6c6f 6320 5d20 696e  c1,c2], loc ] in
-0000bfa0: 2073 756d 6d65 645f 696e 6465 785f 696e   summed_index_in
-0000bfb0: 666f 3a0d 0a20 2020 2020 2020 2053 325f  fo:..        S2_
-0000bfc0: 6469 6d6c 6973 7420 2b3d 2073 6861 7065  dimlist += shape
-0000bfd0: 5f6c 6973 745b 2073 756d 6d61 6e64 2e69  _list[ summand.i
-0000bfe0: 6e64 6578 2863 3129 205d 2c0d 0a20 2020  ndex(c1) ],..   
-0000bff0: 2020 2020 2053 325f 696e 6465 785f 7374       S2_index_st
-0000c000: 7269 6e67 202b 3d20 222c 222b 6331 0d0a  ring += ","+c1..
-0000c010: 2020 2020 2020 2020 7375 6d6d 6564 5f69          summed_i
-0000c020: 6e64 6963 6573 203d 2073 756d 6d65 645f  ndices = summed_
-0000c030: 696e 6469 6365 732e 7265 706c 6163 6528  indices.replace(
-0000c040: 6331 2b63 322c 2222 290d 0a20 2020 2053  c1+c2,"")..    S
-0000c050: 325f 696e 6465 785f 7374 7269 6e67 203d  2_index_string =
-0000c060: 2053 325f 696e 6465 785f 7374 7269 6e67   S2_index_string
-0000c070: 5b31 3a5d 0d0a 2020 2020 6e53 3220 3d20  [1:]..    nS2 = 
-0000c080: 6c65 6e28 5332 5f64 696d 6c69 7374 290d  len(S2_dimlist).
-0000c090: 0a20 2020 200d 0a20 2020 200d 0a20 2020  .    ..    ..   
-0000c0a0: 2073 6b69 705f 5332 203d 206e 5332 203d   skip_S2 = nS2 =
-0000c0b0: 3d20 300d 0a20 2020 200d 0a20 2020 2069  = 0..    ..    i
-0000c0c0: 6620 6465 6275 675f 6d6f 6465 203a 0d0a  f debug_mode :..
-0000c0d0: 2020 2020 2020 2020 7072 696e 7428 290d          print().
-0000c0e0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-0000c0f0: 203a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a   :::::::::::::::
-0000c100: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a20  ::::::::::::::: 
-0000c110: 5332 2073 7475 6666 203a 3a3a 3a3a 3a3a  S2 stuff :::::::
-0000c120: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000c130: 3a3a 3a3a 3a3a 2022 290d 0a20 2020 2020  :::::: ")..     
-0000c140: 2020 2069 6620 736b 6970 5f53 3220 3a0d     if skip_S2 :.
-0000c150: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-0000c160: 6e74 2822 5468 6572 6520 6973 206e 6f20  nt("There is no 
-0000c170: 7375 6d6d 6564 2069 6e64 6963 6573 2e22  summed indices."
-0000c180: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
-0000c190: 7269 6e74 2822 5332 2063 616c 6375 6c61  rint("S2 calcula
-0000c1a0: 7469 6f6e 2069 7320 736b 6970 7065 642e  tion is skipped.
-0000c1b0: 2229 0d0a 2020 2020 2020 2020 656c 7365  ")..        else
-0000c1c0: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
-0000c1d0: 7072 696e 7428 6673 756d 6d61 6e64 2c22  print(fsummand,"
-0000c1e0: 3c2d 2d2d 2066 7375 6d6d 616e 6422 290d  <--- fsummand").
-0000c1f0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-0000c200: 6e74 2853 325f 696e 6465 785f 7374 7269  nt(S2_index_stri
-0000c210: 6e67 2c22 3c2d 2d2d 2053 3220 696e 6465  ng,"<--- S2 inde
-0000c220: 7820 7374 7269 6e67 2229 0d0a 2020 2020  x string")..    
-0000c230: 2020 2020 2020 2020 7072 696e 7428 5332          print(S2
-0000c240: 5f64 696d 6c69 7374 2c22 3c2d 2d2d 2053  _dimlist,"<--- S
-0000c250: 3227 7320 6469 6d20 6c69 7374 2229 0d0a  2's dim list")..
-0000c260: 2020 2020 0d0a 2020 2020 6966 206e 6f74      ..    if not
-0000c270: 2073 6b69 705f 5332 203a 0d0a 0d0a 2020   skip_S2 :....  
-0000c280: 2020 2020 2020 5332 5f6c 6973 7420 3d20        S2_list = 
-0000c290: 5b5d 0d0a 2020 2020 2020 2020 666f 7220  []..        for 
-0000c2a0: 6920 696e 2072 616e 6765 286e 5332 293a  i in range(nS2):
-0000c2b0: 0d0a 2020 2020 2020 2020 2020 2020 5332  ..            S2
-0000c2c0: 6920 3d20 5b20 7061 7261 6d2e 7367 6e28  i = [ param.sgn(
-0000c2d0: 6a29 2066 6f72 206a 2069 6e20 7261 6e67  j) for j in rang
-0000c2e0: 6528 5332 5f64 696d 6c69 7374 5b69 5d29  e(S2_dimlist[i])
-0000c2f0: 205d 0d0a 2020 2020 2020 2020 2020 2020   ]..            
-0000c300: 5332 5f6c 6973 7420 2b3d 206e 702e 6172  S2_list += np.ar
-0000c310: 7261 7928 5332 6929 2c0d 0a0d 0a20 2020  ray(S2i),....   
-0000c320: 2023 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a   #::::::::::::::
+0000bf00: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a 0d0a  ::::::::::::....
+0000bf10: 2020 2020 5332 5f64 696d 6c69 7374 203d      S2_dimlist =
+0000bf20: 205b 5d0d 0a20 2020 2053 325f 696e 6465   []..    S2_inde
+0000bf30: 785f 7374 7269 6e67 203d 2022 220d 0a20  x_string = "".. 
+0000bf40: 2020 2073 756d 6d65 645f 696e 6469 6365     summed_indice
+0000bf50: 7320 3d20 6673 756d 6d61 6e64 5f75 720d  s = fsummand_ur.
+0000bf60: 0a20 2020 2066 6f72 205b 205b 6331 2c63  .    for [ [c1,c
+0000bf70: 325d 2c20 6c6f 6320 5d20 696e 2073 756d  2], loc ] in sum
+0000bf80: 6d65 645f 696e 6465 785f 696e 666f 3a0d  med_index_info:.
+0000bf90: 0a20 2020 2020 2020 2053 325f 6469 6d6c  .        S2_diml
+0000bfa0: 6973 7420 2b3d 2073 6861 7065 5f6c 6973  ist += shape_lis
+0000bfb0: 745b 2073 756d 6d61 6e64 2e69 6e64 6578  t[ summand.index
+0000bfc0: 2863 3129 205d 2c0d 0a20 2020 2020 2020  (c1) ],..       
+0000bfd0: 2053 325f 696e 6465 785f 7374 7269 6e67   S2_index_string
+0000bfe0: 202b 3d20 222c 222b 6331 0d0a 2020 2020   += ","+c1..    
+0000bff0: 2020 2020 7375 6d6d 6564 5f69 6e64 6963      summed_indic
+0000c000: 6573 203d 2073 756d 6d65 645f 696e 6469  es = summed_indi
+0000c010: 6365 732e 7265 706c 6163 6528 6331 2b63  ces.replace(c1+c
+0000c020: 322c 2222 290d 0a20 2020 2053 325f 696e  2,"")..    S2_in
+0000c030: 6465 785f 7374 7269 6e67 203d 2053 325f  dex_string = S2_
+0000c040: 696e 6465 785f 7374 7269 6e67 5b31 3a5d  index_string[1:]
+0000c050: 0d0a 2020 2020 6e53 3220 3d20 6c65 6e28  ..    nS2 = len(
+0000c060: 5332 5f64 696d 6c69 7374 290d 0a20 2020  S2_dimlist)..   
+0000c070: 200d 0a20 2020 200d 0a20 2020 2073 6b69   ..    ..    ski
+0000c080: 705f 5332 203d 206e 5332 203d 3d20 300d  p_S2 = nS2 == 0.
+0000c090: 0a20 2020 200d 0a20 2020 2069 6620 6465  .    ..    if de
+0000c0a0: 6275 675f 6d6f 6465 203a 0d0a 2020 2020  bug_mode :..    
+0000c0b0: 2020 2020 7072 696e 7428 290d 0a20 2020      print()..   
+0000c0c0: 2020 2020 2070 7269 6e74 2822 203a 3a3a       print(" :::
+0000c0d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000c0e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a20 5332 2073  ::::::::::: S2 s
+0000c0f0: 7475 6666 203a 3a3a 3a3a 3a3a 3a3a 3a3a  tuff :::::::::::
+0000c100: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000c110: 3a3a 2022 290d 0a20 2020 2020 2020 2069  :: ")..        i
+0000c120: 6620 736b 6970 5f53 3220 3a0d 0a20 2020  f skip_S2 :..   
+0000c130: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+0000c140: 5468 6572 6520 6973 206e 6f20 7375 6d6d  There is no summ
+0000c150: 6564 2069 6e64 6963 6573 2e22 290d 0a20  ed indices.").. 
+0000c160: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000c170: 2822 5332 2063 616c 6375 6c61 7469 6f6e  ("S2 calculation
+0000c180: 2069 7320 736b 6970 7065 642e 2229 0d0a   is skipped.")..
+0000c190: 2020 2020 2020 2020 656c 7365 203a 0d0a          else :..
+0000c1a0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0000c1b0: 7428 6673 756d 6d61 6e64 2c22 3c2d 2d2d  t(fsummand,"<---
+0000c1c0: 2066 7375 6d6d 616e 6422 290d 0a20 2020   fsummand")..   
+0000c1d0: 2020 2020 2020 2020 2070 7269 6e74 2853           print(S
+0000c1e0: 325f 696e 6465 785f 7374 7269 6e67 2c22  2_index_string,"
+0000c1f0: 3c2d 2d2d 2053 3220 696e 6465 7820 7374  <--- S2 index st
+0000c200: 7269 6e67 2229 0d0a 2020 2020 2020 2020  ring")..        
+0000c210: 2020 2020 7072 696e 7428 5332 5f64 696d      print(S2_dim
+0000c220: 6c69 7374 2c22 3c2d 2d2d 2053 3227 7320  list,"<--- S2's 
+0000c230: 6469 6d20 6c69 7374 2229 0d0a 2020 2020  dim list")..    
+0000c240: 0d0a 2020 2020 6966 206e 6f74 2073 6b69  ..    if not ski
+0000c250: 705f 5332 203a 0d0a 0d0a 2020 2020 2020  p_S2 :....      
+0000c260: 2020 5332 5f6c 6973 7420 3d20 5b5d 0d0a    S2_list = []..
+0000c270: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0000c280: 2072 616e 6765 286e 5332 293a 0d0a 2020   range(nS2):..  
+0000c290: 2020 2020 2020 2020 2020 5332 6920 3d20            S2i = 
+0000c2a0: 5b20 7061 7261 6d2e 7367 6e28 6a29 2066  [ param.sgn(j) f
+0000c2b0: 6f72 206a 2069 6e20 7261 6e67 6528 5332  or j in range(S2
+0000c2c0: 5f64 696d 6c69 7374 5b69 5d29 205d 0d0a  _dimlist[i]) ]..
+0000c2d0: 2020 2020 2020 2020 2020 2020 5332 5f6c              S2_l
+0000c2e0: 6973 7420 2b3d 206e 702e 6172 7261 7928  ist += np.array(
+0000c2f0: 5332 6929 2c0d 0a0d 0a20 2020 2023 3a3a  S2i),....    #::
+0000c300: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000c310: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000c320: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000c330: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000c340: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000c350: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000c360: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000c370: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000c380: 3a3a 0d0a 2020 2020 2320 2020 2020 2020  ::..    #       
-0000c390: 2020 2020 2020 2053 7465 7020 343a 2072         Step 4: r
-0000c3a0: 6561 7272 616e 6765 2074 6f20 7468 6520  earrange to the 
-0000c3b0: 6669 6e61 6c20 666f 726d 0d0a 2020 2020  final form..    
-0000c3c0: 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  #:::::::::::::::
+0000c350: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a  ::::::::::::::..
+0000c360: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0000c370: 2020 2053 7465 7020 343a 2072 6561 7272     Step 4: rearr
+0000c380: 616e 6765 2074 6f20 7468 6520 6669 6e61  ange to the fina
+0000c390: 6c20 666f 726d 0d0a 2020 2020 233a 3a3a  l form..    #:::
+0000c3a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000c3b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000c3c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000c3d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000c3e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000c3f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000c400: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000c410: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000c420: 3a0d 0a20 2020 200d 0a20 2020 2073 6b69  :..    ..    ski
-0000c430: 705f 5333 203d 2054 7275 650d 0a20 2020  p_S3 = True..   
-0000c440: 2069 6620 6861 735f 6f75 7470 7574 203a   if has_output :
-0000c450: 0d0a 0d0a 2020 2020 2020 2020 666f 7574  ....        fout
-0000c460: 7075 7420 3d20 2222 0d0a 2020 2020 2020  put = ""..      
-0000c470: 2020 666f 7220 6320 696e 206f 7574 7075    for c in outpu
-0000c480: 745f 7374 7269 6e67 3a0d 0a20 2020 2020  t_string:..     
-0000c490: 2020 2020 2020 2069 6620 7374 6174 735f         if stats_
-0000c4a0: 6c69 7374 5b20 7375 6d6d 616e 642e 696e  list[ summand.in
-0000c4b0: 6465 7828 6329 205d 203d 3d20 3020 3a0d  dex(c) ] == 0 :.
-0000c4c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c4d0: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
-0000c4e0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0000c4f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000c500: 7574 7075 742b 3d63 0d0a 0d0a 2020 2020  utput+=c....    
-0000c510: 2020 2020 5333 5f73 6861 7065 3d5b 5d0d      S3_shape=[].
-0000c520: 0a20 2020 2020 2020 2066 6f72 2063 2069  .        for c i
-0000c530: 6e20 7375 6d6d 6564 5f69 6e64 6963 6573  n summed_indices
-0000c540: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
-0000c550: 203d 2073 6861 7065 5f6c 6973 745b 2073   = shape_list[ s
-0000c560: 756d 6d61 6e64 2e69 6e64 6578 2863 2920  ummand.index(c) 
-0000c570: 5d0d 0a20 2020 2020 2020 2020 2020 2053  ]..            S
-0000c580: 335f 7368 6170 6520 2b3d 2064 2c0d 0a0d  3_shape += d,...
-0000c590: 0a20 2020 2020 2020 2023 2061 6761 696e  .        # again
-0000c5a0: 2e2e 2e20 7265 6d6f 7665 2074 6865 206c  ... remove the l
-0000c5b0: 6561 6469 6e67 2061 6e64 2074 7261 696c  eading and trail
-0000c5c0: 696e 6720 6475 706c 6963 6174 6573 0d0a  ing duplicates..
-0000c5d0: 0d0a 2020 2020 2020 2020 6e61 6c6c 5f75  ..        nall_u
-0000c5e0: 7220 3d20 6c65 6e28 7375 6d6d 6564 5f69  r = len(summed_i
-0000c5f0: 6e64 6963 6573 290d 0a20 2020 2020 2020  ndices)..       
-0000c600: 206e 6c20 3d20 300d 0a20 2020 2020 2020   nl = 0..       
-0000c610: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-0000c620: 6e61 6c6c 5f75 7229 3a0d 0a20 2020 2020  nall_ur):..     
-0000c630: 2020 2020 2020 2069 6620 7375 6d6d 6564         if summed
-0000c640: 5f69 6e64 6963 6573 5b69 5d20 213d 2066  _indices[i] != f
-0000c650: 6f75 7470 7574 5b69 5d3a 0d0a 2020 2020  output[i]:..    
-0000c660: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-0000c670: 6b0d 0a20 2020 2020 2020 2020 2020 206e  k..            n
-0000c680: 6c2b 3d31 0d0a 0d0a 2020 2020 2020 2020  l+=1....        
-0000c690: 6e72 203d 2030 0d0a 2020 2020 2020 2020  nr = 0..        
-0000c6a0: 666f 7220 6920 696e 2072 616e 6765 286e  for i in range(n
-0000c6b0: 616c 6c5f 7572 293a 0d0a 2020 2020 2020  all_ur):..      
-0000c6c0: 2020 2020 2020 6966 2073 756d 6d65 645f        if summed_
-0000c6d0: 696e 6469 6365 735b 6e61 6c6c 5f75 722d  indices[nall_ur-
-0000c6e0: 312d 695d 2021 3d20 666f 7574 7075 745b  1-i] != foutput[
-0000c6f0: 6e61 6c6c 5f75 722d 312d 695d 3a0d 0a20  nall_ur-1-i]:.. 
-0000c700: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-0000c710: 7265 616b 0d0a 2020 2020 2020 2020 2020  reak..          
-0000c720: 2020 6e72 2b3d 310d 0a20 2020 2020 2020    nr+=1..       
-0000c730: 206e 7220 3d20 6e61 6c6c 5f75 722d 6e72   nr = nall_ur-nr
-0000c740: 0d0a 0d0a 2020 2020 2020 2020 6669 6e61  ....        fina
-0000c750: 6c20 3d20 666f 7574 7075 745b 6e6c 3a6e  l = foutput[nl:n
-0000c760: 725d 0d0a 2020 2020 2020 2020 7072 6566  r]..        pref
-0000c770: 696e 616c 203d 2073 756d 6d65 645f 696e  inal = summed_in
-0000c780: 6469 6365 735b 6e6c 3a6e 725d 0d0a 2020  dices[nl:nr]..  
-0000c790: 2020 2020 2020 5333 5f73 6861 7065 2020        S3_shape  
-0000c7a0: 203d 2053 335f 7368 6170 655b 6e6c 3a6e   = S3_shape[nl:n
-0000c7b0: 725d 0d0a 0d0a 2020 2020 2020 2020 6966  r]....        if
-0000c7c0: 206e 6c3e 6e72 203a 0d0a 2020 2020 2020   nl>nr :..      
-0000c7d0: 2020 2020 2020 736b 6970 5f53 3320 3d20        skip_S3 = 
-0000c7e0: 5472 7565 0d0a 2020 2020 2020 2020 656c  True..        el
-0000c7f0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0000c800: 2073 6b69 705f 5333 203d 2046 616c 7365   skip_S3 = False
-0000c810: 0d0a 0d0a 2020 2020 2020 2020 5333 5f73  ....        S3_s
-0000c820: 676e 5f63 6f6d 7075 7461 7469 6f6e 5f73  gn_computation_s
-0000c830: 7472 696e 6720 3d20 7072 6566 696e 616c  tring = prefinal
-0000c840: 2b22 2d3e 222b 6669 6e61 6c0d 0a20 2020  +"->"+final..   
-0000c850: 2020 2020 2053 335f 696e 6465 785f 7374       S3_index_st
-0000c860: 7269 6e67 203d 2070 7265 6669 6e61 6c0d  ring = prefinal.
-0000c870: 0a0d 0a20 2020 2020 2020 2069 6620 6e6f  ...        if no
-0000c880: 7420 736b 6970 5f53 3320 3a0d 0a0d 0a20  t skip_S3 :.... 
-0000c890: 2020 2020 2020 2020 2020 206b 3d31 0d0a             k=1..
-0000c8a0: 2020 2020 2020 2020 2020 2020 6b6d 6178              kmax
-0000c8b0: 203d 2031 0d0a 2020 2020 2020 2020 2020   = 1..          
-0000c8c0: 2020 666f 7220 6420 696e 2053 335f 7368    for d in S3_sh
-0000c8d0: 6170 653a 0d0a 2020 2020 2020 2020 2020  ape:..          
-0000c8e0: 2020 2020 2020 6b6d 6178 2a3d 640d 0a0d        kmax*=d...
-0000c8f0: 0a20 2020 2020 2020 2020 2020 2073 3020  .            s0 
-0000c900: 3d20 7469 6d65 2e74 696d 6528 290d 0a20  = time.time().. 
-0000c910: 2020 2020 2020 2020 2020 2073 3030 203d             s00 =
-0000c920: 2073 300d 0a20 2020 2020 2020 2020 2020   s0..           
-0000c930: 2070 7269 6e74 2829 2023 203c 3c20 446f   print() # << Do
-0000c940: 6e27 7420 7265 6d6f 7665 2074 6869 732e  n't remove this.
-0000c950: 2054 6869 7320 6973 2066 6f72 2074 6865   This is for the
-0000c960: 2073 686f 775f 7072 6f67 7265 7373 210d   show_progress!.
-0000c970: 0a0d 0a20 2020 2020 2020 2020 2020 2053  ...            S
-0000c980: 3320 3d20 6e70 2e7a 6572 6f73 2853 335f  3 = np.zeros(S3_
-0000c990: 7368 6170 652c 6474 7970 653d 696e 7429  shape,dtype=int)
-0000c9a0: 0d0a 2020 2020 2020 2020 2020 2020 6974  ..            it
-0000c9b0: 6572 6174 6f72 203d 206e 702e 6e64 6974  erator = np.ndit
-0000c9c0: 6572 2853 332c 2066 6c61 6773 3d5b 276d  er(S3, flags=['m
-0000c9d0: 756c 7469 5f69 6e64 6578 275d 290d 0a20  ulti_index']).. 
-0000c9e0: 2020 2020 2020 2020 2020 2069 6e64 6976             indiv
-0000c9f0: 6964 7561 6c5f 7061 7269 7479 5f6c 6973  idual_parity_lis
+0000c3f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a0d 0a20  :::::::::::::.. 
+0000c400: 2020 200d 0a20 2020 2073 6b69 705f 5333     ..    skip_S3
+0000c410: 203d 2054 7275 650d 0a20 2020 2069 6620   = True..    if 
+0000c420: 6861 735f 6f75 7470 7574 203a 0d0a 0d0a  has_output :....
+0000c430: 2020 2020 2020 2020 666f 7574 7075 7420          foutput 
+0000c440: 3d20 2222 0d0a 2020 2020 2020 2020 666f  = ""..        fo
+0000c450: 7220 6320 696e 206f 7574 7075 745f 7374  r c in output_st
+0000c460: 7269 6e67 3a0d 0a20 2020 2020 2020 2020  ring:..         
+0000c470: 2020 2069 6620 7374 6174 735f 6c69 7374     if stats_list
+0000c480: 5b20 7375 6d6d 616e 642e 696e 6465 7828  [ summand.index(
+0000c490: 6329 205d 203d 3d20 3020 3a0d 0a20 2020  c) ] == 0 :..   
+0000c4a0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+0000c4b0: 7469 6e75 650d 0a20 2020 2020 2020 2020  tinue..         
+0000c4c0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+0000c4d0: 2020 2020 2020 2020 2020 666f 7574 7075            foutpu
+0000c4e0: 742b 3d63 0d0a 0d0a 2020 2020 2020 2020  t+=c....        
+0000c4f0: 5333 5f73 6861 7065 3d5b 5d0d 0a20 2020  S3_shape=[]..   
+0000c500: 2020 2020 2066 6f72 2063 2069 6e20 7375       for c in su
+0000c510: 6d6d 6564 5f69 6e64 6963 6573 3a0d 0a20  mmed_indices:.. 
+0000c520: 2020 2020 2020 2020 2020 2064 203d 2073             d = s
+0000c530: 6861 7065 5f6c 6973 745b 2073 756d 6d61  hape_list[ summa
+0000c540: 6e64 2e69 6e64 6578 2863 2920 5d0d 0a20  nd.index(c) ].. 
+0000c550: 2020 2020 2020 2020 2020 2053 335f 7368             S3_sh
+0000c560: 6170 6520 2b3d 2064 2c0d 0a0d 0a20 2020  ape += d,....   
+0000c570: 2020 2020 2023 2061 6761 696e 2e2e 2e20       # again... 
+0000c580: 7265 6d6f 7665 2074 6865 206c 6561 6469  remove the leadi
+0000c590: 6e67 2061 6e64 2074 7261 696c 696e 6720  ng and trailing 
+0000c5a0: 6475 706c 6963 6174 6573 0d0a 0d0a 2020  duplicates....  
+0000c5b0: 2020 2020 2020 6e61 6c6c 5f75 7220 3d20        nall_ur = 
+0000c5c0: 6c65 6e28 7375 6d6d 6564 5f69 6e64 6963  len(summed_indic
+0000c5d0: 6573 290d 0a20 2020 2020 2020 206e 6c20  es)..        nl 
+0000c5e0: 3d20 300d 0a20 2020 2020 2020 2066 6f72  = 0..        for
+0000c5f0: 2069 2069 6e20 7261 6e67 6528 6e61 6c6c   i in range(nall
+0000c600: 5f75 7229 3a0d 0a20 2020 2020 2020 2020  _ur):..         
+0000c610: 2020 2069 6620 7375 6d6d 6564 5f69 6e64     if summed_ind
+0000c620: 6963 6573 5b69 5d20 213d 2066 6f75 7470  ices[i] != foutp
+0000c630: 7574 5b69 5d3a 0d0a 2020 2020 2020 2020  ut[i]:..        
+0000c640: 2020 2020 2020 2020 6272 6561 6b0d 0a20          break.. 
+0000c650: 2020 2020 2020 2020 2020 206e 6c2b 3d31             nl+=1
+0000c660: 0d0a 0d0a 2020 2020 2020 2020 6e72 203d  ....        nr =
+0000c670: 2030 0d0a 2020 2020 2020 2020 666f 7220   0..        for 
+0000c680: 6920 696e 2072 616e 6765 286e 616c 6c5f  i in range(nall_
+0000c690: 7572 293a 0d0a 2020 2020 2020 2020 2020  ur):..          
+0000c6a0: 2020 6966 2073 756d 6d65 645f 696e 6469    if summed_indi
+0000c6b0: 6365 735b 6e61 6c6c 5f75 722d 312d 695d  ces[nall_ur-1-i]
+0000c6c0: 2021 3d20 666f 7574 7075 745b 6e61 6c6c   != foutput[nall
+0000c6d0: 5f75 722d 312d 695d 3a0d 0a20 2020 2020  _ur-1-i]:..     
+0000c6e0: 2020 2020 2020 2020 2020 2062 7265 616b             break
+0000c6f0: 0d0a 2020 2020 2020 2020 2020 2020 6e72  ..            nr
+0000c700: 2b3d 310d 0a20 2020 2020 2020 206e 7220  +=1..        nr 
+0000c710: 3d20 6e61 6c6c 5f75 722d 6e72 0d0a 0d0a  = nall_ur-nr....
+0000c720: 2020 2020 2020 2020 6669 6e61 6c20 3d20          final = 
+0000c730: 666f 7574 7075 745b 6e6c 3a6e 725d 0d0a  foutput[nl:nr]..
+0000c740: 2020 2020 2020 2020 7072 6566 696e 616c          prefinal
+0000c750: 203d 2073 756d 6d65 645f 696e 6469 6365   = summed_indice
+0000c760: 735b 6e6c 3a6e 725d 0d0a 2020 2020 2020  s[nl:nr]..      
+0000c770: 2020 5333 5f73 6861 7065 2020 203d 2053    S3_shape   = S
+0000c780: 335f 7368 6170 655b 6e6c 3a6e 725d 0d0a  3_shape[nl:nr]..
+0000c790: 0d0a 2020 2020 2020 2020 6966 206e 6c3e  ..        if nl>
+0000c7a0: 6e72 203a 0d0a 2020 2020 2020 2020 2020  nr :..          
+0000c7b0: 2020 736b 6970 5f53 3320 3d20 5472 7565    skip_S3 = True
+0000c7c0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+0000c7d0: 0a20 2020 2020 2020 2020 2020 2073 6b69  .            ski
+0000c7e0: 705f 5333 203d 2046 616c 7365 0d0a 0d0a  p_S3 = False....
+0000c7f0: 2020 2020 2020 2020 5333 5f73 676e 5f63          S3_sgn_c
+0000c800: 6f6d 7075 7461 7469 6f6e 5f73 7472 696e  omputation_strin
+0000c810: 6720 3d20 7072 6566 696e 616c 2b22 2d3e  g = prefinal+"->
+0000c820: 222b 6669 6e61 6c0d 0a20 2020 2020 2020  "+final..       
+0000c830: 2053 335f 696e 6465 785f 7374 7269 6e67   S3_index_string
+0000c840: 203d 2070 7265 6669 6e61 6c0d 0a0d 0a20   = prefinal.... 
+0000c850: 2020 2020 2020 2069 6620 6e6f 7420 736b         if not sk
+0000c860: 6970 5f53 3320 3a0d 0a0d 0a20 2020 2020  ip_S3 :....     
+0000c870: 2020 2020 2020 206b 3d31 0d0a 2020 2020         k=1..    
+0000c880: 2020 2020 2020 2020 6b6d 6178 203d 2031          kmax = 1
+0000c890: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+0000c8a0: 7220 6420 696e 2053 335f 7368 6170 653a  r d in S3_shape:
+0000c8b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c8c0: 2020 6b6d 6178 2a3d 640d 0a0d 0a20 2020    kmax*=d....   
+0000c8d0: 2020 2020 2020 2020 2073 3020 3d20 7469           s0 = ti
+0000c8e0: 6d65 2e74 696d 6528 290d 0a20 2020 2020  me.time()..     
+0000c8f0: 2020 2020 2020 2073 3030 203d 2073 300d         s00 = s0.
+0000c900: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+0000c910: 6772 6573 735f 7370 6163 6528 2920 2320  gress_space() # 
+0000c920: 3c3c 2044 6f6e 2774 2072 656d 6f76 6520  << Don't remove 
+0000c930: 7468 6973 2e20 5468 6973 2069 7320 666f  this. This is fo
+0000c940: 7220 7468 6520 7368 6f77 5f70 726f 6772  r the show_progr
+0000c950: 6573 7321 0d0a 0d0a 2020 2020 2020 2020  ess!....        
+0000c960: 2020 2020 5333 203d 206e 702e 7a65 726f      S3 = np.zero
+0000c970: 7328 5333 5f73 6861 7065 2c64 7479 7065  s(S3_shape,dtype
+0000c980: 3d69 6e74 290d 0a20 2020 2020 2020 2020  =int)..         
+0000c990: 2020 2069 7465 7261 746f 7220 3d20 6e70     iterator = np
+0000c9a0: 2e6e 6469 7465 7228 5333 2c20 666c 6167  .nditer(S3, flag
+0000c9b0: 733d 5b27 6d75 6c74 695f 696e 6465 7827  s=['multi_index'
+0000c9c0: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+0000c9d0: 696e 6469 7669 6475 616c 5f70 6172 6974  individual_parit
+0000c9e0: 795f 6c69 7374 203d 205b 5d0d 0a20 2020  y_list = []..   
+0000c9f0: 2020 2020 2020 2020 2073 676e 5f6c 6973           sgn_lis
 0000ca00: 7420 3d20 5b5d 0d0a 2020 2020 2020 2020  t = []..        
-0000ca10: 2020 2020 7367 6e5f 6c69 7374 203d 205b      sgn_list = [
-0000ca20: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
-0000ca30: 6f72 2065 6c65 6d65 6e74 2069 6e20 6974  or element in it
-0000ca40: 6572 6174 6f72 3a0d 0a20 2020 2020 2020  erator:..       
-0000ca50: 2020 2020 2020 2020 2063 6f6f 7264 7320           coords 
-0000ca60: 3d20 6974 6572 6174 6f72 2e6d 756c 7469  = iterator.multi
-0000ca70: 5f69 6e64 6578 0d0a 0d0a 2020 2020 2020  _index....      
-0000ca80: 2020 2020 2020 2020 2020 696e 6469 7669            indivi
-0000ca90: 6475 616c 5f70 6172 6974 7920 3d20 5b20  dual_parity = [ 
-0000caa0: 7061 7261 6d2e 6770 6172 6974 7928 6929  param.gparity(i)
-0000cab0: 2532 2066 6f72 2069 2069 6e20 636f 6f72  %2 for i in coor
-0000cac0: 6473 205d 0d0a 0d0a 2020 2020 2020 2020  ds ]....        
-0000cad0: 2020 2020 2020 2020 6966 2069 6e64 6976          if indiv
-0000cae0: 6964 7561 6c5f 7061 7269 7479 206e 6f74  idual_parity not
-0000caf0: 2069 6e20 696e 6469 7669 6475 616c 5f70   in individual_p
-0000cb00: 6172 6974 795f 6c69 7374 3a0d 0a20 2020  arity_list:..   
-0000cb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb20: 2069 6e64 6976 6964 7561 6c5f 7061 7269   individual_pari
-0000cb30: 7479 5f6c 6973 7420 2b3d 2069 6e64 6976  ty_list += indiv
-0000cb40: 6964 7561 6c5f 7061 7269 7479 2c0d 0a20  idual_parity,.. 
-0000cb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb60: 2020 2073 676e 203d 2072 656c 6174 6976     sgn = relativ
-0000cb70: 655f 7061 7269 7479 2853 335f 7367 6e5f  e_parity(S3_sgn_
-0000cb80: 636f 6d70 7574 6174 696f 6e5f 7374 7269  computation_stri
-0000cb90: 6e67 2c69 6e64 6976 6964 7561 6c5f 7061  ng,individual_pa
-0000cba0: 7269 7479 290d 0a20 2020 2020 2020 2020  rity)..         
-0000cbb0: 2020 2020 2020 2020 2020 2073 676e 5f6c             sgn_l
-0000cbc0: 6973 7420 2b3d 2073 676e 2c0d 0a20 2020  ist += sgn,..   
-0000cbd0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000cbe0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0000cbf0: 2020 2020 2020 2020 696e 6465 7820 3d20          index = 
-0000cc00: 696e 6469 7669 6475 616c 5f70 6172 6974  individual_parit
-0000cc10: 795f 6c69 7374 2e69 6e64 6578 2869 6e64  y_list.index(ind
-0000cc20: 6976 6964 7561 6c5f 7061 7269 7479 290d  ividual_parity).
-0000cc30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cc40: 2020 2020 2073 676e 203d 2073 676e 5f6c       sgn = sgn_l
-0000cc50: 6973 745b 696e 6465 785d 0d0a 0d0a 2020  ist[index]....  
-0000cc60: 2020 2020 2020 2020 2020 2020 2020 5333                S3
-0000cc70: 5b63 6f6f 7264 735d 203d 2073 676e 0d0a  [coords] = sgn..
-0000cc80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000cc90: 2020 6966 2074 696d 652e 7469 6d65 2829    if time.time()
-0000cca0: 2d73 3020 3e20 302e 3520 3a0d 0a20 2020  -s0 > 0.5 :..   
-0000ccb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccc0: 2073 686f 775f 7072 6f67 7265 7373 286b   show_progress(k
-0000ccd0: 2c6b 6d61 782b 312c 7072 6f63 6573 735f  ,kmax+1,process_
-0000cce0: 6e61 6d65 203d 2022 6569 6e73 756d 5f73  name = "einsum_s
-0000ccf0: 676e 3322 2c72 6174 696f 203d 2046 616c  gn3",ratio = Fal
-0000cd00: 7365 2c63 6f6c 6f72 3d22 7265 6422 2c74  se,color="red",t
-0000cd10: 696d 653d 7469 6d65 2e74 696d 6528 292d  ime=time.time()-
-0000cd20: 7330 3029 0d0a 2020 2020 2020 2020 2020  s00)..          
-0000cd30: 2020 2020 2020 2020 2020 7330 203d 2074            s0 = t
-0000cd40: 696d 652e 7469 6d65 2829 0d0a 0d0a 2020  ime.time()....  
-0000cd50: 2020 2020 2020 2020 2020 2020 2020 6b2b                k+
-0000cd60: 3d31 0d0a 2020 2020 2020 2020 2020 2020  =1..            
-0000cd70: 636c 6561 725f 7072 6f67 7265 7373 2829  clear_progress()
-0000cd80: 0d0a 2020 2020 2020 2020 2020 2020 7379  ..            sy
-0000cd90: 732e 7374 646f 7574 2e77 7269 7465 2822  s.stdout.write("
-0000cda0: 5c30 3333 5b46 2229 0d0a 0d0a 2020 2020  \033[F")....    
-0000cdb0: 2020 2020 2020 2020 736b 6970 5f53 3320          skip_S3 
-0000cdc0: 3d20 6c65 6e28 5333 5f73 6861 7065 293d  = len(S3_shape)=
-0000cdd0: 3d30 0d0a 0d0a 2020 2020 2320 203a 3a3a  =0....    #  :::
-0000cde0: 2053 756d 6d61 7279 203a 3a3a 0d0a 2020   Summary :::..  
-0000cdf0: 2020 230d 0a20 2020 2023 2020 5333 2069    #..    #  S3 i
-0000ce00: 7320 7468 6520 7369 676e 2066 6163 746f  s the sign facto
-0000ce10: 7220 6672 6f6d 2074 6865 2066 696e 616c  r from the final
-0000ce20: 2072 6561 7272 616e 6765 6d65 6e74 0d0a   rearrangement..
-0000ce30: 2020 2020 2320 2049 7473 2069 6e64 6578      #  Its index
-0000ce40: 2073 7472 696e 6720 6973 2053 335f 696e   string is S3_in
-0000ce50: 6465 785f 7374 7269 6e67 0d0a 2020 2020  dex_string..    
-0000ce60: 0d0a 2020 2020 6966 2064 6562 7567 5f6d  ..    if debug_m
-0000ce70: 6f64 6520 616e 6420 6e6f 7420 736b 6970  ode and not skip
-0000ce80: 5f53 333a 0d0a 2020 2020 2020 2020 7072  _S3:..        pr
-0000ce90: 696e 7428 290d 0a20 2020 2020 2020 2070  int()..        p
-0000cea0: 7269 6e74 2822 203a 3a3a 3a3a 3a3a 3a3a  rint(" :::::::::
-0000ceb0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000cec0: 3a3a 3a3a 3a20 5333 2073 7475 6666 203a  ::::: S3 stuff :
-0000ced0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000cee0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 2022 290d  :::::::::::: ").
-0000cef0: 0a20 2020 2020 2020 2070 7269 6e74 2853  .        print(S
-0000cf00: 335f 7367 6e5f 636f 6d70 7574 6174 696f  3_sgn_computatio
-0000cf10: 6e5f 7374 7269 6e67 2c22 3c2d 2d2d 2073  n_string,"<--- s
-0000cf20: 7472 696e 6720 7573 6564 2069 6e20 7468  tring used in th
-0000cf30: 6520 5333 2063 6f6d 7075 7461 7469 6f6e  e S3 computation
-0000cf40: 2229 0d0a 2020 2020 2020 2020 7072 696e  ")..        prin
-0000cf50: 7428 5333 5f69 6e64 6578 5f73 7472 696e  t(S3_index_strin
-0000cf60: 672c 223c 2d2d 2d20 5333 5f69 6e64 6578  g,"<--- S3_index
-0000cf70: 5f73 7472 696e 6722 290d 0a20 2020 2020  _string")..     
-0000cf80: 2020 2070 7269 6e74 2853 335f 7368 6170     print(S3_shap
-0000cf90: 652c 223c 2d2d 2d20 5333 5f73 6861 7065  e,"<--- S3_shape
-0000cfa0: 2229 0d0a 2020 2020 0d0a 2020 2020 233a  ")..    ..    #:
+0000ca10: 2020 2020 666f 7220 656c 656d 656e 7420      for element 
+0000ca20: 696e 2069 7465 7261 746f 723a 0d0a 2020  in iterator:..  
+0000ca30: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000ca40: 6f72 6473 203d 2069 7465 7261 746f 722e  ords = iterator.
+0000ca50: 6d75 6c74 695f 696e 6465 780d 0a0d 0a20  multi_index.... 
+0000ca60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000ca70: 6e64 6976 6964 7561 6c5f 7061 7269 7479  ndividual_parity
+0000ca80: 203d 205b 2070 6172 616d 2e67 7061 7269   = [ param.gpari
+0000ca90: 7479 2869 2925 3220 666f 7220 6920 696e  ty(i)%2 for i in
+0000caa0: 2063 6f6f 7264 7320 5d0d 0a0d 0a20 2020   coords ]....   
+0000cab0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000cac0: 696e 6469 7669 6475 616c 5f70 6172 6974  individual_parit
+0000cad0: 7920 6e6f 7420 696e 2069 6e64 6976 6964  y not in individ
+0000cae0: 7561 6c5f 7061 7269 7479 5f6c 6973 743a  ual_parity_list:
+0000caf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000cb00: 2020 2020 2020 696e 6469 7669 6475 616c        individual
+0000cb10: 5f70 6172 6974 795f 6c69 7374 202b 3d20  _parity_list += 
+0000cb20: 696e 6469 7669 6475 616c 5f70 6172 6974  individual_parit
+0000cb30: 792c 0d0a 2020 2020 2020 2020 2020 2020  y,..            
+0000cb40: 2020 2020 2020 2020 7367 6e20 3d20 7265          sgn = re
+0000cb50: 6c61 7469 7665 5f70 6172 6974 7928 5333  lative_parity(S3
+0000cb60: 5f73 676e 5f63 6f6d 7075 7461 7469 6f6e  _sgn_computation
+0000cb70: 5f73 7472 696e 672c 696e 6469 7669 6475  _string,individu
+0000cb80: 616c 5f70 6172 6974 7929 0d0a 2020 2020  al_parity)..    
+0000cb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cba0: 7367 6e5f 6c69 7374 202b 3d20 7367 6e2c  sgn_list += sgn,
+0000cbb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000cbc0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+0000cbd0: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+0000cbe0: 6578 203d 2069 6e64 6976 6964 7561 6c5f  ex = individual_
+0000cbf0: 7061 7269 7479 5f6c 6973 742e 696e 6465  parity_list.inde
+0000cc00: 7828 696e 6469 7669 6475 616c 5f70 6172  x(individual_par
+0000cc10: 6974 7929 0d0a 2020 2020 2020 2020 2020  ity)..          
+0000cc20: 2020 2020 2020 2020 2020 7367 6e20 3d20            sgn = 
+0000cc30: 7367 6e5f 6c69 7374 5b69 6e64 6578 5d0d  sgn_list[index].
+0000cc40: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000cc50: 2020 2053 335b 636f 6f72 6473 5d20 3d20     S3[coords] = 
+0000cc60: 7367 6e0d 0a0d 0a20 2020 2020 2020 2020  sgn....         
+0000cc70: 2020 2020 2020 2069 6620 7469 6d65 2e74         if time.t
+0000cc80: 696d 6528 292d 7330 203e 2030 2e35 203a  ime()-s0 > 0.5 :
+0000cc90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000cca0: 2020 2020 2020 7368 6f77 5f70 726f 6772        show_progr
+0000ccb0: 6573 7328 6b2c 6b6d 6178 2b31 2c70 726f  ess(k,kmax+1,pro
+0000ccc0: 6365 7373 5f6e 616d 6520 3d20 2265 696e  cess_name = "ein
+0000ccd0: 7375 6d5f 7367 6e33 222c 7261 7469 6f20  sum_sgn3",ratio 
+0000cce0: 3d20 4661 6c73 652c 636f 6c6f 723d 2272  = False,color="r
+0000ccf0: 6564 222c 7469 6d65 3d74 696d 652e 7469  ed",time=time.ti
+0000cd00: 6d65 2829 2d73 3030 290d 0a20 2020 2020  me()-s00)..     
+0000cd10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000cd20: 3020 3d20 7469 6d65 2e74 696d 6528 290d  0 = time.time().
+0000cd30: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0000cd40: 2020 206b 2b3d 310d 0a20 2020 2020 2020     k+=1..       
+0000cd50: 2020 2020 2063 6c65 6172 5f70 726f 6772       clear_progr
+0000cd60: 6573 7328 290d 0a20 2020 2020 2020 2020  ess()..         
+0000cd70: 2020 2074 6162 5f75 7028 290d 0a0d 0a20     tab_up().... 
+0000cd80: 2020 2020 2020 2020 2020 2073 6b69 705f             skip_
+0000cd90: 5333 203d 206c 656e 2853 335f 7368 6170  S3 = len(S3_shap
+0000cda0: 6529 3d3d 300d 0a0d 0a20 2020 2023 2020  e)==0....    #  
+0000cdb0: 3a3a 3a20 5375 6d6d 6172 7920 3a3a 3a0d  ::: Summary :::.
+0000cdc0: 0a20 2020 2023 0d0a 2020 2020 2320 2053  .    #..    #  S
+0000cdd0: 3320 6973 2074 6865 2073 6967 6e20 6661  3 is the sign fa
+0000cde0: 6374 6f72 2066 726f 6d20 7468 6520 6669  ctor from the fi
+0000cdf0: 6e61 6c20 7265 6172 7261 6e67 656d 656e  nal rearrangemen
+0000ce00: 740d 0a20 2020 2023 2020 4974 7320 696e  t..    #  Its in
+0000ce10: 6465 7820 7374 7269 6e67 2069 7320 5333  dex string is S3
+0000ce20: 5f69 6e64 6578 5f73 7472 696e 670d 0a20  _index_string.. 
+0000ce30: 2020 200d 0a20 2020 2069 6620 6465 6275     ..    if debu
+0000ce40: 675f 6d6f 6465 2061 6e64 206e 6f74 2073  g_mode and not s
+0000ce50: 6b69 705f 5333 3a0d 0a20 2020 2020 2020  kip_S3:..       
+0000ce60: 2070 7269 6e74 2829 0d0a 2020 2020 2020   print()..      
+0000ce70: 2020 7072 696e 7428 2220 3a3a 3a3a 3a3a    print(" ::::::
+0000ce80: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000ce90: 3a3a 3a3a 3a3a 3a3a 2053 3320 7374 7566  :::::::: S3 stuf
+0000cea0: 6620 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  f ::::::::::::::
+0000ceb0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a20  ::::::::::::::: 
+0000cec0: 2229 0d0a 2020 2020 2020 2020 7072 696e  ")..        prin
+0000ced0: 7428 5333 5f73 676e 5f63 6f6d 7075 7461  t(S3_sgn_computa
+0000cee0: 7469 6f6e 5f73 7472 696e 672c 223c 2d2d  tion_string,"<--
+0000cef0: 2d20 7374 7269 6e67 2075 7365 6420 696e  - string used in
+0000cf00: 2074 6865 2053 3320 636f 6d70 7574 6174   the S3 computat
+0000cf10: 696f 6e22 290d 0a20 2020 2020 2020 2070  ion")..        p
+0000cf20: 7269 6e74 2853 335f 696e 6465 785f 7374  rint(S3_index_st
+0000cf30: 7269 6e67 2c22 3c2d 2d2d 2053 335f 696e  ring,"<--- S3_in
+0000cf40: 6465 785f 7374 7269 6e67 2229 0d0a 2020  dex_string")..  
+0000cf50: 2020 2020 2020 7072 696e 7428 5333 5f73        print(S3_s
+0000cf60: 6861 7065 2c22 3c2d 2d2d 2053 335f 7368  hape,"<--- S3_sh
+0000cf70: 6170 6522 290d 0a20 2020 200d 0a20 2020  ape")..    ..   
+0000cf80: 2023 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a   #::::::::::::::
+0000cf90: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000cfa0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000cfb0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000cfc0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000cfd0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000cfe0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000cff0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000d000: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a0d  :::::::::::::::.
-0000d010: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
-0000d020: 2020 2020 5374 6570 2035 3a20 6164 6420      Step 5: add 
-0000d030: 7468 6520 7665 7274 6963 6573 0d0a 2020  the vertices..  
-0000d040: 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a    #:::::::::::::
+0000cfe0: 3a3a 0d0a 2020 2020 2320 2020 2020 2020  ::..    #       
+0000cff0: 2020 2020 2020 2053 7465 7020 353a 2061         Step 5: a
+0000d000: 6464 2074 6865 2076 6572 7469 6365 730d  dd the vertices.
+0000d010: 0a20 2020 2023 3a3a 3a3a 3a3a 3a3a 3a3a  .    #::::::::::
+0000d020: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000d030: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000d040: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000d050: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000d060: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000d070: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000d080: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000d090: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000d0a0: 3a3a 3a0d 0a20 2020 200d 0a20 2020 2065  :::..    ..    e
-0000d0b0: 696e 7375 6d5f 696e 7075 7420 3d20 696e  insum_input = in
-0000d0c0: 7075 745f 7374 7269 6e67 0d0a 2020 2020  put_string..    
-0000d0d0: 6569 6e73 756d 5f6f 626a 5f6c 6973 7420  einsum_obj_list 
-0000d0e0: 3d20 6f62 6a5f 6c69 7374 0d0a 0d0a 2020  = obj_list....  
-0000d0f0: 2020 6966 2053 3164 696d 3e30 2061 6e64    if S1dim>0 and
-0000d100: 206e 6f74 2073 6b69 705f 5331 3a0d 0a20   not skip_S1:.. 
-0000d110: 2020 2020 2020 2065 696e 7375 6d5f 696e         einsum_in
-0000d120: 7075 7420 2b3d 2022 2c22 2b53 315f 696e  put += ","+S1_in
-0000d130: 6465 785f 7374 7269 6e67 0d0a 2020 2020  dex_string..    
-0000d140: 2020 2020 6569 6e73 756d 5f6f 626a 5f6c      einsum_obj_l
-0000d150: 6973 7420 2b3d 2053 312c 0d0a 0d0a 2020  ist += S1,....  
-0000d160: 2020 6966 206e 5332 3e30 203a 0d0a 2020    if nS2>0 :..  
-0000d170: 2020 2020 2020 6569 6e73 756d 5f69 6e70        einsum_inp
-0000d180: 7574 202b 3d20 5332 5f69 6e64 6578 5f73  ut += S2_index_s
-0000d190: 7472 696e 670d 0a20 2020 2020 2020 2065  tring..        e
-0000d1a0: 696e 7375 6d5f 6f62 6a5f 6c69 7374 202b  insum_obj_list +
-0000d1b0: 3d20 5332 5f6c 6973 740d 0a0d 0a20 2020  = S2_list....   
-0000d1c0: 2069 6620 6861 735f 6f75 7470 7574 203a   if has_output :
-0000d1d0: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-0000d1e0: 2073 6b69 705f 5333 203a 0d0a 2020 2020   skip_S3 :..    
-0000d1f0: 2020 2020 2020 2020 6569 6e73 756d 5f69          einsum_i
-0000d200: 6e70 7574 202b 3d20 222c 222b 5333 5f69  nput += ","+S3_i
-0000d210: 6e64 6578 5f73 7472 696e 670d 0a20 2020  ndex_string..   
-0000d220: 2020 2020 2020 2020 2065 696e 7375 6d5f           einsum_
-0000d230: 6f62 6a5f 6c69 7374 202b 3d20 5333 2c0d  obj_list += S3,.
-0000d240: 0a0d 0a20 2020 2069 6620 7468 6973 5f74  ...    if this_t
-0000d250: 7970 6520 3d3d 2073 7061 7273 6520 3a0d  ype == sparse :.
-0000d260: 0a20 2020 2020 2020 200d 0a0d 0a20 2020  .        ....   
-0000d270: 2020 2020 2069 6e73 7472 7563 7469 6f6e       instruction
-0000d280: 5f61 6c6c 5f69 6e64 6963 6573 203d 2069  _all_indices = i
-0000d290: 6e73 7472 7563 7469 6f6e 5f73 7472 696e  nstruction_strin
-0000d2a0: 672e 7265 706c 6163 6528 222c 222c 2222  g.replace(",",""
-0000d2b0: 290d 0a20 2020 2020 2020 2069 6e73 7472  )..        instr
-0000d2c0: 7563 7469 6f6e 5f61 6c6c 5f69 6e64 6963  uction_all_indic
-0000d2d0: 6573 203d 2069 6e73 7472 7563 7469 6f6e  es = instruction
-0000d2e0: 5f61 6c6c 5f69 6e64 6963 6573 2e72 6570  _all_indices.rep
-0000d2f0: 6c61 6365 2822 2d3e 222c 2222 290d 0a20  lace("->","").. 
-0000d300: 2020 2020 2020 2069 6e73 7472 7563 7469         instructi
-0000d310: 6f6e 5f61 6c6c 5f69 6e64 6963 6573 203d  on_all_indices =
-0000d320: 2069 6e73 7472 7563 7469 6f6e 5f61 6c6c   instruction_all
-0000d330: 5f69 6e64 6963 6573 2e72 6570 6c61 6365  _indices.replace
-0000d340: 2822 2022 2c22 2229 0d0a 2020 2020 2020  (" ","")..      
-0000d350: 2020 6966 206e 6f74 2073 6b69 705f 5331    if not skip_S1
-0000d360: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-0000d370: 6e73 7472 7563 7469 6f6e 5f61 6c6c 5f69  nstruction_all_i
-0000d380: 6e64 6963 6573 3d69 6e73 7472 7563 7469  ndices=instructi
-0000d390: 6f6e 5f61 6c6c 5f69 6e64 6963 6573 2b53  on_all_indices+S
-0000d3a0: 315f 696e 6465 785f 7374 7269 6e67 0d0a  1_index_string..
-0000d3b0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-0000d3c0: 6b69 705f 5332 3a0d 0a20 2020 2020 2020  kip_S2:..       
-0000d3d0: 2020 2020 2069 6e73 7472 7563 7469 6f6e       instruction
-0000d3e0: 5f61 6c6c 5f69 6e64 6963 6573 3d69 6e73  _all_indices=ins
-0000d3f0: 7472 7563 7469 6f6e 5f61 6c6c 5f69 6e64  truction_all_ind
-0000d400: 6963 6573 2b53 325f 696e 6465 785f 7374  ices+S2_index_st
-0000d410: 7269 6e67 0d0a 2020 2020 2020 2020 6966  ring..        if
-0000d420: 206e 6f74 2073 6b69 705f 5333 3a0d 0a20   not skip_S3:.. 
-0000d430: 2020 2020 2020 2020 2020 2069 6e73 7472             instr
-0000d440: 7563 7469 6f6e 5f61 6c6c 5f69 6e64 6963  uction_all_indic
-0000d450: 6573 3d69 6e73 7472 7563 7469 6f6e 5f61  es=instruction_a
-0000d460: 6c6c 5f69 6e64 6963 6573 2b53 335f 696e  ll_indices+S3_in
-0000d470: 6465 785f 7374 7269 6e67 0d0a 0d0a 2020  dex_string....  
-0000d480: 2020 2020 2020 2320 6d61 6b65 2061 206c        # make a l
-0000d490: 6973 7469 6e67 206f 6620 6475 706c 6963  isting of duplic
-0000d4a0: 6174 6564 2069 6e64 6963 6573 0d0a 2020  ated indices..  
-0000d4b0: 2020 2020 2020 6569 6e73 756d 5f69 6e70        einsum_inp
-0000d4c0: 7574 5f75 6e69 7175 6520 3d20 2222 0d0a  ut_unique = ""..
-0000d4d0: 2020 2020 2020 2020 7665 7274 6578 5f6c          vertex_l
-0000d4e0: 6973 7420 3d20 5b5d 2023 205b 2069 6e64  ist = [] # [ ind
-0000d4f0: 6963 6573 202c 2073 6861 7065 202c 206e  ices , shape , n
-0000d500: 756d 6265 725f 6f66 5f6c 6567 7320 5d0d  umber_of_legs ].
-0000d510: 0a20 2020 2020 2020 2075 6e69 7175 655f  .        unique_
-0000d520: 6368 6172 203d 2022 220d 0a20 2020 2020  char = ""..     
-0000d530: 2020 2066 6f72 2069 2c63 2069 6e20 656e     for i,c in en
-0000d540: 756d 6572 6174 6528 696e 7374 7275 6374  umerate(instruct
-0000d550: 696f 6e5f 616c 6c5f 696e 6469 6365 7329  ion_all_indices)
-0000d560: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-0000d570: 6620 633d 3d22 2c22 203a 0d0a 2020 2020  f c=="," :..    
-0000d580: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-0000d590: 696e 7565 0d0a 2020 2020 2020 2020 2020  inue..          
-0000d5a0: 2020 6966 2069 6e73 7472 7563 7469 6f6e    if instruction
-0000d5b0: 5f61 6c6c 5f69 6e64 6963 6573 5b3a 695d  _all_indices[:i]
-0000d5c0: 2e63 6f75 6e74 2863 2920 3d3d 2030 203a  .count(c) == 0 :
-0000d5d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d5e0: 2020 7665 7274 6578 5f6c 6973 7420 2b3d    vertex_list +=
-0000d5f0: 205b 2063 2c20 7368 6170 655f 6c69 7374   [ c, shape_list
-0000d600: 5b20 7375 6d6d 616e 642e 696e 6465 7828  [ summand.index(
-0000d610: 6329 205d 202c 2069 6e73 7472 7563 7469  c) ] , instructi
-0000d620: 6f6e 5f61 6c6c 5f69 6e64 6963 6573 2e63  on_all_indices.c
-0000d630: 6f75 6e74 2863 2920 5d2c 0d0a 2020 2020  ount(c) ],..    
-0000d640: 2020 2020 2020 2020 2020 2020 756e 6971              uniq
-0000d650: 7565 5f63 6861 7220 2b3d 2063 0d0a 0d0a  ue_char += c....
-0000d660: 2020 2020 2020 2020 666f 7220 692c 5b63          for i,[c
-0000d670: 6861 722c 6469 6d2c 6e6c 6567 735d 2069  har,dim,nlegs] i
-0000d680: 6e20 656e 756d 6572 6174 6528 7665 7274  n enumerate(vert
-0000d690: 6578 5f6c 6973 7429 203a 0d0a 2020 2020  ex_list) :..    
-0000d6a0: 2020 2020 2020 2020 6c65 6763 6861 7220          legchar 
-0000d6b0: 3d20 6368 6172 0d0a 2020 2020 2020 2020  = char..        
-0000d6c0: 2020 2020 666f 7220 6c65 6720 696e 2072      for leg in r
-0000d6d0: 616e 6765 286e 6c65 6773 2d31 293a 0d0a  ange(nlegs-1):..
-0000d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6f0: 6e65 775f 6368 6172 203d 2067 6574 5f63  new_char = get_c
-0000d700: 6861 7228 756e 6971 7565 5f63 6861 7229  har(unique_char)
-0000d710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d720: 2020 756e 6971 7565 5f63 6861 7220 2b3d    unique_char +=
-0000d730: 206e 6577 5f63 6861 720d 0a20 2020 2020   new_char..     
-0000d740: 2020 2020 2020 2020 2020 206c 6567 6368             legch
-0000d750: 6172 202b 3d20 6e65 775f 6368 6172 0d0a  ar += new_char..
-0000d760: 2020 2020 2020 2020 2020 2020 7665 7274              vert
-0000d770: 6578 5f6c 6973 745b 695d 5b30 5d20 3d20  ex_list[i][0] = 
-0000d780: 6c65 6763 6861 720d 0a0d 0a20 2020 2020  legchar....     
-0000d790: 2020 2076 6572 7465 785f 6c69 7374 5f66     vertex_list_f
-0000d7a0: 696e 616c 203d 205b 5d0d 0a20 2020 2020  inal = []..     
-0000d7b0: 2020 2066 6f72 2065 6c65 6d20 696e 2076     for elem in v
-0000d7c0: 6572 7465 785f 6c69 7374 203a 0d0a 2020  ertex_list :..  
-0000d7d0: 2020 2020 2020 2020 2020 6966 2065 6c65            if ele
-0000d7e0: 6d5b 325d 203e 2032 3a0d 0a20 2020 2020  m[2] > 2:..     
-0000d7f0: 2020 2020 2020 2020 2020 2076 6572 7465             verte
-0000d800: 785f 6c69 7374 5f66 696e 616c 202b 3d20  x_list_final += 
-0000d810: 656c 656d 5b3a 325d 2c0d 0a20 2020 2020  elem[:2],..     
-0000d820: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000d830: 2020 2020 2066 6f72 2069 2c65 6c65 6d20       for i,elem 
-0000d840: 696e 2065 6e75 6d65 7261 7465 2876 6572  in enumerate(ver
-0000d850: 7465 785f 6c69 7374 5f66 696e 616c 293a  tex_list_final):
-0000d860: 0d0a 2020 2020 2020 2020 2020 2020 7820  ..            x 
-0000d870: 3d20 6c69 7374 2865 6c65 6d5b 305d 290d  = list(elem[0]).
-0000d880: 0a20 2020 2020 2020 2020 2020 2078 2e72  .            x.r
-0000d890: 6576 6572 7365 2829 0d0a 2020 2020 2020  everse()..      
-0000d8a0: 2020 2020 2020 7665 7274 6578 5f6c 6973        vertex_lis
-0000d8b0: 745f 6669 6e61 6c5b 695d 5b30 5d20 3d20  t_final[i][0] = 
-0000d8c0: 2727 2e6a 6f69 6e28 7829 0d0a 2020 2020  ''.join(x)..    
-0000d8d0: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
-0000d8e0: 2064 6562 7567 5f6d 6f64 6520 3a20 2020   debug_mode :   
-0000d8f0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-0000d900: 696e 7428 2920 2020 200d 0a20 2020 2020  int()    ..     
-0000d910: 2020 2020 2020 2070 7269 6e74 2822 203a         print(" :
+0000d070: 3a3a 3a3a 3a3a 0d0a 2020 2020 0d0a 2020  ::::::..    ..  
+0000d080: 2020 6569 6e73 756d 5f69 6e70 7574 203d    einsum_input =
+0000d090: 2069 6e70 7574 5f73 7472 696e 670d 0a20   input_string.. 
+0000d0a0: 2020 2065 696e 7375 6d5f 6f62 6a5f 6c69     einsum_obj_li
+0000d0b0: 7374 203d 206f 626a 5f6c 6973 740d 0a0d  st = obj_list...
+0000d0c0: 0a20 2020 2069 6620 5331 6469 6d3e 3020  .    if S1dim>0 
+0000d0d0: 616e 6420 6e6f 7420 736b 6970 5f53 313a  and not skip_S1:
+0000d0e0: 0d0a 2020 2020 2020 2020 6569 6e73 756d  ..        einsum
+0000d0f0: 5f69 6e70 7574 202b 3d20 222c 222b 5331  _input += ","+S1
+0000d100: 5f69 6e64 6578 5f73 7472 696e 670d 0a20  _index_string.. 
+0000d110: 2020 2020 2020 2065 696e 7375 6d5f 6f62         einsum_ob
+0000d120: 6a5f 6c69 7374 202b 3d20 5331 2c0d 0a0d  j_list += S1,...
+0000d130: 0a20 2020 2069 6620 6e53 323e 3020 3a0d  .    if nS2>0 :.
+0000d140: 0a20 2020 2020 2020 2065 696e 7375 6d5f  .        einsum_
+0000d150: 696e 7075 7420 2b3d 2053 325f 696e 6465  input += S2_inde
+0000d160: 785f 7374 7269 6e67 0d0a 2020 2020 2020  x_string..      
+0000d170: 2020 6569 6e73 756d 5f6f 626a 5f6c 6973    einsum_obj_lis
+0000d180: 7420 2b3d 2053 325f 6c69 7374 0d0a 0d0a  t += S2_list....
+0000d190: 2020 2020 6966 2068 6173 5f6f 7574 7075      if has_outpu
+0000d1a0: 7420 3a0d 0a20 2020 2020 2020 2069 6620  t :..        if 
+0000d1b0: 6e6f 7420 736b 6970 5f53 3320 3a0d 0a20  not skip_S3 :.. 
+0000d1c0: 2020 2020 2020 2020 2020 2065 696e 7375             einsu
+0000d1d0: 6d5f 696e 7075 7420 2b3d 2022 2c22 2b53  m_input += ","+S
+0000d1e0: 335f 696e 6465 785f 7374 7269 6e67 0d0a  3_index_string..
+0000d1f0: 2020 2020 2020 2020 2020 2020 6569 6e73              eins
+0000d200: 756d 5f6f 626a 5f6c 6973 7420 2b3d 2053  um_obj_list += S
+0000d210: 332c 0d0a 0d0a 2020 2020 6966 2074 6869  3,....    if thi
+0000d220: 735f 7479 7065 203d 3d20 7370 6172 7365  s_type == sparse
+0000d230: 203a 0d0a 2020 2020 2020 2020 0d0a 0d0a   :..        ....
+0000d240: 2020 2020 2020 2020 696e 7374 7275 6374          instruct
+0000d250: 696f 6e5f 616c 6c5f 696e 6469 6365 7320  ion_all_indices 
+0000d260: 3d20 696e 7374 7275 6374 696f 6e5f 7374  = instruction_st
+0000d270: 7269 6e67 2e72 6570 6c61 6365 2822 2c22  ring.replace(","
+0000d280: 2c22 2229 0d0a 2020 2020 2020 2020 696e  ,"")..        in
+0000d290: 7374 7275 6374 696f 6e5f 616c 6c5f 696e  struction_all_in
+0000d2a0: 6469 6365 7320 3d20 696e 7374 7275 6374  dices = instruct
+0000d2b0: 696f 6e5f 616c 6c5f 696e 6469 6365 732e  ion_all_indices.
+0000d2c0: 7265 706c 6163 6528 222d 3e22 2c22 2229  replace("->","")
+0000d2d0: 0d0a 2020 2020 2020 2020 696e 7374 7275  ..        instru
+0000d2e0: 6374 696f 6e5f 616c 6c5f 696e 6469 6365  ction_all_indice
+0000d2f0: 7320 3d20 696e 7374 7275 6374 696f 6e5f  s = instruction_
+0000d300: 616c 6c5f 696e 6469 6365 732e 7265 706c  all_indices.repl
+0000d310: 6163 6528 2220 222c 2222 290d 0a20 2020  ace(" ","")..   
+0000d320: 2020 2020 2069 6620 6e6f 7420 736b 6970       if not skip
+0000d330: 5f53 313a 0d0a 2020 2020 2020 2020 2020  _S1:..          
+0000d340: 2020 696e 7374 7275 6374 696f 6e5f 616c    instruction_al
+0000d350: 6c5f 696e 6469 6365 733d 696e 7374 7275  l_indices=instru
+0000d360: 6374 696f 6e5f 616c 6c5f 696e 6469 6365  ction_all_indice
+0000d370: 732b 5331 5f69 6e64 6578 5f73 7472 696e  s+S1_index_strin
+0000d380: 670d 0a20 2020 2020 2020 2069 6620 6e6f  g..        if no
+0000d390: 7420 736b 6970 5f53 323a 0d0a 2020 2020  t skip_S2:..    
+0000d3a0: 2020 2020 2020 2020 696e 7374 7275 6374          instruct
+0000d3b0: 696f 6e5f 616c 6c5f 696e 6469 6365 733d  ion_all_indices=
+0000d3c0: 696e 7374 7275 6374 696f 6e5f 616c 6c5f  instruction_all_
+0000d3d0: 696e 6469 6365 732b 5332 5f69 6e64 6578  indices+S2_index
+0000d3e0: 5f73 7472 696e 670d 0a20 2020 2020 2020  _string..       
+0000d3f0: 2069 6620 6e6f 7420 736b 6970 5f53 333a   if not skip_S3:
+0000d400: 0d0a 2020 2020 2020 2020 2020 2020 696e  ..            in
+0000d410: 7374 7275 6374 696f 6e5f 616c 6c5f 696e  struction_all_in
+0000d420: 6469 6365 733d 696e 7374 7275 6374 696f  dices=instructio
+0000d430: 6e5f 616c 6c5f 696e 6469 6365 732b 5333  n_all_indices+S3
+0000d440: 5f69 6e64 6578 5f73 7472 696e 670d 0a0d  _index_string...
+0000d450: 0a20 2020 2020 2020 2023 206d 616b 6520  .        # make 
+0000d460: 6120 6c69 7374 696e 6720 6f66 2064 7570  a listing of dup
+0000d470: 6c69 6361 7465 6420 696e 6469 6365 730d  licated indices.
+0000d480: 0a20 2020 2020 2020 2065 696e 7375 6d5f  .        einsum_
+0000d490: 696e 7075 745f 756e 6971 7565 203d 2022  input_unique = "
+0000d4a0: 220d 0a20 2020 2020 2020 2076 6572 7465  "..        verte
+0000d4b0: 785f 6c69 7374 203d 205b 5d20 2320 5b20  x_list = [] # [ 
+0000d4c0: 696e 6469 6365 7320 2c20 7368 6170 6520  indices , shape 
+0000d4d0: 2c20 6e75 6d62 6572 5f6f 665f 6c65 6773  , number_of_legs
+0000d4e0: 205d 0d0a 2020 2020 2020 2020 756e 6971   ]..        uniq
+0000d4f0: 7565 5f63 6861 7220 3d20 2222 0d0a 2020  ue_char = ""..  
+0000d500: 2020 2020 2020 666f 7220 692c 6320 696e        for i,c in
+0000d510: 2065 6e75 6d65 7261 7465 2869 6e73 7472   enumerate(instr
+0000d520: 7563 7469 6f6e 5f61 6c6c 5f69 6e64 6963  uction_all_indic
+0000d530: 6573 293a 0d0a 2020 2020 2020 2020 2020  es):..          
+0000d540: 2020 6966 2063 3d3d 222c 2220 3a0d 0a20    if c=="," :.. 
+0000d550: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000d560: 6f6e 7469 6e75 650d 0a20 2020 2020 2020  ontinue..       
+0000d570: 2020 2020 2069 6620 696e 7374 7275 6374       if instruct
+0000d580: 696f 6e5f 616c 6c5f 696e 6469 6365 735b  ion_all_indices[
+0000d590: 3a69 5d2e 636f 756e 7428 6329 203d 3d20  :i].count(c) == 
+0000d5a0: 3020 3a0d 0a20 2020 2020 2020 2020 2020  0 :..           
+0000d5b0: 2020 2020 2076 6572 7465 785f 6c69 7374       vertex_list
+0000d5c0: 202b 3d20 5b20 632c 2073 6861 7065 5f6c   += [ c, shape_l
+0000d5d0: 6973 745b 2073 756d 6d61 6e64 2e69 6e64  ist[ summand.ind
+0000d5e0: 6578 2863 2920 5d20 2c20 696e 7374 7275  ex(c) ] , instru
+0000d5f0: 6374 696f 6e5f 616c 6c5f 696e 6469 6365  ction_all_indice
+0000d600: 732e 636f 756e 7428 6329 205d 2c0d 0a20  s.count(c) ],.. 
+0000d610: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+0000d620: 6e69 7175 655f 6368 6172 202b 3d20 630d  nique_char += c.
+0000d630: 0a0d 0a20 2020 2020 2020 2066 6f72 2069  ...        for i
+0000d640: 2c5b 6368 6172 2c64 696d 2c6e 6c65 6773  ,[char,dim,nlegs
+0000d650: 5d20 696e 2065 6e75 6d65 7261 7465 2876  ] in enumerate(v
+0000d660: 6572 7465 785f 6c69 7374 2920 3a0d 0a20  ertex_list) :.. 
+0000d670: 2020 2020 2020 2020 2020 206c 6567 6368             legch
+0000d680: 6172 203d 2063 6861 720d 0a20 2020 2020  ar = char..     
+0000d690: 2020 2020 2020 2066 6f72 206c 6567 2069         for leg i
+0000d6a0: 6e20 7261 6e67 6528 6e6c 6567 732d 3129  n range(nlegs-1)
+0000d6b0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000d6c0: 2020 206e 6577 5f63 6861 7220 3d20 6765     new_char = ge
+0000d6d0: 745f 6368 6172 2875 6e69 7175 655f 6368  t_char(unique_ch
+0000d6e0: 6172 290d 0a20 2020 2020 2020 2020 2020  ar)..           
+0000d6f0: 2020 2020 2075 6e69 7175 655f 6368 6172       unique_char
+0000d700: 202b 3d20 6e65 775f 6368 6172 0d0a 2020   += new_char..  
+0000d710: 2020 2020 2020 2020 2020 2020 2020 6c65                le
+0000d720: 6763 6861 7220 2b3d 206e 6577 5f63 6861  gchar += new_cha
+0000d730: 720d 0a20 2020 2020 2020 2020 2020 2076  r..            v
+0000d740: 6572 7465 785f 6c69 7374 5b69 5d5b 305d  ertex_list[i][0]
+0000d750: 203d 206c 6567 6368 6172 0d0a 0d0a 2020   = legchar....  
+0000d760: 2020 2020 2020 7665 7274 6578 5f6c 6973        vertex_lis
+0000d770: 745f 6669 6e61 6c20 3d20 5b5d 0d0a 2020  t_final = []..  
+0000d780: 2020 2020 2020 666f 7220 656c 656d 2069        for elem i
+0000d790: 6e20 7665 7274 6578 5f6c 6973 7420 3a0d  n vertex_list :.
+0000d7a0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000d7b0: 656c 656d 5b32 5d20 3e20 323a 0d0a 2020  elem[2] > 2:..  
+0000d7c0: 2020 2020 2020 2020 2020 2020 2020 7665                ve
+0000d7d0: 7274 6578 5f6c 6973 745f 6669 6e61 6c20  rtex_list_final 
+0000d7e0: 2b3d 2065 6c65 6d5b 3a32 5d2c 0d0a 2020  += elem[:2],..  
+0000d7f0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0000d800: 2020 2020 2020 2020 666f 7220 692c 656c          for i,el
+0000d810: 656d 2069 6e20 656e 756d 6572 6174 6528  em in enumerate(
+0000d820: 7665 7274 6578 5f6c 6973 745f 6669 6e61  vertex_list_fina
+0000d830: 6c29 3a0d 0a20 2020 2020 2020 2020 2020  l):..           
+0000d840: 2078 203d 206c 6973 7428 656c 656d 5b30   x = list(elem[0
+0000d850: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
+0000d860: 782e 7265 7665 7273 6528 290d 0a20 2020  x.reverse()..   
+0000d870: 2020 2020 2020 2020 2076 6572 7465 785f           vertex_
+0000d880: 6c69 7374 5f66 696e 616c 5b69 5d5b 305d  list_final[i][0]
+0000d890: 203d 2027 272e 6a6f 696e 2878 290d 0a20   = ''.join(x).. 
+0000d8a0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000d8b0: 2069 6620 6465 6275 675f 6d6f 6465 203a   if debug_mode :
+0000d8c0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000d8d0: 2070 7269 6e74 2829 0d0a 2020 2020 2020   print()..      
+0000d8e0: 2020 2020 2020 7072 696e 7428 2220 3a3a        print(" ::
+0000d8f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000d900: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 2076 6572  :::::::::::: ver
+0000d910: 7469 6365 7320 3a3a 3a3a 3a3a 3a3a 3a3a  tices ::::::::::
 0000d920: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000d930: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a20 7665  ::::::::::::: ve
-0000d940: 7274 6963 6573 203a 3a3a 3a3a 3a3a 3a3a  rtices :::::::::
-0000d950: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000d960: 3a3a 3a3a 2022 290d 0a20 2020 2020 2020  :::: ")..       
-0000d970: 2020 2020 2070 7269 6e74 2869 6e73 7472       print(instr
-0000d980: 7563 7469 6f6e 5f61 6c6c 5f69 6e64 6963  uction_all_indic
-0000d990: 6573 2c22 3c2d 2d20 7468 6520 696e 7374  es,"<-- the inst
-0000d9a0: 7275 6374 696f 6e20 7374 7269 6e67 7320  ruction strings 
-0000d9b0: 7769 7468 2061 6c6c 2063 6861 7220 636f  with all char co
-0000d9c0: 6d62 696e 6564 2069 6e74 6f20 6f6e 6520  mbined into one 
-0000d9d0: 7374 7269 6e67 2229 0d0a 2020 2020 2020  string")..      
-0000d9e0: 2020 2020 2020 7072 696e 7428 2276 6572        print("ver
-0000d9f0: 7465 7820 6c69 7374 3a22 290d 0a20 2020  tex list:")..   
-0000da00: 2020 2020 2020 2020 2066 6f72 2076 6572           for ver
-0000da10: 7420 696e 2076 6572 7465 785f 6c69 7374  t in vertex_list
-0000da20: 5f66 696e 616c 3a0d 0a20 2020 2020 2020  _final:..       
-0000da30: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-0000da40: 2022 2c76 6572 7429 0d0a 2020 2020 0d0a   ",vert)..    ..
-0000da50: 2020 2020 0d0a 2020 2020 2320 6e6f 7720      ..    # now 
-0000da60: 7265 706c 6163 6520 7468 6520 6569 6e73  replace the eins
-0000da70: 756d 2073 7472 696e 6720 7769 7468 2074  um string with t
-0000da80: 6865 7365 206e 6577 2063 6861 7261 6374  hese new charact
-0000da90: 6572 730d 0a20 2020 200d 0a20 2020 2023  ers..    ..    #
-0000daa0: 6765 7420 7468 6520 636f 7272 6563 7420  get the correct 
-0000dab0: 6569 6e73 756d 2073 7472 696e 6720 6669  einsum string fi
-0000dac0: 7273 740d 0a20 2020 2065 696e 7375 6d5f  rst..    einsum_
-0000dad0: 7374 7269 6e67 203d 2069 6e70 7574 5f73  string = input_s
-0000dae0: 7472 696e 670d 0a20 2020 2069 6620 6e6f  tring..    if no
-0000daf0: 7420 736b 6970 5f53 3120 3a0d 0a20 2020  t skip_S1 :..   
-0000db00: 2020 2020 2065 696e 7375 6d5f 7374 7269       einsum_stri
-0000db10: 6e67 202b 3d20 222c 222b 5331 5f69 6e64  ng += ","+S1_ind
-0000db20: 6578 5f73 7472 696e 670d 0a20 2020 2069  ex_string..    i
-0000db30: 6620 6e6f 7420 736b 6970 5f53 3220 3a0d  f not skip_S2 :.
-0000db40: 0a20 2020 2020 2020 2065 696e 7375 6d5f  .        einsum_
-0000db50: 7374 7269 6e67 202b 3d20 222c 222b 5332  string += ","+S2
-0000db60: 5f69 6e64 6578 5f73 7472 696e 670d 0a20  _index_string.. 
-0000db70: 2020 2069 6620 6e6f 7420 736b 6970 5f53     if not skip_S
-0000db80: 3320 3a0d 0a20 2020 2020 2020 2065 696e  3 :..        ein
-0000db90: 7375 6d5f 7374 7269 6e67 202b 3d20 222c  sum_string += ",
-0000dba0: 222b 5333 5f69 6e64 6578 5f73 7472 696e  "+S3_index_strin
-0000dbb0: 670d 0a20 2020 2069 6620 6465 6275 675f  g..    if debug_
-0000dbc0: 6d6f 6465 203a 2020 200d 0a20 2020 2020  mode :   ..     
-0000dbd0: 2020 2070 7269 6e74 2829 2020 2020 0d0a     print()    ..
-0000dbe0: 2020 2020 2020 2020 7072 696e 7428 6569          print(ei
-0000dbf0: 6e73 756d 5f73 7472 696e 672c 223c 2d2d  nsum_string,"<--
-0000dc00: 2065 696e 7375 6d5f 7374 7269 6e67 203d   einsum_string =
-0000dc10: 2065 696e 7375 6d20 7374 7269 6e67 2077   einsum string w
-0000dc20: 6974 686f 7574 2076 6572 7469 6365 7322  ithout vertices"
-0000dc30: 290d 0a20 2020 200d 0a20 2020 2069 6620  )..    ..    if 
-0000dc40: 7468 6973 5f74 7970 6520 3d3d 2073 7061  this_type == spa
-0000dc50: 7273 6520 3a0d 0a20 2020 2020 2020 2065  rse :..        e
-0000dc60: 696e 7375 6d5f 7374 7269 6e67 5f72 6570  insum_string_rep
-0000dc70: 6c61 6365 6420 3d20 6569 6e73 756d 5f73  laced = einsum_s
-0000dc80: 7472 696e 670d 0a20 2020 2020 2020 2066  tring..        f
-0000dc90: 6f72 205b 7665 7274 2c64 696d 5d20 696e  or [vert,dim] in
-0000dca0: 2076 6572 7465 785f 6c69 7374 5f66 696e   vertex_list_fin
-0000dcb0: 616c 3a0d 0a20 2020 2020 2020 2020 2020  al:..           
-0000dcc0: 2063 203d 2076 6572 745b 6c65 6e28 7665   c = vert[len(ve
-0000dcd0: 7274 292d 315d 0d0a 2020 2020 2020 2020  rt)-1]..        
-0000dce0: 2020 2020 6e72 6570 6c61 6365 203d 2065      nreplace = e
-0000dcf0: 696e 7375 6d5f 7374 7269 6e67 5f72 6570  insum_string_rep
-0000dd00: 6c61 6365 642e 636f 756e 7428 6329 0d0a  laced.count(c)..
-0000dd10: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000dd20: 6920 696e 2072 616e 6765 286e 7265 706c  i in range(nrepl
-0000dd30: 6163 6529 3a0d 0a20 2020 2020 2020 2020  ace):..         
-0000dd40: 2020 2020 2020 2065 696e 7375 6d5f 7374         einsum_st
-0000dd50: 7269 6e67 5f72 6570 6c61 6365 6420 3d20  ring_replaced = 
-0000dd60: 6569 6e73 756d 5f73 7472 696e 675f 7265  einsum_string_re
-0000dd70: 706c 6163 6564 2e72 6570 6c61 6365 2863  placed.replace(c
-0000dd80: 2c76 6572 745b 695d 2c31 290d 0a20 2020  ,vert[i],1)..   
-0000dd90: 2020 2020 2020 2020 2065 696e 7375 6d5f           einsum_
-0000dda0: 7374 7269 6e67 5f72 6570 6c61 6365 642b  string_replaced+
-0000ddb0: 3d22 2c22 2b76 6572 740d 0a20 2020 2020  =","+vert..     
-0000ddc0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000ddd0: 2069 6620 6465 6275 675f 6d6f 6465 203a   if debug_mode :
-0000dde0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000ddf0: 2070 7269 6e74 2829 2020 2020 0d0a 2020   print()    ..  
-0000de00: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0000de10: 6569 6e73 756d 5f73 7472 696e 675f 7265  einsum_string_re
-0000de20: 706c 6163 6564 2c22 3c2d 2d20 6569 6e73  placed,"<-- eins
-0000de30: 756d 5f73 7472 696e 6720 7769 7468 2072  um_string with r
-0000de40: 6570 6c61 6365 6d65 6e74 2229 0d0a 2020  eplacement")..  
-0000de50: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000de60: 2320 636f 6e73 7472 7563 7420 7468 6520  # construct the 
-0000de70: 7665 7274 6578 2074 656e 736f 7273 0d0a  vertex tensors..
-0000de80: 2020 2020 2020 2020 7665 7274 6578 5f6f          vertex_o
-0000de90: 626a 5f6c 6973 7420 3d20 5b5d 0d0a 2020  bj_list = []..  
-0000dea0: 2020 2020 2020 666f 7220 5b73 7472 696e        for [strin
-0000deb0: 672c 6469 6d5d 2069 6e20 7665 7274 6578  g,dim] in vertex
-0000dec0: 5f6c 6973 745f 6669 6e61 6c20 3a0d 0a20  _list_final :.. 
-0000ded0: 2020 2020 2020 2020 2020 2073 6861 7065             shape
-0000dee0: 3d74 7570 6c65 285b 6469 6d5d 2a6c 656e  =tuple([dim]*len
-0000def0: 2873 7472 696e 6729 290d 0a20 2020 2020  (string))..     
-0000df00: 2020 2020 2020 2063 6f6f 7264 7320 3d20         coords = 
-0000df10: 6e70 2e61 7272 6179 285b 205b 2069 2066  np.array([ [ i f
-0000df20: 6f72 2069 2069 6e20 7261 6e67 6528 6469  or i in range(di
-0000df30: 6d29 205d 2066 6f72 206a 2069 6e20 7261  m) ] for j in ra
-0000df40: 6e67 6528 6c65 6e28 7374 7269 6e67 2929  nge(len(string))
-0000df50: 5d29 0d0a 2020 2020 2020 2020 2020 2020  ])..            
-0000df60: 6461 7461 203d 206e 702e 6172 7261 7928  data = np.array(
-0000df70: 205b 2031 2066 6f72 2069 2069 6e20 7261   [ 1 for i in ra
-0000df80: 6e67 6528 6469 6d29 205d 2029 0d0a 2020  nge(dim) ] )..  
-0000df90: 2020 2020 2020 2020 2020 7665 7274 6578            vertex
-0000dfa0: 203d 2073 702e 434f 4f28 2063 6f6f 7264   = sp.COO( coord
-0000dfb0: 732c 2064 6174 612c 2073 6861 7065 3d73  s, data, shape=s
-0000dfc0: 6861 7065 2029 0d0a 2020 2020 2020 2020  hape )..        
-0000dfd0: 2020 2020 7665 7274 6578 5f6f 626a 5f6c      vertex_obj_l
-0000dfe0: 6973 7420 2b3d 2076 6572 7465 782e 636f  ist += vertex.co
-0000dff0: 7079 2829 2c0d 0a0d 0a20 2020 2023 3a3a  py(),....    #::
+0000d930: 3a3a 3a20 2229 0d0a 2020 2020 2020 2020  ::: ")..        
+0000d940: 2020 2020 7072 696e 7428 696e 7374 7275      print(instru
+0000d950: 6374 696f 6e5f 616c 6c5f 696e 6469 6365  ction_all_indice
+0000d960: 732c 223c 2d2d 2074 6865 2069 6e73 7472  s,"<-- the instr
+0000d970: 7563 7469 6f6e 2073 7472 696e 6773 2077  uction strings w
+0000d980: 6974 6820 616c 6c20 6368 6172 2063 6f6d  ith all char com
+0000d990: 6269 6e65 6420 696e 746f 206f 6e65 2073  bined into one s
+0000d9a0: 7472 696e 6722 290d 0a20 2020 2020 2020  tring")..       
+0000d9b0: 2020 2020 2070 7269 6e74 2822 7665 7274       print("vert
+0000d9c0: 6578 206c 6973 743a 2229 0d0a 2020 2020  ex list:")..    
+0000d9d0: 2020 2020 2020 2020 666f 7220 7665 7274          for vert
+0000d9e0: 2069 6e20 7665 7274 6578 5f6c 6973 745f   in vertex_list_
+0000d9f0: 6669 6e61 6c3a 0d0a 2020 2020 2020 2020  final:..        
+0000da00: 2020 2020 2020 2020 7072 696e 7428 2220          print(" 
+0000da10: 222c 7665 7274 290d 0a20 2020 200d 0a20  ",vert)..    .. 
+0000da20: 2020 200d 0a20 2020 2023 206e 6f77 2072     ..    # now r
+0000da30: 6570 6c61 6365 2074 6865 2065 696e 7375  eplace the einsu
+0000da40: 6d20 7374 7269 6e67 2077 6974 6820 7468  m string with th
+0000da50: 6573 6520 6e65 7720 6368 6172 6163 7465  ese new characte
+0000da60: 7273 0d0a 2020 2020 0d0a 2020 2020 2367  rs..    ..    #g
+0000da70: 6574 2074 6865 2063 6f72 7265 6374 2065  et the correct e
+0000da80: 696e 7375 6d20 7374 7269 6e67 2066 6972  insum string fir
+0000da90: 7374 0d0a 2020 2020 6569 6e73 756d 5f73  st..    einsum_s
+0000daa0: 7472 696e 6720 3d20 696e 7075 745f 7374  tring = input_st
+0000dab0: 7269 6e67 0d0a 2020 2020 6966 206e 6f74  ring..    if not
+0000dac0: 2073 6b69 705f 5331 203a 0d0a 2020 2020   skip_S1 :..    
+0000dad0: 2020 2020 6569 6e73 756d 5f73 7472 696e      einsum_strin
+0000dae0: 6720 2b3d 2022 2c22 2b53 315f 696e 6465  g += ","+S1_inde
+0000daf0: 785f 7374 7269 6e67 0d0a 2020 2020 6966  x_string..    if
+0000db00: 206e 6f74 2073 6b69 705f 5332 203a 0d0a   not skip_S2 :..
+0000db10: 2020 2020 2020 2020 6569 6e73 756d 5f73          einsum_s
+0000db20: 7472 696e 6720 2b3d 2022 2c22 2b53 325f  tring += ","+S2_
+0000db30: 696e 6465 785f 7374 7269 6e67 0d0a 2020  index_string..  
+0000db40: 2020 6966 206e 6f74 2073 6b69 705f 5333    if not skip_S3
+0000db50: 203a 0d0a 2020 2020 2020 2020 6569 6e73   :..        eins
+0000db60: 756d 5f73 7472 696e 6720 2b3d 2022 2c22  um_string += ","
+0000db70: 2b53 335f 696e 6465 785f 7374 7269 6e67  +S3_index_string
+0000db80: 0d0a 2020 2020 6966 2064 6562 7567 5f6d  ..    if debug_m
+0000db90: 6f64 6520 3a20 2020 0d0a 2020 2020 2020  ode :   ..      
+0000dba0: 2020 7072 696e 7428 2920 200d 0a20 2020    print()  ..   
+0000dbb0: 2020 2020 2070 7269 6e74 2865 696e 7375       print(einsu
+0000dbc0: 6d5f 7374 7269 6e67 2c22 3c2d 2d20 6569  m_string,"<-- ei
+0000dbd0: 6e73 756d 5f73 7472 696e 6720 3d20 6569  nsum_string = ei
+0000dbe0: 6e73 756d 2073 7472 696e 6720 7769 7468  nsum string with
+0000dbf0: 6f75 7420 7665 7274 6963 6573 2229 0d0a  out vertices")..
+0000dc00: 2020 2020 0d0a 2020 2020 6966 2074 6869      ..    if thi
+0000dc10: 735f 7479 7065 203d 3d20 7370 6172 7365  s_type == sparse
+0000dc20: 203a 0d0a 2020 2020 2020 2020 6569 6e73   :..        eins
+0000dc30: 756d 5f73 7472 696e 675f 7265 706c 6163  um_string_replac
+0000dc40: 6564 203d 2065 696e 7375 6d5f 7374 7269  ed = einsum_stri
+0000dc50: 6e67 0d0a 2020 2020 2020 2020 666f 7220  ng..        for 
+0000dc60: 5b76 6572 742c 6469 6d5d 2069 6e20 7665  [vert,dim] in ve
+0000dc70: 7274 6578 5f6c 6973 745f 6669 6e61 6c3a  rtex_list_final:
+0000dc80: 0d0a 2020 2020 2020 2020 2020 2020 6320  ..            c 
+0000dc90: 3d20 7665 7274 5b6c 656e 2876 6572 7429  = vert[len(vert)
+0000dca0: 2d31 5d0d 0a20 2020 2020 2020 2020 2020  -1]..           
+0000dcb0: 206e 7265 706c 6163 6520 3d20 6569 6e73   nreplace = eins
+0000dcc0: 756d 5f73 7472 696e 675f 7265 706c 6163  um_string_replac
+0000dcd0: 6564 2e63 6f75 6e74 2863 290d 0a20 2020  ed.count(c)..   
+0000dce0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+0000dcf0: 6e20 7261 6e67 6528 6e72 6570 6c61 6365  n range(nreplace
+0000dd00: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000dd10: 2020 2020 6569 6e73 756d 5f73 7472 696e      einsum_strin
+0000dd20: 675f 7265 706c 6163 6564 203d 2065 696e  g_replaced = ein
+0000dd30: 7375 6d5f 7374 7269 6e67 5f72 6570 6c61  sum_string_repla
+0000dd40: 6365 642e 7265 706c 6163 6528 632c 7665  ced.replace(c,ve
+0000dd50: 7274 5b69 5d2c 3129 0d0a 2020 2020 2020  rt[i],1)..      
+0000dd60: 2020 2020 2020 6569 6e73 756d 5f73 7472        einsum_str
+0000dd70: 696e 675f 7265 706c 6163 6564 2b3d 222c  ing_replaced+=",
+0000dd80: 222b 7665 7274 0d0a 2020 2020 2020 2020  "+vert..        
+0000dd90: 2020 2020 0d0a 2020 2020 2020 2020 6966      ..        if
+0000dda0: 2064 6562 7567 5f6d 6f64 6520 3a20 2020   debug_mode :   
+0000ddb0: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+0000ddc0: 696e 7428 290d 0a20 2020 2020 2020 2020  int()..         
+0000ddd0: 2020 2070 7269 6e74 2865 696e 7375 6d5f     print(einsum_
+0000dde0: 7374 7269 6e67 5f72 6570 6c61 6365 642c  string_replaced,
+0000ddf0: 223c 2d2d 2065 696e 7375 6d5f 7374 7269  "<-- einsum_stri
+0000de00: 6e67 2077 6974 6820 7265 706c 6163 656d  ng with replacem
+0000de10: 656e 7422 290d 0a20 2020 2020 2020 200d  ent")..        .
+0000de20: 0a20 2020 2020 2020 2023 2063 6f6e 7374  .        # const
+0000de30: 7275 6374 2074 6865 2076 6572 7465 7820  ruct the vertex 
+0000de40: 7465 6e73 6f72 730d 0a20 2020 2020 2020  tensors..       
+0000de50: 2076 6572 7465 785f 6f62 6a5f 6c69 7374   vertex_obj_list
+0000de60: 203d 205b 5d0d 0a20 2020 2020 2020 2066   = []..        f
+0000de70: 6f72 205b 7374 7269 6e67 2c64 696d 5d20  or [string,dim] 
+0000de80: 696e 2076 6572 7465 785f 6c69 7374 5f66  in vertex_list_f
+0000de90: 696e 616c 203a 0d0a 2020 2020 2020 2020  inal :..        
+0000dea0: 2020 2020 7368 6170 653d 7475 706c 6528      shape=tuple(
+0000deb0: 5b64 696d 5d2a 6c65 6e28 7374 7269 6e67  [dim]*len(string
+0000dec0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+0000ded0: 636f 6f72 6473 203d 206e 702e 6172 7261  coords = np.arra
+0000dee0: 7928 5b20 5b20 6920 666f 7220 6920 696e  y([ [ i for i in
+0000def0: 2072 616e 6765 2864 696d 2920 5d20 666f   range(dim) ] fo
+0000df00: 7220 6a20 696e 2072 616e 6765 286c 656e  r j in range(len
+0000df10: 2873 7472 696e 6729 295d 290d 0a20 2020  (string))])..   
+0000df20: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
+0000df30: 6e70 2e61 7272 6179 2820 5b20 3120 666f  np.array( [ 1 fo
+0000df40: 7220 6920 696e 2072 616e 6765 2864 696d  r i in range(dim
+0000df50: 2920 5d20 290d 0a20 2020 2020 2020 2020  ) ] )..         
+0000df60: 2020 2076 6572 7465 7820 3d20 7370 2e43     vertex = sp.C
+0000df70: 4f4f 2820 636f 6f72 6473 2c20 6461 7461  OO( coords, data
+0000df80: 2c20 7368 6170 653d 7368 6170 6520 290d  , shape=shape ).
+0000df90: 0a20 2020 2020 2020 2020 2020 2076 6572  .            ver
+0000dfa0: 7465 785f 6f62 6a5f 6c69 7374 202b 3d20  tex_obj_list += 
+0000dfb0: 7665 7274 6578 2e63 6f70 7928 292c 0d0a  vertex.copy(),..
+0000dfc0: 0d0a 2020 2020 233a 3a3a 3a3a 3a3a 3a3a  ..    #:::::::::
+0000dfd0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000dfe0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000dff0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000e000: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000e010: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e020: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e030: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e040: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e050: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a  ::::::::::::::..
-0000e060: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0000e070: 2020 2053 7465 7020 363a 2067 6574 2074     Step 6: get t
-0000e080: 6865 2066 696e 616c 2073 7461 7469 7374  he final statist
-0000e090: 6963 730d 0a20 2020 2023 3a3a 3a3a 3a3a  ics..    #::::::
+0000e020: 3a3a 3a3a 3a3a 3a0d 0a20 2020 2023 2020  :::::::..    #  
+0000e030: 2020 2020 2020 2020 2020 2020 5374 6570              Step
+0000e040: 2036 3a20 6765 7420 7468 6520 6669 6e61   6: get the fina
+0000e050: 6c20 7374 6174 6973 7469 6373 0d0a 2020  l statistics..  
+0000e060: 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a    #:::::::::::::
+0000e070: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000e080: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000e090: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000e0a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000e0b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e0c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e0d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e0e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e0f0: 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a 0d0a 2020  ::::::::::....  
-0000e100: 2020 6669 6e61 6c5f 7374 6174 7320 3d20    final_stats = 
-0000e110: 5b5d 0d0a 2020 2020 6966 2068 6173 5f6f  []..    if has_o
-0000e120: 7574 7075 7420 3a0d 0a20 2020 2020 2020  utput :..       
-0000e130: 2066 6f72 2063 2069 6e20 6f75 7470 7574   for c in output
-0000e140: 5f73 7472 696e 6720 3a0d 0a20 2020 2020  _string :..     
-0000e150: 2020 2020 2020 2066 696e 616c 5f73 7461         final_sta
-0000e160: 7473 202b 3d20 7374 6174 735f 6c69 7374  ts += stats_list
-0000e170: 5b20 7375 6d6d 616e 642e 696e 6465 7828  [ summand.index(
-0000e180: 6329 205d 2c0d 0a0d 0a20 2020 2069 6620  c) ],....    if 
-0000e190: 6465 6275 675f 6d6f 6465 2061 6e64 2068  debug_mode and h
-0000e1a0: 6173 5f6f 7574 7075 743a 0d0a 2020 2020  as_output:..    
-0000e1b0: 2020 2020 7072 696e 7428 290d 0a20 2020      print()..   
-0000e1c0: 2020 2020 2070 7269 6e74 2822 203a 3a3a       print(" :::
-0000e1d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e1e0: 3a3a 3a3a 3a3a 3a20 6669 6e61 6c20 7374  ::::::: final st
-0000e1f0: 6174 6973 7469 6373 203a 3a3a 3a3a 3a3a  atistics :::::::
-0000e200: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e210: 3a3a 2022 290d 0a20 2020 2020 2020 2070  :: ")..        p
-0000e220: 7269 6e74 2866 696e 616c 5f73 7461 7473  rint(final_stats
-0000e230: 2c22 3c2d 2d2d 2066 696e 616c 2073 7461  ,"<--- final sta
-0000e240: 7473 2229 0d0a 2020 2020 2020 2020 0d0a  ts")..        ..
-0000e250: 2020 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a      #:::::::::::
+0000e0c0: 3a3a 3a0d 0a0d 0a20 2020 2066 696e 616c  :::....    final
+0000e0d0: 5f73 7461 7473 203d 205b 5d0d 0a20 2020  _stats = []..   
+0000e0e0: 2069 6620 6861 735f 6f75 7470 7574 203a   if has_output :
+0000e0f0: 0d0a 2020 2020 2020 2020 666f 7220 6320  ..        for c 
+0000e100: 696e 206f 7574 7075 745f 7374 7269 6e67  in output_string
+0000e110: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
+0000e120: 6669 6e61 6c5f 7374 6174 7320 2b3d 2073  final_stats += s
+0000e130: 7461 7473 5f6c 6973 745b 2073 756d 6d61  tats_list[ summa
+0000e140: 6e64 2e69 6e64 6578 2863 2920 5d2c 0d0a  nd.index(c) ],..
+0000e150: 0d0a 2020 2020 6966 2064 6562 7567 5f6d  ..    if debug_m
+0000e160: 6f64 6520 616e 6420 6861 735f 6f75 7470  ode and has_outp
+0000e170: 7574 3a0d 0a20 2020 2020 2020 2070 7269  ut:..        pri
+0000e180: 6e74 2829 0d0a 2020 2020 2020 2020 7072  nt()..        pr
+0000e190: 696e 7428 2220 3a3a 3a3a 3a3a 3a3a 3a3a  int(" ::::::::::
+0000e1a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000e1b0: 2066 696e 616c 2073 7461 7469 7374 6963   final statistic
+0000e1c0: 7320 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  s ::::::::::::::
+0000e1d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a20 2229 0d0a  ::::::::::: ")..
+0000e1e0: 2020 2020 2020 2020 7072 696e 7428 6669          print(fi
+0000e1f0: 6e61 6c5f 7374 6174 732c 223c 2d2d 2d20  nal_stats,"<--- 
+0000e200: 6669 6e61 6c20 7374 6174 7322 290d 0a20  final stats").. 
+0000e210: 2020 2020 2020 200d 0a20 2020 2023 3a3a         ..    #::
+0000e220: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000e230: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000e240: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000e250: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000e260: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e270: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e280: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e290: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e2a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e2b0: 3a3a 3a3a 3a0d 0a20 2020 2023 2020 2020  :::::..    #    
-0000e2c0: 2020 2020 2020 2020 2020 5374 6570 2037            Step 7
-0000e2d0: 3a20 7468 6520 6163 7475 616c 2073 756d  : the actual sum
-0000e2e0: 0d0a 2020 2020 233a 3a3a 3a3a 3a3a 3a3a  ..    #:::::::::
+0000e270: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a  ::::::::::::::..
+0000e280: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0000e290: 2020 2053 7465 7020 373a 2074 6865 2061     Step 7: the a
+0000e2a0: 6374 7561 6c20 7375 6d0d 0a20 2020 2023  ctual sum..    #
+0000e2b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000e2c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000e2d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000e2e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000e2f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 0000e300: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e310: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e320: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e330: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e340: 3a3a 3a3a 3a3a 3a0d 0a0d 0a20 2020 2069  :::::::....    i
-0000e350: 6620 7468 6973 5f74 7970 653d 3d73 7061  f this_type==spa
-0000e360: 7273 6520 3a0d 0a20 2020 2020 2020 2065  rse :..        e
-0000e370: 696e 7375 6d5f 6f62 6a5f 6c69 7374 202b  insum_obj_list +
-0000e380: 3d20 7665 7274 6578 5f6f 626a 5f6c 6973  = vertex_obj_lis
-0000e390: 740d 0a20 2020 2020 2020 2065 696e 7375  t..        einsu
-0000e3a0: 6d5f 7374 7269 6e67 203d 2065 696e 7375  m_string = einsu
-0000e3b0: 6d5f 7374 7269 6e67 5f72 6570 6c61 6365  m_string_replace
-0000e3c0: 640d 0a20 2020 200d 0a20 2020 2069 6620  d..    ..    if 
-0000e3d0: 6861 735f 6f75 7470 7574 203a 0d0a 2020  has_output :..  
-0000e3e0: 2020 2020 2020 6569 6e73 756d 5f73 7472        einsum_str
-0000e3f0: 696e 6720 2b3d 2022 2d3e 222b 6f75 7470  ing += "->"+outp
-0000e400: 7574 5f73 7472 696e 670d 0a0d 0a20 2020  ut_string....   
-0000e410: 2023 2063 6f6e 7665 7274 2061 6c6c 206f   # convert all o
-0000e420: 626a 6563 7420 746f 2074 6869 735f 7479  bject to this_ty
-0000e430: 7065 0d0a 2020 2020 6966 2074 6869 735f  pe..    if this_
-0000e440: 7479 7065 203d 3d20 7370 6172 7365 203a  type == sparse :
-0000e450: 0d0a 2020 2020 2020 2020 666f 7220 692c  ..        for i,
-0000e460: 206f 626a 2069 6e20 656e 756d 6572 6174   obj in enumerat
-0000e470: 6528 6569 6e73 756d 5f6f 626a 5f6c 6973  e(einsum_obj_lis
-0000e480: 7429 3a0d 0a20 2020 2020 2020 2020 2020  t):..           
-0000e490: 2069 6620 7479 7065 286f 626a 2920 3d3d   if type(obj) ==
-0000e4a0: 206e 702e 6e64 6172 7261 793a 0d0a 2020   np.ndarray:..  
-0000e4b0: 2020 2020 2020 2020 2020 2020 2020 6569                ei
-0000e4c0: 6e73 756d 5f6f 626a 5f6c 6973 745b 695d  nsum_obj_list[i]
-0000e4d0: 203d 2073 702e 434f 4f2e 6672 6f6d 5f6e   = sp.COO.from_n
-0000e4e0: 756d 7079 286f 626a 290d 0a20 2020 2069  umpy(obj)..    i
-0000e4f0: 6620 7468 6973 5f74 7970 6520 3d3d 2064  f this_type == d
-0000e500: 656e 7365 203a 0d0a 2020 2020 2020 2020  ense :..        
-0000e510: 666f 7220 692c 206f 626a 2069 6e20 656e  for i, obj in en
-0000e520: 756d 6572 6174 6528 6569 6e73 756d 5f6f  umerate(einsum_o
-0000e530: 626a 5f6c 6973 7429 3a0d 0a20 2020 2020  bj_list):..     
-0000e540: 2020 2020 2020 2069 6620 7479 7065 286f         if type(o
-0000e550: 626a 2920 213d 206e 702e 6e64 6172 7261  bj) != np.ndarra
-0000e560: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-0000e570: 2020 2020 6569 6e73 756d 5f6f 626a 5f6c      einsum_obj_l
-0000e580: 6973 745b 695d 203d 2073 702e 434f 4f2e  ist[i] = sp.COO.
-0000e590: 746f 6465 6e73 6528 6f62 6a29 0d0a 2020  todense(obj)..  
-0000e5a0: 2020 0d0a 2020 2020 6966 2064 6562 7567    ..    if debug
-0000e5b0: 5f6d 6f64 6520 3a0d 0a20 2020 2020 2020  _mode :..       
-0000e5c0: 2070 7269 6e74 2822 203a 3a3a 3a3a 3a3a   print(" :::::::
-0000e5d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0000e5e0: 3a3a 3a3a 2074 6865 2061 6374 7561 6c20  :::: the actual 
-0000e5f0: 7375 6d20 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  sum ::::::::::::
-0000e600: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 2022  :::::::::::::: "
-0000e610: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-0000e620: 2865 696e 7375 6d5f 7374 7269 6e67 2c22  (einsum_string,"
-0000e630: 3c2d 2d20 6569 6e73 756d 2073 7472 696e  <-- einsum strin
-0000e640: 6722 290d 0a20 2020 2020 2020 2070 7269  g")..        pri
-0000e650: 6e74 2822 5b73 6861 7065 2c74 7970 655d  nt("[shape,type]
-0000e660: 3a22 290d 0a20 2020 2020 2020 2066 6f72  :")..        for
-0000e670: 206f 626a 2069 6e20 6569 6e73 756d 5f6f   obj in einsum_o
-0000e680: 626a 5f6c 6973 743a 0d0a 2020 2020 2020  bj_list:..      
-0000e690: 2020 2020 2020 7072 696e 7428 2220 222c        print(" ",
-0000e6a0: 5b6f 626a 2e73 6861 7065 2c74 7970 6528  [obj.shape,type(
-0000e6b0: 6f62 6a29 5d29 0d0a 0d0a 2020 2020 2020  obj)])....      
-0000e6c0: 2020 2020 2020 0d0a 2020 2020 7265 7420        ..    ret 
-0000e6d0: 3d20 6f65 2e63 6f6e 7472 6163 7428 2a74  = oe.contract(*t
-0000e6e0: 7570 6c65 285b 6569 6e73 756d 5f73 7472  uple([einsum_str
-0000e6f0: 696e 675d 2b65 696e 7375 6d5f 6f62 6a5f  ing]+einsum_obj_
-0000e700: 6c69 7374 2929 0d0a 0d0a 2020 2020 6966  list))....    if
-0000e710: 2068 6173 5f6f 7574 7075 7420 3a0d 0a20   has_output :.. 
-0000e720: 2020 2020 2020 2072 6574 7572 6e20 7468         return th
-0000e730: 6973 5f74 7970 6528 7265 742c 7374 6174  is_type(ret,stat
-0000e740: 6973 7469 633d 6669 6e61 6c5f 7374 6174  istic=final_stat
-0000e750: 7329 2e66 6f72 6365 5f65 6e63 6f64 6572  s).force_encoder
-0000e760: 2874 6869 735f 656e 636f 6465 7229 2e66  (this_encoder).f
-0000e770: 6f72 6365 5f66 6f72 6d61 7428 7468 6973  orce_format(this
-0000e780: 5f66 6f72 6d61 7429 0d0a 2020 2020 656c  _format)..    el
-0000e790: 7365 3a0d 0a20 2020 2020 2020 2069 6620  se:..        if 
-0000e7a0: 7468 6973 5f74 7970 6520 3d3d 2073 7061  this_type == spa
-0000e7b0: 7273 6520 3a0d 0a20 2020 2020 2020 2020  rse :..         
-0000e7c0: 2020 2069 6620 7479 7065 2872 6574 2e64     if type(ret.d
-0000e7d0: 6174 6129 3d3d 6d65 6d6f 7279 7669 6577  ata)==memoryview
-0000e7e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000e7f0: 2020 2072 6574 7572 6e20 7265 740d 0a20     return ret.. 
-0000e800: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000e810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e820: 2020 7265 7475 726e 2072 6574 2e64 6174    return ret.dat
-0000e830: 615b 305d 0d0a 2020 2020 2020 2020 656c  a[0]..        el
-0000e840: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0000e850: 2072 6574 7572 6e20 6e70 2e61 7272 6179   return np.array
-0000e860: 2872 6574 292e 666c 6174 7465 6e28 295b  (ret).flatten()[
-0000e870: 305d 0d0a 0d0a 2323 2323 2323 2323 2323  0]....##########
-0000e880: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e890: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e8a0: 2323 2323 2323 2323 2323 0d0a 2323 2020  ##########..##  
-0000e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e8c0: 2020 2052 6573 6861 7065 2020 2020 2020     Reshape      
-0000e8d0: 2020 2020 2020 2020 2020 2020 2020 2323                ##
-0000e8e0: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
-0000e8f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e900: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e910: 2323 2323 2323 0d0a 0d0a 6465 6620 6a6f  ######....def jo
-0000e920: 696e 5f6c 6567 7328 496e 704f 626a 2c73  in_legs(InpObj,s
-0000e930: 7472 696e 675f 696e 702c 6d61 6b65 5f66  tring_inp,make_f
-0000e940: 6f72 6d61 743d 2773 7461 6e64 6172 6427  ormat='standard'
-0000e950: 2c69 6e74 6572 6d65 6469 6174 655f 7374  ,intermediate_st
-0000e960: 6174 3d28 2d31 2c31 292c 7361 7665 5f6d  at=(-1,1),save_m
-0000e970: 656d 6f72 793d 4661 6c73 6529 3a0d 0a0d  emory=False):...
-0000e980: 0a20 2020 2070 726f 6365 7373 5f6e 616d  .    process_nam
-0000e990: 6520 3d20 226a 6f69 6e5f 6c65 6773 220d  e = "join_legs".
-0000e9a0: 0a20 2020 2070 726f 6365 7373 5f6c 656e  .    process_len
-0000e9b0: 6774 6820 3d20 360d 0a20 2020 2070 726f  gth = 6..    pro
-0000e9c0: 6365 7373 5f63 6f6c 6f72 3d22 6772 6565  cess_color="gree
-0000e9d0: 6e22 0d0a 2020 2020 7374 6570 203d 2031  n"..    step = 1
-0000e9e0: 0d0a 2020 2020 7330 3020 3d20 7469 6d65  ..    s00 = time
-0000e9f0: 2e74 696d 6528 290d 0a20 2020 2070 7269  .time()..    pri
-0000ea00: 6e74 2829 2023 203c 3c20 446f 6e27 7420  nt() # << Don't 
-0000ea10: 7265 6d6f 7665 2074 6869 732e 2054 6869  remove this. Thi
-0000ea20: 7320 6973 2066 6f72 2074 6865 2073 686f  s is for the sho
-0000ea30: 775f 7072 6f67 7265 7373 210d 0a0d 0a20  w_progress!.... 
-0000ea40: 2020 2073 7472 696e 675f 696e 7020 3d20     string_inp = 
-0000ea50: 6465 6e75 6d65 7261 7465 2873 7472 696e  denumerate(strin
-0000ea60: 675f 696e 7029 0d0a 0d0a 2020 2020 696e  g_inp)....    in
-0000ea70: 7465 726d 6564 6961 7465 5f73 7461 7420  termediate_stat 
-0000ea80: 3d20 6d61 6b65 5f74 7570 6c65 2869 6e74  = make_tuple(int
-0000ea90: 6572 6d65 6469 6174 655f 7374 6174 290d  ermediate_stat).
-0000eaa0: 0a20 2020 200d 0a20 2020 2073 7465 7020  .    ..    step 
-0000eab0: 3d20 7368 6f77 5f70 726f 6772 6573 7328  = show_progress(
-0000eac0: 7374 6570 2c70 726f 6365 7373 5f6c 656e  step,process_len
-0000ead0: 6774 682c 7072 6f63 6573 735f 6e61 6d65  gth,process_name
-0000eae0: 2b22 2022 2b22 3c22 2b63 7572 7265 6e74  +" "+"<"+current
-0000eaf0: 5f6d 656d 6f72 795f 6469 7370 6c61 7928  _memory_display(
-0000eb00: 292b 223e 222c 636f 6c6f 723d 7072 6f63  )+">",color=proc
-0000eb10: 6573 735f 636f 6c6f 722c 7469 6d65 3d74  ess_color,time=t
-0000eb20: 696d 652e 7469 6d65 2829 2d73 3030 290d  ime.time()-s00).
-0000eb30: 0a20 2020 2023 2041 6c77 6179 7320 6f75  .    # Always ou
-0000eb40: 7470 7574 2074 6865 2070 6172 6974 792d  tput the parity-
-0000eb50: 7072 6573 6572 7669 6e67 2065 6e63 6f64  preserving encod
-0000eb60: 6572 0d0a 2020 2020 233d 3d3d 3d3d 3d3d  er..    #=======
+0000e310: 0d0a 0d0a 2020 2020 6966 2074 6869 735f  ....    if this_
+0000e320: 7479 7065 3d3d 7370 6172 7365 203a 0d0a  type==sparse :..
+0000e330: 2020 2020 2020 2020 6569 6e73 756d 5f6f          einsum_o
+0000e340: 626a 5f6c 6973 7420 2b3d 2076 6572 7465  bj_list += verte
+0000e350: 785f 6f62 6a5f 6c69 7374 0d0a 2020 2020  x_obj_list..    
+0000e360: 2020 2020 6569 6e73 756d 5f73 7472 696e      einsum_strin
+0000e370: 6720 3d20 6569 6e73 756d 5f73 7472 696e  g = einsum_strin
+0000e380: 675f 7265 706c 6163 6564 0d0a 2020 2020  g_replaced..    
+0000e390: 0d0a 2020 2020 6966 2068 6173 5f6f 7574  ..    if has_out
+0000e3a0: 7075 7420 3a0d 0a20 2020 2020 2020 2065  put :..        e
+0000e3b0: 696e 7375 6d5f 7374 7269 6e67 202b 3d20  insum_string += 
+0000e3c0: 222d 3e22 2b6f 7574 7075 745f 7374 7269  "->"+output_stri
+0000e3d0: 6e67 0d0a 0d0a 2020 2020 2320 636f 6e76  ng....    # conv
+0000e3e0: 6572 7420 616c 6c20 6f62 6a65 6374 2074  ert all object t
+0000e3f0: 6f20 7468 6973 5f74 7970 650d 0a20 2020  o this_type..   
+0000e400: 2069 6620 7468 6973 5f74 7970 6520 3d3d   if this_type ==
+0000e410: 2073 7061 7273 6520 3a0d 0a20 2020 2020   sparse :..     
+0000e420: 2020 2066 6f72 2069 2c20 6f62 6a20 696e     for i, obj in
+0000e430: 2065 6e75 6d65 7261 7465 2865 696e 7375   enumerate(einsu
+0000e440: 6d5f 6f62 6a5f 6c69 7374 293a 0d0a 2020  m_obj_list):..  
+0000e450: 2020 2020 2020 2020 2020 6966 2074 7970            if typ
+0000e460: 6528 6f62 6a29 203d 3d20 6e70 2e6e 6461  e(obj) == np.nda
+0000e470: 7272 6179 3a0d 0a20 2020 2020 2020 2020  rray:..         
+0000e480: 2020 2020 2020 2065 696e 7375 6d5f 6f62         einsum_ob
+0000e490: 6a5f 6c69 7374 5b69 5d20 3d20 7370 2e43  j_list[i] = sp.C
+0000e4a0: 4f4f 2e66 726f 6d5f 6e75 6d70 7928 6f62  OO.from_numpy(ob
+0000e4b0: 6a29 0d0a 2020 2020 6966 2074 6869 735f  j)..    if this_
+0000e4c0: 7479 7065 203d 3d20 6465 6e73 6520 3a0d  type == dense :.
+0000e4d0: 0a20 2020 2020 2020 2066 6f72 2069 2c20  .        for i, 
+0000e4e0: 6f62 6a20 696e 2065 6e75 6d65 7261 7465  obj in enumerate
+0000e4f0: 2865 696e 7375 6d5f 6f62 6a5f 6c69 7374  (einsum_obj_list
+0000e500: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0000e510: 6966 2074 7970 6528 6f62 6a29 2021 3d20  if type(obj) != 
+0000e520: 6e70 2e6e 6461 7272 6179 3a0d 0a20 2020  np.ndarray:..   
+0000e530: 2020 2020 2020 2020 2020 2020 2065 696e               ein
+0000e540: 7375 6d5f 6f62 6a5f 6c69 7374 5b69 5d20  sum_obj_list[i] 
+0000e550: 3d20 7370 2e43 4f4f 2e74 6f64 656e 7365  = sp.COO.todense
+0000e560: 286f 626a 290d 0a20 2020 200d 0a20 2020  (obj)..    ..   
+0000e570: 2069 6620 6465 6275 675f 6d6f 6465 203a   if debug_mode :
+0000e580: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+0000e590: 2220 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  " ::::::::::::::
+0000e5a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a20 7468  ::::::::::::: th
+0000e5b0: 6520 6163 7475 616c 2073 756d 203a 3a3a  e actual sum :::
+0000e5c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0000e5d0: 3a3a 3a3a 3a3a 3a20 2229 0d0a 2020 2020  ::::::: ")..    
+0000e5e0: 2020 2020 7072 696e 7428 6569 6e73 756d      print(einsum
+0000e5f0: 5f73 7472 696e 672c 223c 2d2d 2065 696e  _string,"<-- ein
+0000e600: 7375 6d20 7374 7269 6e67 2229 0d0a 2020  sum string")..  
+0000e610: 2020 2020 2020 7072 696e 7428 225b 7368        print("[sh
+0000e620: 6170 652c 7479 7065 5d3a 2229 0d0a 2020  ape,type]:")..  
+0000e630: 2020 2020 2020 666f 7220 6f62 6a20 696e        for obj in
+0000e640: 2065 696e 7375 6d5f 6f62 6a5f 6c69 7374   einsum_obj_list
+0000e650: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+0000e660: 7269 6e74 2822 2022 2c5b 6f62 6a2e 7368  rint(" ",[obj.sh
+0000e670: 6170 652c 7479 7065 286f 626a 295d 290d  ape,type(obj)]).
+0000e680: 0a0d 0a20 2020 2020 2020 2020 2020 200d  ...            .
+0000e690: 0a20 2020 2072 6574 203d 206f 652e 636f  .    ret = oe.co
+0000e6a0: 6e74 7261 6374 282a 7475 706c 6528 5b65  ntract(*tuple([e
+0000e6b0: 696e 7375 6d5f 7374 7269 6e67 5d2b 6569  insum_string]+ei
+0000e6c0: 6e73 756d 5f6f 626a 5f6c 6973 7429 290d  nsum_obj_list)).
+0000e6d0: 0a0d 0a20 2020 2069 6620 6861 735f 6f75  ...    if has_ou
+0000e6e0: 7470 7574 203a 0d0a 2020 2020 2020 2020  tput :..        
+0000e6f0: 7265 7475 726e 2074 6869 735f 7479 7065  return this_type
+0000e700: 2872 6574 2c73 7461 7469 7374 6963 3d66  (ret,statistic=f
+0000e710: 696e 616c 5f73 7461 7473 292e 666f 7263  inal_stats).forc
+0000e720: 655f 656e 636f 6465 7228 7468 6973 5f65  e_encoder(this_e
+0000e730: 6e63 6f64 6572 292e 666f 7263 655f 666f  ncoder).force_fo
+0000e740: 726d 6174 2874 6869 735f 666f 726d 6174  rmat(this_format
+0000e750: 290d 0a20 2020 2065 6c73 653a 0d0a 2020  )..    else:..  
+0000e760: 2020 2020 2020 6966 2074 6869 735f 7479        if this_ty
+0000e770: 7065 203d 3d20 7370 6172 7365 203a 0d0a  pe == sparse :..
+0000e780: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+0000e790: 7970 6528 7265 742e 6461 7461 293d 3d6d  ype(ret.data)==m
+0000e7a0: 656d 6f72 7976 6965 773a 0d0a 2020 2020  emoryview:..    
+0000e7b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000e7c0: 726e 2072 6574 0d0a 2020 2020 2020 2020  rn ret..        
+0000e7d0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0000e7e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000e7f0: 6e20 7265 742e 6461 7461 5b30 5d0d 0a20  n ret.data[0].. 
+0000e800: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0000e810: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000e820: 206e 702e 6172 7261 7928 7265 7429 2e66   np.array(ret).f
+0000e830: 6c61 7474 656e 2829 5b30 5d0d 0a0d 0a23  latten()[0]....#
+0000e840: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000e850: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000e860: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000e870: 2323 230d 0a23 2320 2020 2020 2020 2020  ###..##         
+0000e880: 2020 2020 2020 2020 2020 2020 5265 7368              Resh
+0000e890: 6170 6520 2020 2020 2020 2020 2020 2020  ape             
+0000e8a0: 2020 2020 2020 2023 230d 0a23 2323 2323         ##..#####
+0000e8b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000e8c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000e8d0: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
+0000e8e0: 0a0d 0a64 6566 206a 6f69 6e5f 6c65 6773  ...def join_legs
+0000e8f0: 2849 6e70 4f62 6a2c 7374 7269 6e67 5f69  (InpObj,string_i
+0000e900: 6e70 2c6d 616b 655f 666f 726d 6174 3d27  np,make_format='
+0000e910: 7374 616e 6461 7264 272c 696e 7465 726d  standard',interm
+0000e920: 6564 6961 7465 5f73 7461 743d 282d 312c  ediate_stat=(-1,
+0000e930: 3129 2c73 6176 655f 6d65 6d6f 7279 3d46  1),save_memory=F
+0000e940: 616c 7365 293a 0d0a 0d0a 2020 2020 7072  alse):....    pr
+0000e950: 6f63 6573 735f 6e61 6d65 203d 2022 6a6f  ocess_name = "jo
+0000e960: 696e 5f6c 6567 7322 0d0a 2020 2020 7072  in_legs"..    pr
+0000e970: 6f63 6573 735f 6c65 6e67 7468 203d 2036  ocess_length = 6
+0000e980: 0d0a 2020 2020 7072 6f63 6573 735f 636f  ..    process_co
+0000e990: 6c6f 723d 2267 7265 656e 220d 0a20 2020  lor="green"..   
+0000e9a0: 2073 7465 7020 3d20 310d 0a20 2020 2073   step = 1..    s
+0000e9b0: 3030 203d 2074 696d 652e 7469 6d65 2829  00 = time.time()
+0000e9c0: 0d0a 2020 2020 7072 6f67 7265 7373 5f73  ..    progress_s
+0000e9d0: 7061 6365 2829 2023 203c 3c20 446f 6e27  pace() # << Don'
+0000e9e0: 7420 7265 6d6f 7665 2074 6869 732e 2054  t remove this. T
+0000e9f0: 6869 7320 6973 2066 6f72 2074 6865 2073  his is for the s
+0000ea00: 686f 775f 7072 6f67 7265 7373 210d 0a0d  how_progress!...
+0000ea10: 0a20 2020 2073 7472 696e 675f 696e 7020  .    string_inp 
+0000ea20: 3d20 6465 6e75 6d65 7261 7465 2873 7472  = denumerate(str
+0000ea30: 696e 675f 696e 7029 0d0a 0d0a 2020 2020  ing_inp)....    
+0000ea40: 696e 7465 726d 6564 6961 7465 5f73 7461  intermediate_sta
+0000ea50: 7420 3d20 6d61 6b65 5f74 7570 6c65 2869  t = make_tuple(i
+0000ea60: 6e74 6572 6d65 6469 6174 655f 7374 6174  ntermediate_stat
+0000ea70: 290d 0a20 2020 200d 0a20 2020 2073 7465  )..    ..    ste
+0000ea80: 7020 3d20 7368 6f77 5f70 726f 6772 6573  p = show_progres
+0000ea90: 7328 7374 6570 2c70 726f 6365 7373 5f6c  s(step,process_l
+0000eaa0: 656e 6774 682c 7072 6f63 6573 735f 6e61  ength,process_na
+0000eab0: 6d65 2b22 2022 2b22 3c22 2b63 7572 7265  me+" "+"<"+curre
+0000eac0: 6e74 5f6d 656d 6f72 795f 6469 7370 6c61  nt_memory_displa
+0000ead0: 7928 292b 223e 222c 636f 6c6f 723d 7072  y()+">",color=pr
+0000eae0: 6f63 6573 735f 636f 6c6f 722c 7469 6d65  ocess_color,time
+0000eaf0: 3d74 696d 652e 7469 6d65 2829 2d73 3030  =time.time()-s00
+0000eb00: 290d 0a20 2020 2023 2041 6c77 6179 7320  )..    # Always 
+0000eb10: 6f75 7470 7574 2074 6865 2070 6172 6974  output the parit
+0000eb20: 792d 7072 6573 6572 7669 6e67 2065 6e63  y-preserving enc
+0000eb30: 6f64 6572 0d0a 2020 2020 233d 3d3d 3d3d  oder..    #=====
+0000eb40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000eb50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000eb60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0000eb70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000eb80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000eb90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000eba0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000ebb0: 3d3d 3d3d 3d3d 3d3d 230d 0a20 2020 2023  ========#..    #
-0000ebc0: 2020 2053 7465 7020 303a 2050 7265 636f     Step 0: Preco
-0000ebd0: 6e64 6974 696f 6e69 6e67 2074 6865 2069  nditioning the i
-0000ebe0: 6e69 7469 616c 204f 626a 6563 7420 746f  nitial Object to
-0000ebf0: 2073 7461 6e64 6172 6420 2620 6361 6e6f   standard & cano
-0000ec00: 6e69 6361 6c20 2020 2020 2020 2020 2023  nical          #
-0000ec10: 0d0a 2020 2020 233d 3d3d 3d3d 3d3d 3d3d  ..    #=========
+0000eb80: 3d3d 3d3d 3d3d 3d3d 3d3d 230d 0a20 2020  ==========#..   
+0000eb90: 2023 2020 2053 7465 7020 303a 2050 7265   #   Step 0: Pre
+0000eba0: 636f 6e64 6974 696f 6e69 6e67 2074 6865  conditioning the
+0000ebb0: 2069 6e69 7469 616c 204f 626a 6563 7420   initial Object 
+0000ebc0: 746f 2073 7461 6e64 6172 6420 2620 6361  to standard & ca
+0000ebd0: 6e6f 6e69 6361 6c20 2020 2020 2020 2020  nonical         
+0000ebe0: 2023 0d0a 2020 2020 233d 3d3d 3d3d 3d3d   #..    #=======
+0000ebf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ec00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ec10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0000ec20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000ec30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000ec40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000ec50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000ec60: 3d3d 3d3d 3d3d 230d 0a20 2020 200d 0a20  ======#..    .. 
-0000ec70: 2020 204f 626a 203d 2049 6e70 4f62 6a2e     Obj = InpObj.
-0000ec80: 636f 7079 2829 0d0a 2020 2020 7468 6973  copy()..    this
-0000ec90: 5f74 7970 6520 3d20 7479 7065 284f 626a  _type = type(Obj
-0000eca0: 290d 0a20 2020 2074 6869 735f 666f 726d  )..    this_form
-0000ecb0: 6174 203d 204f 626a 2e66 6f72 6d61 740d  at = Obj.format.
-0000ecc0: 0a20 2020 2074 6869 735f 656e 636f 6465  .    this_encode
-0000ecd0: 7220 3d20 4f62 6a2e 656e 636f 6465 720d  r = Obj.encoder.
-0000ece0: 0a20 2020 2058 4f62 6a5f 7374 6174 7320  .    XObj_stats 
-0000ecf0: 3d20 4f62 6a2e 7374 6174 6973 7469 630d  = Obj.statistic.
-0000ed00: 0a20 2020 2058 4f62 6a5f 7368 6170 6520  .    XObj_shape 
-0000ed10: 3d20 4f62 6a2e 7368 6170 650d 0a0d 0a20  = Obj.shape.... 
-0000ed20: 2020 2069 6620 7361 7665 5f6d 656d 6f72     if save_memor
-0000ed30: 7920 3a0d 0a20 2020 2020 2020 2064 656c  y :..        del
-0000ed40: 2049 6e70 4f62 6a2e 6461 7461 0d0a 2020   InpObj.data..  
-0000ed50: 2020 2020 2020 6465 6c20 496e 704f 626a        del InpObj
-0000ed60: 0d0a 2020 2020 2020 2020 6763 2e63 6f6c  ..        gc.col
-0000ed70: 6c65 6374 2829 0d0a 2020 2020 2020 2020  lect()..        
-0000ed80: 0d0a 2020 2020 2369 6620 7468 6973 5f74  ..    #if this_t
-0000ed90: 7970 6520 2020 3d3d 2073 7061 7273 653a  ype   == sparse:
-0000eda0: 0d0a 2020 2020 2320 2020 204f 626a 203d  ..    #    Obj =
-0000edb0: 2064 656e 7365 284f 626a 290d 0a20 2020   dense(Obj)..   
-0000edc0: 2069 6620 7468 6973 5f66 6f72 6d61 7420   if this_format 
-0000edd0: 3d3d 2027 6d61 7472 6978 273a 0d0a 2020  == 'matrix':..  
-0000ede0: 2020 2020 2020 2366 6f72 6365 2063 6f6e        #force con
-0000edf0: 7665 7274 2074 6f20 7374 616e 6461 7264  vert to standard
-0000ee00: 0d0a 2020 2020 2020 2020 4f62 6a20 3d20  ..        Obj = 
-0000ee10: 4f62 6a2e 7377 6974 6368 5f66 6f72 6d61  Obj.switch_forma
-0000ee20: 7428 7361 7665 5f6d 656d 6f72 793d 5472  t(save_memory=Tr
-0000ee30: 7565 290d 0a20 2020 2069 6620 7468 6973  ue)..    if this
-0000ee40: 5f65 6e63 6f64 6572 203d 3d20 2770 6172  _encoder == 'par
-0000ee50: 6974 792d 7072 6573 6572 7669 6e67 273a  ity-preserving':
-0000ee60: 0d0a 2020 2020 2020 2020 2366 6f72 6365  ..        #force
-0000ee70: 2063 6f6e 7665 7274 2074 6f20 7374 616e   convert to stan
-0000ee80: 6461 7264 0d0a 2020 2020 2020 2020 4f62  dard..        Ob
-0000ee90: 6a20 3d20 4f62 6a2e 7377 6974 6368 5f65  j = Obj.switch_e
-0000eea0: 6e63 6f64 6572 2873 6176 655f 6d65 6d6f  ncoder(save_memo
-0000eeb0: 7279 3d54 7275 6529 0d0a 0d0a 2020 2020  ry=True)....    
-0000eec0: 7374 6570 203d 2073 686f 775f 7072 6f67  step = show_prog
-0000eed0: 7265 7373 2873 7465 702c 7072 6f63 6573  ress(step,proces
-0000eee0: 735f 6c65 6e67 7468 2c70 726f 6365 7373  s_length,process
-0000eef0: 5f6e 616d 652b 2220 222b 223c 222b 6375  _name+" "+"<"+cu
-0000ef00: 7272 656e 745f 6d65 6d6f 7279 5f64 6973  rrent_memory_dis
-0000ef10: 706c 6179 2829 2b22 3e22 2c63 6f6c 6f72  play()+">",color
-0000ef20: 3d70 726f 6365 7373 5f63 6f6c 6f72 2c74  =process_color,t
-0000ef30: 696d 653d 7469 6d65 2e74 696d 6528 292d  ime=time.time()-
-0000ef40: 7330 3029 0d0a 2020 2020 233d 3d3d 3d3d  s00)..    #=====
+0000ec30: 3d3d 3d3d 3d3d 3d3d 230d 0a20 2020 200d  ========#..    .
+0000ec40: 0a20 2020 204f 626a 203d 2049 6e70 4f62  .    Obj = InpOb
+0000ec50: 6a2e 636f 7079 2829 0d0a 2020 2020 7468  j.copy()..    th
+0000ec60: 6973 5f74 7970 6520 3d20 7479 7065 284f  is_type = type(O
+0000ec70: 626a 290d 0a20 2020 2074 6869 735f 666f  bj)..    this_fo
+0000ec80: 726d 6174 203d 204f 626a 2e66 6f72 6d61  rmat = Obj.forma
+0000ec90: 740d 0a20 2020 2074 6869 735f 656e 636f  t..    this_enco
+0000eca0: 6465 7220 3d20 4f62 6a2e 656e 636f 6465  der = Obj.encode
+0000ecb0: 720d 0a20 2020 2058 4f62 6a5f 7374 6174  r..    XObj_stat
+0000ecc0: 7320 3d20 4f62 6a2e 7374 6174 6973 7469  s = Obj.statisti
+0000ecd0: 630d 0a20 2020 2058 4f62 6a5f 7368 6170  c..    XObj_shap
+0000ece0: 6520 3d20 4f62 6a2e 7368 6170 650d 0a0d  e = Obj.shape...
+0000ecf0: 0a20 2020 2069 6620 7361 7665 5f6d 656d  .    if save_mem
+0000ed00: 6f72 7920 3a0d 0a20 2020 2020 2020 2064  ory :..        d
+0000ed10: 656c 2049 6e70 4f62 6a2e 6461 7461 0d0a  el InpObj.data..
+0000ed20: 2020 2020 2020 2020 6465 6c20 496e 704f          del InpO
+0000ed30: 626a 0d0a 2020 2020 2020 2020 6763 2e63  bj..        gc.c
+0000ed40: 6f6c 6c65 6374 2829 0d0a 2020 2020 2020  ollect()..      
+0000ed50: 2020 0d0a 2020 2020 2369 6620 7468 6973    ..    #if this
+0000ed60: 5f74 7970 6520 2020 3d3d 2073 7061 7273  _type   == spars
+0000ed70: 653a 0d0a 2020 2020 2320 2020 204f 626a  e:..    #    Obj
+0000ed80: 203d 2064 656e 7365 284f 626a 290d 0a20   = dense(Obj).. 
+0000ed90: 2020 2069 6620 7468 6973 5f66 6f72 6d61     if this_forma
+0000eda0: 7420 3d3d 2027 6d61 7472 6978 273a 0d0a  t == 'matrix':..
+0000edb0: 2020 2020 2020 2020 2366 6f72 6365 2063          #force c
+0000edc0: 6f6e 7665 7274 2074 6f20 7374 616e 6461  onvert to standa
+0000edd0: 7264 0d0a 2020 2020 2020 2020 4f62 6a20  rd..        Obj 
+0000ede0: 3d20 4f62 6a2e 7377 6974 6368 5f66 6f72  = Obj.switch_for
+0000edf0: 6d61 7428 7361 7665 5f6d 656d 6f72 793d  mat(save_memory=
+0000ee00: 5472 7565 290d 0a20 2020 2069 6620 7468  True)..    if th
+0000ee10: 6973 5f65 6e63 6f64 6572 203d 3d20 2770  is_encoder == 'p
+0000ee20: 6172 6974 792d 7072 6573 6572 7669 6e67  arity-preserving
+0000ee30: 273a 0d0a 2020 2020 2020 2020 2366 6f72  ':..        #for
+0000ee40: 6365 2063 6f6e 7665 7274 2074 6f20 7374  ce convert to st
+0000ee50: 616e 6461 7264 0d0a 2020 2020 2020 2020  andard..        
+0000ee60: 4f62 6a20 3d20 4f62 6a2e 7377 6974 6368  Obj = Obj.switch
+0000ee70: 5f65 6e63 6f64 6572 2873 6176 655f 6d65  _encoder(save_me
+0000ee80: 6d6f 7279 3d54 7275 6529 0d0a 0d0a 2020  mory=True)....  
+0000ee90: 2020 7374 6570 203d 2073 686f 775f 7072    step = show_pr
+0000eea0: 6f67 7265 7373 2873 7465 702c 7072 6f63  ogress(step,proc
+0000eeb0: 6573 735f 6c65 6e67 7468 2c70 726f 6365  ess_length,proce
+0000eec0: 7373 5f6e 616d 652b 2220 222b 223c 222b  ss_name+" "+"<"+
+0000eed0: 6375 7272 656e 745f 6d65 6d6f 7279 5f64  current_memory_d
+0000eee0: 6973 706c 6179 2829 2b22 3e22 2c63 6f6c  isplay()+">",col
+0000eef0: 6f72 3d70 726f 6365 7373 5f63 6f6c 6f72  or=process_color
+0000ef00: 2c74 696d 653d 7469 6d65 2e74 696d 6528  ,time=time.time(
+0000ef10: 292d 7330 3029 0d0a 2020 2020 233d 3d3d  )-s00)..    #===
+0000ef20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ef30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ef40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0000ef50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000ef60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000ef70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000ef80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000ef90: 3d3d 3d3d 3d3d 3d3d 3d3d 230d 0a20 2020  ==========#..   
-0000efa0: 2023 2020 2053 7465 7020 313a 204d 6f76   #   Step 1: Mov
-0000efb0: 6520 626f 736f 6e69 6320 696e 6469 6365  e bosonic indice
-0000efc0: 7320 746f 2074 6865 206c 6566 7420 6f66  s to the left of
-0000efd0: 2065 6163 6820 6772 6f75 7020 2020 2020   each group     
-0000efe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eff0: 2023 0d0a 2020 2020 233d 3d3d 3d3d 3d3d   #..    #=======
+0000ef60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 230d 0a20  ============#.. 
+0000ef70: 2020 2023 2020 2053 7465 7020 313a 204d     #   Step 1: M
+0000ef80: 6f76 6520 626f 736f 6e69 6320 696e 6469  ove bosonic indi
+0000ef90: 6365 7320 746f 2074 6865 206c 6566 7420  ces to the left 
+0000efa0: 6f66 2065 6163 6820 6772 6f75 7020 2020  of each group   
+0000efb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efc0: 2020 2023 0d0a 2020 2020 233d 3d3d 3d3d     #..    #=====
+0000efd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000efe0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000eff0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0000f000: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f010: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f030: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f040: 3d3d 3d3d 3d3d 3d3d 230d 0a20 2020 200d  ========#..    .
-0000f050: 0a20 2020 2023 2067 6574 2074 6865 2067  .    # get the g
-0000f060: 726f 7570 696e 6720 696e 666f 2066 6972  rouping info fir
-0000f070: 7374 0d0a 2020 2020 6772 6f75 705f 696e  st..    group_in
-0000f080: 666f 2c20 736f 7274 6564 5f67 726f 7570  fo, sorted_group
-0000f090: 5f69 6e66 6f20 3d20 6765 745f 6772 6f75  _info = get_grou
-0000f0a0: 705f 696e 666f 2873 7472 696e 675f 696e  p_info(string_in
-0000f0b0: 702c 204f 626a 2e73 7461 7469 7374 6963  p, Obj.statistic
-0000f0c0: 2c20 4f62 6a2e 7368 6170 6529 0d0a 2020  , Obj.shape)..  
-0000f0d0: 2020 2367 726f 7570 5f69 6e66 6f20 636f    #group_info co
-0000f0e0: 6e74 6169 6e73 2074 6865 2069 6e64 6578  ntains the index
-0000f0f0: 5f73 7472 696e 672c 2073 7461 7469 7374  _string, statist
-0000f100: 6963 732c 2061 6e64 2073 6861 7065 206f  ics, and shape o
-0000f110: 6620 6561 6368 2067 726f 7570 0d0a 2020  f each group..  
-0000f120: 2020 2373 6f72 7465 645f 6772 6f75 705f    #sorted_group_
-0000f130: 696e 666f 2069 7320 7468 6520 7361 6d65  info is the same
-0000f140: 2c20 6275 7420 7769 7468 2062 6f73 6f6e  , but with boson
-0000f150: 6963 2069 6e64 6963 6573 2073 6f72 7465  ic indices sorte
-0000f160: 6420 746f 2074 6865 206c 6566 740d 0a20  d to the left.. 
-0000f170: 2020 200d 0a20 2020 206e 5f69 6e64 6963     ..    n_indic
-0000f180: 6573 203d 2073 756d 285b 206c 656e 2869  es = sum([ len(i
-0000f190: 6e64 6963 6573 2920 666f 7220 5b69 6e64  ndices) for [ind
-0000f1a0: 6963 6573 2c73 7461 7473 2c73 6861 7065  ices,stats,shape
-0000f1b0: 5d20 696e 2067 726f 7570 5f69 6e66 6f20  ] in group_info 
-0000f1c0: 5d29 0d0a 2020 2020 0d0a 2020 2020 6966  ])..    ..    if
-0000f1d0: 206e 5f69 6e64 6963 6573 2021 3d20 4f62   n_indices != Ob
-0000f1e0: 6a2e 6e64 696d 203a 0d0a 2020 2020 2020  j.ndim :..      
-0000f1f0: 2020 6572 726f 7228 2245 7272 6f72 5b6a    error("Error[j
-0000f200: 6f69 6e5f 6c65 6773 5d3a 2054 6865 206e  oin_legs]: The n
-0000f210: 756d 6265 7220 6f66 2069 6e64 6963 6573  umber of indices
-0000f220: 2069 7320 6e6f 7420 636f 6e73 6973 7465   is not consiste
-0000f230: 6e74 2077 6974 6820 7468 6520 6f62 6a65  nt with the obje
-0000f240: 6374 2773 2073 6861 7065 2e22 290d 0a20  ct's shape.").. 
-0000f250: 2020 200d 0a20 2020 2073 6967 6e5f 6661     ..    sign_fa
-0000f260: 6374 6f72 735f 6c69 7374 203d 2067 6574  ctors_list = get
-0000f270: 5f67 726f 7570 696e 675f 7369 676e 5f66  _grouping_sign_f
-0000f280: 6163 746f 7273 2873 6f72 7465 645f 6772  actors(sorted_gr
-0000f290: 6f75 705f 696e 666f 2c20 696e 7465 726d  oup_info, interm
-0000f2a0: 6564 6961 7465 5f73 7461 7429 0d0a 2020  ediate_stat)..  
-0000f2b0: 2020 0d0a 2020 2020 756e 736f 7274 6564    ..    unsorted
-0000f2c0: 5f73 7472 696e 6720 3d20 2727 2e6a 6f69  _string = ''.joi
-0000f2d0: 6e28 205b 2069 6e64 6963 6573 2066 6f72  n( [ indices for
-0000f2e0: 205b 696e 6469 6365 732c 2073 7461 7473   [indices, stats
-0000f2f0: 2c20 7368 6170 655d 2069 6e20 6772 6f75  , shape] in grou
-0000f300: 705f 696e 666f 205d 2029 0d0a 2020 2020  p_info ] )..    
-0000f310: 736f 7274 6564 5f73 7472 696e 6720 3d20  sorted_string = 
-0000f320: 2727 2e6a 6f69 6e28 205b 2069 6e64 6963  ''.join( [ indic
-0000f330: 6573 2066 6f72 205b 696e 6469 6365 732c  es for [indices,
-0000f340: 2073 7461 7473 2c20 7368 6170 655d 2069   stats, shape] i
-0000f350: 6e20 736f 7274 6564 5f67 726f 7570 5f69  n sorted_group_i
-0000f360: 6e66 6f20 5d20 290d 0a20 2020 206e 7065  nfo ] )..    npe
-0000f370: 696e 7375 6d5f 7374 7269 6e67 203d 2075  insum_string = u
-0000f380: 6e73 6f72 7465 645f 7374 7269 6e67 2b73  nsorted_string+s
-0000f390: 6967 6e5f 6661 6374 6f72 735f 6c69 7374  ign_factors_list
-0000f3a0: 5b30 5d2b 222d 3e22 2b73 6f72 7465 645f  [0]+"->"+sorted_
-0000f3b0: 7374 7269 6e67 0d0a 2020 2020 6e70 6569  string..    npei
-0000f3c0: 6e73 756d 5f6f 626a 203d 205b 4f62 6a2e  nsum_obj = [Obj.
-0000f3d0: 6461 7461 5d20 2b20 7369 676e 5f66 6163  data] + sign_fac
-0000f3e0: 746f 7273 5f6c 6973 745b 315d 0d0a 2020  tors_list[1]..  
-0000f3f0: 2020 0d0a 2020 2020 736f 7274 6564 5f73    ..    sorted_s
-0000f400: 7461 7420 3d20 6d61 6b65 5f74 7570 6c65  tat = make_tuple
-0000f410: 2873 756d 280d 0a20 2020 2020 2020 2020  (sum(..         
-0000f420: 2020 205b 206d 616b 655f 6c69 7374 2873     [ make_list(s
-0000f430: 7461 7473 2920 666f 7220 5b69 6e64 6963  tats) for [indic
-0000f440: 6573 2c20 7374 6174 732c 2073 6861 7065  es, stats, shape
-0000f450: 5d20 696e 2073 6f72 7465 645f 6772 6f75  ] in sorted_grou
-0000f460: 705f 696e 666f 205d 202c 5b5d 0d0a 2020  p_info ] ,[]..  
-0000f470: 2020 2020 2020 2929 0d0a 2020 2020 0d0a        ))..    ..
-0000f480: 2020 2020 2373 6f72 7465 6420 7465 6e73      #sorted tens
-0000f490: 6f72 0d0a 2020 2020 4f62 6a2e 6461 7461  or..    Obj.data
-0000f4a0: 203d 206f 652e 636f 6e74 7261 6374 282a   = oe.contract(*
-0000f4b0: 6d61 6b65 5f74 7570 6c65 2820 5b6e 7065  make_tuple( [npe
-0000f4c0: 696e 7375 6d5f 7374 7269 6e67 5d20 2b20  insum_string] + 
-0000f4d0: 6e70 6569 6e73 756d 5f6f 626a 2029 290d  npeinsum_obj )).
-0000f4e0: 0a20 2020 204f 626a 2e73 7461 7469 7374  .    Obj.statist
-0000f4f0: 6963 203d 2073 6f72 7465 645f 7374 6174  ic = sorted_stat
-0000f500: 0d0a 2020 2020 0d0a 2020 2020 7374 6570  ..    ..    step
-0000f510: 203d 2073 686f 775f 7072 6f67 7265 7373   = show_progress
-0000f520: 2873 7465 702c 7072 6f63 6573 735f 6c65  (step,process_le
-0000f530: 6e67 7468 2c70 726f 6365 7373 5f6e 616d  ngth,process_nam
-0000f540: 652b 2220 222b 223c 222b 6375 7272 656e  e+" "+"<"+curren
-0000f550: 745f 6d65 6d6f 7279 5f64 6973 706c 6179  t_memory_display
-0000f560: 2829 2b22 3e22 2c63 6f6c 6f72 3d70 726f  ()+">",color=pro
-0000f570: 6365 7373 5f63 6f6c 6f72 2c74 696d 653d  cess_color,time=
-0000f580: 7469 6d65 2e74 696d 6528 292d 7330 3029  time.time()-s00)
-0000f590: 0d0a 2020 2020 0d0a 2020 2020 233d 3d3d  ..    ..    #===
+0000f010: 3d3d 3d3d 3d3d 3d3d 3d3d 230d 0a20 2020  ==========#..   
+0000f020: 200d 0a20 2020 2023 2067 6574 2074 6865   ..    # get the
+0000f030: 2067 726f 7570 696e 6720 696e 666f 2066   grouping info f
+0000f040: 6972 7374 0d0a 2020 2020 6772 6f75 705f  irst..    group_
+0000f050: 696e 666f 2c20 736f 7274 6564 5f67 726f  info, sorted_gro
+0000f060: 7570 5f69 6e66 6f20 3d20 6765 745f 6772  up_info = get_gr
+0000f070: 6f75 705f 696e 666f 2873 7472 696e 675f  oup_info(string_
+0000f080: 696e 702c 204f 626a 2e73 7461 7469 7374  inp, Obj.statist
+0000f090: 6963 2c20 4f62 6a2e 7368 6170 6529 0d0a  ic, Obj.shape)..
+0000f0a0: 2020 2020 2367 726f 7570 5f69 6e66 6f20      #group_info 
+0000f0b0: 636f 6e74 6169 6e73 2074 6865 2069 6e64  contains the ind
+0000f0c0: 6578 5f73 7472 696e 672c 2073 7461 7469  ex_string, stati
+0000f0d0: 7374 6963 732c 2061 6e64 2073 6861 7065  stics, and shape
+0000f0e0: 206f 6620 6561 6368 2067 726f 7570 0d0a   of each group..
+0000f0f0: 2020 2020 2373 6f72 7465 645f 6772 6f75      #sorted_grou
+0000f100: 705f 696e 666f 2069 7320 7468 6520 7361  p_info is the sa
+0000f110: 6d65 2c20 6275 7420 7769 7468 2062 6f73  me, but with bos
+0000f120: 6f6e 6963 2069 6e64 6963 6573 2073 6f72  onic indices sor
+0000f130: 7465 6420 746f 2074 6865 206c 6566 740d  ted to the left.
+0000f140: 0a20 2020 200d 0a20 2020 206e 5f69 6e64  .    ..    n_ind
+0000f150: 6963 6573 203d 2073 756d 285b 206c 656e  ices = sum([ len
+0000f160: 2869 6e64 6963 6573 2920 666f 7220 5b69  (indices) for [i
+0000f170: 6e64 6963 6573 2c73 7461 7473 2c73 6861  ndices,stats,sha
+0000f180: 7065 5d20 696e 2067 726f 7570 5f69 6e66  pe] in group_inf
+0000f190: 6f20 5d29 0d0a 2020 2020 0d0a 2020 2020  o ])..    ..    
+0000f1a0: 6966 206e 5f69 6e64 6963 6573 2021 3d20  if n_indices != 
+0000f1b0: 4f62 6a2e 6e64 696d 203a 0d0a 2020 2020  Obj.ndim :..    
+0000f1c0: 2020 2020 6572 726f 7228 2245 7272 6f72      error("Error
+0000f1d0: 5b6a 6f69 6e5f 6c65 6773 5d3a 2054 6865  [join_legs]: The
+0000f1e0: 206e 756d 6265 7220 6f66 2069 6e64 6963   number of indic
+0000f1f0: 6573 2069 7320 6e6f 7420 636f 6e73 6973  es is not consis
+0000f200: 7465 6e74 2077 6974 6820 7468 6520 6f62  tent with the ob
+0000f210: 6a65 6374 2773 2073 6861 7065 2e22 290d  ject's shape.").
+0000f220: 0a20 2020 200d 0a20 2020 2073 6967 6e5f  .    ..    sign_
+0000f230: 6661 6374 6f72 735f 6c69 7374 203d 2067  factors_list = g
+0000f240: 6574 5f67 726f 7570 696e 675f 7369 676e  et_grouping_sign
+0000f250: 5f66 6163 746f 7273 2873 6f72 7465 645f  _factors(sorted_
+0000f260: 6772 6f75 705f 696e 666f 2c20 696e 7465  group_info, inte
+0000f270: 726d 6564 6961 7465 5f73 7461 7429 0d0a  rmediate_stat)..
+0000f280: 2020 2020 0d0a 2020 2020 756e 736f 7274      ..    unsort
+0000f290: 6564 5f73 7472 696e 6720 3d20 2727 2e6a  ed_string = ''.j
+0000f2a0: 6f69 6e28 205b 2069 6e64 6963 6573 2066  oin( [ indices f
+0000f2b0: 6f72 205b 696e 6469 6365 732c 2073 7461  or [indices, sta
+0000f2c0: 7473 2c20 7368 6170 655d 2069 6e20 6772  ts, shape] in gr
+0000f2d0: 6f75 705f 696e 666f 205d 2029 0d0a 2020  oup_info ] )..  
+0000f2e0: 2020 736f 7274 6564 5f73 7472 696e 6720    sorted_string 
+0000f2f0: 3d20 2727 2e6a 6f69 6e28 205b 2069 6e64  = ''.join( [ ind
+0000f300: 6963 6573 2066 6f72 205b 696e 6469 6365  ices for [indice
+0000f310: 732c 2073 7461 7473 2c20 7368 6170 655d  s, stats, shape]
+0000f320: 2069 6e20 736f 7274 6564 5f67 726f 7570   in sorted_group
+0000f330: 5f69 6e66 6f20 5d20 290d 0a20 2020 206e  _info ] )..    n
+0000f340: 7065 696e 7375 6d5f 7374 7269 6e67 203d  peinsum_string =
+0000f350: 2075 6e73 6f72 7465 645f 7374 7269 6e67   unsorted_string
+0000f360: 2b73 6967 6e5f 6661 6374 6f72 735f 6c69  +sign_factors_li
+0000f370: 7374 5b30 5d2b 222d 3e22 2b73 6f72 7465  st[0]+"->"+sorte
+0000f380: 645f 7374 7269 6e67 0d0a 2020 2020 6e70  d_string..    np
+0000f390: 6569 6e73 756d 5f6f 626a 203d 205b 4f62  einsum_obj = [Ob
+0000f3a0: 6a2e 6461 7461 5d20 2b20 7369 676e 5f66  j.data] + sign_f
+0000f3b0: 6163 746f 7273 5f6c 6973 745b 315d 0d0a  actors_list[1]..
+0000f3c0: 2020 2020 0d0a 2020 2020 736f 7274 6564      ..    sorted
+0000f3d0: 5f73 7461 7420 3d20 6d61 6b65 5f74 7570  _stat = make_tup
+0000f3e0: 6c65 2873 756d 280d 0a20 2020 2020 2020  le(sum(..       
+0000f3f0: 2020 2020 205b 206d 616b 655f 6c69 7374       [ make_list
+0000f400: 2873 7461 7473 2920 666f 7220 5b69 6e64  (stats) for [ind
+0000f410: 6963 6573 2c20 7374 6174 732c 2073 6861  ices, stats, sha
+0000f420: 7065 5d20 696e 2073 6f72 7465 645f 6772  pe] in sorted_gr
+0000f430: 6f75 705f 696e 666f 205d 202c 5b5d 0d0a  oup_info ] ,[]..
+0000f440: 2020 2020 2020 2020 2929 0d0a 2020 2020          ))..    
+0000f450: 0d0a 2020 2020 2373 6f72 7465 6420 7465  ..    #sorted te
+0000f460: 6e73 6f72 0d0a 2020 2020 4f62 6a2e 6461  nsor..    Obj.da
+0000f470: 7461 203d 206f 652e 636f 6e74 7261 6374  ta = oe.contract
+0000f480: 282a 6d61 6b65 5f74 7570 6c65 2820 5b6e  (*make_tuple( [n
+0000f490: 7065 696e 7375 6d5f 7374 7269 6e67 5d20  peinsum_string] 
+0000f4a0: 2b20 6e70 6569 6e73 756d 5f6f 626a 2029  + npeinsum_obj )
+0000f4b0: 290d 0a20 2020 204f 626a 2e73 7461 7469  )..    Obj.stati
+0000f4c0: 7374 6963 203d 2073 6f72 7465 645f 7374  stic = sorted_st
+0000f4d0: 6174 0d0a 2020 2020 0d0a 2020 2020 7374  at..    ..    st
+0000f4e0: 6570 203d 2073 686f 775f 7072 6f67 7265  ep = show_progre
+0000f4f0: 7373 2873 7465 702c 7072 6f63 6573 735f  ss(step,process_
+0000f500: 6c65 6e67 7468 2c70 726f 6365 7373 5f6e  length,process_n
+0000f510: 616d 652b 2220 222b 223c 222b 6375 7272  ame+" "+"<"+curr
+0000f520: 656e 745f 6d65 6d6f 7279 5f64 6973 706c  ent_memory_displ
+0000f530: 6179 2829 2b22 3e22 2c63 6f6c 6f72 3d70  ay()+">",color=p
+0000f540: 726f 6365 7373 5f63 6f6c 6f72 2c74 696d  rocess_color,tim
+0000f550: 653d 7469 6d65 2e74 696d 6528 292d 7330  e=time.time()-s0
+0000f560: 3029 0d0a 2020 2020 0d0a 2020 2020 233d  0)..    ..    #=
+0000f570: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000f580: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000f590: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0000f5a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f5b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f5c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f5d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f5e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 230d 0a20  ============#.. 
-0000f5f0: 2020 2023 2020 2053 7465 7020 323a 204a     #   Step 2: J
-0000f600: 6f69 6e20 6665 726d 696f 6e69 6320 696e  oin fermionic in
-0000f610: 6469 6365 7320 7769 7468 206e 702e 7265  dices with np.re
-0000f620: 7368 6170 6520 2020 2020 2020 2020 2020  shape           
-0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f640: 2020 2023 0d0a 2020 2020 233d 3d3d 3d3d     #..    #=====
+0000f5b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 230d  ==============#.
+0000f5c0: 0a20 2020 2023 2020 2053 7465 7020 323a  .    #   Step 2:
+0000f5d0: 204a 6f69 6e20 6665 726d 696f 6e69 6320   Join fermionic 
+0000f5e0: 696e 6469 6365 7320 7769 7468 206e 702e  indices with np.
+0000f5f0: 7265 7368 6170 6520 2020 2020 2020 2020  reshape         
+0000f600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f610: 2020 2020 2023 0d0a 2020 2020 233d 3d3d       #..    #===
+0000f620: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000f630: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000f640: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0000f650: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f660: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f670: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f680: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f690: 3d3d 3d3d 3d3d 3d3d 3d3d 230d 0a20 2020  ==========#..   
-0000f6a0: 200d 0a20 2020 206e 6577 5f73 7461 7473   ..    new_stats
-0000f6b0: 2c20 6e65 775f 7368 6170 652c 2066 696e  , new_shape, fin
-0000f6c0: 616c 5f73 7461 7473 2c20 6669 6e61 6c5f  al_stats, final_
-0000f6d0: 7368 6170 6520 3d20 6765 745f 696e 7465  shape = get_inte
-0000f6e0: 726d 6564 6961 7465 5f69 6e66 6f28 736f  rmediate_info(so
-0000f6f0: 7274 6564 5f67 726f 7570 5f69 6e66 6f2c  rted_group_info,
-0000f700: 696e 7465 726d 6564 6961 7465 5f73 7461  intermediate_sta
-0000f710: 7429 0d0a 2020 2020 2369 6e74 6572 6d65  t)..    #interme
-0000f720: 6469 6174 655f 7465 6e73 6f72 0d0a 2020  diate_tensor..  
-0000f730: 2020 0d0a 2020 2020 4f62 6a2e 6461 7461    ..    Obj.data
-0000f740: 203d 206e 702e 7265 7368 6170 6528 4f62   = np.reshape(Ob
-0000f750: 6a2e 6461 7461 2c6e 6577 5f73 6861 7065  j.data,new_shape
-0000f760: 290d 0a20 2020 204f 626a 2e73 7461 7469  )..    Obj.stati
-0000f770: 7374 6963 203d 206e 6577 5f73 7461 7473  stic = new_stats
-0000f780: 0d0a 2020 2020 0d0a 2020 2020 7374 6570  ..    ..    step
-0000f790: 203d 2073 686f 775f 7072 6f67 7265 7373   = show_progress
-0000f7a0: 2873 7465 702c 7072 6f63 6573 735f 6c65  (step,process_le
-0000f7b0: 6e67 7468 2c70 726f 6365 7373 5f6e 616d  ngth,process_nam
-0000f7c0: 652b 2220 222b 223c 222b 6375 7272 656e  e+" "+"<"+curren
-0000f7d0: 745f 6d65 6d6f 7279 5f64 6973 706c 6179  t_memory_display
-0000f7e0: 2829 2b22 3e22 2c63 6f6c 6f72 3d70 726f  ()+">",color=pro
-0000f7f0: 6365 7373 5f63 6f6c 6f72 2c74 696d 653d  cess_color,time=
-0000f800: 7469 6d65 2e74 696d 6528 292d 7330 3029  time.time()-s00)
-0000f810: 0d0a 2020 2020 233d 3d3d 3d3d 3d3d 3d3d  ..    #=========
+0000f660: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 230d 0a20  ============#.. 
+0000f670: 2020 200d 0a20 2020 206e 6577 5f73 7461     ..    new_sta
+0000f680: 7473 2c20 6e65 775f 7368 6170 652c 2066  ts, new_shape, f
+0000f690: 696e 616c 5f73 7461 7473 2c20 6669 6e61  inal_stats, fina
+0000f6a0: 6c5f 7368 6170 6520 3d20 6765 745f 696e  l_shape = get_in
+0000f6b0: 7465 726d 6564 6961 7465 5f69 6e66 6f28  termediate_info(
+0000f6c0: 736f 7274 6564 5f67 726f 7570 5f69 6e66  sorted_group_inf
+0000f6d0: 6f2c 696e 7465 726d 6564 6961 7465 5f73  o,intermediate_s
+0000f6e0: 7461 7429 0d0a 2020 2020 2369 6e74 6572  tat)..    #inter
+0000f6f0: 6d65 6469 6174 655f 7465 6e73 6f72 0d0a  mediate_tensor..
+0000f700: 2020 2020 0d0a 2020 2020 4f62 6a2e 6461      ..    Obj.da
+0000f710: 7461 203d 206e 702e 7265 7368 6170 6528  ta = np.reshape(
+0000f720: 4f62 6a2e 6461 7461 2c6e 6577 5f73 6861  Obj.data,new_sha
+0000f730: 7065 290d 0a20 2020 204f 626a 2e73 7461  pe)..    Obj.sta
+0000f740: 7469 7374 6963 203d 206e 6577 5f73 7461  tistic = new_sta
+0000f750: 7473 0d0a 2020 2020 0d0a 2020 2020 7374  ts..    ..    st
+0000f760: 6570 203d 2073 686f 775f 7072 6f67 7265  ep = show_progre
+0000f770: 7373 2873 7465 702c 7072 6f63 6573 735f  ss(step,process_
+0000f780: 6c65 6e67 7468 2c70 726f 6365 7373 5f6e  length,process_n
+0000f790: 616d 652b 2220 222b 223c 222b 6375 7272  ame+" "+"<"+curr
+0000f7a0: 656e 745f 6d65 6d6f 7279 5f64 6973 706c  ent_memory_displ
+0000f7b0: 6179 2829 2b22 3e22 2c63 6f6c 6f72 3d70  ay()+">",color=p
+0000f7c0: 726f 6365 7373 5f63 6f6c 6f72 2c74 696d  rocess_color,tim
+0000f7d0: 653d 7469 6d65 2e74 696d 6528 292d 7330  e=time.time()-s0
+0000f7e0: 3029 0d0a 2020 2020 233d 3d3d 3d3d 3d3d  0)..    #=======
+0000f7f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000f800: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000f810: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0000f820: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f830: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f840: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f850: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f860: 3d3d 3d3d 3d3d 230d 0a20 2020 2023 2020  ======#..    #  
-0000f870: 2053 7465 7020 333a 2053 7769 7463 6820   Step 3: Switch 
-0000f880: 666f 726d 6174 2069 6620 6d61 6b65 5f66  format if make_f
-0000f890: 6f72 6d61 743d 276d 6174 7269 7827 2020  ormat='matrix'  
-0000f8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8b0: 2020 2020 2020 2020 2020 2020 2023 0d0a               #..
-0000f8c0: 2020 2020 233d 3d3d 3d3d 3d3d 3d3d 3d3d      #===========
+0000f830: 3d3d 3d3d 3d3d 3d3d 230d 0a20 2020 2023  ========#..    #
+0000f840: 2020 2053 7465 7020 333a 2053 7769 7463     Step 3: Switc
+0000f850: 6820 666f 726d 6174 2069 6620 6d61 6b65  h format if make
+0000f860: 5f66 6f72 6d61 743d 276d 6174 7269 7827  _format='matrix'
+0000f870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f880: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000f890: 0d0a 2020 2020 233d 3d3d 3d3d 3d3d 3d3d  ..    #=========
+0000f8a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000f8b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000f8c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0000f8d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f8e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f8f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f900: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000f910: 3d3d 3d3d 230d 0a20 2020 200d 0a20 2020  ====#..    ..   
-0000f920: 2069 6620 6d61 6b65 5f66 6f72 6d61 7420   if make_format 
-0000f930: 3d3d 2027 6d61 7472 6978 273a 0d0a 2020  == 'matrix':..  
-0000f940: 2020 2020 2020 4f62 6a20 3d20 4f62 6a2e        Obj = Obj.
-0000f950: 7377 6974 6368 5f66 6f72 6d61 7428 7361  switch_format(sa
-0000f960: 7665 5f6d 656d 6f72 793d 5472 7565 290d  ve_memory=True).
-0000f970: 0a20 2020 200d 0a20 2020 2073 7465 7020  .    ..    step 
-0000f980: 3d20 7368 6f77 5f70 726f 6772 6573 7328  = show_progress(
-0000f990: 7374 6570 2c70 726f 6365 7373 5f6c 656e  step,process_len
-0000f9a0: 6774 682c 7072 6f63 6573 735f 6e61 6d65  gth,process_name
-0000f9b0: 2b22 2022 2b22 3c22 2b63 7572 7265 6e74  +" "+"<"+current
-0000f9c0: 5f6d 656d 6f72 795f 6469 7370 6c61 7928  _memory_display(
-0000f9d0: 292b 223e 222c 636f 6c6f 723d 7072 6f63  )+">",color=proc
-0000f9e0: 6573 735f 636f 6c6f 722c 7469 6d65 3d74  ess_color,time=t
-0000f9f0: 696d 652e 7469 6d65 2829 2d73 3030 290d  ime.time()-s00).
-0000fa00: 0a20 2020 2023 3d3d 3d3d 3d3d 3d3d 3d3d  .    #==========
+0000f8e0: 3d3d 3d3d 3d3d 230d 0a20 2020 200d 0a20  ======#..    .. 
+0000f8f0: 2020 2069 6620 6d61 6b65 5f66 6f72 6d61     if make_forma
+0000f900: 7420 3d3d 2027 6d61 7472 6978 273a 0d0a  t == 'matrix':..
+0000f910: 2020 2020 2020 2020 4f62 6a20 3d20 4f62          Obj = Ob
+0000f920: 6a2e 7377 6974 6368 5f66 6f72 6d61 7428  j.switch_format(
+0000f930: 7361 7665 5f6d 656d 6f72 793d 5472 7565  save_memory=True
+0000f940: 290d 0a20 2020 200d 0a20 2020 2073 7465  )..    ..    ste
+0000f950: 7020 3d20 7368 6f77 5f70 726f 6772 6573  p = show_progres
+0000f960: 7328 7374 6570 2c70 726f 6365 7373 5f6c  s(step,process_l
+0000f970: 656e 6774 682c 7072 6f63 6573 735f 6e61  ength,process_na
+0000f980: 6d65 2b22 2022 2b22 3c22 2b63 7572 7265  me+" "+"<"+curre
+0000f990: 6e74 5f6d 656d 6f72 795f 6469 7370 6c61  nt_memory_displa
+0000f9a0: 7928 292b 223e 222c 636f 6c6f 723d 7072  y()+">",color=pr
+0000f9b0: 6f63 6573 735f 636f 6c6f 722c 7469 6d65  ocess_color,time
+0000f9c0: 3d74 696d 652e 7469 6d65 2829 2d73 3030  =time.time()-s00
+0000f9d0: 290d 0a20 2020 2023 3d3d 3d3d 3d3d 3d3d  )..    #========
+0000f9e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000f9f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000fa00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0000fa10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fa20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fa30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fa40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fa50: 3d3d 3d3d 3d23 0d0a 2020 2020 2320 2020  =====#..    #   
-0000fa60: 5374 6570 2034 3a20 5377 6974 6368 2065  Step 4: Switch e
-0000fa70: 6e63 6f64 6572 2020 2020 2020 2020 2020  ncoder          
-0000fa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000faa0: 2020 2020 2020 2020 2020 2020 230d 0a20              #.. 
-0000fab0: 2020 2023 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d     #============
+0000fa20: 3d3d 3d3d 3d3d 3d23 0d0a 2020 2020 2320  =======#..    # 
+0000fa30: 2020 5374 6570 2034 3a20 5377 6974 6368    Step 4: Switch
+0000fa40: 2065 6e63 6f64 6572 2020 2020 2020 2020   encoder        
+0000fa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa70: 2020 2020 2020 2020 2020 2020 2020 230d                #.
+0000fa80: 0a20 2020 2023 3d3d 3d3d 3d3d 3d3d 3d3d  .    #==========
+0000fa90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000faa0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000fab0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0000fac0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fad0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fae0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000faf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fb00: 3d3d 3d23 0d0a 0d0a 2020 2020 4f62 6a20  ===#....    Obj 
-0000fb10: 3d20 4f62 6a2e 7377 6974 6368 5f65 6e63  = Obj.switch_enc
-0000fb20: 6f64 6572 2873 6176 655f 6d65 6d6f 7279  oder(save_memory
-0000fb30: 3d54 7275 6529 0d0a 2020 2020 0d0a 2020  =True)..    ..  
-0000fb40: 2020 7374 6570 203d 2073 686f 775f 7072    step = show_pr
-0000fb50: 6f67 7265 7373 2873 7465 702c 7072 6f63  ogress(step,proc
-0000fb60: 6573 735f 6c65 6e67 7468 2c70 726f 6365  ess_length,proce
-0000fb70: 7373 5f6e 616d 652b 2220 222b 223c 222b  ss_name+" "+"<"+
-0000fb80: 6375 7272 656e 745f 6d65 6d6f 7279 5f64  current_memory_d
-0000fb90: 6973 706c 6179 2829 2b22 3e22 2c63 6f6c  isplay()+">",col
-0000fba0: 6f72 3d70 726f 6365 7373 5f63 6f6c 6f72  or=process_color
-0000fbb0: 2c74 696d 653d 7469 6d65 2e74 696d 6528  ,time=time.time(
-0000fbc0: 292d 7330 3029 0d0a 2020 2020 233d 3d3d  )-s00)..    #===
+0000fad0: 3d3d 3d3d 3d23 0d0a 0d0a 2020 2020 4f62  =====#....    Ob
+0000fae0: 6a20 3d20 4f62 6a2e 7377 6974 6368 5f65  j = Obj.switch_e
+0000faf0: 6e63 6f64 6572 2873 6176 655f 6d65 6d6f  ncoder(save_memo
+0000fb00: 7279 3d54 7275 6529 0d0a 2020 2020 0d0a  ry=True)..    ..
+0000fb10: 2020 2020 7374 6570 203d 2073 686f 775f      step = show_
+0000fb20: 7072 6f67 7265 7373 2873 7465 702c 7072  progress(step,pr
+0000fb30: 6f63 6573 735f 6c65 6e67 7468 2c70 726f  ocess_length,pro
+0000fb40: 6365 7373 5f6e 616d 652b 2220 222b 223c  cess_name+" "+"<
+0000fb50: 222b 6375 7272 656e 745f 6d65 6d6f 7279  "+current_memory
+0000fb60: 5f64 6973 706c 6179 2829 2b22 3e22 2c63  _display()+">",c
+0000fb70: 6f6c 6f72 3d70 726f 6365 7373 5f63 6f6c  olor=process_col
+0000fb80: 6f72 2c74 696d 653d 7469 6d65 2e74 696d  or,time=time.tim
+0000fb90: 6528 292d 7330 3029 0d0a 2020 2020 233d  e()-s00)..    #=
+0000fba0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000fbb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000fbc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0000fbd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fbe0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fbf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fc00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fc10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 230d 0a20  ============#.. 
-0000fc20: 2020 2023 2020 2053 7465 7020 353a 204d     #   Step 5: M
-0000fc30: 6572 6765 2062 6f73 6f6e 7320 616e 6420  erge bosons and 
-0000fc40: 6665 726d 696f 6e73 2020 2020 2020 2020  fermions        
-0000fc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc70: 2020 2023 0d0a 2020 2020 233d 3d3d 3d3d     #..    #=====
+0000fbe0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 230d  ==============#.
+0000fbf0: 0a20 2020 2023 2020 2053 7465 7020 353a  .    #   Step 5:
+0000fc00: 204d 6572 6765 2062 6f73 6f6e 7320 616e   Merge bosons an
+0000fc10: 6420 6665 726d 696f 6e73 2020 2020 2020  d fermions      
+0000fc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc40: 2020 2020 2023 0d0a 2020 2020 233d 3d3d       #..    #===
+0000fc50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000fc60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000fc70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0000fc80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fc90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fca0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fcb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fcc0: 3d3d 3d3d 3d3d 3d3d 3d3d 230d 0a20 2020  ==========#..   
-0000fcd0: 200d 0a20 2020 204f 626a 2e64 6174 6120   ..    Obj.data 
-0000fce0: 3d20 6e70 2e72 6573 6861 7065 284f 626a  = np.reshape(Obj
-0000fcf0: 2e64 6174 612c 6669 6e61 6c5f 7368 6170  .data,final_shap
-0000fd00: 6529 0d0a 2020 2020 4f62 6a2e 7374 6174  e)..    Obj.stat
-0000fd10: 6973 7469 6320 3d20 6669 6e61 6c5f 7374  istic = final_st
-0000fd20: 6174 730d 0a20 2020 200d 0a20 2020 2063  ats..    ..    c
-0000fd30: 6c65 6172 5f70 726f 6772 6573 7328 290d  lear_progress().
-0000fd40: 0a20 2020 2073 7973 2e73 7464 6f75 742e  .    sys.stdout.
-0000fd50: 7772 6974 6528 225c 3033 335b 4622 290d  write("\033[F").
-0000fd60: 0a0d 0a20 2020 2072 6574 7572 6e20 4f62  ...    return Ob
-0000fd70: 6a0d 0a20 2020 200d 0a64 6566 2073 706c  j..    ..def spl
-0000fd80: 6974 5f6c 6567 7328 496e 704f 626a 2c73  it_legs(InpObj,s
-0000fd90: 7472 696e 675f 696e 702c 6669 6e61 6c5f  tring_inp,final_
-0000fda0: 7374 6174 2c66 696e 616c 5f73 6861 7065  stat,final_shape
-0000fdb0: 2c69 6e74 6572 6d65 6469 6174 655f 7374  ,intermediate_st
-0000fdc0: 6174 3d28 2d31 2c31 292c 7361 7665 5f6d  at=(-1,1),save_m
-0000fdd0: 656d 6f72 793d 4661 6c73 6529 3a0d 0a0d  emory=False):...
-0000fde0: 0a20 2020 2070 726f 6365 7373 5f6e 616d  .    process_nam
-0000fdf0: 6520 3d20 2273 706c 6974 5f6c 6567 7322  e = "split_legs"
-0000fe00: 0d0a 2020 2020 7072 6f63 6573 735f 6c65  ..    process_le
-0000fe10: 6e67 7468 203d 2036 0d0a 2020 2020 7072  ngth = 6..    pr
-0000fe20: 6f63 6573 735f 636f 6c6f 723d 2267 7265  ocess_color="gre
-0000fe30: 656e 220d 0a20 2020 2073 7465 7020 3d20  en"..    step = 
-0000fe40: 310d 0a20 2020 2073 3030 203d 2074 696d  1..    s00 = tim
-0000fe50: 652e 7469 6d65 2829 0d0a 2020 2020 7072  e.time()..    pr
-0000fe60: 696e 7428 2920 2320 3c3c 2044 6f6e 2774  int() # << Don't
-0000fe70: 2072 656d 6f76 6520 7468 6973 2e20 5468   remove this. Th
-0000fe80: 6973 2069 7320 666f 7220 7468 6520 7368  is is for the sh
-0000fe90: 6f77 5f70 726f 6772 6573 7321 0d0a 0d0a  ow_progress!....
-0000fea0: 2020 2020 7374 7269 6e67 5f69 6e70 203d      string_inp =
-0000feb0: 2064 656e 756d 6572 6174 6528 7374 7269   denumerate(stri
-0000fec0: 6e67 5f69 6e70 290d 0a0d 0a20 2020 2069  ng_inp)....    i
-0000fed0: 6e74 6572 6d65 6469 6174 655f 7374 6174  ntermediate_stat
-0000fee0: 203d 206d 616b 655f 7475 706c 6528 696e   = make_tuple(in
-0000fef0: 7465 726d 6564 6961 7465 5f73 7461 7429  termediate_stat)
-0000ff00: 0d0a 2020 2020 6669 6e61 6c5f 7374 6174  ..    final_stat
-0000ff10: 203d 206d 616b 655f 7475 706c 6528 6669   = make_tuple(fi
-0000ff20: 6e61 6c5f 7374 6174 290d 0a20 2020 2066  nal_stat)..    f
-0000ff30: 696e 616c 5f73 6861 7065 203d 206d 616b  inal_shape = mak
-0000ff40: 655f 7475 706c 6528 6669 6e61 6c5f 7368  e_tuple(final_sh
-0000ff50: 6170 6529 0d0a 0d0a 2020 2020 7374 6570  ape)....    step
-0000ff60: 203d 2073 686f 775f 7072 6f67 7265 7373   = show_progress
-0000ff70: 2873 7465 702c 7072 6f63 6573 735f 6c65  (step,process_le
-0000ff80: 6e67 7468 2c70 726f 6365 7373 5f6e 616d  ngth,process_nam
-0000ff90: 652b 2220 222b 223c 222b 6375 7272 656e  e+" "+"<"+curren
-0000ffa0: 745f 6d65 6d6f 7279 5f64 6973 706c 6179  t_memory_display
-0000ffb0: 2829 2b22 3e22 2c63 6f6c 6f72 3d70 726f  ()+">",color=pro
-0000ffc0: 6365 7373 5f63 6f6c 6f72 2c74 696d 653d  cess_color,time=
-0000ffd0: 7469 6d65 2e74 696d 6528 292d 7330 3029  time.time()-s00)
-0000ffe0: 0d0a 2020 2020 233d 3d3d 3d3d 3d3d 3d3d  ..    #=========
-0000fff0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010000: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010010: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010030: 3d3d 3d3d 3d3d 230d 0a20 2020 2023 2020  ======#..    #  
-00010040: 2053 7465 7020 303a 2050 7265 7061 7261   Step 0: Prepara
-00010050: 7469 6f6e 2020 2020 2020 2020 2020 2020  tion            
-00010060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010080: 2020 2020 2020 2020 2020 2020 2023 0d0a               #..
-00010090: 2020 2020 233d 3d3d 3d3d 3d3d 3d3d 3d3d      #===========
-000100a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000100b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000100c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000100d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000100e0: 3d3d 3d3d 230d 0a20 2020 200d 0a20 2020  ====#..    ..   
-000100f0: 204f 626a 203d 2049 6e70 4f62 6a2e 636f   Obj = InpObj.co
-00010100: 7079 2829 0d0a 2020 2020 7468 6973 5f74  py()..    this_t
-00010110: 7970 6520 3d20 7479 7065 284f 626a 290d  ype = type(Obj).
-00010120: 0a20 2020 2074 6869 735f 666f 726d 6174  .    this_format
-00010130: 203d 204f 626a 2e66 6f72 6d61 740d 0a20   = Obj.format.. 
-00010140: 2020 2074 6869 735f 656e 636f 6465 7220     this_encoder 
-00010150: 3d20 4f62 6a2e 656e 636f 6465 720d 0a20  = Obj.encoder.. 
-00010160: 2020 2058 4f62 6a5f 7374 6174 7320 3d20     XObj_stats = 
-00010170: 4f62 6a2e 7374 6174 6973 7469 630d 0a20  Obj.statistic.. 
-00010180: 2020 2058 4f62 6a5f 7368 6170 6520 3d20     XObj_shape = 
-00010190: 4f62 6a2e 7368 6170 650d 0a0d 0a20 2020  Obj.shape....   
-000101a0: 2069 6620 7361 7665 5f6d 656d 6f72 7920   if save_memory 
-000101b0: 3a0d 0a20 2020 2020 2020 2064 656c 2049  :..        del I
-000101c0: 6e70 4f62 6a2e 6461 7461 0d0a 2020 2020  npObj.data..    
-000101d0: 2020 2020 6465 6c20 496e 704f 626a 0d0a      del InpObj..
-000101e0: 2020 2020 2020 2020 6763 2e63 6f6c 6c65          gc.colle
-000101f0: 6374 2829 0d0a 0d0a 2020 2020 7374 6570  ct()....    step
-00010200: 203d 2073 686f 775f 7072 6f67 7265 7373   = show_progress
-00010210: 2873 7465 702c 7072 6f63 6573 735f 6c65  (step,process_le
-00010220: 6e67 7468 2c70 726f 6365 7373 5f6e 616d  ngth,process_nam
-00010230: 652b 2220 222b 223c 222b 6375 7272 656e  e+" "+"<"+curren
-00010240: 745f 6d65 6d6f 7279 5f64 6973 706c 6179  t_memory_display
-00010250: 2829 2b22 3e22 2c63 6f6c 6f72 3d70 726f  ()+">",color=pro
-00010260: 6365 7373 5f63 6f6c 6f72 2c74 696d 653d  cess_color,time=
-00010270: 7469 6d65 2e74 696d 6528 292d 7330 3029  time.time()-s00)
-00010280: 0d0a 2020 2020 233d 3d3d 3d3d 3d3d 3d3d  ..    #=========
-00010290: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000102a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000102b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000102c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000102d0: 3d3d 3d3d 3d3d 230d 0a20 2020 2023 2020  ======#..    #  
-000102e0: 2053 7465 7020 353a 2053 706c 6974 2062   Step 5: Split b
-000102f0: 6f73 6f6e 7320 616e 6420 6665 726d 696f  osons and fermio
-00010300: 6e73 2020 2020 2020 2020 2020 2020 2020  ns              
-00010310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010320: 2020 2020 2020 2020 2020 2020 2023 0d0a               #..
-00010330: 2020 2020 233d 3d3d 3d3d 3d3d 3d3d 3d3d      #===========
-00010340: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010360: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010370: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010380: 3d3d 3d3d 230d 0a20 2020 200d 0a20 2020  ====#..    ..   
-00010390: 2067 726f 7570 5f69 6e66 6f2c 2073 6f72   group_info, sor
-000103a0: 7465 645f 6772 6f75 705f 696e 666f 203d  ted_group_info =
-000103b0: 2067 6574 5f67 726f 7570 5f69 6e66 6f28   get_group_info(
-000103c0: 7374 7269 6e67 5f69 6e70 2c20 6669 6e61  string_inp, fina
-000103d0: 6c5f 7374 6174 2c20 6669 6e61 6c5f 7368  l_stat, final_sh
-000103e0: 6170 6529 0d0a 2020 2020 6e65 775f 7374  ape)..    new_st
-000103f0: 6174 732c 206e 6577 5f73 6861 7065 2c20  ats, new_shape, 
-00010400: 5f2c 205f 203d 2067 6574 5f69 6e74 6572  _, _ = get_inter
-00010410: 6d65 6469 6174 655f 696e 666f 2873 6f72  mediate_info(sor
-00010420: 7465 645f 6772 6f75 705f 696e 666f 2c69  ted_group_info,i
-00010430: 6e74 6572 6d65 6469 6174 655f 7374 6174  ntermediate_stat
-00010440: 290d 0a20 2020 2073 6967 6e5f 6661 6374  )..    sign_fact
-00010450: 6f72 735f 6c69 7374 203d 2067 6574 5f67  ors_list = get_g
-00010460: 726f 7570 696e 675f 7369 676e 5f66 6163  rouping_sign_fac
-00010470: 746f 7273 2873 6f72 7465 645f 6772 6f75  tors(sorted_grou
-00010480: 705f 696e 666f 2c20 696e 7465 726d 6564  p_info, intermed
-00010490: 6961 7465 5f73 7461 7429 0d0a 2020 2020  iate_stat)..    
-000104a0: 0d0a 2020 2020 4f62 6a2e 6461 7461 203d  ..    Obj.data =
-000104b0: 206e 702e 7265 7368 6170 6528 4f62 6a2e   np.reshape(Obj.
-000104c0: 6461 7461 2c6e 6577 5f73 6861 7065 290d  data,new_shape).
-000104d0: 0a20 2020 204f 626a 2e73 7461 7469 7374  .    Obj.statist
-000104e0: 6963 203d 206e 6577 5f73 7461 7473 0d0a  ic = new_stats..
-000104f0: 2020 2020 0d0a 2020 2020 7374 6570 203d      ..    step =
-00010500: 2073 686f 775f 7072 6f67 7265 7373 2873   show_progress(s
-00010510: 7465 702c 7072 6f63 6573 735f 6c65 6e67  tep,process_leng
-00010520: 7468 2c70 726f 6365 7373 5f6e 616d 652b  th,process_name+
-00010530: 2220 222b 223c 222b 6375 7272 656e 745f  " "+"<"+current_
-00010540: 6d65 6d6f 7279 5f64 6973 706c 6179 2829  memory_display()
-00010550: 2b22 3e22 2c63 6f6c 6f72 3d70 726f 6365  +">",color=proce
-00010560: 7373 5f63 6f6c 6f72 2c74 696d 653d 7469  ss_color,time=ti
-00010570: 6d65 2e74 696d 6528 292d 7330 3029 0d0a  me.time()-s00)..
-00010580: 2020 2020 233d 3d3d 3d3d 3d3d 3d3d 3d3d      #===========
-00010590: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000105a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000105b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000105c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000105d0: 3d3d 3d3d 230d 0a20 2020 2023 2020 2053  ====#..    #   S
-000105e0: 7465 7020 343a 2053 7769 7463 6820 656e  tep 4: Switch en
-000105f0: 636f 6465 7220 2020 2020 2020 2020 2020  coder           
-00010600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010620: 2020 2020 2020 2020 2020 2023 0d0a 2020             #..  
-00010630: 2020 233d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    #=============
-00010640: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010650: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010660: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010670: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010680: 3d3d 230d 0a20 2020 200d 0a20 2020 204f  ==#..    ..    O
-00010690: 626a 203d 204f 626a 2e73 7769 7463 685f  bj = Obj.switch_
-000106a0: 656e 636f 6465 7228 7361 7665 5f6d 656d  encoder(save_mem
-000106b0: 6f72 793d 5472 7565 290d 0a20 2020 200d  ory=True)..    .
-000106c0: 0a20 2020 2073 7465 7020 3d20 7368 6f77  .    step = show
-000106d0: 5f70 726f 6772 6573 7328 7374 6570 2c70  _progress(step,p
-000106e0: 726f 6365 7373 5f6c 656e 6774 682c 7072  rocess_length,pr
-000106f0: 6f63 6573 735f 6e61 6d65 2b22 2022 2b22  ocess_name+" "+"
-00010700: 3c22 2b63 7572 7265 6e74 5f6d 656d 6f72  <"+current_memor
-00010710: 795f 6469 7370 6c61 7928 292b 223e 222c  y_display()+">",
-00010720: 636f 6c6f 723d 7072 6f63 6573 735f 636f  color=process_co
-00010730: 6c6f 722c 7469 6d65 3d74 696d 652e 7469  lor,time=time.ti
-00010740: 6d65 2829 2d73 3030 290d 0a20 2020 2023  me()-s00)..    #
+0000fc90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 230d 0a20  ============#.. 
+0000fca0: 2020 200d 0a20 2020 204f 626a 2e64 6174     ..    Obj.dat
+0000fcb0: 6120 3d20 6e70 2e72 6573 6861 7065 284f  a = np.reshape(O
+0000fcc0: 626a 2e64 6174 612c 6669 6e61 6c5f 7368  bj.data,final_sh
+0000fcd0: 6170 6529 0d0a 2020 2020 4f62 6a2e 7374  ape)..    Obj.st
+0000fce0: 6174 6973 7469 6320 3d20 6669 6e61 6c5f  atistic = final_
+0000fcf0: 7374 6174 730d 0a20 2020 200d 0a20 2020  stats..    ..   
+0000fd00: 2063 6c65 6172 5f70 726f 6772 6573 7328   clear_progress(
+0000fd10: 290d 0a20 2020 2074 6162 5f75 7028 290d  )..    tab_up().
+0000fd20: 0a0d 0a20 2020 2072 6574 7572 6e20 4f62  ...    return Ob
+0000fd30: 6a0d 0a20 2020 200d 0a64 6566 2073 706c  j..    ..def spl
+0000fd40: 6974 5f6c 6567 7328 496e 704f 626a 2c73  it_legs(InpObj,s
+0000fd50: 7472 696e 675f 696e 702c 6669 6e61 6c5f  tring_inp,final_
+0000fd60: 7374 6174 2c66 696e 616c 5f73 6861 7065  stat,final_shape
+0000fd70: 2c69 6e74 6572 6d65 6469 6174 655f 7374  ,intermediate_st
+0000fd80: 6174 3d28 2d31 2c31 292c 7361 7665 5f6d  at=(-1,1),save_m
+0000fd90: 656d 6f72 793d 4661 6c73 6529 3a0d 0a0d  emory=False):...
+0000fda0: 0a20 2020 2070 726f 6365 7373 5f6e 616d  .    process_nam
+0000fdb0: 6520 3d20 2273 706c 6974 5f6c 6567 7322  e = "split_legs"
+0000fdc0: 0d0a 2020 2020 7072 6f63 6573 735f 6c65  ..    process_le
+0000fdd0: 6e67 7468 203d 2036 0d0a 2020 2020 7072  ngth = 6..    pr
+0000fde0: 6f63 6573 735f 636f 6c6f 723d 2267 7265  ocess_color="gre
+0000fdf0: 656e 220d 0a20 2020 2073 7465 7020 3d20  en"..    step = 
+0000fe00: 310d 0a20 2020 2073 3030 203d 2074 696d  1..    s00 = tim
+0000fe10: 652e 7469 6d65 2829 0d0a 2020 2020 7072  e.time()..    pr
+0000fe20: 6f67 7265 7373 5f73 7061 6365 2829 2023  ogress_space() #
+0000fe30: 203c 3c20 446f 6e27 7420 7265 6d6f 7665   << Don't remove
+0000fe40: 2074 6869 732e 2054 6869 7320 6973 2066   this. This is f
+0000fe50: 6f72 2074 6865 2073 686f 775f 7072 6f67  or the show_prog
+0000fe60: 7265 7373 210d 0a0d 0a20 2020 2073 7472  ress!....    str
+0000fe70: 696e 675f 696e 7020 3d20 6465 6e75 6d65  ing_inp = denume
+0000fe80: 7261 7465 2873 7472 696e 675f 696e 7029  rate(string_inp)
+0000fe90: 0d0a 0d0a 2020 2020 696e 7465 726d 6564  ....    intermed
+0000fea0: 6961 7465 5f73 7461 7420 3d20 6d61 6b65  iate_stat = make
+0000feb0: 5f74 7570 6c65 2869 6e74 6572 6d65 6469  _tuple(intermedi
+0000fec0: 6174 655f 7374 6174 290d 0a20 2020 2066  ate_stat)..    f
+0000fed0: 696e 616c 5f73 7461 7420 3d20 6d61 6b65  inal_stat = make
+0000fee0: 5f74 7570 6c65 2866 696e 616c 5f73 7461  _tuple(final_sta
+0000fef0: 7429 0d0a 2020 2020 6669 6e61 6c5f 7368  t)..    final_sh
+0000ff00: 6170 6520 3d20 6d61 6b65 5f74 7570 6c65  ape = make_tuple
+0000ff10: 2866 696e 616c 5f73 6861 7065 290d 0a0d  (final_shape)...
+0000ff20: 0a20 2020 2073 7465 7020 3d20 7368 6f77  .    step = show
+0000ff30: 5f70 726f 6772 6573 7328 7374 6570 2c70  _progress(step,p
+0000ff40: 726f 6365 7373 5f6c 656e 6774 682c 7072  rocess_length,pr
+0000ff50: 6f63 6573 735f 6e61 6d65 2b22 2022 2b22  ocess_name+" "+"
+0000ff60: 3c22 2b63 7572 7265 6e74 5f6d 656d 6f72  <"+current_memor
+0000ff70: 795f 6469 7370 6c61 7928 292b 223e 222c  y_display()+">",
+0000ff80: 636f 6c6f 723d 7072 6f63 6573 735f 636f  color=process_co
+0000ff90: 6c6f 722c 7469 6d65 3d74 696d 652e 7469  lor,time=time.ti
+0000ffa0: 6d65 2829 2d73 3030 290d 0a20 2020 2023  me()-s00)..    #
+0000ffb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ffc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ffd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ffe0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000fff0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d23  ===============#
+00010000: 0d0a 2020 2020 2320 2020 5374 6570 2030  ..    #   Step 0
+00010010: 3a20 5072 6570 6172 6174 696f 6e20 2020  : Preparation   
+00010020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010050: 2020 2020 2020 230d 0a20 2020 2023 3d3d        #..    #==
+00010060: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010070: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010080: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010090: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000100a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d23 0d0a  =============#..
+000100b0: 2020 2020 0d0a 2020 2020 4f62 6a20 3d20      ..    Obj = 
+000100c0: 496e 704f 626a 2e63 6f70 7928 290d 0a20  InpObj.copy().. 
+000100d0: 2020 2074 6869 735f 7479 7065 203d 2074     this_type = t
+000100e0: 7970 6528 4f62 6a29 0d0a 2020 2020 7468  ype(Obj)..    th
+000100f0: 6973 5f66 6f72 6d61 7420 3d20 4f62 6a2e  is_format = Obj.
+00010100: 666f 726d 6174 0d0a 2020 2020 7468 6973  format..    this
+00010110: 5f65 6e63 6f64 6572 203d 204f 626a 2e65  _encoder = Obj.e
+00010120: 6e63 6f64 6572 0d0a 2020 2020 584f 626a  ncoder..    XObj
+00010130: 5f73 7461 7473 203d 204f 626a 2e73 7461  _stats = Obj.sta
+00010140: 7469 7374 6963 0d0a 2020 2020 584f 626a  tistic..    XObj
+00010150: 5f73 6861 7065 203d 204f 626a 2e73 6861  _shape = Obj.sha
+00010160: 7065 0d0a 0d0a 2020 2020 6966 2073 6176  pe....    if sav
+00010170: 655f 6d65 6d6f 7279 203a 0d0a 2020 2020  e_memory :..    
+00010180: 2020 2020 6465 6c20 496e 704f 626a 2e64      del InpObj.d
+00010190: 6174 610d 0a20 2020 2020 2020 2064 656c  ata..        del
+000101a0: 2049 6e70 4f62 6a0d 0a20 2020 2020 2020   InpObj..       
+000101b0: 2067 632e 636f 6c6c 6563 7428 290d 0a0d   gc.collect()...
+000101c0: 0a20 2020 2073 7465 7020 3d20 7368 6f77  .    step = show
+000101d0: 5f70 726f 6772 6573 7328 7374 6570 2c70  _progress(step,p
+000101e0: 726f 6365 7373 5f6c 656e 6774 682c 7072  rocess_length,pr
+000101f0: 6f63 6573 735f 6e61 6d65 2b22 2022 2b22  ocess_name+" "+"
+00010200: 3c22 2b63 7572 7265 6e74 5f6d 656d 6f72  <"+current_memor
+00010210: 795f 6469 7370 6c61 7928 292b 223e 222c  y_display()+">",
+00010220: 636f 6c6f 723d 7072 6f63 6573 735f 636f  color=process_co
+00010230: 6c6f 722c 7469 6d65 3d74 696d 652e 7469  lor,time=time.ti
+00010240: 6d65 2829 2d73 3030 290d 0a20 2020 2023  me()-s00)..    #
+00010250: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010260: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010270: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010280: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010290: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d23  ===============#
+000102a0: 0d0a 2020 2020 2320 2020 5374 6570 2035  ..    #   Step 5
+000102b0: 3a20 5370 6c69 7420 626f 736f 6e73 2061  : Split bosons a
+000102c0: 6e64 2066 6572 6d69 6f6e 7320 2020 2020  nd fermions     
+000102d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102f0: 2020 2020 2020 230d 0a20 2020 2023 3d3d        #..    #==
+00010300: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010310: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010320: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010330: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010340: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d23 0d0a  =============#..
+00010350: 2020 2020 0d0a 2020 2020 6772 6f75 705f      ..    group_
+00010360: 696e 666f 2c20 736f 7274 6564 5f67 726f  info, sorted_gro
+00010370: 7570 5f69 6e66 6f20 3d20 6765 745f 6772  up_info = get_gr
+00010380: 6f75 705f 696e 666f 2873 7472 696e 675f  oup_info(string_
+00010390: 696e 702c 2066 696e 616c 5f73 7461 742c  inp, final_stat,
+000103a0: 2066 696e 616c 5f73 6861 7065 290d 0a20   final_shape).. 
+000103b0: 2020 206e 6577 5f73 7461 7473 2c20 6e65     new_stats, ne
+000103c0: 775f 7368 6170 652c 205f 2c20 5f20 3d20  w_shape, _, _ = 
+000103d0: 6765 745f 696e 7465 726d 6564 6961 7465  get_intermediate
+000103e0: 5f69 6e66 6f28 736f 7274 6564 5f67 726f  _info(sorted_gro
+000103f0: 7570 5f69 6e66 6f2c 696e 7465 726d 6564  up_info,intermed
+00010400: 6961 7465 5f73 7461 7429 0d0a 2020 2020  iate_stat)..    
+00010410: 7369 676e 5f66 6163 746f 7273 5f6c 6973  sign_factors_lis
+00010420: 7420 3d20 6765 745f 6772 6f75 7069 6e67  t = get_grouping
+00010430: 5f73 6967 6e5f 6661 6374 6f72 7328 736f  _sign_factors(so
+00010440: 7274 6564 5f67 726f 7570 5f69 6e66 6f2c  rted_group_info,
+00010450: 2069 6e74 6572 6d65 6469 6174 655f 7374   intermediate_st
+00010460: 6174 290d 0a20 2020 200d 0a20 2020 204f  at)..    ..    O
+00010470: 626a 2e64 6174 6120 3d20 6e70 2e72 6573  bj.data = np.res
+00010480: 6861 7065 284f 626a 2e64 6174 612c 6e65  hape(Obj.data,ne
+00010490: 775f 7368 6170 6529 0d0a 2020 2020 4f62  w_shape)..    Ob
+000104a0: 6a2e 7374 6174 6973 7469 6320 3d20 6e65  j.statistic = ne
+000104b0: 775f 7374 6174 730d 0a20 2020 200d 0a20  w_stats..    .. 
+000104c0: 2020 2073 7465 7020 3d20 7368 6f77 5f70     step = show_p
+000104d0: 726f 6772 6573 7328 7374 6570 2c70 726f  rogress(step,pro
+000104e0: 6365 7373 5f6c 656e 6774 682c 7072 6f63  cess_length,proc
+000104f0: 6573 735f 6e61 6d65 2b22 2022 2b22 3c22  ess_name+" "+"<"
+00010500: 2b63 7572 7265 6e74 5f6d 656d 6f72 795f  +current_memory_
+00010510: 6469 7370 6c61 7928 292b 223e 222c 636f  display()+">",co
+00010520: 6c6f 723d 7072 6f63 6573 735f 636f 6c6f  lor=process_colo
+00010530: 722c 7469 6d65 3d74 696d 652e 7469 6d65  r,time=time.time
+00010540: 2829 2d73 3030 290d 0a20 2020 2023 3d3d  ()-s00)..    #==
+00010550: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010560: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010570: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010580: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010590: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d23 0d0a  =============#..
+000105a0: 2020 2020 2320 2020 5374 6570 2034 3a20      #   Step 4: 
+000105b0: 5377 6974 6368 2065 6e63 6f64 6572 2020  Switch encoder  
+000105c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105f0: 2020 2020 230d 0a20 2020 2023 3d3d 3d3d      #..    #====
+00010600: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010610: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010620: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010630: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010640: 3d3d 3d3d 3d3d 3d3d 3d3d 3d23 0d0a 2020  ===========#..  
+00010650: 2020 0d0a 2020 2020 4f62 6a20 3d20 4f62    ..    Obj = Ob
+00010660: 6a2e 7377 6974 6368 5f65 6e63 6f64 6572  j.switch_encoder
+00010670: 2873 6176 655f 6d65 6d6f 7279 3d54 7275  (save_memory=Tru
+00010680: 6529 0d0a 2020 2020 0d0a 2020 2020 7374  e)..    ..    st
+00010690: 6570 203d 2073 686f 775f 7072 6f67 7265  ep = show_progre
+000106a0: 7373 2873 7465 702c 7072 6f63 6573 735f  ss(step,process_
+000106b0: 6c65 6e67 7468 2c70 726f 6365 7373 5f6e  length,process_n
+000106c0: 616d 652b 2220 222b 223c 222b 6375 7272  ame+" "+"<"+curr
+000106d0: 656e 745f 6d65 6d6f 7279 5f64 6973 706c  ent_memory_displ
+000106e0: 6179 2829 2b22 3e22 2c63 6f6c 6f72 3d70  ay()+">",color=p
+000106f0: 726f 6365 7373 5f63 6f6c 6f72 2c74 696d  rocess_color,tim
+00010700: 653d 7469 6d65 2e74 696d 6528 292d 7330  e=time.time()-s0
+00010710: 3029 0d0a 2020 2020 233d 3d3d 3d3d 3d3d  0)..    #=======
+00010720: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010730: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010740: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00010750: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010760: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010770: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010780: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010790: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d23  ===============#
-000107a0: 0d0a 2020 2020 2320 2020 5374 6570 2033  ..    #   Step 3
-000107b0: 3a20 5377 6974 6368 2066 6f72 6d61 7420  : Switch format 
-000107c0: 6966 2074 6869 735f 666f 726d 6174 3d27  if this_format='
-000107d0: 6d61 7472 6978 2720 2020 2020 2020 2020  matrix'         
-000107e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000107f0: 2020 2020 2020 230d 0a20 2020 2023 3d3d        #..    #==
+00010760: 3d3d 3d3d 3d3d 3d3d 230d 0a20 2020 2023  ========#..    #
+00010770: 2020 2053 7465 7020 333a 2053 7769 7463     Step 3: Switc
+00010780: 6820 666f 726d 6174 2069 6620 7468 6973  h format if this
+00010790: 5f66 6f72 6d61 743d 276d 6174 7269 7827  _format='matrix'
+000107a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000107b0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000107c0: 0d0a 2020 2020 233d 3d3d 3d3d 3d3d 3d3d  ..    #=========
+000107d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000107e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000107f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00010800: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010810: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010820: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010830: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010840: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d23 0d0a  =============#..
-00010850: 2020 2020 0d0a 2020 2020 6966 2074 6869      ..    if thi
-00010860: 735f 666f 726d 6174 203d 3d20 276d 6174  s_format == 'mat
-00010870: 7269 7827 3a0d 0a20 2020 2020 2020 204f  rix':..        O
-00010880: 626a 203d 204f 626a 2e73 7769 7463 685f  bj = Obj.switch_
-00010890: 666f 726d 6174 2873 6176 655f 6d65 6d6f  format(save_memo
-000108a0: 7279 3d54 7275 6529 0d0a 2020 2020 2020  ry=True)..      
-000108b0: 2020 0d0a 2020 2020 7374 6570 203d 2073    ..    step = s
-000108c0: 686f 775f 7072 6f67 7265 7373 2873 7465  how_progress(ste
-000108d0: 702c 7072 6f63 6573 735f 6c65 6e67 7468  p,process_length
-000108e0: 2c70 726f 6365 7373 5f6e 616d 652b 2220  ,process_name+" 
-000108f0: 222b 223c 222b 6375 7272 656e 745f 6d65  "+"<"+current_me
-00010900: 6d6f 7279 5f64 6973 706c 6179 2829 2b22  mory_display()+"
-00010910: 3e22 2c63 6f6c 6f72 3d70 726f 6365 7373  >",color=process
-00010920: 5f63 6f6c 6f72 2c74 696d 653d 7469 6d65  _color,time=time
-00010930: 2e74 696d 6528 292d 7330 3029 0d0a 2020  .time()-s00)..  
-00010940: 2020 233d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    #=============
-00010950: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010960: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010970: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010980: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010990: 3d3d 230d 0a20 2020 2023 2020 2053 7465  ==#..    #   Ste
-000109a0: 7020 323a 2053 706c 6974 2066 6572 6d69  p 2: Split fermi
-000109b0: 6f6e 6963 2069 6e64 6963 6573 2077 6974  onic indices wit
-000109c0: 6820 6e70 2e72 6573 6861 7065 2020 2020  h np.reshape    
-000109d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109e0: 2020 2020 2020 2020 2020 230d 0a20 2020            #..   
-000109f0: 2023 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   #==============
-00010a00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010a10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010a20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010a30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010a40: 3d23 0d0a 2020 2020 0d0a 2020 2020 6e65  =#..    ..    ne
-00010a50: 775f 7374 6174 7320 3d20 5b5d 0d0a 2020  w_stats = []..  
-00010a60: 2020 6e65 775f 7368 6170 6520 3d20 5b5d    new_shape = []
-00010a70: 0d0a 2020 2020 666f 7220 5b69 6e64 6963  ..    for [indic
-00010a80: 6573 2c73 7461 7473 2c73 6861 7065 5d20  es,stats,shape] 
-00010a90: 696e 2073 6f72 7465 645f 6772 6f75 705f  in sorted_group_
-00010aa0: 696e 666f 3a0d 0a20 2020 2020 2020 206e  info:..        n
-00010ab0: 6577 5f73 7461 7473 202b 3d20 6d61 6b65  ew_stats += make
-00010ac0: 5f6c 6973 7428 7374 6174 7329 0d0a 2020  _list(stats)..  
-00010ad0: 2020 2020 2020 6e65 775f 7368 6170 6520        new_shape 
-00010ae0: 2b3d 206d 616b 655f 6c69 7374 2873 6861  += make_list(sha
-00010af0: 7065 290d 0a20 2020 206e 6577 5f73 7461  pe)..    new_sta
-00010b00: 7473 203d 206d 616b 655f 7475 706c 6528  ts = make_tuple(
-00010b10: 6e65 775f 7374 6174 7329 0d0a 2020 2020  new_stats)..    
-00010b20: 6e65 775f 7368 6170 6520 3d20 6d61 6b65  new_shape = make
-00010b30: 5f74 7570 6c65 286e 6577 5f73 6861 7065  _tuple(new_shape
-00010b40: 290d 0a20 2020 200d 0a20 2020 204f 626a  )..    ..    Obj
-00010b50: 2e64 6174 6120 3d20 6e70 2e72 6573 6861  .data = np.resha
-00010b60: 7065 284f 626a 2e64 6174 612c 6e65 775f  pe(Obj.data,new_
-00010b70: 7368 6170 6529 0d0a 2020 2020 4f62 6a2e  shape)..    Obj.
-00010b80: 7374 6174 6973 7469 6320 3d20 6e65 775f  statistic = new_
-00010b90: 7374 6174 730d 0a20 2020 200d 0a20 2020  stats..    ..   
-00010ba0: 2073 7465 7020 3d20 7368 6f77 5f70 726f   step = show_pro
-00010bb0: 6772 6573 7328 7374 6570 2c70 726f 6365  gress(step,proce
-00010bc0: 7373 5f6c 656e 6774 682c 7072 6f63 6573  ss_length,proces
-00010bd0: 735f 6e61 6d65 2b22 2022 2b22 3c22 2b63  s_name+" "+"<"+c
-00010be0: 7572 7265 6e74 5f6d 656d 6f72 795f 6469  urrent_memory_di
-00010bf0: 7370 6c61 7928 292b 223e 222c 636f 6c6f  splay()+">",colo
-00010c00: 723d 7072 6f63 6573 735f 636f 6c6f 722c  r=process_color,
-00010c10: 7469 6d65 3d74 696d 652e 7469 6d65 2829  time=time.time()
-00010c20: 2d73 3030 290d 0a20 2020 2023 3d3d 3d3d  -s00)..    #====
+00010810: 3d3d 3d3d 3d3d 230d 0a20 2020 200d 0a20  ======#..    .. 
+00010820: 2020 2069 6620 7468 6973 5f66 6f72 6d61     if this_forma
+00010830: 7420 3d3d 2027 6d61 7472 6978 273a 0d0a  t == 'matrix':..
+00010840: 2020 2020 2020 2020 4f62 6a20 3d20 4f62          Obj = Ob
+00010850: 6a2e 7377 6974 6368 5f66 6f72 6d61 7428  j.switch_format(
+00010860: 7361 7665 5f6d 656d 6f72 793d 5472 7565  save_memory=True
+00010870: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+00010880: 2073 7465 7020 3d20 7368 6f77 5f70 726f   step = show_pro
+00010890: 6772 6573 7328 7374 6570 2c70 726f 6365  gress(step,proce
+000108a0: 7373 5f6c 656e 6774 682c 7072 6f63 6573  ss_length,proces
+000108b0: 735f 6e61 6d65 2b22 2022 2b22 3c22 2b63  s_name+" "+"<"+c
+000108c0: 7572 7265 6e74 5f6d 656d 6f72 795f 6469  urrent_memory_di
+000108d0: 7370 6c61 7928 292b 223e 222c 636f 6c6f  splay()+">",colo
+000108e0: 723d 7072 6f63 6573 735f 636f 6c6f 722c  r=process_color,
+000108f0: 7469 6d65 3d74 696d 652e 7469 6d65 2829  time=time.time()
+00010900: 2d73 3030 290d 0a20 2020 2023 3d3d 3d3d  -s00)..    #====
+00010910: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010920: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010930: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010940: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010950: 3d3d 3d3d 3d3d 3d3d 3d3d 3d23 0d0a 2020  ===========#..  
+00010960: 2020 2320 2020 5374 6570 2032 3a20 5370    #   Step 2: Sp
+00010970: 6c69 7420 6665 726d 696f 6e69 6320 696e  lit fermionic in
+00010980: 6469 6365 7320 7769 7468 206e 702e 7265  dices with np.re
+00010990: 7368 6170 6520 2020 2020 2020 2020 2020  shape           
+000109a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000109b0: 2020 2023 0d0a 2020 2020 233d 3d3d 3d3d     #..    #=====
+000109c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000109d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000109e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000109f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010a00: 3d3d 3d3d 3d3d 3d3d 3d3d 230d 0a20 2020  ==========#..   
+00010a10: 200d 0a20 2020 206e 6577 5f73 7461 7473   ..    new_stats
+00010a20: 203d 205b 5d0d 0a20 2020 206e 6577 5f73   = []..    new_s
+00010a30: 6861 7065 203d 205b 5d0d 0a20 2020 2066  hape = []..    f
+00010a40: 6f72 205b 696e 6469 6365 732c 7374 6174  or [indices,stat
+00010a50: 732c 7368 6170 655d 2069 6e20 736f 7274  s,shape] in sort
+00010a60: 6564 5f67 726f 7570 5f69 6e66 6f3a 0d0a  ed_group_info:..
+00010a70: 2020 2020 2020 2020 6e65 775f 7374 6174          new_stat
+00010a80: 7320 2b3d 206d 616b 655f 6c69 7374 2873  s += make_list(s
+00010a90: 7461 7473 290d 0a20 2020 2020 2020 206e  tats)..        n
+00010aa0: 6577 5f73 6861 7065 202b 3d20 6d61 6b65  ew_shape += make
+00010ab0: 5f6c 6973 7428 7368 6170 6529 0d0a 2020  _list(shape)..  
+00010ac0: 2020 6e65 775f 7374 6174 7320 3d20 6d61    new_stats = ma
+00010ad0: 6b65 5f74 7570 6c65 286e 6577 5f73 7461  ke_tuple(new_sta
+00010ae0: 7473 290d 0a20 2020 206e 6577 5f73 6861  ts)..    new_sha
+00010af0: 7065 203d 206d 616b 655f 7475 706c 6528  pe = make_tuple(
+00010b00: 6e65 775f 7368 6170 6529 0d0a 2020 2020  new_shape)..    
+00010b10: 0d0a 2020 2020 4f62 6a2e 6461 7461 203d  ..    Obj.data =
+00010b20: 206e 702e 7265 7368 6170 6528 4f62 6a2e   np.reshape(Obj.
+00010b30: 6461 7461 2c6e 6577 5f73 6861 7065 290d  data,new_shape).
+00010b40: 0a20 2020 204f 626a 2e73 7461 7469 7374  .    Obj.statist
+00010b50: 6963 203d 206e 6577 5f73 7461 7473 0d0a  ic = new_stats..
+00010b60: 2020 2020 0d0a 2020 2020 7374 6570 203d      ..    step =
+00010b70: 2073 686f 775f 7072 6f67 7265 7373 2873   show_progress(s
+00010b80: 7465 702c 7072 6f63 6573 735f 6c65 6e67  tep,process_leng
+00010b90: 7468 2c70 726f 6365 7373 5f6e 616d 652b  th,process_name+
+00010ba0: 2220 222b 223c 222b 6375 7272 656e 745f  " "+"<"+current_
+00010bb0: 6d65 6d6f 7279 5f64 6973 706c 6179 2829  memory_display()
+00010bc0: 2b22 3e22 2c63 6f6c 6f72 3d70 726f 6365  +">",color=proce
+00010bd0: 7373 5f63 6f6c 6f72 2c74 696d 653d 7469  ss_color,time=ti
+00010be0: 6d65 2e74 696d 6528 292d 7330 3029 0d0a  me.time()-s00)..
+00010bf0: 2020 2020 233d 3d3d 3d3d 3d3d 3d3d 3d3d      #===========
+00010c00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010c10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010c20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00010c30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010c40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010c50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010c60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010c70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d23 0d0a 2020  ===========#..  
-00010c80: 2020 2320 2020 5374 6570 2031 3a20 4d6f    #   Step 1: Mo
-00010c90: 7665 2062 6f73 6f6e 6963 2069 6e64 6963  ve bosonic indic
-00010ca0: 6573 2074 6f20 7468 6520 6c65 6674 206f  es to the left o
-00010cb0: 6620 6561 6368 2067 726f 7570 2020 2020  f each group    
-00010cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cd0: 2020 230d 0a20 2020 2023 3d3d 3d3d 3d3d    #..    #======
+00010c40: 3d3d 3d3d 230d 0a20 2020 2023 2020 2053  ====#..    #   S
+00010c50: 7465 7020 313a 204d 6f76 6520 626f 736f  tep 1: Move boso
+00010c60: 6e69 6320 696e 6469 6365 7320 746f 2074  nic indices to t
+00010c70: 6865 206c 6566 7420 6f66 2065 6163 6820  he left of each 
+00010c80: 6772 6f75 7020 2020 2020 2020 2020 2020  group           
+00010c90: 2020 2020 2020 2020 2020 2023 0d0a 2020             #..  
+00010ca0: 2020 233d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    #=============
+00010cb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010cc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00010cd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00010ce0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010cf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010d00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010d10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00010d20: 3d3d 3d3d 3d3d 3d3d 3d23 0d0a 2020 2020  =========#..    
-00010d30: 0d0a 2020 2020 756e 736f 7274 6564 5f73  ..    unsorted_s
-00010d40: 7472 696e 6720 3d20 2727 2e6a 6f69 6e28  tring = ''.join(
-00010d50: 205b 2069 6e64 6963 6573 2066 6f72 205b   [ indices for [
-00010d60: 696e 6469 6365 732c 2073 7461 7473 2c20  indices, stats, 
-00010d70: 7368 6170 655d 2069 6e20 6772 6f75 705f  shape] in group_
-00010d80: 696e 666f 205d 2029 0d0a 2020 2020 736f  info ] )..    so
-00010d90: 7274 6564 5f73 7472 696e 6720 3d20 2727  rted_string = ''
-00010da0: 2e6a 6f69 6e28 205b 2069 6e64 6963 6573  .join( [ indices
-00010db0: 2066 6f72 205b 696e 6469 6365 732c 2073   for [indices, s
-00010dc0: 7461 7473 2c20 7368 6170 655d 2069 6e20  tats, shape] in 
-00010dd0: 736f 7274 6564 5f67 726f 7570 5f69 6e66  sorted_group_inf
-00010de0: 6f20 5d20 290d 0a20 2020 206e 7065 696e  o ] )..    npein
-00010df0: 7375 6d5f 7374 7269 6e67 203d 2073 6f72  sum_string = sor
-00010e00: 7465 645f 7374 7269 6e67 2b73 6967 6e5f  ted_string+sign_
-00010e10: 6661 6374 6f72 735f 6c69 7374 5b30 5d2b  factors_list[0]+
-00010e20: 222d 3e22 2b75 6e73 6f72 7465 645f 7374  "->"+unsorted_st
-00010e30: 7269 6e67 0d0a 2020 2020 6e70 6569 6e73  ring..    npeins
-00010e40: 756d 5f6f 626a 203d 205b 4f62 6a2e 6461  um_obj = [Obj.da
-00010e50: 7461 5d20 2b20 7369 676e 5f66 6163 746f  ta] + sign_facto
-00010e60: 7273 5f6c 6973 745b 315d 0d0a 2020 2020  rs_list[1]..    
-00010e70: 4f62 6a2e 6461 7461 203d 206f 652e 636f  Obj.data = oe.co
-00010e80: 6e74 7261 6374 282a 6d61 6b65 5f74 7570  ntract(*make_tup
-00010e90: 6c65 2820 5b6e 7065 696e 7375 6d5f 7374  le( [npeinsum_st
-00010ea0: 7269 6e67 5d20 2b20 6e70 6569 6e73 756d  ring] + npeinsum
-00010eb0: 5f6f 626a 2029 290d 0a20 2020 204f 626a  _obj ))..    Obj
-00010ec0: 2e73 7461 7469 7374 6963 203d 2066 696e  .statistic = fin
-00010ed0: 616c 5f73 7461 740d 0a20 2020 200d 0a20  al_stat..    .. 
-00010ee0: 2020 2063 6c65 6172 5f70 726f 6772 6573     clear_progres
-00010ef0: 7328 290d 0a20 2020 2073 7973 2e73 7464  s()..    sys.std
-00010f00: 6f75 742e 7772 6974 6528 225c 3033 335b  out.write("\033[
-00010f10: 4622 290d 0a0d 0a20 2020 2069 6620 7468  F")....    if th
-00010f20: 6973 5f66 6f72 6d61 743d 3d27 6d61 7472  is_format=='matr
-00010f30: 6978 273a 0d0a 2020 2020 2020 2020 7265  ix':..        re
-00010f40: 7475 726e 204f 626a 2e73 7769 7463 685f  turn Obj.switch_
-00010f50: 666f 726d 6174 2873 6176 655f 6d65 6d6f  format(save_memo
-00010f60: 7279 3d54 7275 6529 0d0a 2020 2020 0d0a  ry=True)..    ..
-00010f70: 2020 2020 7265 7475 726e 204f 626a 0d0a      return Obj..
-00010f80: 2020 2020 0d0a 6465 6620 6765 745f 6772      ..def get_gr
-00010f90: 6f75 705f 696e 666f 2867 726f 7570 696e  oup_info(groupin
-00010fa0: 675f 7374 7269 6e67 2c20 756e 6772 6f75  g_string, ungrou
-00010fb0: 705f 7374 6174 2c20 756e 6772 6f75 705f  p_stat, ungroup_
-00010fc0: 7368 6170 6529 3a0d 0a20 2020 2023 7072  shape):..    #pr
-00010fd0: 696e 7428 226f 7269 6769 6e61 6c20 7374  int("original st
-00010fe0: 7269 6e67 3a22 2c67 726f 7570 696e 675f  ring:",grouping_
-00010ff0: 7374 7269 6e67 290d 0a20 2020 2066 6f72  string)..    for
-00011000: 6d61 7474 6564 5f73 7472 696e 6720 3d20  matted_string = 
-00011010: 6772 6f75 7069 6e67 5f73 7472 696e 670d  grouping_string.
-00011020: 0a20 2020 200d 0a20 2020 2023 2063 6865  .    ..    # che
-00011030: 636b 2074 6865 2073 7472 696e 6720 666f  ck the string fo
-00011040: 726d 6174 202d 2d2d 2d2d 2d2d 2d2d 2d2d  rmat -----------
-00011050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20  -------------.. 
-00011080: 2020 2069 6620 666f 726d 6174 7465 645f     if formatted_
-00011090: 7374 7269 6e67 2e63 6f75 6e74 2822 2822  string.count("("
-000110a0: 2920 3d3d 2030 2061 6e64 2066 6f72 6d61  ) == 0 and forma
-000110b0: 7474 6564 5f73 7472 696e 672e 636f 756e  tted_string.coun
-000110c0: 7428 2229 2229 203d 3d20 3020 3a0d 0a20  t(")") == 0 :.. 
-000110d0: 2020 2020 2020 2023 7468 6973 2069 7320         #this is 
-000110e0: 7468 6520 6162 6272 6576 6961 7465 6420  the abbreviated 
-000110f0: 666f 726d 6174 0d0a 2020 2020 2020 2020  format..        
-00011100: 666f 7220 7365 7061 7261 746f 7220 696e  for separator in
-00011110: 2073 6570 6172 6174 6f72 5f6c 6973 743a   separator_list:
-00011120: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00011130: 726d 6174 7465 645f 7374 7269 6e67 203d  rmatted_string =
-00011140: 2066 6f72 6d61 7474 6564 5f73 7472 696e   formatted_strin
-00011150: 672e 7265 706c 6163 6528 7365 7061 7261  g.replace(separa
-00011160: 746f 722c 2229 2822 290d 0a20 2020 2020  tor,")(")..     
-00011170: 2020 2066 6f72 6d61 7474 6564 5f73 7472     formatted_str
-00011180: 696e 6720 3d20 2228 222b 666f 726d 6174  ing = "("+format
-00011190: 7465 645f 7374 7269 6e67 2b22 2922 0d0a  ted_string+")"..
-000111a0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000111b0: 2020 2073 6570 6172 6174 6f72 5f63 6f75     separator_cou
-000111c0: 6e74 203d 2030 0d0a 2020 2020 2020 2020  nt = 0..        
-000111d0: 666f 7220 7365 7061 7261 746f 7220 696e  for separator in
-000111e0: 2073 6570 6172 6174 6f72 5f6c 6973 743a   separator_list:
-000111f0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00011200: 7061 7261 746f 725f 636f 756e 7420 2b3d  parator_count +=
-00011210: 2066 6f72 6d61 7474 6564 5f73 7472 696e   formatted_strin
-00011220: 672e 636f 756e 7428 7365 7061 7261 746f  g.count(separato
-00011230: 7229 0d0a 2020 2020 2020 2020 6966 2073  r)..        if s
-00011240: 6570 6172 6174 6f72 5f63 6f75 6e74 203e  eparator_count >
-00011250: 2030 203a 0d0a 2020 2020 2020 2020 2020   0 :..          
-00011260: 2020 6572 726f 7228 2245 7272 6f72 5b67    error("Error[g
-00011270: 6574 5f67 726f 7570 696e 675f 696e 666f  et_grouping_info
-00011280: 5d3a 2044 6f20 6e6f 7420 6d69 7820 7468  ]: Do not mix th
-00011290: 6520 7374 7269 6e67 2066 6f72 6d61 742e  e string format.
-000112a0: 2229 0d0a 2020 2020 2370 7269 6e74 2822  ")..    #print("
-000112b0: 666f 726d 6174 7465 6420 7374 7269 6e67  formatted string
-000112c0: 3a22 2c66 6f72 6d61 7474 6564 5f73 7472  :",formatted_str
-000112d0: 696e 6729 0d0a 2020 2020 0d0a 2020 2020  ing)..    ..    
-000112e0: 2320 7061 7273 6520 7468 6520 7374 7269  # parse the stri
-000112f0: 6e67 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ng -------------
-00011300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011330: 2d2d 0d0a 2020 2020 6772 6f75 705f 696e  --..    group_in
-00011340: 666f 203d 205b 5d20 2320 5b73 7472 696e  fo = [] # [strin
-00011350: 6720 7465 7874 2c20 7374 6174 6973 7469  g text, statisti
-00011360: 632c 2073 6861 7065 5d0d 0a20 2020 2069  c, shape]..    i
-00011370: 735f 6f75 7473 6964 6520 3d20 5472 7565  s_outside = True
-00011380: 0d0a 2020 2020 6c6f 6361 7469 6f6e 203d  ..    location =
-00011390: 2030 0d0a 2020 2020 666f 7220 6368 6172   0..    for char
-000113a0: 2069 6e20 666f 726d 6174 7465 645f 7374   in formatted_st
-000113b0: 7269 6e67 3a0d 0a20 2020 2020 2020 2069  ring:..        i
-000113c0: 6620 6368 6172 203d 3d20 2228 2220 616e  f char == "(" an
-000113d0: 6420 6973 5f6f 7574 7369 6465 203a 0d0a  d is_outside :..
-000113e0: 2020 2020 2020 2020 2020 2020 6973 5f6f              is_o
-000113f0: 7574 7369 6465 203d 2046 616c 7365 0d0a  utside = False..
-00011400: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
-00011410: 705f 696e 666f 202b 3d20 5b0d 0a20 2020  p_info += [..   
-00011420: 2020 2020 2020 2020 2020 2020 205b 2022               [ "
-00011430: 222c 205b 5d2c 205b 5d20 5d20 236d 616b  ", [], [] ] #mak
-00011440: 6520 6120 626c 616e 6b20 7465 6d70 6c61  e a blank templa
-00011450: 7465 2066 6f72 2074 6869 7320 6772 6f75  te for this grou
-00011460: 700d 0a20 2020 2020 2020 2020 2020 205d  p..            ]
-00011470: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-00011480: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
-00011490: 6966 2063 6861 7220 3d3d 2022 2922 2061  if char == ")" a
-000114a0: 6e64 206e 6f74 2069 735f 6f75 7473 6964  nd not is_outsid
-000114b0: 6520 3a0d 0a20 2020 2020 2020 2020 2020  e :..           
-000114c0: 2069 735f 6f75 7473 6964 6520 3d20 5472   is_outside = Tr
-000114d0: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-000114e0: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
-000114f0: 2020 6966 2028 6368 6172 203d 3d20 2228    if (char == "(
-00011500: 2220 616e 6420 6e6f 7420 6973 5f6f 7574  " and not is_out
-00011510: 7369 6465 2920 6f72 2028 6368 6172 203d  side) or (char =
-00011520: 3d20 2229 2220 616e 6420 6973 5f6f 7574  = ")" and is_out
-00011530: 7369 6465 2920 3a0d 0a20 2020 2020 2020  side) :..       
-00011540: 2020 2020 2065 7272 6f72 2822 4572 726f       error("Erro
-00011550: 725b 6765 745f 6772 6f75 7069 6e67 5f69  r[get_grouping_i
-00011560: 6e66 6f5d 3a20 4e6f 206e 6573 7465 6420  nfo]: No nested 
-00011570: 7061 7265 6e74 6865 7369 7320 616c 6c6f  parenthesis allo
-00011580: 7765 6421 2229 0d0a 2020 2020 2020 2020  wed!")..        
-00011590: 0d0a 2020 2020 2020 2020 6966 2069 735f  ..        if is_
-000115a0: 6f75 7473 6964 6520 3a0d 0a20 2020 2020  outside :..     
-000115b0: 2020 2020 2020 2023 6164 6420 616e 2065         #add an e
-000115c0: 6c65 6d65 6e74 206f 6620 6a75 7374 206f  lement of just o
-000115d0: 6e65 2069 6e64 6578 0d0a 2020 2020 2020  ne index..      
-000115e0: 2020 2020 2020 6772 6f75 705f 696e 666f        group_info
-000115f0: 202b 3d20 5b0d 0a20 2020 2020 2020 2020   += [..         
-00011600: 2020 2020 2020 205b 2063 6861 722c 205b         [ char, [
-00011610: 756e 6772 6f75 705f 7374 6174 5b6c 6f63  ungroup_stat[loc
-00011620: 6174 696f 6e5d 5d2c 205b 756e 6772 6f75  ation]], [ungrou
-00011630: 705f 7368 6170 655b 6c6f 6361 7469 6f6e  p_shape[location
-00011640: 5d5d 205d 0d0a 2020 2020 2020 2020 2020  ]] ]..          
-00011650: 2020 5d0d 0a20 2020 2020 2020 2065 6c73    ]..        els
-00011660: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00011670: 6e20 3d20 6c65 6e28 6772 6f75 705f 696e  n = len(group_in
-00011680: 666f 292d 310d 0a20 2020 2020 2020 2020  fo)-1..         
-00011690: 2020 2067 726f 7570 5f69 6e66 6f5b 6e5d     group_info[n]
-000116a0: 5b30 5d20 2b3d 2063 6861 720d 0a20 2020  [0] += char..   
-000116b0: 2020 2020 2020 2020 2067 726f 7570 5f69           group_i
-000116c0: 6e66 6f5b 6e5d 5b31 5d20 2b3d 205b 756e  nfo[n][1] += [un
-000116d0: 6772 6f75 705f 7374 6174 5b6c 6f63 6174  group_stat[locat
-000116e0: 696f 6e5d 5d0d 0a20 2020 2020 2020 2020  ion]]..         
-000116f0: 2020 2067 726f 7570 5f69 6e66 6f5b 6e5d     group_info[n]
-00011700: 5b32 5d20 2b3d 205b 756e 6772 6f75 705f  [2] += [ungroup_
-00011710: 7368 6170 655b 6c6f 6361 7469 6f6e 5d5d  shape[location]]
-00011720: 0d0a 2020 2020 2020 2020 6c6f 6361 7469  ..        locati
-00011730: 6f6e 202b 3d20 310d 0a20 2020 2066 6f72  on += 1..    for
-00011740: 206e 2069 6e20 7261 6e67 6528 6c65 6e28   n in range(len(
-00011750: 6772 6f75 705f 696e 666f 2929 203a 0d0a  group_info)) :..
-00011760: 2020 2020 2020 2020 6772 6f75 705f 696e          group_in
-00011770: 666f 5b6e 5d5b 315d 203d 206d 616b 655f  fo[n][1] = make_
-00011780: 7475 706c 6528 6772 6f75 705f 696e 666f  tuple(group_info
-00011790: 5b6e 5d5b 315d 290d 0a20 2020 2020 2020  [n][1])..       
-000117a0: 2067 726f 7570 5f69 6e66 6f5b 6e5d 5b32   group_info[n][2
-000117b0: 5d20 3d20 6d61 6b65 5f74 7570 6c65 2867  ] = make_tuple(g
-000117c0: 726f 7570 5f69 6e66 6f5b 6e5d 5b32 5d29  roup_info[n][2])
-000117d0: 0d0a 2020 2020 0d0a 2020 2020 2370 7269  ..    ..    #pri
-000117e0: 6e74 2822 6772 6f75 705f 696e 666f 3a22  nt("group_info:"
-000117f0: 290d 0a20 2020 2023 666f 7220 656c 656d  )..    #for elem
-00011800: 2069 6e20 6772 6f75 705f 696e 666f 3a0d   in group_info:.
-00011810: 0a20 2020 2023 2020 2020 7072 696e 7428  .    #    print(
-00011820: 656c 656d 290d 0a20 2020 2020 2020 200d  elem)..        .
-00011830: 0a20 2020 2023 206d 616b 6520 7468 6520  .    # make the 
-00011840: 736f 7274 6564 5f67 726f 7570 5f69 6e66  sorted_group_inf
-00011850: 6f20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  o --------------
-00011860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011880: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2073 6f72  -------..    sor
-00011890: 7465 645f 6772 6f75 705f 696e 666f 203d  ted_group_info =
-000118a0: 205b 5d0d 0a20 2020 2066 6f72 205b 696e   []..    for [in
-000118b0: 6469 6365 732c 2073 7461 7473 2c20 7368  dices, stats, sh
-000118c0: 6170 655d 2069 6e20 6772 6f75 705f 696e  ape] in group_in
-000118d0: 666f 203a 0d0a 2020 2020 2020 2020 6420  fo :..        d 
-000118e0: 3d20 6c65 6e28 696e 6469 6365 7329 0d0a  = len(indices)..
-000118f0: 2020 2020 2020 2020 736f 7274 6564 5f69          sorted_i
-00011900: 6e64 6963 6573 203d 2022 220d 0a20 2020  ndices = ""..   
-00011910: 2020 2020 2073 6f72 7465 645f 7374 6174       sorted_stat
-00011920: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-00011930: 736f 7274 6564 5f73 6861 7065 203d 205b  sorted_shape = [
-00011940: 5d0d 0a20 2020 2020 2020 2066 6f72 2069  ]..        for i
-00011950: 2069 6e20 7261 6e67 6528 6429 3a0d 0a20   in range(d):.. 
-00011960: 2020 2020 2020 2020 2020 2069 6620 7374             if st
-00011970: 6174 735b 695d 2069 6e20 626f 7365 5f74  ats[i] in bose_t
-00011980: 7970 653a 0d0a 2020 2020 2020 2020 2020  ype:..          
-00011990: 2020 2020 2020 736f 7274 6564 5f69 6e64        sorted_ind
-000119a0: 6963 6573 203d 2069 6e64 6963 6573 5b69  ices = indices[i
-000119b0: 5d20 2b20 736f 7274 6564 5f69 6e64 6963  ] + sorted_indic
-000119c0: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
-000119d0: 2020 2020 736f 7274 6564 5f73 7461 7473      sorted_stats
-000119e0: 203d 205b 7374 6174 735b 695d 5d20 2b20   = [stats[i]] + 
-000119f0: 736f 7274 6564 5f73 7461 7473 0d0a 2020  sorted_stats..  
-00011a00: 2020 2020 2020 2020 2020 2020 2020 736f                so
-00011a10: 7274 6564 5f73 6861 7065 203d 205b 7368  rted_shape = [sh
-00011a20: 6170 655b 695d 5d20 2b20 736f 7274 6564  ape[i]] + sorted
-00011a30: 5f73 6861 7065 0d0a 2020 2020 2020 2020  _shape..        
-00011a40: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00011a50: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
-00011a60: 645f 696e 6469 6365 7320 3d20 736f 7274  d_indices = sort
-00011a70: 6564 5f69 6e64 6963 6573 202b 2069 6e64  ed_indices + ind
-00011a80: 6963 6573 5b69 5d0d 0a20 2020 2020 2020  ices[i]..       
-00011a90: 2020 2020 2020 2020 2073 6f72 7465 645f           sorted_
-00011aa0: 7374 6174 7320 3d20 736f 7274 6564 5f73  stats = sorted_s
-00011ab0: 7461 7473 202b 205b 7374 6174 735b 695d  tats + [stats[i]
-00011ac0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00011ad0: 2020 2073 6f72 7465 645f 7368 6170 6520     sorted_shape 
-00011ae0: 3d20 736f 7274 6564 5f73 6861 7065 202b  = sorted_shape +
-00011af0: 205b 7368 6170 655b 695d 5d0d 0a20 2020   [shape[i]]..   
-00011b00: 2020 2020 2073 6f72 7465 645f 6772 6f75       sorted_grou
-00011b10: 705f 696e 666f 202b 3d20 5b5b 2073 6f72  p_info += [[ sor
-00011b20: 7465 645f 696e 6469 6365 732c 6d61 6b65  ted_indices,make
-00011b30: 5f74 7570 6c65 2873 6f72 7465 645f 7374  _tuple(sorted_st
-00011b40: 6174 7329 2c6d 616b 655f 7475 706c 6528  ats),make_tuple(
-00011b50: 736f 7274 6564 5f73 6861 7065 2920 5d5d  sorted_shape) ]]
-00011b60: 0d0a 2020 2020 0d0a 2020 2020 2370 7269  ..    ..    #pri
-00011b70: 6e74 2822 736f 7274 6564 5f67 726f 7570  nt("sorted_group
-00011b80: 5f69 6e66 6f3a 2229 0d0a 2020 2020 2366  _info:")..    #f
-00011b90: 6f72 2065 6c65 6d20 696e 2073 6f72 7465  or elem in sorte
-00011ba0: 645f 6772 6f75 705f 696e 666f 3a0d 0a20  d_group_info:.. 
-00011bb0: 2020 2023 2020 2020 7072 696e 7428 656c     #    print(el
-00011bc0: 656d 290d 0a20 2020 200d 0a20 2020 2072  em)..    ..    r
-00011bd0: 6574 7572 6e20 6772 6f75 705f 696e 666f  eturn group_info
-00011be0: 2c20 736f 7274 6564 5f67 726f 7570 5f69  , sorted_group_i
-00011bf0: 6e66 6f0d 0a20 2020 200d 0a64 6566 2067  nfo..    ..def g
-00011c00: 6574 5f67 726f 7570 696e 675f 7369 676e  et_grouping_sign
-00011c10: 5f66 6163 746f 7273 2873 6f72 7465 645f  _factors(sorted_
-00011c20: 6772 6f75 705f 696e 666f 2c20 696e 7465  group_info, inte
-00011c30: 726d 6564 6961 7465 5f73 7461 7429 3a0d  rmediate_stat):.
-00011c40: 0a20 2020 2023 7072 696e 7428 696e 7465  .    #print(inte
-00011c50: 726d 6564 6961 7465 5f73 7461 7429 0d0a  rmediate_stat)..
-00011c60: 2020 2020 0d0a 2020 2020 6966 206c 656e      ..    if len
-00011c70: 2873 6f72 7465 645f 6772 6f75 705f 696e  (sorted_group_in
-00011c80: 666f 2920 213d 206c 656e 2869 6e74 6572  fo) != len(inter
-00011c90: 6d65 6469 6174 655f 7374 6174 2920 3a0d  mediate_stat) :.
-00011ca0: 0a20 2020 2020 2020 2065 7272 6f72 2822  .        error("
-00011cb0: 4572 726f 725b 6765 745f 6772 6f75 7069  Error[get_groupi
-00011cc0: 6e67 5f73 6967 6e5f 6661 6374 6f72 735d  ng_sign_factors]
-00011cd0: 3a20 496e 636f 6e73 6973 7465 6e74 206e  : Inconsistent n
-00011ce0: 756d 6265 7220 6f66 2069 6e74 6572 6d65  umber of interme
-00011cf0: 6469 6174 655f 7374 6174 2061 6e64 2067  diate_stat and g
-00011d00: 726f 7570 696e 6773 2122 290d 0a20 2020  roupings!")..   
-00011d10: 200d 0a20 2020 2073 6967 6e5f 6661 6374   ..    sign_fact
-00011d20: 6f72 735f 696e 666f 203d 205b 2022 2220  ors_info = [ "" 
-00011d30: 2c20 5b5d 205d 2023 696e 6469 6365 7320  , [] ] #indices 
-00011d40: 616e 6420 6469 6d65 6e73 696f 6e73 0d0a  and dimensions..
-00011d50: 2020 2020 666f 7220 692c 5b73 7472 696e      for i,[strin
-00011d60: 6773 2c73 7461 7473 2c73 6861 7065 735d  gs,stats,shapes]
-00011d70: 2069 6e20 656e 756d 6572 6174 6528 736f   in enumerate(so
-00011d80: 7274 6564 5f67 726f 7570 5f69 6e66 6f29  rted_group_info)
-00011d90: 3a0d 0a20 2020 2020 2020 200d 0a20 2020  :..        ..   
-00011da0: 2020 2020 2066 6f72 2064 2069 6e20 7261       for d in ra
-00011db0: 6e67 6528 6c65 6e28 7374 6174 7329 293a  nge(len(stats)):
-00011dc0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00011dd0: 2073 7461 7473 5b64 5d20 3d3d 2031 2061   stats[d] == 1 a
-00011de0: 6e64 2069 6e74 6572 6d65 6469 6174 655f  nd intermediate_
-00011df0: 7374 6174 5b69 5d20 3d3d 202d 3120 3a0d  stat[i] == -1 :.
-00011e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011e10: 2073 6967 6e5f 6661 6374 6f72 735f 696e   sign_factors_in
-00011e20: 666f 5b30 5d20 2b3d 2022 2c22 2b73 7472  fo[0] += ","+str
-00011e30: 696e 6773 5b64 5d0d 0a20 2020 2020 2020  ings[d]..       
-00011e40: 2020 2020 2020 2020 2073 6967 6e5f 6661           sign_fa
-00011e50: 6374 6f72 735f 696e 666f 5b31 5d20 2b3d  ctors_info[1] +=
-00011e60: 205b 7368 6170 6573 5b64 5d5d 0d0a 2020   [shapes[d]]..  
-00011e70: 2020 2020 2020 2370 7269 6e74 2873 7461        #print(sta
-00011e80: 7473 2c22 2d2d 2d3e 222c 696e 7465 726d  ts,"--->",interm
-00011e90: 6564 6961 7465 5f73 7461 745b 695d 290d  ediate_stat[i]).
-00011ea0: 0a20 2020 200d 0a20 2020 2023 7072 696e  .    ..    #prin
-00011eb0: 7428 7369 676e 5f66 6163 746f 7273 5f69  t(sign_factors_i
-00011ec0: 6e66 6f29 0d0a 2020 2020 0d0a 2020 2020  nfo)..    ..    
-00011ed0: 2320 6765 6e65 7261 7465 2074 6865 2073  # generate the s
-00011ee0: 6967 6e20 6661 6374 6f72 2074 656e 736f  ign factor tenso
-00011ef0: 7220 2873 6570 6172 6174 656c 7929 0d0a  r (separately)..
-00011f00: 2020 2020 7369 676e 5f66 6163 746f 7273      sign_factors
-00011f10: 5f6c 6973 7420 3d20 5b20 7369 676e 5f66  _list = [ sign_f
-00011f20: 6163 746f 7273 5f69 6e66 6f5b 305d 2c20  actors_info[0], 
-00011f30: 5b5d 205d 0d0a 2020 2020 666f 7220 6420  [] ]..    for d 
-00011f40: 696e 2073 6967 6e5f 6661 6374 6f72 735f  in sign_factors_
-00011f50: 696e 666f 5b31 5d20 3a0d 0a20 2020 2020  info[1] :..     
-00011f60: 2020 2073 676e 203d 206e 702e 6172 7261     sgn = np.arra
-00011f70: 7928 5b20 282d 3129 2a2a 7061 7261 6d2e  y([ (-1)**param.
-00011f80: 6770 6172 6974 7928 696e 6429 2066 6f72  gparity(ind) for
-00011f90: 2069 6e64 2069 6e20 7261 6e67 6528 6429   ind in range(d)
-00011fa0: 205d 290d 0a20 2020 2020 2020 2073 6967   ])..        sig
-00011fb0: 6e5f 6661 6374 6f72 735f 6c69 7374 5b31  n_factors_list[1
-00011fc0: 5d20 2b3d 205b 7367 6e5d 0d0a 2020 2020  ] += [sgn]..    
-00011fd0: 0d0a 2020 2020 2370 7269 6e74 2873 6967  ..    #print(sig
-00011fe0: 6e5f 6661 6374 6f72 735f 6c69 7374 290d  n_factors_list).
-00011ff0: 0a20 2020 200d 0a20 2020 2072 6574 7572  .    ..    retur
-00012000: 6e20 7369 676e 5f66 6163 746f 7273 5f6c  n sign_factors_l
-00012010: 6973 740d 0a0d 0a64 6566 2067 6574 5f69  ist....def get_i
-00012020: 6e74 6572 6d65 6469 6174 655f 696e 666f  ntermediate_info
-00012030: 2873 6f72 7465 645f 6772 6f75 705f 696e  (sorted_group_in
-00012040: 666f 2c69 6e74 6572 6d65 6469 6174 655f  fo,intermediate_
-00012050: 7374 6174 293a 0d0a 2020 2020 6e65 775f  stat):..    new_
-00012060: 7368 6170 6520 3d20 5b5d 0d0a 2020 2020  shape = []..    
-00012070: 6e65 775f 7374 6174 7320 3d20 5b5d 0d0a  new_stats = []..
-00012080: 2020 2020 6669 6e61 6c5f 7368 6170 6520      final_shape 
-00012090: 3d20 5b5d 0d0a 2020 2020 6669 6e61 6c5f  = []..    final_
-000120a0: 7374 6174 7320 3d20 5b5d 0d0a 2020 2020  stats = []..    
-000120b0: 0d0a 2020 2020 6966 206c 656e 2873 6f72  ..    if len(sor
-000120c0: 7465 645f 6772 6f75 705f 696e 666f 2920  ted_group_info) 
-000120d0: 213d 206c 656e 2869 6e74 6572 6d65 6469  != len(intermedi
-000120e0: 6174 655f 7374 6174 293a 0d0a 2020 2020  ate_stat):..    
-000120f0: 2020 2020 6572 726f 7228 2245 7272 6f72      error("Error
-00012100: 5b67 6574 5f69 6e74 6572 6d65 6469 6174  [get_intermediat
-00012110: 655f 696e 666f 5d3a 2049 6e63 6f6e 7369  e_info]: Inconsi
-00012120: 7374 656e 7420 6e75 6d62 6572 206f 6620  stent number of 
-00012130: 696e 7465 726d 6564 6961 7465 5f73 7461  intermediate_sta
-00012140: 7420 616e 6420 6772 6f75 7069 6e67 7321  t and groupings!
-00012150: 2229 0d0a 2020 2020 666f 7220 692c 5b69  ")..    for i,[i
-00012160: 6e64 6963 6573 2c20 7374 6174 732c 2073  ndices, stats, s
-00012170: 6861 7065 5d20 696e 2065 6e75 6d65 7261  hape] in enumera
-00012180: 7465 2873 6f72 7465 645f 6772 6f75 705f  te(sorted_group_
-00012190: 696e 666f 293a 0d0a 2020 2020 2020 2020  info):..        
-000121a0: 6665 726d 695f 6420 3d20 310d 0a20 2020  fermi_d = 1..   
-000121b0: 2020 2020 2062 6f73 655f 6420 203d 2031       bose_d  = 1
-000121c0: 0d0a 2020 2020 2020 2020 6665 726d 695f  ..        fermi_
-000121d0: 6e20 3d20 300d 0a20 2020 2020 2020 2062  n = 0..        b
-000121e0: 6f73 655f 6e20 203d 2030 0d0a 2020 2020  ose_n  = 0..    
-000121f0: 2020 2020 666f 7220 6420 696e 2072 616e      for d in ran
-00012200: 6765 286c 656e 2873 7461 7473 2929 3a0d  ge(len(stats)):.
-00012210: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00012220: 7374 6174 735b 645d 2069 6e20 6665 726d  stats[d] in ferm
-00012230: 695f 7479 7065 203a 0d0a 2020 2020 2020  i_type :..      
-00012240: 2020 2020 2020 2020 2020 6665 726d 695f            fermi_
-00012250: 6420 2a3d 2073 6861 7065 5b64 5d0d 0a20  d *= shape[d].. 
-00012260: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00012270: 6572 6d69 5f6e 202b 3d20 310d 0a20 2020  ermi_n += 1..   
-00012280: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00012290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122a0: 626f 7365 5f64 202a 3d20 7368 6170 655b  bose_d *= shape[
-000122b0: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
-000122c0: 2020 2020 626f 7365 5f6e 202b 3d20 310d      bose_n += 1.
-000122d0: 0a20 2020 2020 2020 2069 6620 626f 7365  .        if bose
-000122e0: 5f6e 203e 2030 203a 0d0a 2020 2020 2020  _n > 0 :..      
-000122f0: 2020 2020 2020 6e65 775f 7368 6170 6520        new_shape 
-00012300: 2b3d 205b 626f 7365 5f64 5d0d 0a20 2020  += [bose_d]..   
-00012310: 2020 2020 2020 2020 206e 6577 5f73 7461           new_sta
-00012320: 7473 202b 3d20 5b30 5d0d 0a20 2020 2020  ts += [0]..     
-00012330: 2020 2069 6620 6665 726d 695f 6e20 3e20     if fermi_n > 
-00012340: 3020 3a0d 0a20 2020 2020 2020 2020 2020  0 :..           
-00012350: 206e 6577 5f73 6861 7065 202b 3d20 5b66   new_shape += [f
-00012360: 6572 6d69 5f64 5d0d 0a20 2020 2020 2020  ermi_d]..       
-00012370: 2020 2020 206e 6577 5f73 7461 7473 202b       new_stats +
-00012380: 3d20 5b69 6e74 6572 6d65 6469 6174 655f  = [intermediate_
-00012390: 7374 6174 5b69 5d5d 0d0a 2020 2020 2020  stat[i]]..      
-000123a0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-000123b0: 6669 6e61 6c5f 7368 6170 6520 2b3d 205b  final_shape += [
-000123c0: 626f 7365 5f64 2a66 6572 6d69 5f64 5d0d  bose_d*fermi_d].
-000123d0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-000123e0: 2020 2069 6620 626f 7365 5f6e 203e 2030     if bose_n > 0
-000123f0: 2061 6e64 2066 6572 6d69 5f6e 203e 2030   and fermi_n > 0
-00012400: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
-00012410: 6669 6e61 6c5f 7374 6174 7320 2b3d 205b  final_stats += [
-00012420: 6879 6272 6964 5f73 796d 626f 6c5d 0d0a  hybrid_symbol]..
-00012430: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00012440: 2020 2020 2020 2020 2020 2066 696e 616c             final
-00012450: 5f73 7461 7473 202b 3d20 5b69 6e74 6572  _stats += [inter
-00012460: 6d65 6469 6174 655f 7374 6174 5b69 5d5d  mediate_stat[i]]
-00012470: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-00012480: 2020 2020 6e65 775f 7374 6174 7320 3d20      new_stats = 
-00012490: 6d61 6b65 5f74 7570 6c65 286e 6577 5f73  make_tuple(new_s
-000124a0: 7461 7473 290d 0a20 2020 206e 6577 5f73  tats)..    new_s
-000124b0: 6861 7065 203d 206d 616b 655f 7475 706c  hape = make_tupl
-000124c0: 6528 6e65 775f 7368 6170 6529 0d0a 2020  e(new_shape)..  
-000124d0: 2020 6669 6e61 6c5f 7374 6174 7320 3d20    final_stats = 
-000124e0: 6d61 6b65 5f74 7570 6c65 2866 696e 616c  make_tuple(final
-000124f0: 5f73 7461 7473 290d 0a20 2020 2066 696e  _stats)..    fin
-00012500: 616c 5f73 6861 7065 203d 206d 616b 655f  al_shape = make_
-00012510: 7475 706c 6528 6669 6e61 6c5f 7368 6170  tuple(final_shap
-00012520: 6529 0d0a 2020 2020 0d0a 2020 2020 7265  e)..    ..    re
-00012530: 7475 726e 206e 6577 5f73 7461 7473 2c20  turn new_stats, 
-00012540: 6e65 775f 7368 6170 652c 2066 696e 616c  new_shape, final
-00012550: 5f73 7461 7473 2c20 6669 6e61 6c5f 7368  _stats, final_sh
-00012560: 6170 650d 0a0d 0a23 2323 2323 2323 2323  ape....#########
-00012570: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012580: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012590: 2323 2323 2323 2323 2323 230d 0a23 2320  ###########..## 
-000125a0: 2020 2020 2020 2020 2054 7269 6d20 7468           Trim th
-000125b0: 6520 4772 6173 736d 616e 6e2d 6f64 6420  e Grassmann-odd 
-000125c0: 7061 7274 7320 2020 2020 2020 2020 2023  parts          #
-000125d0: 230d 0a23 2320 2020 2020 2020 2020 2020  #..##           
-000125e0: 2020 2020 2866 6f72 2074 6573 7469 6e67      (for testing
-000125f0: 206f 6e6c 7929 2020 2020 2020 2020 2020   only)          
-00012600: 2020 2020 2023 230d 0a23 2323 2323 2323       ##..#######
-00012610: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012620: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012630: 2323 2323 2323 2323 2323 2323 230d 0a0d  #############...
-00012640: 0a64 6566 2074 7269 6d5f 6772 6173 736d  .def trim_grassm
-00012650: 616e 6e5f 6f64 6428 4f62 6a29 3a0d 0a20  ann_odd(Obj):.. 
-00012660: 2020 206f 626a 7479 7065 3d74 7970 6528     objtype=type(
-00012670: 4f62 6a29 0d0a 0d0a 2020 2020 6966 284f  Obj)....    if(O
-00012680: 626a 2e65 6e63 6f64 6572 203d 3d20 2763  bj.encoder == 'c
-00012690: 616e 6f6e 6963 616c 2729 3a0d 0a20 2020  anonical'):..   
-000126a0: 2020 2020 204f 626a 203d 204f 626a 2e73       Obj = Obj.s
-000126b0: 7769 7463 685f 656e 636f 6465 7228 7361  witch_encoder(sa
-000126c0: 7665 5f6d 656d 6f72 793d 5472 7565 290d  ve_memory=True).
-000126d0: 0a20 2020 2020 2020 200d 0a20 2020 2069  .        ..    i
-000126e0: 6628 6f62 6a74 7970 653d 3d64 656e 7365  f(objtype==dense
-000126f0: 293a 0d0a 2020 2020 2020 2020 4f62 6a20  ):..        Obj 
-00012700: 3d20 7370 6172 7365 284f 626a 290d 0a20  = sparse(Obj).. 
-00012710: 2020 2043 203d 204f 626a 2e63 6f6f 7264     C = Obj.coord
-00012720: 730d 0a20 2020 2070 7269 6e74 2829 2023  s..    print() #
-00012730: 203c 3c20 446f 6e27 7420 7265 6d6f 7665   << Don't remove
-00012740: 2074 6869 732e 2054 6869 7320 6973 2066   this. This is f
-00012750: 6f72 2074 6865 2073 686f 775f 7072 6f67  or the show_prog
-00012760: 7265 7373 210d 0a20 2020 2073 3020 3d20  ress!..    s0 = 
-00012770: 7469 6d65 2e74 696d 6528 290d 0a20 2020  time.time()..   
-00012780: 2073 3030 203d 2073 300d 0a20 2020 2066   s00 = s0..    f
-00012790: 6f72 2069 2069 6e20 7261 6e67 6528 4f62  or i in range(Ob
-000127a0: 6a2e 6e6e 7a29 3a0d 0a20 2020 2020 2020  j.nnz):..       
-000127b0: 2066 636f 6f72 6473 203d 205b 2069 6e64   fcoords = [ ind
-000127c0: 2066 6f72 206a 2c69 6e64 2069 6e20 656e   for j,ind in en
-000127d0: 756d 6572 6174 6528 435b 695d 2920 6966  umerate(C[i]) if
-000127e0: 2028 4f62 6a2e 7374 6174 6973 7469 635b   (Obj.statistic[
-000127f0: 6a5d 2069 6e20 6665 726d 695f 7479 7065  j] in fermi_type
-00012800: 295d 0d0a 2020 2020 2020 2020 6966 2873  )]..        if(s
-00012810: 756d 2866 636f 6f72 6473 2925 3220 3d3d  um(fcoords)%2 ==
-00012820: 2031 293a 0d0a 2020 2020 2020 2020 2020   1):..          
-00012830: 2020 4f62 6a2e 6461 7461 2e64 6174 615b    Obj.data.data[
-00012840: 695d 203d 2030 0d0a 0d0a 2020 2020 2020  i] = 0....      
-00012850: 2020 6966 2074 696d 652e 7469 6d65 2829    if time.time()
-00012860: 2d73 3020 3e20 302e 3520 3a0d 0a20 2020  -s0 > 0.5 :..   
-00012870: 2020 2020 2020 2020 2073 686f 775f 7072           show_pr
-00012880: 6f67 7265 7373 2869 2c4f 626a 2e6e 6e7a  ogress(i,Obj.nnz
-00012890: 2c22 7472 696d 5f67 7261 7373 6d61 6e6e  ,"trim_grassmann
-000128a0: 5f6f 6464 222c 7469 6d65 3d74 696d 652e  _odd",time=time.
-000128b0: 7469 6d65 2829 2d73 3030 290d 0a0d 0a20  time()-s00).... 
-000128c0: 2020 2063 6c65 6172 5f70 726f 6772 6573     clear_progres
-000128d0: 7328 290d 0a20 2020 2073 7973 2e73 7464  s()..    sys.std
-000128e0: 6f75 742e 7772 6974 6528 225c 3033 335b  out.write("\033[
-000128f0: 4622 290d 0a0d 0a0d 0a20 2020 2069 6628  F")......    if(
-00012900: 6f62 6a74 7970 653d 3d64 656e 7365 293a  objtype==dense):
-00012910: 0d0a 2020 2020 2020 2020 4f62 6a20 3d20  ..        Obj = 
-00012920: 6465 6e73 6528 4f62 6a29 0d0a 0d0a 2020  dense(Obj)....  
-00012930: 2020 6966 284f 626a 5f69 6e70 7574 2e65    if(Obj_input.e
-00012940: 6e63 6f64 6572 203d 3d20 2763 616e 6f6e  ncoder == 'canon
-00012950: 6963 616c 2729 3a0d 0a20 2020 2020 2020  ical'):..       
-00012960: 204f 626a 203d 204f 626a 2e73 7769 7463   Obj = Obj.switc
-00012970: 685f 656e 636f 6465 7228 7361 7665 5f6d  h_encoder(save_m
-00012980: 656d 6f72 793d 5472 7565 290d 0a0d 0a20  emory=True).... 
-00012990: 2020 2072 6574 7572 6e20 4f62 6a0d 0a0d     return Obj...
-000129a0: 0a64 6566 2069 735f 6772 6173 736d 616e  .def is_grassman
-000129b0: 6e5f 6576 656e 284f 626a 293a 0d0a 2020  n_even(Obj):..  
-000129c0: 2020 6966 204f 626a 2e65 6e63 6f64 6572    if Obj.encoder
-000129d0: 203d 3d20 2763 616e 6f6e 6963 616c 273a   == 'canonical':
+00010cf0: 3d3d 230d 0a20 2020 200d 0a20 2020 2075  ==#..    ..    u
+00010d00: 6e73 6f72 7465 645f 7374 7269 6e67 203d  nsorted_string =
+00010d10: 2027 272e 6a6f 696e 2820 5b20 696e 6469   ''.join( [ indi
+00010d20: 6365 7320 666f 7220 5b69 6e64 6963 6573  ces for [indices
+00010d30: 2c20 7374 6174 732c 2073 6861 7065 5d20  , stats, shape] 
+00010d40: 696e 2067 726f 7570 5f69 6e66 6f20 5d20  in group_info ] 
+00010d50: 290d 0a20 2020 2073 6f72 7465 645f 7374  )..    sorted_st
+00010d60: 7269 6e67 203d 2027 272e 6a6f 696e 2820  ring = ''.join( 
+00010d70: 5b20 696e 6469 6365 7320 666f 7220 5b69  [ indices for [i
+00010d80: 6e64 6963 6573 2c20 7374 6174 732c 2073  ndices, stats, s
+00010d90: 6861 7065 5d20 696e 2073 6f72 7465 645f  hape] in sorted_
+00010da0: 6772 6f75 705f 696e 666f 205d 2029 0d0a  group_info ] )..
+00010db0: 2020 2020 6e70 6569 6e73 756d 5f73 7472      npeinsum_str
+00010dc0: 696e 6720 3d20 736f 7274 6564 5f73 7472  ing = sorted_str
+00010dd0: 696e 672b 7369 676e 5f66 6163 746f 7273  ing+sign_factors
+00010de0: 5f6c 6973 745b 305d 2b22 2d3e 222b 756e  _list[0]+"->"+un
+00010df0: 736f 7274 6564 5f73 7472 696e 670d 0a20  sorted_string.. 
+00010e00: 2020 206e 7065 696e 7375 6d5f 6f62 6a20     npeinsum_obj 
+00010e10: 3d20 5b4f 626a 2e64 6174 615d 202b 2073  = [Obj.data] + s
+00010e20: 6967 6e5f 6661 6374 6f72 735f 6c69 7374  ign_factors_list
+00010e30: 5b31 5d0d 0a20 2020 204f 626a 2e64 6174  [1]..    Obj.dat
+00010e40: 6120 3d20 6f65 2e63 6f6e 7472 6163 7428  a = oe.contract(
+00010e50: 2a6d 616b 655f 7475 706c 6528 205b 6e70  *make_tuple( [np
+00010e60: 6569 6e73 756d 5f73 7472 696e 675d 202b  einsum_string] +
+00010e70: 206e 7065 696e 7375 6d5f 6f62 6a20 2929   npeinsum_obj ))
+00010e80: 0d0a 2020 2020 4f62 6a2e 7374 6174 6973  ..    Obj.statis
+00010e90: 7469 6320 3d20 6669 6e61 6c5f 7374 6174  tic = final_stat
+00010ea0: 0d0a 2020 2020 0d0a 2020 2020 636c 6561  ..    ..    clea
+00010eb0: 725f 7072 6f67 7265 7373 2829 0d0a 2020  r_progress()..  
+00010ec0: 2020 7461 625f 7570 2829 0d0a 0d0a 2020    tab_up()....  
+00010ed0: 2020 6966 2074 6869 735f 666f 726d 6174    if this_format
+00010ee0: 3d3d 276d 6174 7269 7827 3a0d 0a20 2020  =='matrix':..   
+00010ef0: 2020 2020 2072 6574 7572 6e20 4f62 6a2e       return Obj.
+00010f00: 7377 6974 6368 5f66 6f72 6d61 7428 7361  switch_format(sa
+00010f10: 7665 5f6d 656d 6f72 793d 5472 7565 290d  ve_memory=True).
+00010f20: 0a20 2020 200d 0a20 2020 2072 6574 7572  .    ..    retur
+00010f30: 6e20 4f62 6a0d 0a20 2020 200d 0a64 6566  n Obj..    ..def
+00010f40: 2067 6574 5f67 726f 7570 5f69 6e66 6f28   get_group_info(
+00010f50: 6772 6f75 7069 6e67 5f73 7472 696e 672c  grouping_string,
+00010f60: 2075 6e67 726f 7570 5f73 7461 742c 2075   ungroup_stat, u
+00010f70: 6e67 726f 7570 5f73 6861 7065 293a 0d0a  ngroup_shape):..
+00010f80: 2020 2020 2370 7269 6e74 2822 6f72 6967      #print("orig
+00010f90: 696e 616c 2073 7472 696e 673a 222c 6772  inal string:",gr
+00010fa0: 6f75 7069 6e67 5f73 7472 696e 6729 0d0a  ouping_string)..
+00010fb0: 2020 2020 666f 726d 6174 7465 645f 7374      formatted_st
+00010fc0: 7269 6e67 203d 2067 726f 7570 696e 675f  ring = grouping_
+00010fd0: 7374 7269 6e67 0d0a 2020 2020 0d0a 2020  string..    ..  
+00010fe0: 2020 2320 6368 6563 6b20 7468 6520 7374    # check the st
+00010ff0: 7269 6e67 2066 6f72 6d61 7420 2d2d 2d2d  ring format ----
+00011000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011030: 2d2d 2d2d 0d0a 2020 2020 6966 2066 6f72  ----..    if for
+00011040: 6d61 7474 6564 5f73 7472 696e 672e 636f  matted_string.co
+00011050: 756e 7428 2228 2229 203d 3d20 3020 616e  unt("(") == 0 an
+00011060: 6420 666f 726d 6174 7465 645f 7374 7269  d formatted_stri
+00011070: 6e67 2e63 6f75 6e74 2822 2922 2920 3d3d  ng.count(")") ==
+00011080: 2030 203a 0d0a 2020 2020 2020 2020 2374   0 :..        #t
+00011090: 6869 7320 6973 2074 6865 2061 6262 7265  his is the abbre
+000110a0: 7669 6174 6564 2066 6f72 6d61 740d 0a20  viated format.. 
+000110b0: 2020 2020 2020 2066 6f72 2073 6570 6172         for separ
+000110c0: 6174 6f72 2069 6e20 7365 7061 7261 746f  ator in separato
+000110d0: 725f 6c69 7374 3a0d 0a20 2020 2020 2020  r_list:..       
+000110e0: 2020 2020 2066 6f72 6d61 7474 6564 5f73       formatted_s
+000110f0: 7472 696e 6720 3d20 666f 726d 6174 7465  tring = formatte
+00011100: 645f 7374 7269 6e67 2e72 6570 6c61 6365  d_string.replace
+00011110: 2873 6570 6172 6174 6f72 2c22 2928 2229  (separator,")(")
+00011120: 0d0a 2020 2020 2020 2020 666f 726d 6174  ..        format
+00011130: 7465 645f 7374 7269 6e67 203d 2022 2822  ted_string = "("
+00011140: 2b66 6f72 6d61 7474 6564 5f73 7472 696e  +formatted_strin
+00011150: 672b 2229 220d 0a20 2020 2065 6c73 653a  g+")"..    else:
+00011160: 0d0a 2020 2020 2020 2020 7365 7061 7261  ..        separa
+00011170: 746f 725f 636f 756e 7420 3d20 300d 0a20  tor_count = 0.. 
+00011180: 2020 2020 2020 2066 6f72 2073 6570 6172         for separ
+00011190: 6174 6f72 2069 6e20 7365 7061 7261 746f  ator in separato
+000111a0: 725f 6c69 7374 3a0d 0a20 2020 2020 2020  r_list:..       
+000111b0: 2020 2020 2073 6570 6172 6174 6f72 5f63       separator_c
+000111c0: 6f75 6e74 202b 3d20 666f 726d 6174 7465  ount += formatte
+000111d0: 645f 7374 7269 6e67 2e63 6f75 6e74 2873  d_string.count(s
+000111e0: 6570 6172 6174 6f72 290d 0a20 2020 2020  eparator)..     
+000111f0: 2020 2069 6620 7365 7061 7261 746f 725f     if separator_
+00011200: 636f 756e 7420 3e20 3020 3a0d 0a20 2020  count > 0 :..   
+00011210: 2020 2020 2020 2020 2065 7272 6f72 2822           error("
+00011220: 4572 726f 725b 6765 745f 6772 6f75 7069  Error[get_groupi
+00011230: 6e67 5f69 6e66 6f5d 3a20 446f 206e 6f74  ng_info]: Do not
+00011240: 206d 6978 2074 6865 2073 7472 696e 6720   mix the string 
+00011250: 666f 726d 6174 2e22 290d 0a20 2020 2023  format.")..    #
+00011260: 7072 696e 7428 2266 6f72 6d61 7474 6564  print("formatted
+00011270: 2073 7472 696e 673a 222c 666f 726d 6174   string:",format
+00011280: 7465 645f 7374 7269 6e67 290d 0a20 2020  ted_string)..   
+00011290: 200d 0a20 2020 2023 2070 6172 7365 2074   ..    # parse t
+000112a0: 6865 2073 7472 696e 6720 2d2d 2d2d 2d2d  he string ------
+000112b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000112c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000112d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000112e0: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2067  ---------..    g
+000112f0: 726f 7570 5f69 6e66 6f20 3d20 5b5d 2023  roup_info = [] #
+00011300: 205b 7374 7269 6e67 2074 6578 742c 2073   [string text, s
+00011310: 7461 7469 7374 6963 2c20 7368 6170 655d  tatistic, shape]
+00011320: 0d0a 2020 2020 6973 5f6f 7574 7369 6465  ..    is_outside
+00011330: 203d 2054 7275 650d 0a20 2020 206c 6f63   = True..    loc
+00011340: 6174 696f 6e20 3d20 300d 0a20 2020 2066  ation = 0..    f
+00011350: 6f72 2063 6861 7220 696e 2066 6f72 6d61  or char in forma
+00011360: 7474 6564 5f73 7472 696e 673a 0d0a 2020  tted_string:..  
+00011370: 2020 2020 2020 6966 2063 6861 7220 3d3d        if char ==
+00011380: 2022 2822 2061 6e64 2069 735f 6f75 7473   "(" and is_outs
+00011390: 6964 6520 3a0d 0a20 2020 2020 2020 2020  ide :..         
+000113a0: 2020 2069 735f 6f75 7473 6964 6520 3d20     is_outside = 
+000113b0: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
+000113c0: 2020 2067 726f 7570 5f69 6e66 6f20 2b3d     group_info +=
+000113d0: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
+000113e0: 2020 2020 5b20 2222 2c20 5b5d 2c20 5b5d      [ "", [], []
+000113f0: 205d 2023 6d61 6b65 2061 2062 6c61 6e6b   ] #make a blank
+00011400: 2074 656d 706c 6174 6520 666f 7220 7468   template for th
+00011410: 6973 2067 726f 7570 0d0a 2020 2020 2020  is group..      
+00011420: 2020 2020 2020 5d0d 0a20 2020 2020 2020        ]..       
+00011430: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
+00011440: 2020 2020 2020 2069 6620 6368 6172 203d         if char =
+00011450: 3d20 2229 2220 616e 6420 6e6f 7420 6973  = ")" and not is
+00011460: 5f6f 7574 7369 6465 203a 0d0a 2020 2020  _outside :..    
+00011470: 2020 2020 2020 2020 6973 5f6f 7574 7369          is_outsi
+00011480: 6465 203d 2054 7275 650d 0a20 2020 2020  de = True..     
+00011490: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
+000114a0: 0a20 2020 2020 2020 2069 6620 2863 6861  .        if (cha
+000114b0: 7220 3d3d 2022 2822 2061 6e64 206e 6f74  r == "(" and not
+000114c0: 2069 735f 6f75 7473 6964 6529 206f 7220   is_outside) or 
+000114d0: 2863 6861 7220 3d3d 2022 2922 2061 6e64  (char == ")" and
+000114e0: 2069 735f 6f75 7473 6964 6529 203a 0d0a   is_outside) :..
+000114f0: 2020 2020 2020 2020 2020 2020 6572 726f              erro
+00011500: 7228 2245 7272 6f72 5b67 6574 5f67 726f  r("Error[get_gro
+00011510: 7570 696e 675f 696e 666f 5d3a 204e 6f20  uping_info]: No 
+00011520: 6e65 7374 6564 2070 6172 656e 7468 6573  nested parenthes
+00011530: 6973 2061 6c6c 6f77 6564 2122 290d 0a20  is allowed!").. 
+00011540: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00011550: 2069 6620 6973 5f6f 7574 7369 6465 203a   if is_outside :
+00011560: 0d0a 2020 2020 2020 2020 2020 2020 2361  ..            #a
+00011570: 6464 2061 6e20 656c 656d 656e 7420 6f66  dd an element of
+00011580: 206a 7573 7420 6f6e 6520 696e 6465 780d   just one index.
+00011590: 0a20 2020 2020 2020 2020 2020 2067 726f  .            gro
+000115a0: 7570 5f69 6e66 6f20 2b3d 205b 0d0a 2020  up_info += [..  
+000115b0: 2020 2020 2020 2020 2020 2020 2020 5b20                [ 
+000115c0: 6368 6172 2c20 5b75 6e67 726f 7570 5f73  char, [ungroup_s
+000115d0: 7461 745b 6c6f 6361 7469 6f6e 5d5d 2c20  tat[location]], 
+000115e0: 5b75 6e67 726f 7570 5f73 6861 7065 5b6c  [ungroup_shape[l
+000115f0: 6f63 6174 696f 6e5d 5d20 5d0d 0a20 2020  ocation]] ]..   
+00011600: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
+00011610: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00011620: 2020 2020 2020 206e 203d 206c 656e 2867         n = len(g
+00011630: 726f 7570 5f69 6e66 6f29 2d31 0d0a 2020  roup_info)-1..  
+00011640: 2020 2020 2020 2020 2020 6772 6f75 705f            group_
+00011650: 696e 666f 5b6e 5d5b 305d 202b 3d20 6368  info[n][0] += ch
+00011660: 6172 0d0a 2020 2020 2020 2020 2020 2020  ar..            
+00011670: 6772 6f75 705f 696e 666f 5b6e 5d5b 315d  group_info[n][1]
+00011680: 202b 3d20 5b75 6e67 726f 7570 5f73 7461   += [ungroup_sta
+00011690: 745b 6c6f 6361 7469 6f6e 5d5d 0d0a 2020  t[location]]..  
+000116a0: 2020 2020 2020 2020 2020 6772 6f75 705f            group_
+000116b0: 696e 666f 5b6e 5d5b 325d 202b 3d20 5b75  info[n][2] += [u
+000116c0: 6e67 726f 7570 5f73 6861 7065 5b6c 6f63  ngroup_shape[loc
+000116d0: 6174 696f 6e5d 5d0d 0a20 2020 2020 2020  ation]]..       
+000116e0: 206c 6f63 6174 696f 6e20 2b3d 2031 0d0a   location += 1..
+000116f0: 2020 2020 666f 7220 6e20 696e 2072 616e      for n in ran
+00011700: 6765 286c 656e 2867 726f 7570 5f69 6e66  ge(len(group_inf
+00011710: 6f29 2920 3a0d 0a20 2020 2020 2020 2067  o)) :..        g
+00011720: 726f 7570 5f69 6e66 6f5b 6e5d 5b31 5d20  roup_info[n][1] 
+00011730: 3d20 6d61 6b65 5f74 7570 6c65 2867 726f  = make_tuple(gro
+00011740: 7570 5f69 6e66 6f5b 6e5d 5b31 5d29 0d0a  up_info[n][1])..
+00011750: 2020 2020 2020 2020 6772 6f75 705f 696e          group_in
+00011760: 666f 5b6e 5d5b 325d 203d 206d 616b 655f  fo[n][2] = make_
+00011770: 7475 706c 6528 6772 6f75 705f 696e 666f  tuple(group_info
+00011780: 5b6e 5d5b 325d 290d 0a20 2020 200d 0a20  [n][2])..    .. 
+00011790: 2020 2023 7072 696e 7428 2267 726f 7570     #print("group
+000117a0: 5f69 6e66 6f3a 2229 0d0a 2020 2020 2366  _info:")..    #f
+000117b0: 6f72 2065 6c65 6d20 696e 2067 726f 7570  or elem in group
+000117c0: 5f69 6e66 6f3a 0d0a 2020 2020 2320 2020  _info:..    #   
+000117d0: 2070 7269 6e74 2865 6c65 6d29 0d0a 2020   print(elem)..  
+000117e0: 2020 2020 2020 0d0a 2020 2020 2320 6d61        ..    # ma
+000117f0: 6b65 2074 6865 2073 6f72 7465 645f 6772  ke the sorted_gr
+00011800: 6f75 705f 696e 666f 202d 2d2d 2d2d 2d2d  oup_info -------
+00011810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a  --------------..
+00011840: 2020 2020 736f 7274 6564 5f67 726f 7570      sorted_group
+00011850: 5f69 6e66 6f20 3d20 5b5d 0d0a 2020 2020  _info = []..    
+00011860: 666f 7220 5b69 6e64 6963 6573 2c20 7374  for [indices, st
+00011870: 6174 732c 2073 6861 7065 5d20 696e 2067  ats, shape] in g
+00011880: 726f 7570 5f69 6e66 6f20 3a0d 0a20 2020  roup_info :..   
+00011890: 2020 2020 2064 203d 206c 656e 2869 6e64       d = len(ind
+000118a0: 6963 6573 290d 0a20 2020 2020 2020 2073  ices)..        s
+000118b0: 6f72 7465 645f 696e 6469 6365 7320 3d20  orted_indices = 
+000118c0: 2222 0d0a 2020 2020 2020 2020 736f 7274  ""..        sort
+000118d0: 6564 5f73 7461 7473 203d 205b 5d0d 0a20  ed_stats = [].. 
+000118e0: 2020 2020 2020 2073 6f72 7465 645f 7368         sorted_sh
+000118f0: 6170 6520 3d20 5b5d 0d0a 2020 2020 2020  ape = []..      
+00011900: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00011910: 2864 293a 0d0a 2020 2020 2020 2020 2020  (d):..          
+00011920: 2020 6966 2073 7461 7473 5b69 5d20 696e    if stats[i] in
+00011930: 2062 6f73 655f 7479 7065 3a0d 0a20 2020   bose_type:..   
+00011940: 2020 2020 2020 2020 2020 2020 2073 6f72               sor
+00011950: 7465 645f 696e 6469 6365 7320 3d20 696e  ted_indices = in
+00011960: 6469 6365 735b 695d 202b 2073 6f72 7465  dices[i] + sorte
+00011970: 645f 696e 6469 6365 730d 0a20 2020 2020  d_indices..     
+00011980: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
+00011990: 645f 7374 6174 7320 3d20 5b73 7461 7473  d_stats = [stats
+000119a0: 5b69 5d5d 202b 2073 6f72 7465 645f 7374  [i]] + sorted_st
+000119b0: 6174 730d 0a20 2020 2020 2020 2020 2020  ats..           
+000119c0: 2020 2020 2073 6f72 7465 645f 7368 6170       sorted_shap
+000119d0: 6520 3d20 5b73 6861 7065 5b69 5d5d 202b  e = [shape[i]] +
+000119e0: 2073 6f72 7465 645f 7368 6170 650d 0a20   sorted_shape.. 
+000119f0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00011a00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011a10: 2020 736f 7274 6564 5f69 6e64 6963 6573    sorted_indices
+00011a20: 203d 2073 6f72 7465 645f 696e 6469 6365   = sorted_indice
+00011a30: 7320 2b20 696e 6469 6365 735b 695d 0d0a  s + indices[i]..
+00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a50: 736f 7274 6564 5f73 7461 7473 203d 2073  sorted_stats = s
+00011a60: 6f72 7465 645f 7374 6174 7320 2b20 5b73  orted_stats + [s
+00011a70: 7461 7473 5b69 5d5d 0d0a 2020 2020 2020  tats[i]]..      
+00011a80: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
+00011a90: 5f73 6861 7065 203d 2073 6f72 7465 645f  _shape = sorted_
+00011aa0: 7368 6170 6520 2b20 5b73 6861 7065 5b69  shape + [shape[i
+00011ab0: 5d5d 0d0a 2020 2020 2020 2020 736f 7274  ]]..        sort
+00011ac0: 6564 5f67 726f 7570 5f69 6e66 6f20 2b3d  ed_group_info +=
+00011ad0: 205b 5b20 736f 7274 6564 5f69 6e64 6963   [[ sorted_indic
+00011ae0: 6573 2c6d 616b 655f 7475 706c 6528 736f  es,make_tuple(so
+00011af0: 7274 6564 5f73 7461 7473 292c 6d61 6b65  rted_stats),make
+00011b00: 5f74 7570 6c65 2873 6f72 7465 645f 7368  _tuple(sorted_sh
+00011b10: 6170 6529 205d 5d0d 0a20 2020 200d 0a20  ape) ]]..    .. 
+00011b20: 2020 2023 7072 696e 7428 2273 6f72 7465     #print("sorte
+00011b30: 645f 6772 6f75 705f 696e 666f 3a22 290d  d_group_info:").
+00011b40: 0a20 2020 2023 666f 7220 656c 656d 2069  .    #for elem i
+00011b50: 6e20 736f 7274 6564 5f67 726f 7570 5f69  n sorted_group_i
+00011b60: 6e66 6f3a 0d0a 2020 2020 2320 2020 2070  nfo:..    #    p
+00011b70: 7269 6e74 2865 6c65 6d29 0d0a 2020 2020  rint(elem)..    
+00011b80: 0d0a 2020 2020 7265 7475 726e 2067 726f  ..    return gro
+00011b90: 7570 5f69 6e66 6f2c 2073 6f72 7465 645f  up_info, sorted_
+00011ba0: 6772 6f75 705f 696e 666f 0d0a 2020 2020  group_info..    
+00011bb0: 0d0a 6465 6620 6765 745f 6772 6f75 7069  ..def get_groupi
+00011bc0: 6e67 5f73 6967 6e5f 6661 6374 6f72 7328  ng_sign_factors(
+00011bd0: 736f 7274 6564 5f67 726f 7570 5f69 6e66  sorted_group_inf
+00011be0: 6f2c 2069 6e74 6572 6d65 6469 6174 655f  o, intermediate_
+00011bf0: 7374 6174 293a 0d0a 2020 2020 2370 7269  stat):..    #pri
+00011c00: 6e74 2869 6e74 6572 6d65 6469 6174 655f  nt(intermediate_
+00011c10: 7374 6174 290d 0a20 2020 200d 0a20 2020  stat)..    ..   
+00011c20: 2069 6620 6c65 6e28 736f 7274 6564 5f67   if len(sorted_g
+00011c30: 726f 7570 5f69 6e66 6f29 2021 3d20 6c65  roup_info) != le
+00011c40: 6e28 696e 7465 726d 6564 6961 7465 5f73  n(intermediate_s
+00011c50: 7461 7429 203a 0d0a 2020 2020 2020 2020  tat) :..        
+00011c60: 6572 726f 7228 2245 7272 6f72 5b67 6574  error("Error[get
+00011c70: 5f67 726f 7570 696e 675f 7369 676e 5f66  _grouping_sign_f
+00011c80: 6163 746f 7273 5d3a 2049 6e63 6f6e 7369  actors]: Inconsi
+00011c90: 7374 656e 7420 6e75 6d62 6572 206f 6620  stent number of 
+00011ca0: 696e 7465 726d 6564 6961 7465 5f73 7461  intermediate_sta
+00011cb0: 7420 616e 6420 6772 6f75 7069 6e67 7321  t and groupings!
+00011cc0: 2229 0d0a 2020 2020 0d0a 2020 2020 7369  ")..    ..    si
+00011cd0: 676e 5f66 6163 746f 7273 5f69 6e66 6f20  gn_factors_info 
+00011ce0: 3d20 5b20 2222 202c 205b 5d20 5d20 2369  = [ "" , [] ] #i
+00011cf0: 6e64 6963 6573 2061 6e64 2064 696d 656e  ndices and dimen
+00011d00: 7369 6f6e 730d 0a20 2020 2066 6f72 2069  sions..    for i
+00011d10: 2c5b 7374 7269 6e67 732c 7374 6174 732c  ,[strings,stats,
+00011d20: 7368 6170 6573 5d20 696e 2065 6e75 6d65  shapes] in enume
+00011d30: 7261 7465 2873 6f72 7465 645f 6772 6f75  rate(sorted_grou
+00011d40: 705f 696e 666f 293a 0d0a 2020 2020 2020  p_info):..      
+00011d50: 2020 0d0a 2020 2020 2020 2020 666f 7220    ..        for 
+00011d60: 6420 696e 2072 616e 6765 286c 656e 2873  d in range(len(s
+00011d70: 7461 7473 2929 3a0d 0a20 2020 2020 2020  tats)):..       
+00011d80: 2020 2020 2069 6620 7374 6174 735b 645d       if stats[d]
+00011d90: 203d 3d20 3120 616e 6420 696e 7465 726d   == 1 and interm
+00011da0: 6564 6961 7465 5f73 7461 745b 695d 203d  ediate_stat[i] =
+00011db0: 3d20 2d31 203a 0d0a 2020 2020 2020 2020  = -1 :..        
+00011dc0: 2020 2020 2020 2020 7369 676e 5f66 6163          sign_fac
+00011dd0: 746f 7273 5f69 6e66 6f5b 305d 202b 3d20  tors_info[0] += 
+00011de0: 222c 222b 7374 7269 6e67 735b 645d 0d0a  ","+strings[d]..
+00011df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e00: 7369 676e 5f66 6163 746f 7273 5f69 6e66  sign_factors_inf
+00011e10: 6f5b 315d 202b 3d20 5b73 6861 7065 735b  o[1] += [shapes[
+00011e20: 645d 5d0d 0a20 2020 2020 2020 2023 7072  d]]..        #pr
+00011e30: 696e 7428 7374 6174 732c 222d 2d2d 3e22  int(stats,"--->"
+00011e40: 2c69 6e74 6572 6d65 6469 6174 655f 7374  ,intermediate_st
+00011e50: 6174 5b69 5d29 0d0a 2020 2020 0d0a 2020  at[i])..    ..  
+00011e60: 2020 2370 7269 6e74 2873 6967 6e5f 6661    #print(sign_fa
+00011e70: 6374 6f72 735f 696e 666f 290d 0a20 2020  ctors_info)..   
+00011e80: 200d 0a20 2020 2023 2067 656e 6572 6174   ..    # generat
+00011e90: 6520 7468 6520 7369 676e 2066 6163 746f  e the sign facto
+00011ea0: 7220 7465 6e73 6f72 2028 7365 7061 7261  r tensor (separa
+00011eb0: 7465 6c79 290d 0a20 2020 2073 6967 6e5f  tely)..    sign_
+00011ec0: 6661 6374 6f72 735f 6c69 7374 203d 205b  factors_list = [
+00011ed0: 2073 6967 6e5f 6661 6374 6f72 735f 696e   sign_factors_in
+00011ee0: 666f 5b30 5d2c 205b 5d20 5d0d 0a20 2020  fo[0], [] ]..   
+00011ef0: 2066 6f72 2064 2069 6e20 7369 676e 5f66   for d in sign_f
+00011f00: 6163 746f 7273 5f69 6e66 6f5b 315d 203a  actors_info[1] :
+00011f10: 0d0a 2020 2020 2020 2020 7367 6e20 3d20  ..        sgn = 
+00011f20: 6e70 2e61 7272 6179 285b 2028 2d31 292a  np.array([ (-1)*
+00011f30: 2a70 6172 616d 2e67 7061 7269 7479 2869  *param.gparity(i
+00011f40: 6e64 2920 666f 7220 696e 6420 696e 2072  nd) for ind in r
+00011f50: 616e 6765 2864 2920 5d29 0d0a 2020 2020  ange(d) ])..    
+00011f60: 2020 2020 7369 676e 5f66 6163 746f 7273      sign_factors
+00011f70: 5f6c 6973 745b 315d 202b 3d20 5b73 676e  _list[1] += [sgn
+00011f80: 5d0d 0a20 2020 200d 0a20 2020 2023 7072  ]..    ..    #pr
+00011f90: 696e 7428 7369 676e 5f66 6163 746f 7273  int(sign_factors
+00011fa0: 5f6c 6973 7429 0d0a 2020 2020 0d0a 2020  _list)..    ..  
+00011fb0: 2020 7265 7475 726e 2073 6967 6e5f 6661    return sign_fa
+00011fc0: 6374 6f72 735f 6c69 7374 0d0a 0d0a 6465  ctors_list....de
+00011fd0: 6620 6765 745f 696e 7465 726d 6564 6961  f get_intermedia
+00011fe0: 7465 5f69 6e66 6f28 736f 7274 6564 5f67  te_info(sorted_g
+00011ff0: 726f 7570 5f69 6e66 6f2c 696e 7465 726d  roup_info,interm
+00012000: 6564 6961 7465 5f73 7461 7429 3a0d 0a20  ediate_stat):.. 
+00012010: 2020 206e 6577 5f73 6861 7065 203d 205b     new_shape = [
+00012020: 5d0d 0a20 2020 206e 6577 5f73 7461 7473  ]..    new_stats
+00012030: 203d 205b 5d0d 0a20 2020 2066 696e 616c   = []..    final
+00012040: 5f73 6861 7065 203d 205b 5d0d 0a20 2020  _shape = []..   
+00012050: 2066 696e 616c 5f73 7461 7473 203d 205b   final_stats = [
+00012060: 5d0d 0a20 2020 200d 0a20 2020 2069 6620  ]..    ..    if 
+00012070: 6c65 6e28 736f 7274 6564 5f67 726f 7570  len(sorted_group
+00012080: 5f69 6e66 6f29 2021 3d20 6c65 6e28 696e  _info) != len(in
+00012090: 7465 726d 6564 6961 7465 5f73 7461 7429  termediate_stat)
+000120a0: 3a0d 0a20 2020 2020 2020 2065 7272 6f72  :..        error
+000120b0: 2822 4572 726f 725b 6765 745f 696e 7465  ("Error[get_inte
+000120c0: 726d 6564 6961 7465 5f69 6e66 6f5d 3a20  rmediate_info]: 
+000120d0: 496e 636f 6e73 6973 7465 6e74 206e 756d  Inconsistent num
+000120e0: 6265 7220 6f66 2069 6e74 6572 6d65 6469  ber of intermedi
+000120f0: 6174 655f 7374 6174 2061 6e64 2067 726f  ate_stat and gro
+00012100: 7570 696e 6773 2122 290d 0a20 2020 2066  upings!")..    f
+00012110: 6f72 2069 2c5b 696e 6469 6365 732c 2073  or i,[indices, s
+00012120: 7461 7473 2c20 7368 6170 655d 2069 6e20  tats, shape] in 
+00012130: 656e 756d 6572 6174 6528 736f 7274 6564  enumerate(sorted
+00012140: 5f67 726f 7570 5f69 6e66 6f29 3a0d 0a20  _group_info):.. 
+00012150: 2020 2020 2020 2066 6572 6d69 5f64 203d         fermi_d =
+00012160: 2031 0d0a 2020 2020 2020 2020 626f 7365   1..        bose
+00012170: 5f64 2020 3d20 310d 0a20 2020 2020 2020  _d  = 1..       
+00012180: 2066 6572 6d69 5f6e 203d 2030 0d0a 2020   fermi_n = 0..  
+00012190: 2020 2020 2020 626f 7365 5f6e 2020 3d20        bose_n  = 
+000121a0: 300d 0a20 2020 2020 2020 2066 6f72 2064  0..        for d
+000121b0: 2069 6e20 7261 6e67 6528 6c65 6e28 7374   in range(len(st
+000121c0: 6174 7329 293a 0d0a 2020 2020 2020 2020  ats)):..        
+000121d0: 2020 2020 6966 2073 7461 7473 5b64 5d20      if stats[d] 
+000121e0: 696e 2066 6572 6d69 5f74 7970 6520 3a0d  in fermi_type :.
+000121f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012200: 2066 6572 6d69 5f64 202a 3d20 7368 6170   fermi_d *= shap
+00012210: 655b 645d 0d0a 2020 2020 2020 2020 2020  e[d]..          
+00012220: 2020 2020 2020 6665 726d 695f 6e20 2b3d        fermi_n +=
+00012230: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
+00012240: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00012250: 2020 2020 2020 2062 6f73 655f 6420 2a3d         bose_d *=
+00012260: 2073 6861 7065 5b64 5d0d 0a20 2020 2020   shape[d]..     
+00012270: 2020 2020 2020 2020 2020 2062 6f73 655f             bose_
+00012280: 6e20 2b3d 2031 0d0a 2020 2020 2020 2020  n += 1..        
+00012290: 6966 2062 6f73 655f 6e20 3e20 3020 3a0d  if bose_n > 0 :.
+000122a0: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
+000122b0: 5f73 6861 7065 202b 3d20 5b62 6f73 655f  _shape += [bose_
+000122c0: 645d 0d0a 2020 2020 2020 2020 2020 2020  d]..            
+000122d0: 6e65 775f 7374 6174 7320 2b3d 205b 305d  new_stats += [0]
+000122e0: 0d0a 2020 2020 2020 2020 6966 2066 6572  ..        if fer
+000122f0: 6d69 5f6e 203e 2030 203a 0d0a 2020 2020  mi_n > 0 :..    
+00012300: 2020 2020 2020 2020 6e65 775f 7368 6170          new_shap
+00012310: 6520 2b3d 205b 6665 726d 695f 645d 0d0a  e += [fermi_d]..
+00012320: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00012330: 7374 6174 7320 2b3d 205b 696e 7465 726d  stats += [interm
+00012340: 6564 6961 7465 5f73 7461 745b 695d 5d0d  ediate_stat[i]].
+00012350: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+00012360: 2020 2020 2020 2066 696e 616c 5f73 6861         final_sha
+00012370: 7065 202b 3d20 5b62 6f73 655f 642a 6665  pe += [bose_d*fe
+00012380: 726d 695f 645d 0d0a 2020 2020 2020 2020  rmi_d]..        
+00012390: 0d0a 2020 2020 2020 2020 6966 2062 6f73  ..        if bos
+000123a0: 655f 6e20 3e20 3020 616e 6420 6665 726d  e_n > 0 and ferm
+000123b0: 695f 6e20 3e20 3020 3a0d 0a20 2020 2020  i_n > 0 :..     
+000123c0: 2020 2020 2020 2066 696e 616c 5f73 7461         final_sta
+000123d0: 7473 202b 3d20 5b68 7962 7269 645f 7379  ts += [hybrid_sy
+000123e0: 6d62 6f6c 5d0d 0a20 2020 2020 2020 2065  mbol]..        e
+000123f0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00012400: 2020 6669 6e61 6c5f 7374 6174 7320 2b3d    final_stats +=
+00012410: 205b 696e 7465 726d 6564 6961 7465 5f73   [intermediate_s
+00012420: 7461 745b 695d 5d0d 0a20 2020 2020 2020  tat[i]]..       
+00012430: 2020 2020 200d 0a20 2020 206e 6577 5f73       ..    new_s
+00012440: 7461 7473 203d 206d 616b 655f 7475 706c  tats = make_tupl
+00012450: 6528 6e65 775f 7374 6174 7329 0d0a 2020  e(new_stats)..  
+00012460: 2020 6e65 775f 7368 6170 6520 3d20 6d61    new_shape = ma
+00012470: 6b65 5f74 7570 6c65 286e 6577 5f73 6861  ke_tuple(new_sha
+00012480: 7065 290d 0a20 2020 2066 696e 616c 5f73  pe)..    final_s
+00012490: 7461 7473 203d 206d 616b 655f 7475 706c  tats = make_tupl
+000124a0: 6528 6669 6e61 6c5f 7374 6174 7329 0d0a  e(final_stats)..
+000124b0: 2020 2020 6669 6e61 6c5f 7368 6170 6520      final_shape 
+000124c0: 3d20 6d61 6b65 5f74 7570 6c65 2866 696e  = make_tuple(fin
+000124d0: 616c 5f73 6861 7065 290d 0a20 2020 200d  al_shape)..    .
+000124e0: 0a20 2020 2072 6574 7572 6e20 6e65 775f  .    return new_
+000124f0: 7374 6174 732c 206e 6577 5f73 6861 7065  stats, new_shape
+00012500: 2c20 6669 6e61 6c5f 7374 6174 732c 2066  , final_stats, f
+00012510: 696e 616c 5f73 6861 7065 0d0a 0d0a 2323  inal_shape....##
+00012520: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00012530: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00012540: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00012550: 2323 0d0a 2323 2020 2020 2020 2020 2020  ##..##          
+00012560: 5472 696d 2074 6865 2047 7261 7373 6d61  Trim the Grassma
+00012570: 6e6e 2d6f 6464 2070 6172 7473 2020 2020  nn-odd parts    
+00012580: 2020 2020 2020 2323 0d0a 2323 2020 2020        ##..##    
+00012590: 2020 2020 2020 2020 2020 2028 666f 7220             (for 
+000125a0: 7465 7374 696e 6720 6f6e 6c79 2920 2020  testing only)   
+000125b0: 2020 2020 2020 2020 2020 2020 2323 0d0a              ##..
+000125c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000125d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000125e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000125f0: 2323 2323 0d0a 0d0a 6465 6620 7472 696d  ####....def trim
+00012600: 5f67 7261 7373 6d61 6e6e 5f6f 6464 284f  _grassmann_odd(O
+00012610: 626a 293a 0d0a 2020 2020 6f62 6a74 7970  bj):..    objtyp
+00012620: 653d 7479 7065 284f 626a 290d 0a0d 0a20  e=type(Obj).... 
+00012630: 2020 2069 6628 4f62 6a2e 656e 636f 6465     if(Obj.encode
+00012640: 7220 3d3d 2027 6361 6e6f 6e69 6361 6c27  r == 'canonical'
+00012650: 293a 0d0a 2020 2020 2020 2020 4f62 6a20  ):..        Obj 
+00012660: 3d20 4f62 6a2e 7377 6974 6368 5f65 6e63  = Obj.switch_enc
+00012670: 6f64 6572 2873 6176 655f 6d65 6d6f 7279  oder(save_memory
+00012680: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00012690: 0d0a 2020 2020 6966 286f 626a 7479 7065  ..    if(objtype
+000126a0: 3d3d 6465 6e73 6529 3a0d 0a20 2020 2020  ==dense):..     
+000126b0: 2020 204f 626a 203d 2073 7061 7273 6528     Obj = sparse(
+000126c0: 4f62 6a29 0d0a 2020 2020 4320 3d20 4f62  Obj)..    C = Ob
+000126d0: 6a2e 636f 6f72 6473 0d0a 2020 2020 7330  j.coords..    s0
+000126e0: 203d 2074 696d 652e 7469 6d65 2829 0d0a   = time.time()..
+000126f0: 2020 2020 7330 3020 3d20 7330 0d0a 2020      s00 = s0..  
+00012700: 2020 7072 6f67 7265 7373 5f73 7061 6365    progress_space
+00012710: 2829 2023 203c 3c20 446f 6e27 7420 7265  () # << Don't re
+00012720: 6d6f 7665 2074 6869 732e 2054 6869 7320  move this. This 
+00012730: 6973 2066 6f72 2074 6865 2073 686f 775f  is for the show_
+00012740: 7072 6f67 7265 7373 210d 0a0d 0a20 2020  progress!....   
+00012750: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00012760: 4f62 6a2e 6e6e 7a29 3a0d 0a20 2020 2020  Obj.nnz):..     
+00012770: 2020 2066 636f 6f72 6473 203d 205b 2069     fcoords = [ i
+00012780: 6e64 2066 6f72 206a 2c69 6e64 2069 6e20  nd for j,ind in 
+00012790: 656e 756d 6572 6174 6528 435b 695d 2920  enumerate(C[i]) 
+000127a0: 6966 2028 4f62 6a2e 7374 6174 6973 7469  if (Obj.statisti
+000127b0: 635b 6a5d 2069 6e20 6665 726d 695f 7479  c[j] in fermi_ty
+000127c0: 7065 295d 0d0a 2020 2020 2020 2020 6966  pe)]..        if
+000127d0: 2873 756d 2866 636f 6f72 6473 2925 3220  (sum(fcoords)%2 
+000127e0: 3d3d 2031 293a 0d0a 2020 2020 2020 2020  == 1):..        
+000127f0: 2020 2020 4f62 6a2e 6461 7461 2e64 6174      Obj.data.dat
+00012800: 615b 695d 203d 2030 0d0a 0d0a 2020 2020  a[i] = 0....    
+00012810: 2020 2020 6966 2074 696d 652e 7469 6d65      if time.time
+00012820: 2829 2d73 3020 3e20 302e 3520 3a0d 0a20  ()-s0 > 0.5 :.. 
+00012830: 2020 2020 2020 2020 2020 2073 686f 775f             show_
+00012840: 7072 6f67 7265 7373 2869 2c4f 626a 2e6e  progress(i,Obj.n
+00012850: 6e7a 2c22 7472 696d 5f67 7261 7373 6d61  nz,"trim_grassma
+00012860: 6e6e 5f6f 6464 222c 7469 6d65 3d74 696d  nn_odd",time=tim
+00012870: 652e 7469 6d65 2829 2d73 3030 290d 0a0d  e.time()-s00)...
+00012880: 0a20 2020 2063 6c65 6172 5f70 726f 6772  .    clear_progr
+00012890: 6573 7328 290d 0a20 2020 2074 6162 5f75  ess()..    tab_u
+000128a0: 7028 290d 0a0d 0a0d 0a20 2020 2069 6628  p()......    if(
+000128b0: 6f62 6a74 7970 653d 3d64 656e 7365 293a  objtype==dense):
+000128c0: 0d0a 2020 2020 2020 2020 4f62 6a20 3d20  ..        Obj = 
+000128d0: 6465 6e73 6528 4f62 6a29 0d0a 0d0a 2020  dense(Obj)....  
+000128e0: 2020 6966 284f 626a 5f69 6e70 7574 2e65    if(Obj_input.e
+000128f0: 6e63 6f64 6572 203d 3d20 2763 616e 6f6e  ncoder == 'canon
+00012900: 6963 616c 2729 3a0d 0a20 2020 2020 2020  ical'):..       
+00012910: 204f 626a 203d 204f 626a 2e73 7769 7463   Obj = Obj.switc
+00012920: 685f 656e 636f 6465 7228 7361 7665 5f6d  h_encoder(save_m
+00012930: 656d 6f72 793d 5472 7565 290d 0a0d 0a20  emory=True).... 
+00012940: 2020 2072 6574 7572 6e20 4f62 6a0d 0a0d     return Obj...
+00012950: 0a64 6566 2069 735f 6772 6173 736d 616e  .def is_grassman
+00012960: 6e5f 6576 656e 284f 626a 293a 0d0a 2020  n_even(Obj):..  
+00012970: 2020 6966 204f 626a 2e65 6e63 6f64 6572    if Obj.encoder
+00012980: 203d 3d20 2763 616e 6f6e 6963 616c 273a   == 'canonical':
+00012990: 0d0a 2020 2020 2020 2020 4f62 6a20 3d20  ..        Obj = 
+000129a0: 4f62 6a2e 7377 6974 6368 5f65 6e63 6f64  Obj.switch_encod
+000129b0: 6572 2873 6176 655f 6d65 6d6f 7279 3d54  er(save_memory=T
+000129c0: 7275 6529 0d0a 2020 2020 6966 2074 7970  rue)..    if typ
+000129d0: 6528 4f62 6a29 203d 3d20 6465 6e73 653a  e(Obj) == dense:
 000129e0: 0d0a 2020 2020 2020 2020 4f62 6a20 3d20  ..        Obj = 
-000129f0: 4f62 6a2e 7377 6974 6368 5f65 6e63 6f64  Obj.switch_encod
-00012a00: 6572 2873 6176 655f 6d65 6d6f 7279 3d54  er(save_memory=T
-00012a10: 7275 6529 0d0a 2020 2020 6966 2074 7970  rue)..    if typ
-00012a20: 6528 4f62 6a29 203d 3d20 6465 6e73 653a  e(Obj) == dense:
-00012a30: 0d0a 2020 2020 2020 2020 4f62 6a20 3d20  ..        Obj = 
-00012a40: 7370 6172 7365 284f 626a 290d 0a0d 0a20  sparse(Obj).... 
-00012a50: 2020 2043 203d 204f 626a 2e63 6f6f 7264     C = Obj.coord
-00012a60: 730d 0a20 2020 2066 6f72 2078 2069 6e20  s..    for x in 
-00012a70: 433a 0d0a 2020 2020 2020 2020 7061 7269  C:..        pari
-00012a80: 7479 203d 2073 756d 285b 2069 6e64 2066  ty = sum([ ind f
-00012a90: 6f72 2069 2c69 6e64 2069 6e20 656e 756d  or i,ind in enum
-00012aa0: 6572 6174 6528 7829 2069 6620 4f62 6a2e  erate(x) if Obj.
-00012ab0: 7374 6174 6973 7469 635b 695d 2069 6e20  statistic[i] in 
-00012ac0: 6665 726d 695f 7479 7065 205d 290d 0a20  fermi_type ]).. 
-00012ad0: 2020 2020 2020 2069 6620 7061 7269 7479         if parity
-00012ae0: 2532 213d 3020 3a0d 0a20 2020 2020 2020  %2!=0 :..       
-00012af0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00012b00: 650d 0a20 2020 2072 6574 7572 6e20 5472  e..    return Tr
-00012b10: 7565 0d0a 0d0a 2323 2323 2323 2323 2323  ue....##########
-00012b20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012b30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012b40: 2323 2323 2323 2323 2323 0d0a 2323 2020  ##########..##  
-00012b50: 2020 2020 2020 2020 5369 6e67 756c 6172          Singular
-00012b60: 2076 616c 7565 2064 6563 6f6d 706f 7369   value decomposi
-00012b70: 7469 6f6e 2020 2020 2020 2020 2020 2323  tion          ##
-00012b80: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
-00012b90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012ba0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012bb0: 2323 2323 2323 0d0a 0d0a 6465 6620 536f  ######....def So
-00012bc0: 7274 6564 5356 4428 4d2c 6375 746f 6666  rtedSVD(M,cutoff
-00012bd0: 3d4e 6f6e 6529 3a0d 0a20 2020 2055 2c20  =None):..    U, 
-00012be0: ce9b 2c20 5620 3d20 6e70 2e6c 696e 616c  .., V = np.linal
-00012bf0: 672e 7376 6428 4d2c 2066 756c 6c5f 6d61  g.svd(M, full_ma
-00012c00: 7472 6963 6573 3d46 616c 7365 290d 0a0d  trices=False)...
-00012c10: 0a0d 0a20 2020 206e 6e7a 203d 2030 0d0a  ...    nnz = 0..
-00012c20: 2020 2020 2369 6620 6e70 2e61 6273 28ce      #if np.abs(.
-00012c30: 9b5b 305d 2920 3c20 6e75 6d65 725f 6375  .[0]) < numer_cu
-00012c40: 746f 6666 3a0d 0a20 2020 2023 2020 2020  toff:..    #    
-00012c50: 6572 726f 7228 2245 7272 6f72 5b53 6f72  error("Error[Sor
-00012c60: 7465 6453 5644 5d3a 206e 702e 6c69 6e61  tedSVD]: np.lina
-00012c70: 6c67 2e73 7664 2829 2072 6574 7572 6e73  lg.svd() returns
-00012c80: 207a 6572 6f20 7369 6e67 756c 6172 2076   zero singular v
-00012c90: 616c 7565 2076 6563 746f 7221 2229 0d0a  alue vector!")..
-00012ca0: 0d0a 2020 2020 666f 7220 692c 7320 696e  ..    for i,s in
-00012cb0: 2065 6e75 6d65 7261 7465 28ce 9b29 3a0d   enumerate(..):.
-00012cc0: 0a20 2020 2020 2020 2069 6620 6e70 2e61  .        if np.a
-00012cd0: 6273 2873 2fce 9b5b 305d 2920 3e20 6e75  bs(s/..[0]) > nu
-00012ce0: 6d65 725f 6375 746f 6666 3a0d 0a20 2020  mer_cutoff:..   
-00012cf0: 2020 2020 2020 2020 206e 6e7a 2b3d 310d           nnz+=1.
-00012d00: 0a0d 0a20 2020 2069 6620 6375 746f 6666  ...    if cutoff
-00012d10: 213d 4e6f 6e65 2061 6e64 2063 7574 6f66  !=None and cutof
-00012d20: 6620 3c20 6e6e 7a3a 0d0a 2020 2020 2020  f < nnz:..      
-00012d30: 2020 6e6e 7a20 3d20 6375 746f 6666 0d0a    nnz = cutoff..
-00012d40: 0d0a 2020 2020 ce9b 203d 20ce 9b5b 3a6e  ..    .. = ..[:n
-00012d50: 6e7a 5d0d 0a20 2020 2055 203d 2055 5b3a  nz]..    U = U[:
-00012d60: 2c3a 6e6e 7a5d 0d0a 2020 2020 5620 3d20  ,:nnz]..    V = 
-00012d70: 565b 3a6e 6e7a 2c3a 5d0d 0a0d 0a0d 0a20  V[:nnz,:]...... 
-00012d80: 2020 2072 6574 7572 6e20 552c 20ce 9b2c     return U, ..,
-00012d90: 2056 0d0a 2320 4920 3d20 6355 5520 3d20   V..# I = cUU = 
-00012da0: 5663 560d 0a64 6566 2042 6c6f 636b 5356  VcV..def BlockSV
-00012db0: 4428 4f62 6a2c 6375 746f 6666 3d4e 6f6e  D(Obj,cutoff=Non
-00012dc0: 6529 3a0d 0a20 2020 200d 0a20 2020 2023  e):..    ..    #
-00012dd0: 2070 6572 666f 726d 696e 6720 616e 2073   performing an s
-00012de0: 7664 206f 6620 6120 6d61 7472 6978 2062  vd of a matrix b
-00012df0: 6c6f 636b 2062 7920 626c 6f63 6b0d 0a0d  lock by block...
-00012e00: 0a20 2020 2069 6628 7479 7065 284f 626a  .    if(type(Obj
-00012e10: 2921 3d6e 702e 6172 7261 7920 616e 6420  )!=np.array and 
-00012e20: 7479 7065 284f 626a 2921 3d6e 702e 6e64  type(Obj)!=np.nd
-00012e30: 6172 7261 7929 3a0d 0a20 2020 2020 2020  array):..       
-00012e40: 2065 7272 6f72 2822 4572 726f 725b 426c   error("Error[Bl
-00012e50: 6f63 6b53 5644 5d3a 2041 6e20 696e 7075  ockSVD]: An inpu
-00012e60: 7420 6d75 7374 2062 6520 6f66 2074 7970  t must be of typ
-00012e70: 6520 6e75 6d70 792e 6172 7261 7920 6f72  e numpy.array or
-00012e80: 206e 756d 7079 2e6e 6461 7272 6179 206f   numpy.ndarray o
-00012e90: 6e6c 7921 2229 0d0a 2020 2020 2020 2020  nly!")..        
-00012ea0: 0d0a 0d0a 2020 2020 6966 284f 626a 2e6e  ....    if(Obj.n
-00012eb0: 6469 6d21 3d32 293a 0d0a 2020 2020 2020  dim!=2):..      
-00012ec0: 2020 6572 726f 7228 2245 7272 6f72 5b42    error("Error[B
-00012ed0: 6c6f 636b 5356 445d 3a20 416e 2069 6e70  lockSVD]: An inp
-00012ee0: 7574 206d 7573 7420 6265 2061 206d 6174  ut must be a mat
-00012ef0: 7269 7820 6f6e 6c79 2122 290d 0a20 2020  rix only!")..   
-00012f00: 2020 2020 200d 0a0d 0a20 2020 206d 203d       ....    m =
-00012f10: 204f 626a 2e73 6861 7065 5b30 5d0d 0a20   Obj.shape[0].. 
-00012f20: 2020 206e 203d 204f 626a 2e73 6861 7065     n = Obj.shape
-00012f30: 5b31 5d0d 0a0d 0a20 2020 2069 6628 6d25  [1]....    if(m%
-00012f40: 3221 3d30 2061 6e64 206e 2532 213d 3029  2!=0 and n%2!=0)
-00012f50: 3a0d 0a20 2020 2020 2020 2065 7272 6f72  :..        error
-00012f60: 2822 4572 726f 725b 426c 6f63 6b53 5644  ("Error[BlockSVD
-00012f70: 5d3a 2054 6865 206d 6174 7269 7820 6469  ]: The matrix di
-00012f80: 6d65 6e73 696f 6e73 206d 7573 7420 6265  mensions must be
-00012f90: 2065 7665 6e21 2229 0d0a 2020 2020 2020   even!")..      
-00012fa0: 2020 0d0a 0d0a 0d0a 2020 2020 6966 286d    ......    if(m
-00012fb0: 3d3d 3020 616e 6420 6e3d 3d30 293a 0d0a  ==0 and n==0):..
-00012fc0: 2020 2020 2020 2020 6572 726f 7228 2245          error("E
-00012fd0: 7272 6f72 5b42 6c6f 636b 5356 445d 3a20  rror[BlockSVD]: 
-00012fe0: 5468 6520 6d61 7472 6978 2064 696d 656e  The matrix dimen
-00012ff0: 7369 6f6e 7320 6d75 7374 2062 6520 6174  sions must be at
-00013000: 206c 6561 7374 2032 2122 290d 0a20 2020   least 2!")..   
-00013010: 2020 2020 200d 0a0d 0a20 2020 2070 6172       ....    par
-00013020: 6974 795f 6e6f 726d 203d 2030 0d0a 2020  ity_norm = 0..  
-00013030: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00013040: 286d 293a 0d0a 2020 2020 2020 2020 666f  (m):..        fo
-00013050: 7220 6a20 696e 2072 616e 6765 286e 293a  r j in range(n):
-00013060: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00013070: 2028 692b 6a29 2532 213d 303a 0d0a 2020   (i+j)%2!=0:..  
-00013080: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00013090: 7269 7479 5f6e 6f72 6d20 2b3d 206e 702e  rity_norm += np.
-000130a0: 6c69 6e61 6c67 2e6e 6f72 6d28 4f62 6a5b  linalg.norm(Obj[
-000130b0: 692c 6a5d 290d 0a20 2020 2069 6628 2028  i,j])..    if( (
-000130c0: 6e6f 7420 736b 6970 5f70 6172 6974 795f  not skip_parity_
-000130d0: 626c 6f63 6b69 6e67 5f63 6865 636b 2920  blocking_check) 
-000130e0: 616e 6420 7061 7269 7479 5f6e 6f72 6d2f  and parity_norm/
-000130f0: 286d 2a6e 2f32 293e 312e 3065 2d31 3429  (m*n/2)>1.0e-14)
-00013100: 3a0d 0a20 2020 2020 2020 2065 7272 6f72  :..        error
-00013110: 2822 4572 726f 725b 426c 6f63 6b53 5644  ("Error[BlockSVD
-00013120: 5d3a 2054 6869 7320 6d61 7472 6978 2069  ]: This matrix i
-00013130: 7320 6e6f 7420 636f 6e73 7472 7563 7465  s not constructe
-00013140: 6420 6672 6f6d 2061 2047 7261 7373 6d61  d from a Grassma
-00013150: 6e6e 2d65 7665 6e20 7465 6e73 6f72 2e22  nn-even tensor."
-00013160: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-00013170: 2822 2020 2020 2020 2020 2020 2020 2020  ("              
-00013180: 2020 2028 4f72 2074 6861 7420 6f6e 6520     (Or that one 
-00013190: 6f66 2074 6865 2069 6e64 6963 6573 2061  of the indices a
-000131a0: 7265 206e 6f6e 2d66 6572 6d69 6f6e 6963  re non-fermionic
-000131b0: 2e29 2229 0d0a 2020 2020 2020 2020 0d0a  .)")..        ..
-000131c0: 0d0a 2020 2020 2320 4174 2074 6869 7320  ..    # At this 
-000131d0: 706f 696e 7420 7468 6520 6d61 7472 6978  point the matrix
-000131e0: 2069 7320 7765 6c6c 2d62 6568 6176 6564   is well-behaved
-000131f0: 0d0a 0d0a 2020 2020 2320 7469 6d65 2074  ....    # time t
-00013200: 6f20 7365 7061 7261 7465 2074 6865 2062  o separate the b
-00013210: 6c6f 636b 730d 0a20 2020 204d 4520 3d20  locks..    ME = 
-00013220: 6e70 2e7a 6572 6f73 285b 696e 7428 6d2f  np.zeros([int(m/
-00013230: 3229 2c69 6e74 286e 2f32 295d 2c64 7479  2),int(n/2)],dty
-00013240: 7065 3d74 7970 6528 4f62 6a5b 305d 5b30  pe=type(Obj[0][0
-00013250: 5d29 290d 0a20 2020 204d 4f20 3d20 6e70  ]))..    MO = np
-00013260: 2e7a 6572 6f73 285b 696e 7428 6d2f 3229  .zeros([int(m/2)
-00013270: 2c69 6e74 286e 2f32 295d 2c64 7479 7065  ,int(n/2)],dtype
-00013280: 3d74 7970 6528 4f62 6a5b 305d 5b30 5d29  =type(Obj[0][0])
-00013290: 290d 0a0d 0a20 2020 2066 6f72 2069 2069  )....    for i i
-000132a0: 6e20 7261 6e67 6528 696e 7428 6d2f 3229  n range(int(m/2)
-000132b0: 293a 0d0a 2020 2020 2020 2020 666f 7220  ):..        for 
-000132c0: 6a20 696e 2072 616e 6765 2869 6e74 286e  j in range(int(n
-000132d0: 2f32 2929 3a0d 0a20 2020 2020 2020 2020  /2)):..         
-000132e0: 2020 204d 455b 692c 6a5d 203d 204f 626a     ME[i,j] = Obj
-000132f0: 5b32 2a69 2c32 2a6a 5d0d 0a20 2020 2020  [2*i,2*j]..     
-00013300: 2020 2020 2020 204d 4f5b 692c 6a5d 203d         MO[i,j] =
-00013310: 204f 626a 5b32 2a69 2b31 2c32 2a6a 2b31   Obj[2*i+1,2*j+1
-00013320: 5d0d 0a0d 0a20 2020 2068 616c 6663 7574  ]....    halfcut
-00013330: 6f66 6620 3d20 4e6f 6e65 0d0a 2020 2020  off = None..    
-00013340: 6966 2063 7574 6f66 6621 3d4e 6f6e 6520  if cutoff!=None 
-00013350: 3a0d 0a20 2020 2020 2020 2068 616c 6663  :..        halfc
-00013360: 7574 6f66 6620 3d20 696e 7428 6375 746f  utoff = int(cuto
-00013370: 6666 2f32 290d 0a0d 0a20 2020 2055 452c  ff/2)....    UE,
-00013380: 20ce 9b45 2c20 5645 203d 2053 6f72 7465   ..E, VE = Sorte
-00013390: 6453 5644 284d 452c 6861 6c66 6375 746f  dSVD(ME,halfcuto
-000133a0: 6666 290d 0a20 2020 2055 4f2c 20ce 9b4f  ff)..    UO, ..O
-000133b0: 2c20 564f 203d 2053 6f72 7465 6453 5644  , VO = SortedSVD
-000133c0: 284d 4f2c 6861 6c66 6375 746f 6666 290d  (MO,halfcutoff).
-000133d0: 0a0d 0a20 2020 2064 203d 206d 6178 286c  ...    d = max(l
-000133e0: 656e 28ce 9b45 292c 6c65 6e28 ce9b 4f29  en(..E),len(..O)
-000133f0: 290d 0a20 2020 2064 203d 2069 6e74 2832  )..    d = int(2
-00013400: 2a2a 6d61 7468 2e63 6569 6c28 6e70 2e6c  **math.ceil(np.l
-00013410: 6f67 3228 6429 2929 0d0a 0d0a 2020 2020  og2(d)))....    
-00013420: 6465 6620 7061 6464 696e 6728 5578 2c20  def padding(Ux, 
-00013430: ce9b 782c 2056 782c 2070 6164 6469 6e67  ..x, Vx, padding
-00013440: 5f64 696d 656e 7369 6f6e 293a 0d0a 2020  _dimension):..  
-00013450: 2020 2020 2020 5578 203d 206e 702e 7061        Ux = np.pa
-00013460: 6428 5578 2c28 2830 2c30 292c 2830 2c70  d(Ux,((0,0),(0,p
-00013470: 6164 6469 6e67 5f64 696d 656e 7369 6f6e  adding_dimension
-00013480: 2929 2c27 636f 6e73 7461 6e74 272c 636f  )),'constant',co
-00013490: 6e73 7461 6e74 5f76 616c 7565 733d 2828  nstant_values=((
-000134a0: 302c 3029 2c28 302c 3029 2929 0d0a 2020  0,0),(0,0)))..  
-000134b0: 2020 2020 2020 ce9b 7820 3d20 6e70 2e64        ..x = np.d
-000134c0: 6961 6728 6e70 2e70 6164 28ce 9b78 2c28  iag(np.pad(..x,(
-000134d0: 302c 7061 6464 696e 675f 6469 6d65 6e73  0,padding_dimens
-000134e0: 696f 6e29 2c27 636f 6e73 7461 6e74 272c  ion),'constant',
-000134f0: 636f 6e73 7461 6e74 5f76 616c 7565 733d  constant_values=
-00013500: 2020 2028 302c 3029 2020 2020 2929 0d0a     (0,0)    ))..
-00013510: 2020 2020 2020 2020 5678 203d 206e 702e          Vx = np.
-00013520: 7061 6428 5678 2c28 2830 2c70 6164 6469  pad(Vx,((0,paddi
-00013530: 6e67 5f64 696d 656e 7369 6f6e 292c 2830  ng_dimension),(0
-00013540: 2c30 2929 2c27 636f 6e73 7461 6e74 272c  ,0)),'constant',
-00013550: 636f 6e73 7461 6e74 5f76 616c 7565 733d  constant_values=
-00013560: 2828 302c 3029 2c28 302c 3029 2929 0d0a  ((0,0),(0,0)))..
-00013570: 2020 2020 2020 2020 7265 7475 726e 2055          return U
-00013580: 782c 20ce 9b78 2c20 5678 0d0a 0d0a 2020  x, ..x, Vx....  
-00013590: 2020 5545 2c20 ce9b 452c 2056 4520 3d20    UE, ..E, VE = 
-000135a0: 7061 6464 696e 6728 5545 2c20 ce9b 452c  padding(UE, ..E,
-000135b0: 2056 452c 2064 2d6c 656e 28ce 9b45 2929   VE, d-len(..E))
-000135c0: 0d0a 2020 2020 554f 2c20 ce9b 4f2c 2056  ..    UO, ..O, V
-000135d0: 4f20 3d20 7061 6464 696e 6728 554f 2c20  O = padding(UO, 
-000135e0: ce9b 4f2c 2056 4f2c 2064 2d6c 656e 28ce  ..O, VO, d-len(.
-000135f0: 9b4f 2929 0d0a 0d0a 2020 2020 6465 6620  .O))....    def 
-00013600: 6765 745f 6675 6c6c 5f6d 6174 7269 7828  get_full_matrix(
-00013610: 4145 2c20 414f 293a 0d0a 2020 2020 2020  AE, AO):..      
-00013620: 2020 6d68 616c 662c 6e68 616c 6620 3d20    mhalf,nhalf = 
-00013630: 4145 2e73 6861 7065 0d0a 2020 2020 2020  AE.shape..      
-00013640: 2020 4120 3d20 6e70 2e7a 6572 6f73 285b    A = np.zeros([
-00013650: 322a 6d68 616c 662c 322a 6e68 616c 665d  2*mhalf,2*nhalf]
-00013660: 2c64 7479 7065 3d74 7970 6528 4145 5b30  ,dtype=type(AE[0
-00013670: 5d5b 305d 2929 0d0a 2020 2020 2020 2020  ][0]))..        
-00013680: 666f 7220 6920 696e 2072 616e 6765 286d  for i in range(m
-00013690: 6861 6c66 293a 0d0a 2020 2020 2020 2020  half):..        
-000136a0: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
-000136b0: 6765 286e 6861 6c66 293a 0d0a 2020 2020  ge(nhalf):..    
-000136c0: 2020 2020 2020 2020 2020 2020 415b 322a              A[2*
-000136d0: 692c 322a 6a5d 203d 2041 455b 692c 6a5d  i,2*j] = AE[i,j]
-000136e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000136f0: 2020 415b 322a 692b 312c 322a 6a2b 315d    A[2*i+1,2*j+1]
-00013700: 203d 2041 4f5b 692c 6a5d 0d0a 2020 2020   = AO[i,j]..    
-00013710: 2020 2020 7265 7475 726e 2041 0d0a 0d0a      return A....
-00013720: 2020 2020 5520 3d20 6765 745f 6675 6c6c      U = get_full
-00013730: 5f6d 6174 7269 7828 5545 2c55 4f29 0d0a  _matrix(UE,UO)..
-00013740: 2020 2020 ce9b 203d 2067 6574 5f66 756c      .. = get_ful
-00013750: 6c5f 6d61 7472 6978 28ce 9b45 2cce 9b4f  l_matrix(..E,..O
-00013760: 290d 0a20 2020 2056 203d 2067 6574 5f66  )..    V = get_f
-00013770: 756c 6c5f 6d61 7472 6978 2856 452c 564f  ull_matrix(VE,VO
-00013780: 290d 0a20 2020 200d 0a0d 0a20 2020 2072  )..    ....    r
-00013790: 6574 7572 6e20 552c 20ce 9b2c 2056 0d0a  eturn U, .., V..
-000137a0: 0d0a 6465 6620 7376 6428 496e 704f 626a  ..def svd(InpObj
-000137b0: 2c73 7472 696e 672c 6375 746f 6666 3d4e  ,string,cutoff=N
-000137c0: 6f6e 652c 7361 7665 5f6d 656d 6f72 793d  one,save_memory=
-000137d0: 4661 6c73 6529 3a0d 0a0d 0a20 2020 2070  False):....    p
-000137e0: 726f 6365 7373 5f6e 616d 6520 3d20 2273  rocess_name = "s
-000137f0: 7664 220d 0a20 2020 2070 726f 6365 7373  vd"..    process
-00013800: 5f63 6f6c 6f72 203d 2022 7965 6c6c 6f77  _color = "yellow
-00013810: 220d 0a20 2020 2070 726f 6365 7373 5f6c  "..    process_l
-00013820: 656e 6774 6820 3d20 360d 0a20 2020 2073  ength = 6..    s
-00013830: 7465 7020 3d20 310d 0a20 2020 2073 3030  tep = 1..    s00
-00013840: 203d 2074 696d 652e 7469 6d65 2829 0d0a   = time.time()..
-00013850: 2020 2020 7072 696e 7428 290d 0a0d 0a20      print().... 
-00013860: 2020 2067 6c6f 6261 6c20 736b 6970 5f70     global skip_p
-00013870: 6f77 6572 5f6f 665f 7477 6f5f 6368 6563  ower_of_two_chec
-00013880: 6b0d 0a0d 0a20 2020 2023 2074 6865 2073  k....    # the s
-00013890: 7472 696e 6720 6973 206f 6620 7468 6520  tring is of the 
-000138a0: 666f 726d 2061 6161 617c 6262 620d 0a0d  form aaaa|bbb...
-000138b0: 0a20 2020 2073 7472 696e 6720 3d20 6465  .    string = de
-000138c0: 6e75 6d65 7261 7465 2873 7472 696e 6729  numerate(string)
-000138d0: 0d0a 0d0a 2020 2020 0d0a 2020 2020 4f62  ....    ..    Ob
-000138e0: 6a20 3d20 496e 704f 626a 2e63 6f70 7928  j = InpObj.copy(
-000138f0: 290d 0a20 2020 2074 6869 735f 7479 7065  )..    this_type
-00013900: 203d 2074 7970 6528 4f62 6a29 0d0a 2020   = type(Obj)..  
-00013910: 2020 7468 6973 5f66 6f72 6d61 7420 3d20    this_format = 
-00013920: 4f62 6a2e 666f 726d 6174 0d0a 2020 2020  Obj.format..    
-00013930: 7468 6973 5f65 6e63 6f64 6572 203d 204f  this_encoder = O
-00013940: 626a 2e65 6e63 6f64 6572 0d0a 2020 2020  bj.encoder..    
-00013950: 584f 626a 5f73 7461 7473 203d 204f 626a  XObj_stats = Obj
-00013960: 2e73 7461 7469 7374 6963 0d0a 2020 2020  .statistic..    
-00013970: 584f 626a 5f73 6861 7065 203d 204f 626a  XObj_shape = Obj
-00013980: 2e73 6861 7065 0d0a 0d0a 2020 2020 6966  .shape....    if
-00013990: 2073 6176 655f 6d65 6d6f 7279 203a 0d0a   save_memory :..
-000139a0: 2020 2020 2020 2020 6465 6c20 496e 704f          del InpO
-000139b0: 626a 2e64 6174 610d 0a20 2020 2020 2020  bj.data..       
-000139c0: 2064 656c 2049 6e70 4f62 6a0d 0a20 2020   del InpObj..   
-000139d0: 2020 2020 2067 632e 636f 6c6c 6563 7428       gc.collect(
-000139e0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-000139f0: 2020 2020 200d 0a20 2020 2069 6628 7468       ..    if(th
-00013a00: 6973 5f74 7970 653d 3d73 7061 7273 6529  is_type==sparse)
-00013a10: 3a0d 0a20 2020 2020 2020 204f 626a 203d  :..        Obj =
-00013a20: 2064 656e 7365 284f 626a 290d 0a20 2020   dense(Obj)..   
-00013a30: 2069 6628 7468 6973 5f74 7970 6520 6e6f   if(this_type no
-00013a40: 7420 696e 205b 6465 6e73 652c 7370 6172  t in [dense,spar
-00013a50: 7365 5d29 3a0d 0a20 2020 2020 2020 2065  se]):..        e
-00013a60: 7272 6f72 2822 4572 726f 725b 7376 645d  rror("Error[svd]
-00013a70: 3a20 4f62 6a65 6374 2074 7970 6520 6d75  : Object type mu
-00013a80: 7374 206f 6e6c 7920 6265 2064 656e 7365  st only be dense
-00013a90: 206f 7220 7370 6172 7365 2122 290d 0a20   or sparse!").. 
-00013aa0: 2020 2020 2020 200d 0a20 2020 2023 2063         ..    # c
-00013ab0: 6865 636b 2069 6620 4f62 6a2e 7374 6174  heck if Obj.stat
-00013ac0: 6973 7469 6320 6f72 2066 696e 616c 5f73  istic or final_s
-00013ad0: 7461 7469 7374 6963 2069 7320 7765 6972  tatistic is weir
-00013ae0: 6420 6f72 206e 6f74 0d0a 2020 2020 666f  d or not..    fo
-00013af0: 7220 7374 6174 2069 6e20 4f62 6a2e 7374  r stat in Obj.st
-00013b00: 6174 6973 7469 633a 0d0a 2020 2020 2020  atistic:..      
-00013b10: 2020 6966 2873 7461 7420 6e6f 7420 696e    if(stat not in
-00013b20: 2061 6c6c 6f77 6564 5f73 7461 7429 3a0d   allowed_stat):.
-00013b30: 0a20 2020 2020 2020 2020 2020 2065 7272  .            err
-00013b40: 6f72 2822 4572 726f 725b 7376 645d 3a20  or("Error[svd]: 
-00013b50: 5468 6520 696e 7075 7420 6f62 6a65 6374  The input object
-00013b60: 2063 6f6e 7461 696e 7320 696c 6c65 6761   contains illega
-00013b70: 6c20 7374 6174 6973 7469 632e 2028 302c  l statistic. (0,
-00013b80: 2031 2c20 2d31 2c20 6f72 2022 2b68 7962   1, -1, or "+hyb
-00013b90: 7269 645f 7379 6d62 6f6c 2b22 206f 6e6c  rid_symbol+" onl
-00013ba0: 7929 2229 0d0a 0d0a 2020 2020 6966 2073  y)")....    if s
-00013bb0: 7472 696e 672e 636f 756e 7428 2228 2229  tring.count("(")
-00013bc0: 3d3d 7374 7269 6e67 2e63 6f75 6e74 2822  ==string.count("
-00013bd0: 2922 2920 616e 6420 7374 7269 6e67 2e63  )") and string.c
-00013be0: 6f75 6e74 2822 2822 293e 303a 0d0a 2020  ount("(")>0:..  
-00013bf0: 2020 2020 2020 7374 7269 6e67 203d 2073        string = s
-00013c00: 7472 696e 672e 7265 706c 6163 6528 2220  tring.replace(" 
-00013c10: 222c 2222 290d 0a20 2020 2020 2020 2073  ","")..        s
-00013c20: 7472 696e 6720 3d20 7374 7269 6e67 2e72  tring = string.r
-00013c30: 6570 6c61 6365 2822 2928 222c 2220 2229  eplace(")("," ")
-00013c40: 0d0a 2020 2020 2020 2020 6966 2073 7472  ..        if str
-00013c50: 696e 672e 636f 756e 7428 2228 2229 3e31  ing.count("(")>1
-00013c60: 206f 7220 7374 7269 6e67 2e63 6f75 6e74   or string.count
-00013c70: 2822 2922 293c 313a 0d0a 2020 2020 2020  (")")<1:..      
-00013c80: 2020 2020 2020 6572 726f 7228 2245 7272        error("Err
-00013c90: 6f72 5b73 7664 5d3a 2050 6172 656e 7468  or[svd]: Parenth
-00013ca0: 6573 6573 2064 6f6e 2774 206d 6174 6368  eses don't match
-00013cb0: 2229 0d0a 2020 2020 2020 2020 7374 7269  ")..        stri
-00013cc0: 6e67 203d 2073 7472 696e 672e 7265 706c  ng = string.repl
-00013cd0: 6163 6528 2229 222c 2222 290d 0a20 2020  ace(")","")..   
-00013ce0: 2020 2020 2073 7472 696e 6720 3d20 7374       string = st
-00013cf0: 7269 6e67 2e72 6570 6c61 6365 2822 2822  ring.replace("("
-00013d00: 2c22 2229 0d0a 0d0a 2020 2020 7061 7274  ,"")....    part
-00013d10: 6974 696f 6e5f 636f 756e 7420 3d20 300d  ition_count = 0.
-00013d20: 0a20 2020 2066 6f72 2070 6172 7469 7469  .    for partiti
-00013d30: 6f6e 2069 6e20 7365 7061 7261 746f 725f  on in separator_
-00013d40: 6c69 7374 3a0d 0a20 2020 2020 2020 2070  list:..        p
-00013d50: 6172 7469 7469 6f6e 5f63 6f75 6e74 202b  artition_count +
-00013d60: 3d20 7374 7269 6e67 2e63 6f75 6e74 2870  = string.count(p
-00013d70: 6172 7469 7469 6f6e 290d 0a20 2020 2069  artition)..    i
-00013d80: 6628 7061 7274 6974 696f 6e5f 636f 756e  f(partition_coun
-00013d90: 7421 3d31 293a 0d0a 2020 2020 2020 2020  t!=1):..        
-00013da0: 7061 7274 6974 696f 6e5f 7374 7269 6e67  partition_string
-00013db0: 203d 2022 220d 0a20 2020 2020 2020 2066   = ""..        f
-00013dc0: 6f72 2069 2c20 7061 7274 6974 696f 6e20  or i, partition 
-00013dd0: 696e 2065 6e75 6d65 7261 7465 2873 6570  in enumerate(sep
-00013de0: 6172 6174 6f72 5f6c 6973 7429 3a0d 0a20  arator_list):.. 
-00013df0: 2020 2020 2020 2020 2020 2069 6628 693d             if(i=
-00013e00: 3d30 293a 0d0a 2020 2020 2020 2020 2020  =0):..          
-00013e10: 2020 2020 2020 7061 7274 6974 696f 6e5f        partition_
-00013e20: 7374 7269 6e67 202b 3d20 2228 2022 0d0a  string += "( "..
-00013e30: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00013e40: 2869 3d3d 6c65 6e28 7365 7061 7261 746f  (i==len(separato
-00013e50: 725f 6c69 7374 292d 3129 3a0d 0a20 2020  r_list)-1):..   
-00013e60: 2020 2020 2020 2020 2020 2020 2070 6172               par
-00013e70: 7469 7469 6f6e 5f73 7472 696e 6720 2b3d  tition_string +=
-00013e80: 2022 2c20 6f72 2022 0d0a 2020 2020 2020   ", or "..      
-00013e90: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00013ea0: 2020 2020 2020 2020 2020 2020 2070 6172               par
-00013eb0: 7469 7469 6f6e 5f73 7472 696e 6720 2b3d  tition_string +=
-00013ec0: 2022 2c20 220d 0a0d 0a20 2020 2020 2020   ", "....       
-00013ed0: 2020 2020 2070 6172 7469 7469 6f6e 5f73       partition_s
-00013ee0: 7472 696e 6720 2b3d 2022 2722 2b70 6172  tring += "'"+par
-00013ef0: 7469 7469 6f6e 2b22 2722 0d0a 0d0a 2020  tition+"'"....  
-00013f00: 2020 2020 2020 2020 2020 6966 2869 3d3d            if(i==
-00013f10: 6c65 6e28 7365 7061 7261 746f 725f 6c69  len(separator_li
-00013f20: 7374 292d 3129 3a0d 0a20 2020 2020 2020  st)-1):..       
-00013f30: 2020 2020 2020 2020 2070 6172 7469 7469           partiti
-00013f40: 6f6e 5f73 7472 696e 6720 2b3d 2022 2029  on_string += " )
-00013f50: 220d 0a0d 0a20 2020 2020 2020 2065 7272  "....        err
-00013f60: 6f72 2822 4572 726f 725b 7376 645d 3a20  or("Error[svd]: 
-00013f70: 5468 6520 696e 7075 7420 7374 7269 6e67  The input string
-00013f80: 206d 7573 7420 636f 6e74 6169 6e20 6f6e   must contain on
-00013f90: 6520 616e 6420 6f6e 6c79 206f 6e65 2070  e and only one p
-00013fa0: 6172 7469 7469 6f6e 2022 2b70 6172 7469  artition "+parti
-00013fb0: 7469 6f6e 5f73 7472 696e 672b 2220 696e  tion_string+" in
-00013fc0: 2069 742e 2229 0d0a 0d0a 2020 2020 7374   it.")....    st
-00013fd0: 6570 203d 2073 686f 775f 7072 6f67 7265  ep = show_progre
-00013fe0: 7373 2873 7465 702c 7072 6f63 6573 735f  ss(step,process_
-00013ff0: 6c65 6e67 7468 2c70 726f 6365 7373 5f6e  length,process_n
-00014000: 616d 652b 2220 222b 223c 222b 6375 7272  ame+" "+"<"+curr
-00014010: 656e 745f 6d65 6d6f 7279 5f64 6973 706c  ent_memory_displ
-00014020: 6179 2829 2b22 3e22 2c63 6f6c 6f72 3d70  ay()+">",color=p
-00014030: 726f 6365 7373 5f63 6f6c 6f72 2c74 696d  rocess_color,tim
-00014040: 653d 7469 6d65 2e74 696d 6528 292d 7330  e=time.time()-s0
-00014050: 3029 2023 310d 0a20 2020 2023 3a3a 3a3a  0) #1..    #::::
+000129f0: 7370 6172 7365 284f 626a 290d 0a0d 0a20  sparse(Obj).... 
+00012a00: 2020 2043 203d 204f 626a 2e63 6f6f 7264     C = Obj.coord
+00012a10: 730d 0a20 2020 2066 6f72 2078 2069 6e20  s..    for x in 
+00012a20: 433a 0d0a 2020 2020 2020 2020 7061 7269  C:..        pari
+00012a30: 7479 203d 2073 756d 285b 2069 6e64 2066  ty = sum([ ind f
+00012a40: 6f72 2069 2c69 6e64 2069 6e20 656e 756d  or i,ind in enum
+00012a50: 6572 6174 6528 7829 2069 6620 4f62 6a2e  erate(x) if Obj.
+00012a60: 7374 6174 6973 7469 635b 695d 2069 6e20  statistic[i] in 
+00012a70: 6665 726d 695f 7479 7065 205d 290d 0a20  fermi_type ]).. 
+00012a80: 2020 2020 2020 2069 6620 7061 7269 7479         if parity
+00012a90: 2532 213d 3020 3a0d 0a20 2020 2020 2020  %2!=0 :..       
+00012aa0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00012ab0: 650d 0a20 2020 2072 6574 7572 6e20 5472  e..    return Tr
+00012ac0: 7565 0d0a 0d0a 2323 2323 2323 2323 2323  ue....##########
+00012ad0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00012ae0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00012af0: 2323 2323 2323 2323 2323 0d0a 2323 2020  ##########..##  
+00012b00: 2020 2020 2020 2020 5369 6e67 756c 6172          Singular
+00012b10: 2076 616c 7565 2064 6563 6f6d 706f 7369   value decomposi
+00012b20: 7469 6f6e 2020 2020 2020 2020 2020 2323  tion          ##
+00012b30: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+00012b40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00012b50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00012b60: 2323 2323 2323 0d0a 0d0a 6465 6620 536f  ######....def So
+00012b70: 7274 6564 5356 4428 4d2c 6375 746f 6666  rtedSVD(M,cutoff
+00012b80: 3d4e 6f6e 6529 3a0d 0a20 2020 2055 2c20  =None):..    U, 
+00012b90: ce9b 2c20 5620 3d20 6e70 2e6c 696e 616c  .., V = np.linal
+00012ba0: 672e 7376 6428 4d2c 2066 756c 6c5f 6d61  g.svd(M, full_ma
+00012bb0: 7472 6963 6573 3d46 616c 7365 290d 0a0d  trices=False)...
+00012bc0: 0a0d 0a20 2020 206e 6e7a 203d 2030 0d0a  ...    nnz = 0..
+00012bd0: 2020 2020 2369 6620 6e70 2e61 6273 28ce      #if np.abs(.
+00012be0: 9b5b 305d 2920 3c20 6e75 6d65 725f 6375  .[0]) < numer_cu
+00012bf0: 746f 6666 3a0d 0a20 2020 2023 2020 2020  toff:..    #    
+00012c00: 6572 726f 7228 2245 7272 6f72 5b53 6f72  error("Error[Sor
+00012c10: 7465 6453 5644 5d3a 206e 702e 6c69 6e61  tedSVD]: np.lina
+00012c20: 6c67 2e73 7664 2829 2072 6574 7572 6e73  lg.svd() returns
+00012c30: 207a 6572 6f20 7369 6e67 756c 6172 2076   zero singular v
+00012c40: 616c 7565 2076 6563 746f 7221 2229 0d0a  alue vector!")..
+00012c50: 0d0a 2020 2020 666f 7220 692c 7320 696e  ..    for i,s in
+00012c60: 2065 6e75 6d65 7261 7465 28ce 9b29 3a0d   enumerate(..):.
+00012c70: 0a20 2020 2020 2020 2069 6620 6e70 2e61  .        if np.a
+00012c80: 6273 2873 2fce 9b5b 305d 2920 3e20 6e75  bs(s/..[0]) > nu
+00012c90: 6d65 725f 6375 746f 6666 3a0d 0a20 2020  mer_cutoff:..   
+00012ca0: 2020 2020 2020 2020 206e 6e7a 2b3d 310d           nnz+=1.
+00012cb0: 0a0d 0a20 2020 2069 6620 6375 746f 6666  ...    if cutoff
+00012cc0: 213d 4e6f 6e65 2061 6e64 2063 7574 6f66  !=None and cutof
+00012cd0: 6620 3c20 6e6e 7a3a 0d0a 2020 2020 2020  f < nnz:..      
+00012ce0: 2020 6e6e 7a20 3d20 6375 746f 6666 0d0a    nnz = cutoff..
+00012cf0: 0d0a 2020 2020 ce9b 203d 20ce 9b5b 3a6e  ..    .. = ..[:n
+00012d00: 6e7a 5d0d 0a20 2020 2055 203d 2055 5b3a  nz]..    U = U[:
+00012d10: 2c3a 6e6e 7a5d 0d0a 2020 2020 5620 3d20  ,:nnz]..    V = 
+00012d20: 565b 3a6e 6e7a 2c3a 5d0d 0a0d 0a0d 0a20  V[:nnz,:]...... 
+00012d30: 2020 2072 6574 7572 6e20 552c 20ce 9b2c     return U, ..,
+00012d40: 2056 0d0a 2320 4920 3d20 6355 5520 3d20   V..# I = cUU = 
+00012d50: 5663 560d 0a64 6566 2042 6c6f 636b 5356  VcV..def BlockSV
+00012d60: 4428 4f62 6a2c 6375 746f 6666 3d4e 6f6e  D(Obj,cutoff=Non
+00012d70: 6529 3a0d 0a20 2020 200d 0a20 2020 2023  e):..    ..    #
+00012d80: 2070 6572 666f 726d 696e 6720 616e 2073   performing an s
+00012d90: 7664 206f 6620 6120 6d61 7472 6978 2062  vd of a matrix b
+00012da0: 6c6f 636b 2062 7920 626c 6f63 6b0d 0a0d  lock by block...
+00012db0: 0a20 2020 2069 6628 7479 7065 284f 626a  .    if(type(Obj
+00012dc0: 2921 3d6e 702e 6172 7261 7920 616e 6420  )!=np.array and 
+00012dd0: 7479 7065 284f 626a 2921 3d6e 702e 6e64  type(Obj)!=np.nd
+00012de0: 6172 7261 7929 3a0d 0a20 2020 2020 2020  array):..       
+00012df0: 2065 7272 6f72 2822 4572 726f 725b 426c   error("Error[Bl
+00012e00: 6f63 6b53 5644 5d3a 2041 6e20 696e 7075  ockSVD]: An inpu
+00012e10: 7420 6d75 7374 2062 6520 6f66 2074 7970  t must be of typ
+00012e20: 6520 6e75 6d70 792e 6172 7261 7920 6f72  e numpy.array or
+00012e30: 206e 756d 7079 2e6e 6461 7272 6179 206f   numpy.ndarray o
+00012e40: 6e6c 7921 2229 0d0a 2020 2020 2020 2020  nly!")..        
+00012e50: 0d0a 0d0a 2020 2020 6966 284f 626a 2e6e  ....    if(Obj.n
+00012e60: 6469 6d21 3d32 293a 0d0a 2020 2020 2020  dim!=2):..      
+00012e70: 2020 6572 726f 7228 2245 7272 6f72 5b42    error("Error[B
+00012e80: 6c6f 636b 5356 445d 3a20 416e 2069 6e70  lockSVD]: An inp
+00012e90: 7574 206d 7573 7420 6265 2061 206d 6174  ut must be a mat
+00012ea0: 7269 7820 6f6e 6c79 2122 290d 0a20 2020  rix only!")..   
+00012eb0: 2020 2020 200d 0a0d 0a20 2020 206d 203d       ....    m =
+00012ec0: 204f 626a 2e73 6861 7065 5b30 5d0d 0a20   Obj.shape[0].. 
+00012ed0: 2020 206e 203d 204f 626a 2e73 6861 7065     n = Obj.shape
+00012ee0: 5b31 5d0d 0a0d 0a20 2020 2069 6628 6d25  [1]....    if(m%
+00012ef0: 3221 3d30 2061 6e64 206e 2532 213d 3029  2!=0 and n%2!=0)
+00012f00: 3a0d 0a20 2020 2020 2020 2065 7272 6f72  :..        error
+00012f10: 2822 4572 726f 725b 426c 6f63 6b53 5644  ("Error[BlockSVD
+00012f20: 5d3a 2054 6865 206d 6174 7269 7820 6469  ]: The matrix di
+00012f30: 6d65 6e73 696f 6e73 206d 7573 7420 6265  mensions must be
+00012f40: 2065 7665 6e21 2229 0d0a 2020 2020 2020   even!")..      
+00012f50: 2020 0d0a 0d0a 0d0a 2020 2020 6966 286d    ......    if(m
+00012f60: 3d3d 3020 616e 6420 6e3d 3d30 293a 0d0a  ==0 and n==0):..
+00012f70: 2020 2020 2020 2020 6572 726f 7228 2245          error("E
+00012f80: 7272 6f72 5b42 6c6f 636b 5356 445d 3a20  rror[BlockSVD]: 
+00012f90: 5468 6520 6d61 7472 6978 2064 696d 656e  The matrix dimen
+00012fa0: 7369 6f6e 7320 6d75 7374 2062 6520 6174  sions must be at
+00012fb0: 206c 6561 7374 2032 2122 290d 0a20 2020   least 2!")..   
+00012fc0: 2020 2020 200d 0a0d 0a20 2020 2070 6172       ....    par
+00012fd0: 6974 795f 6e6f 726d 203d 2030 0d0a 2020  ity_norm = 0..  
+00012fe0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00012ff0: 286d 293a 0d0a 2020 2020 2020 2020 666f  (m):..        fo
+00013000: 7220 6a20 696e 2072 616e 6765 286e 293a  r j in range(n):
+00013010: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00013020: 2028 692b 6a29 2532 213d 303a 0d0a 2020   (i+j)%2!=0:..  
+00013030: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00013040: 7269 7479 5f6e 6f72 6d20 2b3d 206e 702e  rity_norm += np.
+00013050: 6c69 6e61 6c67 2e6e 6f72 6d28 4f62 6a5b  linalg.norm(Obj[
+00013060: 692c 6a5d 290d 0a20 2020 2069 6628 2028  i,j])..    if( (
+00013070: 6e6f 7420 736b 6970 5f70 6172 6974 795f  not skip_parity_
+00013080: 626c 6f63 6b69 6e67 5f63 6865 636b 2920  blocking_check) 
+00013090: 616e 6420 7061 7269 7479 5f6e 6f72 6d2f  and parity_norm/
+000130a0: 286d 2a6e 2f32 293e 312e 3065 2d31 3429  (m*n/2)>1.0e-14)
+000130b0: 3a0d 0a20 2020 2020 2020 2065 7272 6f72  :..        error
+000130c0: 2822 4572 726f 725b 426c 6f63 6b53 5644  ("Error[BlockSVD
+000130d0: 5d3a 2054 6869 7320 6d61 7472 6978 2069  ]: This matrix i
+000130e0: 7320 6e6f 7420 636f 6e73 7472 7563 7465  s not constructe
+000130f0: 6420 6672 6f6d 2061 2047 7261 7373 6d61  d from a Grassma
+00013100: 6e6e 2d65 7665 6e20 7465 6e73 6f72 2e22  nn-even tensor."
+00013110: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
+00013120: 2822 2020 2020 2020 2020 2020 2020 2020  ("              
+00013130: 2020 2028 4f72 2074 6861 7420 6f6e 6520     (Or that one 
+00013140: 6f66 2074 6865 2069 6e64 6963 6573 2061  of the indices a
+00013150: 7265 206e 6f6e 2d66 6572 6d69 6f6e 6963  re non-fermionic
+00013160: 2e29 2229 0d0a 2020 2020 2020 2020 0d0a  .)")..        ..
+00013170: 0d0a 2020 2020 2320 4174 2074 6869 7320  ..    # At this 
+00013180: 706f 696e 7420 7468 6520 6d61 7472 6978  point the matrix
+00013190: 2069 7320 7765 6c6c 2d62 6568 6176 6564   is well-behaved
+000131a0: 0d0a 0d0a 2020 2020 2320 7469 6d65 2074  ....    # time t
+000131b0: 6f20 7365 7061 7261 7465 2074 6865 2062  o separate the b
+000131c0: 6c6f 636b 730d 0a20 2020 204d 4520 3d20  locks..    ME = 
+000131d0: 6e70 2e7a 6572 6f73 285b 696e 7428 6d2f  np.zeros([int(m/
+000131e0: 3229 2c69 6e74 286e 2f32 295d 2c64 7479  2),int(n/2)],dty
+000131f0: 7065 3d74 7970 6528 4f62 6a5b 305d 5b30  pe=type(Obj[0][0
+00013200: 5d29 290d 0a20 2020 204d 4f20 3d20 6e70  ]))..    MO = np
+00013210: 2e7a 6572 6f73 285b 696e 7428 6d2f 3229  .zeros([int(m/2)
+00013220: 2c69 6e74 286e 2f32 295d 2c64 7479 7065  ,int(n/2)],dtype
+00013230: 3d74 7970 6528 4f62 6a5b 305d 5b30 5d29  =type(Obj[0][0])
+00013240: 290d 0a0d 0a20 2020 2066 6f72 2069 2069  )....    for i i
+00013250: 6e20 7261 6e67 6528 696e 7428 6d2f 3229  n range(int(m/2)
+00013260: 293a 0d0a 2020 2020 2020 2020 666f 7220  ):..        for 
+00013270: 6a20 696e 2072 616e 6765 2869 6e74 286e  j in range(int(n
+00013280: 2f32 2929 3a0d 0a20 2020 2020 2020 2020  /2)):..         
+00013290: 2020 204d 455b 692c 6a5d 203d 204f 626a     ME[i,j] = Obj
+000132a0: 5b32 2a69 2c32 2a6a 5d0d 0a20 2020 2020  [2*i,2*j]..     
+000132b0: 2020 2020 2020 204d 4f5b 692c 6a5d 203d         MO[i,j] =
+000132c0: 204f 626a 5b32 2a69 2b31 2c32 2a6a 2b31   Obj[2*i+1,2*j+1
+000132d0: 5d0d 0a0d 0a20 2020 2068 616c 6663 7574  ]....    halfcut
+000132e0: 6f66 6620 3d20 4e6f 6e65 0d0a 2020 2020  off = None..    
+000132f0: 6966 2063 7574 6f66 6621 3d4e 6f6e 6520  if cutoff!=None 
+00013300: 3a0d 0a20 2020 2020 2020 2068 616c 6663  :..        halfc
+00013310: 7574 6f66 6620 3d20 696e 7428 6375 746f  utoff = int(cuto
+00013320: 6666 2f32 290d 0a0d 0a20 2020 2055 452c  ff/2)....    UE,
+00013330: 20ce 9b45 2c20 5645 203d 2053 6f72 7465   ..E, VE = Sorte
+00013340: 6453 5644 284d 452c 6861 6c66 6375 746f  dSVD(ME,halfcuto
+00013350: 6666 290d 0a20 2020 2055 4f2c 20ce 9b4f  ff)..    UO, ..O
+00013360: 2c20 564f 203d 2053 6f72 7465 6453 5644  , VO = SortedSVD
+00013370: 284d 4f2c 6861 6c66 6375 746f 6666 290d  (MO,halfcutoff).
+00013380: 0a0d 0a20 2020 2064 203d 206d 6178 286c  ...    d = max(l
+00013390: 656e 28ce 9b45 292c 6c65 6e28 ce9b 4f29  en(..E),len(..O)
+000133a0: 290d 0a20 2020 2064 203d 2069 6e74 2832  )..    d = int(2
+000133b0: 2a2a 6d61 7468 2e63 6569 6c28 6e70 2e6c  **math.ceil(np.l
+000133c0: 6f67 3228 6429 2929 0d0a 0d0a 2020 2020  og2(d)))....    
+000133d0: 6465 6620 7061 6464 696e 6728 5578 2c20  def padding(Ux, 
+000133e0: ce9b 782c 2056 782c 2070 6164 6469 6e67  ..x, Vx, padding
+000133f0: 5f64 696d 656e 7369 6f6e 293a 0d0a 2020  _dimension):..  
+00013400: 2020 2020 2020 5578 203d 206e 702e 7061        Ux = np.pa
+00013410: 6428 5578 2c28 2830 2c30 292c 2830 2c70  d(Ux,((0,0),(0,p
+00013420: 6164 6469 6e67 5f64 696d 656e 7369 6f6e  adding_dimension
+00013430: 2929 2c27 636f 6e73 7461 6e74 272c 636f  )),'constant',co
+00013440: 6e73 7461 6e74 5f76 616c 7565 733d 2828  nstant_values=((
+00013450: 302c 3029 2c28 302c 3029 2929 0d0a 2020  0,0),(0,0)))..  
+00013460: 2020 2020 2020 ce9b 7820 3d20 6e70 2e64        ..x = np.d
+00013470: 6961 6728 6e70 2e70 6164 28ce 9b78 2c28  iag(np.pad(..x,(
+00013480: 302c 7061 6464 696e 675f 6469 6d65 6e73  0,padding_dimens
+00013490: 696f 6e29 2c27 636f 6e73 7461 6e74 272c  ion),'constant',
+000134a0: 636f 6e73 7461 6e74 5f76 616c 7565 733d  constant_values=
+000134b0: 2020 2028 302c 3029 2020 2020 2929 0d0a     (0,0)    ))..
+000134c0: 2020 2020 2020 2020 5678 203d 206e 702e          Vx = np.
+000134d0: 7061 6428 5678 2c28 2830 2c70 6164 6469  pad(Vx,((0,paddi
+000134e0: 6e67 5f64 696d 656e 7369 6f6e 292c 2830  ng_dimension),(0
+000134f0: 2c30 2929 2c27 636f 6e73 7461 6e74 272c  ,0)),'constant',
+00013500: 636f 6e73 7461 6e74 5f76 616c 7565 733d  constant_values=
+00013510: 2828 302c 3029 2c28 302c 3029 2929 0d0a  ((0,0),(0,0)))..
+00013520: 2020 2020 2020 2020 7265 7475 726e 2055          return U
+00013530: 782c 20ce 9b78 2c20 5678 0d0a 0d0a 2020  x, ..x, Vx....  
+00013540: 2020 5545 2c20 ce9b 452c 2056 4520 3d20    UE, ..E, VE = 
+00013550: 7061 6464 696e 6728 5545 2c20 ce9b 452c  padding(UE, ..E,
+00013560: 2056 452c 2064 2d6c 656e 28ce 9b45 2929   VE, d-len(..E))
+00013570: 0d0a 2020 2020 554f 2c20 ce9b 4f2c 2056  ..    UO, ..O, V
+00013580: 4f20 3d20 7061 6464 696e 6728 554f 2c20  O = padding(UO, 
+00013590: ce9b 4f2c 2056 4f2c 2064 2d6c 656e 28ce  ..O, VO, d-len(.
+000135a0: 9b4f 2929 0d0a 0d0a 2020 2020 6465 6620  .O))....    def 
+000135b0: 6765 745f 6675 6c6c 5f6d 6174 7269 7828  get_full_matrix(
+000135c0: 4145 2c20 414f 293a 0d0a 2020 2020 2020  AE, AO):..      
+000135d0: 2020 6d68 616c 662c 6e68 616c 6620 3d20    mhalf,nhalf = 
+000135e0: 4145 2e73 6861 7065 0d0a 2020 2020 2020  AE.shape..      
+000135f0: 2020 4120 3d20 6e70 2e7a 6572 6f73 285b    A = np.zeros([
+00013600: 322a 6d68 616c 662c 322a 6e68 616c 665d  2*mhalf,2*nhalf]
+00013610: 2c64 7479 7065 3d74 7970 6528 4145 5b30  ,dtype=type(AE[0
+00013620: 5d5b 305d 2929 0d0a 2020 2020 2020 2020  ][0]))..        
+00013630: 666f 7220 6920 696e 2072 616e 6765 286d  for i in range(m
+00013640: 6861 6c66 293a 0d0a 2020 2020 2020 2020  half):..        
+00013650: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+00013660: 6765 286e 6861 6c66 293a 0d0a 2020 2020  ge(nhalf):..    
+00013670: 2020 2020 2020 2020 2020 2020 415b 322a              A[2*
+00013680: 692c 322a 6a5d 203d 2041 455b 692c 6a5d  i,2*j] = AE[i,j]
+00013690: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000136a0: 2020 415b 322a 692b 312c 322a 6a2b 315d    A[2*i+1,2*j+1]
+000136b0: 203d 2041 4f5b 692c 6a5d 0d0a 2020 2020   = AO[i,j]..    
+000136c0: 2020 2020 7265 7475 726e 2041 0d0a 0d0a      return A....
+000136d0: 2020 2020 5520 3d20 6765 745f 6675 6c6c      U = get_full
+000136e0: 5f6d 6174 7269 7828 5545 2c55 4f29 0d0a  _matrix(UE,UO)..
+000136f0: 2020 2020 ce9b 203d 2067 6574 5f66 756c      .. = get_ful
+00013700: 6c5f 6d61 7472 6978 28ce 9b45 2cce 9b4f  l_matrix(..E,..O
+00013710: 290d 0a20 2020 2056 203d 2067 6574 5f66  )..    V = get_f
+00013720: 756c 6c5f 6d61 7472 6978 2856 452c 564f  ull_matrix(VE,VO
+00013730: 290d 0a20 2020 200d 0a0d 0a20 2020 2072  )..    ....    r
+00013740: 6574 7572 6e20 552c 20ce 9b2c 2056 0d0a  eturn U, .., V..
+00013750: 0d0a 6465 6620 7376 6428 496e 704f 626a  ..def svd(InpObj
+00013760: 2c73 7472 696e 672c 6375 746f 6666 3d4e  ,string,cutoff=N
+00013770: 6f6e 652c 7361 7665 5f6d 656d 6f72 793d  one,save_memory=
+00013780: 4661 6c73 6529 3a0d 0a0d 0a20 2020 2070  False):....    p
+00013790: 726f 6365 7373 5f6e 616d 6520 3d20 2273  rocess_name = "s
+000137a0: 7664 220d 0a20 2020 2070 726f 6365 7373  vd"..    process
+000137b0: 5f63 6f6c 6f72 203d 2022 7965 6c6c 6f77  _color = "yellow
+000137c0: 220d 0a20 2020 2070 726f 6365 7373 5f6c  "..    process_l
+000137d0: 656e 6774 6820 3d20 360d 0a20 2020 2073  ength = 6..    s
+000137e0: 7465 7020 3d20 310d 0a20 2020 2073 3030  tep = 1..    s00
+000137f0: 203d 2074 696d 652e 7469 6d65 2829 0d0a   = time.time()..
+00013800: 2020 2020 7072 6f67 7265 7373 5f73 7061      progress_spa
+00013810: 6365 2829 0d0a 0d0a 2020 2020 676c 6f62  ce()....    glob
+00013820: 616c 2073 6b69 705f 706f 7765 725f 6f66  al skip_power_of
+00013830: 5f74 776f 5f63 6865 636b 0d0a 0d0a 2020  _two_check....  
+00013840: 2020 2320 7468 6520 7374 7269 6e67 2069    # the string i
+00013850: 7320 6f66 2074 6865 2066 6f72 6d20 6161  s of the form aa
+00013860: 6161 7c62 6262 0d0a 0d0a 2020 2020 7374  aa|bbb....    st
+00013870: 7269 6e67 203d 2064 656e 756d 6572 6174  ring = denumerat
+00013880: 6528 7374 7269 6e67 290d 0a0d 0a20 2020  e(string)....   
+00013890: 200d 0a20 2020 204f 626a 203d 2049 6e70   ..    Obj = Inp
+000138a0: 4f62 6a2e 636f 7079 2829 0d0a 2020 2020  Obj.copy()..    
+000138b0: 7468 6973 5f74 7970 6520 3d20 7479 7065  this_type = type
+000138c0: 284f 626a 290d 0a20 2020 2074 6869 735f  (Obj)..    this_
+000138d0: 666f 726d 6174 203d 204f 626a 2e66 6f72  format = Obj.for
+000138e0: 6d61 740d 0a20 2020 2074 6869 735f 656e  mat..    this_en
+000138f0: 636f 6465 7220 3d20 4f62 6a2e 656e 636f  coder = Obj.enco
+00013900: 6465 720d 0a20 2020 2058 4f62 6a5f 7374  der..    XObj_st
+00013910: 6174 7320 3d20 4f62 6a2e 7374 6174 6973  ats = Obj.statis
+00013920: 7469 630d 0a20 2020 2058 4f62 6a5f 7368  tic..    XObj_sh
+00013930: 6170 6520 3d20 4f62 6a2e 7368 6170 650d  ape = Obj.shape.
+00013940: 0a0d 0a20 2020 2069 6620 7361 7665 5f6d  ...    if save_m
+00013950: 656d 6f72 7920 3a0d 0a20 2020 2020 2020  emory :..       
+00013960: 2064 656c 2049 6e70 4f62 6a2e 6461 7461   del InpObj.data
+00013970: 0d0a 2020 2020 2020 2020 6465 6c20 496e  ..        del In
+00013980: 704f 626a 0d0a 2020 2020 2020 2020 6763  pObj..        gc
+00013990: 2e63 6f6c 6c65 6374 2829 0d0a 2020 2020  .collect()..    
+000139a0: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
+000139b0: 2020 2020 6966 2874 6869 735f 7479 7065      if(this_type
+000139c0: 3d3d 7370 6172 7365 293a 0d0a 2020 2020  ==sparse):..    
+000139d0: 2020 2020 4f62 6a20 3d20 6465 6e73 6528      Obj = dense(
+000139e0: 4f62 6a29 0d0a 2020 2020 6966 2874 6869  Obj)..    if(thi
+000139f0: 735f 7479 7065 206e 6f74 2069 6e20 5b64  s_type not in [d
+00013a00: 656e 7365 2c73 7061 7273 655d 293a 0d0a  ense,sparse]):..
+00013a10: 2020 2020 2020 2020 6572 726f 7228 2245          error("E
+00013a20: 7272 6f72 5b73 7664 5d3a 204f 626a 6563  rror[svd]: Objec
+00013a30: 7420 7479 7065 206d 7573 7420 6f6e 6c79  t type must only
+00013a40: 2062 6520 6465 6e73 6520 6f72 2073 7061   be dense or spa
+00013a50: 7273 6521 2229 0d0a 2020 2020 2020 2020  rse!")..        
+00013a60: 0d0a 2020 2020 2320 6368 6563 6b20 6966  ..    # check if
+00013a70: 204f 626a 2e73 7461 7469 7374 6963 206f   Obj.statistic o
+00013a80: 7220 6669 6e61 6c5f 7374 6174 6973 7469  r final_statisti
+00013a90: 6320 6973 2077 6569 7264 206f 7220 6e6f  c is weird or no
+00013aa0: 740d 0a20 2020 2066 6f72 2073 7461 7420  t..    for stat 
+00013ab0: 696e 204f 626a 2e73 7461 7469 7374 6963  in Obj.statistic
+00013ac0: 3a0d 0a20 2020 2020 2020 2069 6628 7374  :..        if(st
+00013ad0: 6174 206e 6f74 2069 6e20 616c 6c6f 7765  at not in allowe
+00013ae0: 645f 7374 6174 293a 0d0a 2020 2020 2020  d_stat):..      
+00013af0: 2020 2020 2020 6572 726f 7228 2245 7272        error("Err
+00013b00: 6f72 5b73 7664 5d3a 2054 6865 2069 6e70  or[svd]: The inp
+00013b10: 7574 206f 626a 6563 7420 636f 6e74 6169  ut object contai
+00013b20: 6e73 2069 6c6c 6567 616c 2073 7461 7469  ns illegal stati
+00013b30: 7374 6963 2e20 2830 2c20 312c 202d 312c  stic. (0, 1, -1,
+00013b40: 206f 7220 222b 6879 6272 6964 5f73 796d   or "+hybrid_sym
+00013b50: 626f 6c2b 2220 6f6e 6c79 2922 290d 0a0d  bol+" only)")...
+00013b60: 0a20 2020 2069 6620 7374 7269 6e67 2e63  .    if string.c
+00013b70: 6f75 6e74 2822 2822 293d 3d73 7472 696e  ount("(")==strin
+00013b80: 672e 636f 756e 7428 2229 2229 2061 6e64  g.count(")") and
+00013b90: 2073 7472 696e 672e 636f 756e 7428 2228   string.count("(
+00013ba0: 2229 3e30 3a0d 0a20 2020 2020 2020 2073  ")>0:..        s
+00013bb0: 7472 696e 6720 3d20 7374 7269 6e67 2e72  tring = string.r
+00013bc0: 6570 6c61 6365 2822 2022 2c22 2229 0d0a  eplace(" ","")..
+00013bd0: 2020 2020 2020 2020 7374 7269 6e67 203d          string =
+00013be0: 2073 7472 696e 672e 7265 706c 6163 6528   string.replace(
+00013bf0: 2229 2822 2c22 2022 290d 0a20 2020 2020  ")("," ")..     
+00013c00: 2020 2069 6620 7374 7269 6e67 2e63 6f75     if string.cou
+00013c10: 6e74 2822 2822 293e 3120 6f72 2073 7472  nt("(")>1 or str
+00013c20: 696e 672e 636f 756e 7428 2229 2229 3c31  ing.count(")")<1
+00013c30: 3a0d 0a20 2020 2020 2020 2020 2020 2065  :..            e
+00013c40: 7272 6f72 2822 4572 726f 725b 7376 645d  rror("Error[svd]
+00013c50: 3a20 5061 7265 6e74 6865 7365 7320 646f  : Parentheses do
+00013c60: 6e27 7420 6d61 7463 6822 290d 0a20 2020  n't match")..   
+00013c70: 2020 2020 2073 7472 696e 6720 3d20 7374       string = st
+00013c80: 7269 6e67 2e72 6570 6c61 6365 2822 2922  ring.replace(")"
+00013c90: 2c22 2229 0d0a 2020 2020 2020 2020 7374  ,"")..        st
+00013ca0: 7269 6e67 203d 2073 7472 696e 672e 7265  ring = string.re
+00013cb0: 706c 6163 6528 2228 222c 2222 290d 0a0d  place("(","")...
+00013cc0: 0a20 2020 2070 6172 7469 7469 6f6e 5f63  .    partition_c
+00013cd0: 6f75 6e74 203d 2030 0d0a 2020 2020 666f  ount = 0..    fo
+00013ce0: 7220 7061 7274 6974 696f 6e20 696e 2073  r partition in s
+00013cf0: 6570 6172 6174 6f72 5f6c 6973 743a 0d0a  eparator_list:..
+00013d00: 2020 2020 2020 2020 7061 7274 6974 696f          partitio
+00013d10: 6e5f 636f 756e 7420 2b3d 2073 7472 696e  n_count += strin
+00013d20: 672e 636f 756e 7428 7061 7274 6974 696f  g.count(partitio
+00013d30: 6e29 0d0a 2020 2020 6966 2870 6172 7469  n)..    if(parti
+00013d40: 7469 6f6e 5f63 6f75 6e74 213d 3129 3a0d  tion_count!=1):.
+00013d50: 0a20 2020 2020 2020 2070 6172 7469 7469  .        partiti
+00013d60: 6f6e 5f73 7472 696e 6720 3d20 2222 0d0a  on_string = ""..
+00013d70: 2020 2020 2020 2020 666f 7220 692c 2070          for i, p
+00013d80: 6172 7469 7469 6f6e 2069 6e20 656e 756d  artition in enum
+00013d90: 6572 6174 6528 7365 7061 7261 746f 725f  erate(separator_
+00013da0: 6c69 7374 293a 0d0a 2020 2020 2020 2020  list):..        
+00013db0: 2020 2020 6966 2869 3d3d 3029 3a0d 0a20      if(i==0):.. 
+00013dc0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00013dd0: 6172 7469 7469 6f6e 5f73 7472 696e 6720  artition_string 
+00013de0: 2b3d 2022 2820 220d 0a20 2020 2020 2020  += "( "..       
+00013df0: 2020 2020 2065 6c69 6628 693d 3d6c 656e       elif(i==len
+00013e00: 2873 6570 6172 6174 6f72 5f6c 6973 7429  (separator_list)
+00013e10: 2d31 293a 0d0a 2020 2020 2020 2020 2020  -1):..          
+00013e20: 2020 2020 2020 7061 7274 6974 696f 6e5f        partition_
+00013e30: 7374 7269 6e67 202b 3d20 222c 206f 7220  string += ", or 
+00013e40: 220d 0a20 2020 2020 2020 2020 2020 2065  "..            e
+00013e50: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00013e60: 2020 2020 2020 7061 7274 6974 696f 6e5f        partition_
+00013e70: 7374 7269 6e67 202b 3d20 222c 2022 0d0a  string += ", "..
+00013e80: 0d0a 2020 2020 2020 2020 2020 2020 7061  ..            pa
+00013e90: 7274 6974 696f 6e5f 7374 7269 6e67 202b  rtition_string +
+00013ea0: 3d20 2227 222b 7061 7274 6974 696f 6e2b  = "'"+partition+
+00013eb0: 2227 220d 0a0d 0a20 2020 2020 2020 2020  "'"....         
+00013ec0: 2020 2069 6628 693d 3d6c 656e 2873 6570     if(i==len(sep
+00013ed0: 6172 6174 6f72 5f6c 6973 7429 2d31 293a  arator_list)-1):
+00013ee0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013ef0: 2020 7061 7274 6974 696f 6e5f 7374 7269    partition_stri
+00013f00: 6e67 202b 3d20 2220 2922 0d0a 0d0a 2020  ng += " )"....  
+00013f10: 2020 2020 2020 6572 726f 7228 2245 7272        error("Err
+00013f20: 6f72 5b73 7664 5d3a 2054 6865 2069 6e70  or[svd]: The inp
+00013f30: 7574 2073 7472 696e 6720 6d75 7374 2063  ut string must c
+00013f40: 6f6e 7461 696e 206f 6e65 2061 6e64 206f  ontain one and o
+00013f50: 6e6c 7920 6f6e 6520 7061 7274 6974 696f  nly one partitio
+00013f60: 6e20 222b 7061 7274 6974 696f 6e5f 7374  n "+partition_st
+00013f70: 7269 6e67 2b22 2069 6e20 6974 2e22 290d  ring+" in it.").
+00013f80: 0a0d 0a20 2020 2073 7465 7020 3d20 7368  ...    step = sh
+00013f90: 6f77 5f70 726f 6772 6573 7328 7374 6570  ow_progress(step
+00013fa0: 2c70 726f 6365 7373 5f6c 656e 6774 682c  ,process_length,
+00013fb0: 7072 6f63 6573 735f 6e61 6d65 2b22 2022  process_name+" "
+00013fc0: 2b22 3c22 2b63 7572 7265 6e74 5f6d 656d  +"<"+current_mem
+00013fd0: 6f72 795f 6469 7370 6c61 7928 292b 223e  ory_display()+">
+00013fe0: 222c 636f 6c6f 723d 7072 6f63 6573 735f  ",color=process_
+00013ff0: 636f 6c6f 722c 7469 6d65 3d74 696d 652e  color,time=time.
+00014000: 7469 6d65 2829 2d73 3030 2920 2331 0d0a  time()-s00) #1..
+00014010: 2020 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a      #:::::::::::
+00014020: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014030: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014040: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014050: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00014060: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014070: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014080: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014090: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000140a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000140b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a 2020  ::::::::::::..  
-000140c0: 2020 233a 3a3a 3a3a 2020 2020 2020 5354    #:::::      ST
-000140d0: 4550 2031 202d 204a 4f49 4e20 4c45 4753  EP 1 - JOIN LEGS
-000140e0: 2042 4145 5344 204f 4e20 5448 4520 4752   BAESD ON THE GR
-000140f0: 4f55 5049 4e47 5320 2020 2020 2020 2020  OUPINGS         
-00014100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014110: 2020 2020 2020 2020 2020 2020 2020 3a3a                ::
-00014120: 3a3a 3a0d 0a20 2020 2023 3a3a 3a3a 3a3a  :::..    #::::::
+00014070: 3a3a 3a3a 3a0d 0a20 2020 2023 3a3a 3a3a  :::::..    #::::
+00014080: 3a20 2020 2020 2053 5445 5020 3120 2d20  :      STEP 1 - 
+00014090: 4a4f 494e 204c 4547 5320 4241 4553 4420  JOIN LEGS BAESD 
+000140a0: 4f4e 2054 4845 2047 524f 5550 494e 4753  ON THE GROUPINGS
+000140b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140d0: 2020 2020 2020 203a 3a3a 3a3a 0d0a 2020         :::::..  
+000140e0: 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a    #:::::::::::::
+000140f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014100: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014110: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014120: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00014130: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014140: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014150: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014160: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014170: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014180: 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a 0d0a 2020  ::::::::::....  
-00014190: 2020 2320 636f 756e 7420 7468 6520 6e75    # count the nu
-000141a0: 6d62 6572 206f 6620 696e 6469 6365 7320  mber of indices 
-000141b0: 696e 2074 6865 2074 776f 2067 726f 7570  in the two group
-000141c0: 730d 0a20 2020 206e 5f6c 6566 7420 3d20  s..    n_left = 
-000141d0: 300d 0a20 2020 206e 5f72 6967 6874 203d  0..    n_right =
-000141e0: 2030 0d0a 2020 2020 7061 7274 6974 696f   0..    partitio
-000141f0: 6e5f 666f 756e 6420 3d20 4661 6c73 650d  n_found = False.
-00014200: 0a20 2020 2066 6f72 2063 6861 7220 696e  .    for char in
-00014210: 2073 7472 696e 673a 0d0a 2020 2020 2020   string:..      
-00014220: 2020 6966 2063 6861 7220 696e 2073 6570    if char in sep
-00014230: 6172 6174 6f72 5f6c 6973 7420 3a0d 0a20  arator_list :.. 
-00014240: 2020 2020 2020 2020 2020 2070 6172 7469             parti
-00014250: 7469 6f6e 5f66 6f75 6e64 203d 2054 7275  tion_found = Tru
-00014260: 650d 0a20 2020 2020 2020 2020 2020 2063  e..            c
-00014270: 6f6e 7469 6e75 650d 0a20 2020 2020 2020  ontinue..       
-00014280: 2069 6628 7061 7274 6974 696f 6e5f 666f   if(partition_fo
-00014290: 756e 6429 3a0d 0a20 2020 2020 2020 2020  und):..         
-000142a0: 2020 206e 5f72 6967 6874 2b3d 310d 0a20     n_right+=1.. 
-000142b0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-000142c0: 2020 2020 2020 2020 2020 6e5f 6c65 6674            n_left
-000142d0: 2b3d 310d 0a0d 0a20 2020 206a 6f69 6e5f  +=1....    join_
-000142e0: 6c65 6773 5f73 7472 696e 675f 696e 7075  legs_string_inpu
-000142f0: 7420 3d20 7374 7269 6e67 0d0a 2020 2020  t = string..    
-00014300: 666f 7220 7061 7274 6974 696f 6e20 696e  for partition in
-00014310: 2073 6570 6172 6174 6f72 5f6c 6973 743a   separator_list:
-00014320: 0d0a 2020 2020 2020 2020 6a6f 696e 5f6c  ..        join_l
-00014330: 6567 735f 7374 7269 6e67 5f69 6e70 7574  egs_string_input
-00014340: 203d 206a 6f69 6e5f 6c65 6773 5f73 7472   = join_legs_str
-00014350: 696e 675f 696e 7075 742e 7265 706c 6163  ing_input.replac
-00014360: 6528 7061 7274 6974 696f 6e2c 2229 2822  e(partition,")("
-00014370: 290d 0a20 2020 206a 6f69 6e5f 6c65 6773  )..    join_legs
-00014380: 5f73 7472 696e 675f 696e 7075 7420 3d20  _string_input = 
-00014390: 2228 222b 6a6f 696e 5f6c 6567 735f 7374  "("+join_legs_st
-000143a0: 7269 6e67 5f69 6e70 7574 2b22 2922 0d0a  ring_input+")"..
-000143b0: 0d0a 2020 2020 7368 6170 655f 6c65 6674  ..    shape_left
-000143c0: 2020 3d20 4f62 6a2e 7368 6170 655b 3a6e    = Obj.shape[:n
-000143d0: 5f6c 6566 745d 0d0a 2020 2020 7374 6174  _left]..    stat
-000143e0: 735f 6c65 6674 2020 3d20 4f62 6a2e 7374  s_left  = Obj.st
-000143f0: 6174 6973 7469 635b 3a6e 5f6c 6566 745d  atistic[:n_left]
-00014400: 0d0a 2020 2020 7368 6170 655f 7269 6768  ..    shape_righ
-00014410: 7420 3d20 4f62 6a2e 7368 6170 655b 6e5f  t = Obj.shape[n_
-00014420: 6c65 6674 3a5d 0d0a 2020 2020 7374 6174  left:]..    stat
-00014430: 735f 7269 6768 7420 3d20 4f62 6a2e 7374  s_right = Obj.st
-00014440: 6174 6973 7469 635b 6e5f 6c65 6674 3a5d  atistic[n_left:]
-00014450: 0d0a 0d0a 2020 2020 6465 6620 7a65 726f  ....    def zero
-00014460: 5f6f 725f 656c 7365 2876 6563 746f 722c  _or_else(vector,
-00014470: 7661 6c75 6529 3a0d 0a20 2020 2020 2020  value):..       
-00014480: 2066 6f72 2065 6c65 6d20 696e 2076 6563   for elem in vec
-00014490: 746f 723a 0d0a 2020 2020 2020 2020 2020  tor:..          
-000144a0: 2020 6966 2065 6c65 6d21 3d30 3a0d 0a20    if elem!=0:.. 
-000144b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000144c0: 6574 7572 6e20 7661 6c75 650d 0a20 2020  eturn value..   
-000144d0: 2020 2020 2072 6574 7572 6e20 300d 0a20       return 0.. 
-000144e0: 2020 2064 6566 2067 6574 5f73 7461 7428     def get_stat(
-000144f0: 7665 6374 6f72 2c70 7265 6665 723d 4e6f  vector,prefer=No
-00014500: 6e65 293a 0d0a 2020 2020 2020 2020 626f  ne):..        bo
-00014510: 736f 6e5f 636f 756e 7420 3d20 300d 0a20  son_count = 0.. 
-00014520: 2020 2020 2020 2066 6572 6d69 5f63 6f75         fermi_cou
-00014530: 6e74 203d 2030 0d0a 2020 2020 2020 2020  nt = 0..        
-00014540: 666f 7220 656c 656d 2069 6e20 7665 6374  for elem in vect
-00014550: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
-00014560: 2069 6620 656c 656d 2069 6e20 626f 7365   if elem in bose
+00014140: 3a3a 3a0d 0a0d 0a20 2020 2023 2063 6f75  :::....    # cou
+00014150: 6e74 2074 6865 206e 756d 6265 7220 6f66  nt the number of
+00014160: 2069 6e64 6963 6573 2069 6e20 7468 6520   indices in the 
+00014170: 7477 6f20 6772 6f75 7073 0d0a 2020 2020  two groups..    
+00014180: 6e5f 6c65 6674 203d 2030 0d0a 2020 2020  n_left = 0..    
+00014190: 6e5f 7269 6768 7420 3d20 300d 0a20 2020  n_right = 0..   
+000141a0: 2070 6172 7469 7469 6f6e 5f66 6f75 6e64   partition_found
+000141b0: 203d 2046 616c 7365 0d0a 2020 2020 666f   = False..    fo
+000141c0: 7220 6368 6172 2069 6e20 7374 7269 6e67  r char in string
+000141d0: 3a0d 0a20 2020 2020 2020 2069 6620 6368  :..        if ch
+000141e0: 6172 2069 6e20 7365 7061 7261 746f 725f  ar in separator_
+000141f0: 6c69 7374 203a 0d0a 2020 2020 2020 2020  list :..        
+00014200: 2020 2020 7061 7274 6974 696f 6e5f 666f      partition_fo
+00014210: 756e 6420 3d20 5472 7565 0d0a 2020 2020  und = True..    
+00014220: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00014230: 0d0a 2020 2020 2020 2020 6966 2870 6172  ..        if(par
+00014240: 7469 7469 6f6e 5f66 6f75 6e64 293a 0d0a  tition_found):..
+00014250: 2020 2020 2020 2020 2020 2020 6e5f 7269              n_ri
+00014260: 6768 742b 3d31 0d0a 2020 2020 2020 2020  ght+=1..        
+00014270: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00014280: 2020 206e 5f6c 6566 742b 3d31 0d0a 0d0a     n_left+=1....
+00014290: 2020 2020 6a6f 696e 5f6c 6567 735f 7374      join_legs_st
+000142a0: 7269 6e67 5f69 6e70 7574 203d 2073 7472  ring_input = str
+000142b0: 696e 670d 0a20 2020 2066 6f72 2070 6172  ing..    for par
+000142c0: 7469 7469 6f6e 2069 6e20 7365 7061 7261  tition in separa
+000142d0: 746f 725f 6c69 7374 3a0d 0a20 2020 2020  tor_list:..     
+000142e0: 2020 206a 6f69 6e5f 6c65 6773 5f73 7472     join_legs_str
+000142f0: 696e 675f 696e 7075 7420 3d20 6a6f 696e  ing_input = join
+00014300: 5f6c 6567 735f 7374 7269 6e67 5f69 6e70  _legs_string_inp
+00014310: 7574 2e72 6570 6c61 6365 2870 6172 7469  ut.replace(parti
+00014320: 7469 6f6e 2c22 2928 2229 0d0a 2020 2020  tion,")(")..    
+00014330: 6a6f 696e 5f6c 6567 735f 7374 7269 6e67  join_legs_string
+00014340: 5f69 6e70 7574 203d 2022 2822 2b6a 6f69  _input = "("+joi
+00014350: 6e5f 6c65 6773 5f73 7472 696e 675f 696e  n_legs_string_in
+00014360: 7075 742b 2229 220d 0a0d 0a20 2020 2073  put+")"....    s
+00014370: 6861 7065 5f6c 6566 7420 203d 204f 626a  hape_left  = Obj
+00014380: 2e73 6861 7065 5b3a 6e5f 6c65 6674 5d0d  .shape[:n_left].
+00014390: 0a20 2020 2073 7461 7473 5f6c 6566 7420  .    stats_left 
+000143a0: 203d 204f 626a 2e73 7461 7469 7374 6963   = Obj.statistic
+000143b0: 5b3a 6e5f 6c65 6674 5d0d 0a20 2020 2073  [:n_left]..    s
+000143c0: 6861 7065 5f72 6967 6874 203d 204f 626a  hape_right = Obj
+000143d0: 2e73 6861 7065 5b6e 5f6c 6566 743a 5d0d  .shape[n_left:].
+000143e0: 0a20 2020 2073 7461 7473 5f72 6967 6874  .    stats_right
+000143f0: 203d 204f 626a 2e73 7461 7469 7374 6963   = Obj.statistic
+00014400: 5b6e 5f6c 6566 743a 5d0d 0a0d 0a20 2020  [n_left:]....   
+00014410: 2064 6566 207a 6572 6f5f 6f72 5f65 6c73   def zero_or_els
+00014420: 6528 7665 6374 6f72 2c76 616c 7565 293a  e(vector,value):
+00014430: 0d0a 2020 2020 2020 2020 666f 7220 656c  ..        for el
+00014440: 656d 2069 6e20 7665 6374 6f72 3a0d 0a20  em in vector:.. 
+00014450: 2020 2020 2020 2020 2020 2069 6620 656c             if el
+00014460: 656d 213d 303a 0d0a 2020 2020 2020 2020  em!=0:..        
+00014470: 2020 2020 2020 2020 7265 7475 726e 2076          return v
+00014480: 616c 7565 0d0a 2020 2020 2020 2020 7265  alue..        re
+00014490: 7475 726e 2030 0d0a 2020 2020 6465 6620  turn 0..    def 
+000144a0: 6765 745f 7374 6174 2876 6563 746f 722c  get_stat(vector,
+000144b0: 7072 6566 6572 3d4e 6f6e 6529 3a0d 0a20  prefer=None):.. 
+000144c0: 2020 2020 2020 2062 6f73 6f6e 5f63 6f75         boson_cou
+000144d0: 6e74 203d 2030 0d0a 2020 2020 2020 2020  nt = 0..        
+000144e0: 6665 726d 695f 636f 756e 7420 3d20 300d  fermi_count = 0.
+000144f0: 0a20 2020 2020 2020 2066 6f72 2065 6c65  .        for ele
+00014500: 6d20 696e 2076 6563 746f 723a 0d0a 2020  m in vector:..  
+00014510: 2020 2020 2020 2020 2020 6966 2065 6c65            if ele
+00014520: 6d20 696e 2062 6f73 655f 7479 7065 203a  m in bose_type :
+00014530: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014540: 2020 626f 736f 6e5f 636f 756e 7420 2b3d    boson_count +=
+00014550: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
+00014560: 6966 2065 6c65 6d20 696e 2066 6572 6d69  if elem in fermi
 00014570: 5f74 7970 6520 3a0d 0a20 2020 2020 2020  _type :..       
-00014580: 2020 2020 2020 2020 2062 6f73 6f6e 5f63           boson_c
-00014590: 6f75 6e74 202b 3d20 310d 0a20 2020 2020  ount += 1..     
-000145a0: 2020 2020 2020 2069 6620 656c 656d 2069         if elem i
-000145b0: 6e20 6665 726d 695f 7479 7065 203a 0d0a  n fermi_type :..
-000145c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145d0: 6665 726d 695f 636f 756e 7420 2b3d 2031  fermi_count += 1
-000145e0: 0d0a 0d0a 2020 2020 2020 2020 6966 2862  ....        if(b
-000145f0: 6f73 6f6e 5f63 6f75 6e74 3d3d 3020 616e  oson_count==0 an
-00014600: 6420 6665 726d 695f 636f 756e 743e 3029  d fermi_count>0)
-00014610: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00014620: 6620 7072 6566 6572 2021 3d20 4e6f 6e65  f prefer != None
-00014630: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00014640: 2020 2072 6574 7572 6e20 7072 6566 6572     return prefer
-00014650: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00014660: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00014670: 2020 2020 2072 6574 7572 6e20 310d 0a20       return 1.. 
-00014680: 2020 2020 2020 2065 6c69 6628 626f 736f         elif(boso
-00014690: 6e5f 636f 756e 743e 3020 616e 6420 6665  n_count>0 and fe
-000146a0: 726d 695f 636f 756e 743d 3d30 293a 0d0a  rmi_count==0):..
-000146b0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-000146c0: 7265 6665 7220 213d 204e 6f6e 653a 0d0a  refer != None:..
-000146d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146e0: 7265 7475 726e 2070 7265 6665 720d 0a20  return prefer.. 
-000146f0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00014700: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00014710: 2020 7265 7475 726e 2030 0d0a 2020 2020    return 0..    
-00014720: 2020 2020 656c 6966 2862 6f73 6f6e 5f63      elif(boson_c
-00014730: 6f75 6e74 3e30 2061 6e64 2066 6572 6d69  ount>0 and fermi
-00014740: 5f63 6f75 6e74 3e30 293a 0d0a 2020 2020  _count>0):..    
-00014750: 2020 2020 2020 2020 7265 7475 726e 2068          return h
-00014760: 7962 7269 645f 7379 6d62 6f6c 0d0a 2020  ybrid_symbol..  
-00014770: 2020 0d0a 2020 2020 696e 7465 726d 6564    ..    intermed
-00014780: 6961 7465 5f73 7461 7420 3d20 2820 7a65  iate_stat = ( ze
-00014790: 726f 5f6f 725f 656c 7365 2873 7461 7473  ro_or_else(stats
-000147a0: 5f6c 6566 742c 2d31 292c 7a65 726f 5f6f  _left,-1),zero_o
-000147b0: 725f 656c 7365 2873 7461 7473 5f72 6967  r_else(stats_rig
-000147c0: 6874 2c31 2920 290d 0a0d 0a20 2020 2073  ht,1) )....    s
-000147d0: 7465 7020 3d20 7368 6f77 5f70 726f 6772  tep = show_progr
-000147e0: 6573 7328 7374 6570 2c70 726f 6365 7373  ess(step,process
-000147f0: 5f6c 656e 6774 682c 7072 6f63 6573 735f  _length,process_
-00014800: 6e61 6d65 2b22 2022 2b22 3c22 2b63 7572  name+" "+"<"+cur
-00014810: 7265 6e74 5f6d 656d 6f72 795f 6469 7370  rent_memory_disp
-00014820: 6c61 7928 292b 223e 222c 636f 6c6f 723d  lay()+">",color=
-00014830: 7072 6f63 6573 735f 636f 6c6f 722c 7469  process_color,ti
-00014840: 6d65 3d74 696d 652e 7469 6d65 2829 2d73  me=time.time()-s
-00014850: 3030 2920 2332 0d0a 2020 2020 4f62 6a20  00) #2..    Obj 
-00014860: 3d20 4f62 6a2e 6a6f 696e 5f6c 6567 7328  = Obj.join_legs(
-00014870: 6a6f 696e 5f6c 6567 735f 7374 7269 6e67  join_legs_string
-00014880: 5f69 6e70 7574 2c22 6d61 7472 6978 222c  _input,"matrix",
-00014890: 696e 7465 726d 6564 6961 7465 5f73 7461  intermediate_sta
-000148a0: 743d 696e 7465 726d 6564 6961 7465 5f73  t=intermediate_s
-000148b0: 7461 742c 7361 7665 5f6d 656d 6f72 793d  tat,save_memory=
-000148c0: 5472 7565 290d 0a0d 0a20 2020 2023 3a3a  True)....    #::
+00014580: 2020 2020 2020 2020 2066 6572 6d69 5f63           fermi_c
+00014590: 6f75 6e74 202b 3d20 310d 0a0d 0a20 2020  ount += 1....   
+000145a0: 2020 2020 2069 6628 626f 736f 6e5f 636f       if(boson_co
+000145b0: 756e 743d 3d30 2061 6e64 2066 6572 6d69  unt==0 and fermi
+000145c0: 5f63 6f75 6e74 3e30 293a 0d0a 2020 2020  _count>0):..    
+000145d0: 2020 2020 2020 2020 6966 2070 7265 6665          if prefe
+000145e0: 7220 213d 204e 6f6e 653a 0d0a 2020 2020  r != None:..    
+000145f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00014600: 726e 2070 7265 6665 720d 0a20 2020 2020  rn prefer..     
+00014610: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00014620: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00014630: 7475 726e 2031 0d0a 2020 2020 2020 2020  turn 1..        
+00014640: 656c 6966 2862 6f73 6f6e 5f63 6f75 6e74  elif(boson_count
+00014650: 3e30 2061 6e64 2066 6572 6d69 5f63 6f75  >0 and fermi_cou
+00014660: 6e74 3d3d 3029 3a0d 0a20 2020 2020 2020  nt==0):..       
+00014670: 2020 2020 2069 6620 7072 6566 6572 2021       if prefer !
+00014680: 3d20 4e6f 6e65 3a0d 0a20 2020 2020 2020  = None:..       
+00014690: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000146a0: 7072 6566 6572 0d0a 2020 2020 2020 2020  prefer..        
+000146b0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000146c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000146d0: 6e20 300d 0a20 2020 2020 2020 2065 6c69  n 0..        eli
+000146e0: 6628 626f 736f 6e5f 636f 756e 743e 3020  f(boson_count>0 
+000146f0: 616e 6420 6665 726d 695f 636f 756e 743e  and fermi_count>
+00014700: 3029 3a0d 0a20 2020 2020 2020 2020 2020  0):..           
+00014710: 2072 6574 7572 6e20 6879 6272 6964 5f73   return hybrid_s
+00014720: 796d 626f 6c0d 0a20 2020 200d 0a20 2020  ymbol..    ..   
+00014730: 2069 6e74 6572 6d65 6469 6174 655f 7374   intermediate_st
+00014740: 6174 203d 2028 207a 6572 6f5f 6f72 5f65  at = ( zero_or_e
+00014750: 6c73 6528 7374 6174 735f 6c65 6674 2c2d  lse(stats_left,-
+00014760: 3129 2c7a 6572 6f5f 6f72 5f65 6c73 6528  1),zero_or_else(
+00014770: 7374 6174 735f 7269 6768 742c 3129 2029  stats_right,1) )
+00014780: 0d0a 0d0a 2020 2020 7374 6570 203d 2073  ....    step = s
+00014790: 686f 775f 7072 6f67 7265 7373 2873 7465  how_progress(ste
+000147a0: 702c 7072 6f63 6573 735f 6c65 6e67 7468  p,process_length
+000147b0: 2c70 726f 6365 7373 5f6e 616d 652b 2220  ,process_name+" 
+000147c0: 222b 223c 222b 6375 7272 656e 745f 6d65  "+"<"+current_me
+000147d0: 6d6f 7279 5f64 6973 706c 6179 2829 2b22  mory_display()+"
+000147e0: 3e22 2c63 6f6c 6f72 3d70 726f 6365 7373  >",color=process
+000147f0: 5f63 6f6c 6f72 2c74 696d 653d 7469 6d65  _color,time=time
+00014800: 2e74 696d 6528 292d 7330 3029 2023 320d  .time()-s00) #2.
+00014810: 0a20 2020 204f 626a 203d 204f 626a 2e6a  .    Obj = Obj.j
+00014820: 6f69 6e5f 6c65 6773 286a 6f69 6e5f 6c65  oin_legs(join_le
+00014830: 6773 5f73 7472 696e 675f 696e 7075 742c  gs_string_input,
+00014840: 226d 6174 7269 7822 2c69 6e74 6572 6d65  "matrix",interme
+00014850: 6469 6174 655f 7374 6174 3d69 6e74 6572  diate_stat=inter
+00014860: 6d65 6469 6174 655f 7374 6174 2c73 6176  mediate_stat,sav
+00014870: 655f 6d65 6d6f 7279 3d54 7275 6529 0d0a  e_memory=True)..
+00014880: 0d0a 2020 2020 233a 3a3a 3a3a 3a3a 3a3a  ..    #:::::::::
+00014890: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000148a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000148b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000148c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 000148d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000148e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000148f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014900: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014910: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014920: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a  ::::::::::::::..
-00014930: 2020 2020 233a 3a3a 3a3a 2020 2020 2020      #:::::      
-00014940: 5354 4550 2032 202d 2042 4c4f 434b 2053  STEP 2 - BLOCK S
-00014950: 5644 2028 4d41 4b45 2053 5552 4520 4954  VD (MAKE SURE IT
-00014960: 2753 2050 4152 4954 592d 5052 4553 4552  'S PARITY-PRESER
-00014970: 5649 4e47 2129 2020 2020 2020 2020 2020  VING!)          
-00014980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014990: 3a3a 3a3a 3a0d 0a20 2020 2023 3a3a 3a3a  :::::..    #::::
+000148e0: 3a3a 3a3a 3a3a 3a0d 0a20 2020 2023 3a3a  :::::::..    #::
+000148f0: 3a3a 3a20 2020 2020 2053 5445 5020 3220  :::      STEP 2 
+00014900: 2d20 424c 4f43 4b20 5356 4420 284d 414b  - BLOCK SVD (MAK
+00014910: 4520 5355 5245 2049 5427 5320 5041 5249  E SURE IT'S PARI
+00014920: 5459 2d50 5245 5345 5256 494e 4721 2920  TY-PRESERVING!) 
+00014930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014940: 2020 2020 2020 2020 203a 3a3a 3a3a 0d0a           :::::..
+00014950: 2020 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a      #:::::::::::
+00014960: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014970: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014980: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014990: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 000149a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000149b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000149c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000149d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000149e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000149f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a 0d0a  ::::::::::::....
-00014a00: 2020 2020 7374 6570 203d 2073 686f 775f      step = show_
-00014a10: 7072 6f67 7265 7373 2873 7465 702c 7072  progress(step,pr
-00014a20: 6f63 6573 735f 6c65 6e67 7468 2c70 726f  ocess_length,pro
-00014a30: 6365 7373 5f6e 616d 652b 2220 222b 223c  cess_name+" "+"<
-00014a40: 222b 6375 7272 656e 745f 6d65 6d6f 7279  "+current_memory
-00014a50: 5f64 6973 706c 6179 2829 2b22 3e22 2c63  _display()+">",c
-00014a60: 6f6c 6f72 3d70 726f 6365 7373 5f63 6f6c  olor=process_col
-00014a70: 6f72 2c74 696d 653d 7469 6d65 2e74 696d  or,time=time.tim
-00014a80: 6528 292d 7330 3029 2023 330d 0a20 2020  e()-s00) #3..   
-00014a90: 2069 6620 4f62 6a2e 7374 6174 6973 7469   if Obj.statisti
-00014aa0: 635b 305d 3d3d 3020 6f72 204f 626a 2e73  c[0]==0 or Obj.s
-00014ab0: 7461 7469 7374 6963 5b31 5d3d 3d30 3a0d  tatistic[1]==0:.
-00014ac0: 0a20 2020 2020 2020 2055 2c20 ce9b 2c20  .        U, .., 
-00014ad0: 5620 3d20 536f 7274 6564 5356 4428 4f62  V = SortedSVD(Ob
-00014ae0: 6a2e 6461 7461 2c63 7574 6f66 6629 0d0a  j.data,cutoff)..
-00014af0: 2020 2020 2020 2020 ce9b 203d 206e 702e          .. = np.
-00014b00: 6469 6167 28ce 9b29 0d0a 2020 2020 656c  diag(..)..    el
-00014b10: 7365 3a0d 0a20 2020 2020 2020 2055 2c20  se:..        U, 
-00014b20: ce9b 2c20 5620 3d20 426c 6f63 6b53 5644  .., V = BlockSVD
-00014b30: 284f 626a 2e64 6174 612c 6375 746f 6666  (Obj.data,cutoff
-00014b40: 290d 0a0d 0a20 2020 2073 7465 7020 3d20  )....    step = 
-00014b50: 7368 6f77 5f70 726f 6772 6573 7328 7374  show_progress(st
-00014b60: 6570 2c70 726f 6365 7373 5f6c 656e 6774  ep,process_lengt
-00014b70: 682c 7072 6f63 6573 735f 6e61 6d65 2b22  h,process_name+"
-00014b80: 2022 2b22 3c22 2b63 7572 7265 6e74 5f6d   "+"<"+current_m
-00014b90: 656d 6f72 795f 6469 7370 6c61 7928 292b  emory_display()+
-00014ba0: 223e 222c 636f 6c6f 723d 7072 6f63 6573  ">",color=proces
-00014bb0: 735f 636f 6c6f 722c 7469 6d65 3d74 696d  s_color,time=tim
-00014bc0: 652e 7469 6d65 2829 2d73 3030 2920 2334  e.time()-s00) #4
-00014bd0: 0d0a 2020 2020 233a 3a3a 3a3a 3a3a 3a3a  ..    #:::::::::
+000149b0: 3a3a 3a3a 3a0d 0a0d 0a20 2020 2073 7465  :::::....    ste
+000149c0: 7020 3d20 7368 6f77 5f70 726f 6772 6573  p = show_progres
+000149d0: 7328 7374 6570 2c70 726f 6365 7373 5f6c  s(step,process_l
+000149e0: 656e 6774 682c 7072 6f63 6573 735f 6e61  ength,process_na
+000149f0: 6d65 2b22 2022 2b22 3c22 2b63 7572 7265  me+" "+"<"+curre
+00014a00: 6e74 5f6d 656d 6f72 795f 6469 7370 6c61  nt_memory_displa
+00014a10: 7928 292b 223e 222c 636f 6c6f 723d 7072  y()+">",color=pr
+00014a20: 6f63 6573 735f 636f 6c6f 722c 7469 6d65  ocess_color,time
+00014a30: 3d74 696d 652e 7469 6d65 2829 2d73 3030  =time.time()-s00
+00014a40: 2920 2333 0d0a 2020 2020 6966 204f 626a  ) #3..    if Obj
+00014a50: 2e73 7461 7469 7374 6963 5b30 5d3d 3d30  .statistic[0]==0
+00014a60: 206f 7220 4f62 6a2e 7374 6174 6973 7469   or Obj.statisti
+00014a70: 635b 315d 3d3d 303a 0d0a 2020 2020 2020  c[1]==0:..      
+00014a80: 2020 552c 20ce 9b2c 2056 203d 2053 6f72    U, .., V = Sor
+00014a90: 7465 6453 5644 284f 626a 2e64 6174 612c  tedSVD(Obj.data,
+00014aa0: 6375 746f 6666 290d 0a20 2020 2020 2020  cutoff)..       
+00014ab0: 20ce 9b20 3d20 6e70 2e64 6961 6728 ce9b   .. = np.diag(..
+00014ac0: 290d 0a20 2020 2065 6c73 653a 0d0a 2020  )..    else:..  
+00014ad0: 2020 2020 2020 552c 20ce 9b2c 2056 203d        U, .., V =
+00014ae0: 2042 6c6f 636b 5356 4428 4f62 6a2e 6461   BlockSVD(Obj.da
+00014af0: 7461 2c63 7574 6f66 6629 0d0a 0d0a 2020  ta,cutoff)....  
+00014b00: 2020 7374 6570 203d 2073 686f 775f 7072    step = show_pr
+00014b10: 6f67 7265 7373 2873 7465 702c 7072 6f63  ogress(step,proc
+00014b20: 6573 735f 6c65 6e67 7468 2c70 726f 6365  ess_length,proce
+00014b30: 7373 5f6e 616d 652b 2220 222b 223c 222b  ss_name+" "+"<"+
+00014b40: 6375 7272 656e 745f 6d65 6d6f 7279 5f64  current_memory_d
+00014b50: 6973 706c 6179 2829 2b22 3e22 2c63 6f6c  isplay()+">",col
+00014b60: 6f72 3d70 726f 6365 7373 5f63 6f6c 6f72  or=process_color
+00014b70: 2c74 696d 653d 7469 6d65 2e74 696d 6528  ,time=time.time(
+00014b80: 292d 7330 3029 2023 340d 0a20 2020 2023  )-s00) #4..    #
+00014b90: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014ba0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014bb0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014bc0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014bd0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00014be0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014bf0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014c00: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014c10: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014c20: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014c30: 3a3a 3a3a 3a3a 3a0d 0a20 2020 2023 3a3a  :::::::..    #::
-00014c40: 3a3a 3a20 2020 2020 2053 5445 5020 3320  :::      STEP 3 
-00014c50: 2d20 5245 434f 4e53 5452 5543 5420 552c  - RECONSTRUCT U,
-00014c60: 20ce 9b2c 2061 6e64 2056 2041 5320 4752   .., and V AS GR
-00014c70: 4153 534d 414e 4e20 5445 4e53 4f52 5320  ASSMANN TENSORS 
-00014c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c90: 2020 2020 2020 2020 2020 3a3a 3a3a 3a0d            :::::.
-00014ca0: 0a20 2020 2023 3a3a 3a3a 3a3a 3a3a 3a3a  .    #::::::::::
-00014cb0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014cc0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014cd0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014ce0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014cf0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00014d00: 3a3a 3a3a 3a3a 0d0a 0d0a 2020 2020 736b  ::::::....    sk
-00014d10: 6970 5f70 6f77 6572 5f6f 665f 7477 6f5f  ip_power_of_two_
-00014d20: 6368 6563 6b20 3d20 5472 7565 0d0a 0d0a  check = True....
-00014d30: 2020 2020 2374 6865 2066 6972 7374 2077      #the first w
-00014d40: 6179 2069 7320 746f 2066 6f72 6d20 7468  ay is to form th
-00014d50: 6520 7465 6e73 6f72 2066 6972 7374 2c20  e tensor first, 
-00014d60: 7468 656e 2073 706c 6974 0d0a 2020 2020  then split..    
-00014d70: ce9b 7374 6174 6c65 6674 203d 202d 310d  ..statleft = -1.
-00014d80: 0a20 2020 20ce 9b73 7461 7472 6967 6874  .    ..statright
-00014d90: 203d 202b 310d 0a20 2020 200d 0a20 2020   = +1..    ..   
-00014da0: 2069 6620 4f62 6a2e 7374 6174 6973 7469   if Obj.statisti
-00014db0: 635b 305d 3d3d 303a 0d0a 2020 2020 2020  c[0]==0:..      
-00014dc0: 2020 5520 3d20 6465 6e73 6528 552c 656e    U = dense(U,en
-00014dd0: 636f 6465 723d 2270 6172 6974 792d 7072  coder="parity-pr
-00014de0: 6573 6572 7669 6e67 222c 666f 726d 6174  eserving",format
-00014df0: 3d22 6d61 7472 6978 222c 7374 6174 6973  ="matrix",statis
-00014e00: 7469 633d 2830 2c30 2929 0d0a 2020 2020  tic=(0,0))..    
-00014e10: 2020 2020 ce9b 203d 2064 656e 7365 28ce      .. = dense(.
-00014e20: 9b2c 656e 636f 6465 723d 2270 6172 6974  .,encoder="parit
-00014e30: 792d 7072 6573 6572 7669 6e67 222c 666f  y-preserving",fo
-00014e40: 726d 6174 3d22 6d61 7472 6978 222c 7374  rmat="matrix",st
-00014e50: 6174 6973 7469 633d 2830 2c30 2929 0d0a  atistic=(0,0))..
-00014e60: 2020 2020 2020 2020 5620 3d20 6465 6e73          V = dens
-00014e70: 6528 562c 656e 636f 6465 723d 2270 6172  e(V,encoder="par
-00014e80: 6974 792d 7072 6573 6572 7669 6e67 222c  ity-preserving",
-00014e90: 666f 726d 6174 3d22 6d61 7472 6978 222c  format="matrix",
-00014ea0: 7374 6174 6973 7469 633d 2830 2c4f 626a  statistic=(0,Obj
-00014eb0: 2e73 7461 7469 7374 6963 5b31 5d29 290d  .statistic[1])).
-00014ec0: 0a20 2020 2020 2020 20ce 9b73 7461 746c  .        ..statl
-00014ed0: 6566 7420 3d20 300d 0a20 2020 2020 2020  eft = 0..       
-00014ee0: 20ce 9b73 7461 7472 6967 6874 203d 2030   ..statright = 0
-00014ef0: 0d0a 2020 2020 656c 6966 204f 626a 2e73  ..    elif Obj.s
-00014f00: 7461 7469 7374 6963 5b31 5d3d 3d30 3a0d  tatistic[1]==0:.
-00014f10: 0a20 2020 2020 2020 2055 203d 2064 656e  .        U = den
-00014f20: 7365 2855 2c65 6e63 6f64 6572 3d22 7061  se(U,encoder="pa
-00014f30: 7269 7479 2d70 7265 7365 7276 696e 6722  rity-preserving"
-00014f40: 2c66 6f72 6d61 743d 226d 6174 7269 7822  ,format="matrix"
-00014f50: 2c73 7461 7469 7374 6963 3d28 4f62 6a2e  ,statistic=(Obj.
-00014f60: 7374 6174 6973 7469 635b 305d 2c30 2929  statistic[0],0))
-00014f70: 0d0a 2020 2020 2020 2020 ce9b 203d 2064  ..        .. = d
-00014f80: 656e 7365 28ce 9b2c 656e 636f 6465 723d  ense(..,encoder=
-00014f90: 2270 6172 6974 792d 7072 6573 6572 7669  "parity-preservi
-00014fa0: 6e67 222c 666f 726d 6174 3d22 6d61 7472  ng",format="matr
-00014fb0: 6978 222c 7374 6174 6973 7469 633d 2830  ix",statistic=(0
-00014fc0: 2c30 2929 0d0a 2020 2020 2020 2020 5620  ,0))..        V 
-00014fd0: 3d20 6465 6e73 6528 562c 656e 636f 6465  = dense(V,encode
-00014fe0: 723d 2270 6172 6974 792d 7072 6573 6572  r="parity-preser
-00014ff0: 7669 6e67 222c 666f 726d 6174 3d22 6d61  ving",format="ma
-00015000: 7472 6978 222c 7374 6174 6973 7469 633d  trix",statistic=
-00015010: 2830 2c30 2929 0d0a 2020 2020 2020 2020  (0,0))..        
-00015020: ce9b 7374 6174 6c65 6674 203d 2030 0d0a  ..statleft = 0..
-00015030: 2020 2020 2020 2020 ce9b 7374 6174 7269          ..statri
-00015040: 6768 7420 3d20 300d 0a20 2020 2065 6c73  ght = 0..    els
-00015050: 653a 0d0a 2020 2020 2020 2020 5520 3d20  e:..        U = 
-00015060: 6465 6e73 6528 552c 656e 636f 6465 723d  dense(U,encoder=
-00015070: 2270 6172 6974 792d 7072 6573 6572 7669  "parity-preservi
-00015080: 6e67 222c 666f 726d 6174 3d22 6d61 7472  ng",format="matr
-00015090: 6978 222c 7374 6174 6973 7469 633d 284f  ix",statistic=(O
-000150a0: 626a 2e73 7461 7469 7374 6963 5b30 5d2c  bj.statistic[0],
-000150b0: 3129 290d 0a20 2020 2020 2020 20ce 9b20  1))..        .. 
-000150c0: 3d20 6465 6e73 6528 ce9b 2c65 6e63 6f64  = dense(..,encod
-000150d0: 6572 3d22 7061 7269 7479 2d70 7265 7365  er="parity-prese
-000150e0: 7276 696e 6722 2c66 6f72 6d61 743d 226d  rving",format="m
-000150f0: 6174 7269 7822 2c73 7461 7469 7374 6963  atrix",statistic
-00015100: 3d28 2d31 2c31 2929 0d0a 2020 2020 2020  =(-1,1))..      
-00015110: 2020 5620 3d20 6465 6e73 6528 562c 656e    V = dense(V,en
-00015120: 636f 6465 723d 2270 6172 6974 792d 7072  coder="parity-pr
-00015130: 6573 6572 7669 6e67 222c 666f 726d 6174  eserving",format
-00015140: 3d22 6d61 7472 6978 222c 7374 6174 6973  ="matrix",statis
-00015150: 7469 633d 282d 312c 4f62 6a2e 7374 6174  tic=(-1,Obj.stat
-00015160: 6973 7469 635b 315d 2929 0d0a 2020 2020  istic[1]))..    
-00015170: 64ce 9b20 3d20 ce9b 2e73 6861 7065 5b30  d.. = ...shape[0
-00015180: 5d0d 0a0d 0a20 2020 2073 6b69 705f 706f  ]....    skip_po
-00015190: 7765 725f 6f66 5f74 776f 5f63 6865 636b  wer_of_two_check
-000151a0: 203d 2046 616c 7365 0d0a 2020 2020 7374   = False..    st
-000151b0: 6570 203d 2073 686f 775f 7072 6f67 7265  ep = show_progre
-000151c0: 7373 2873 7465 702c 7072 6f63 6573 735f  ss(step,process_
-000151d0: 6c65 6e67 7468 2c70 726f 6365 7373 5f6e  length,process_n
-000151e0: 616d 652b 2220 222b 223c 222b 6375 7272  ame+" "+"<"+curr
-000151f0: 656e 745f 6d65 6d6f 7279 5f64 6973 706c  ent_memory_displ
-00015200: 6179 2829 2b22 3e22 2c63 6f6c 6f72 3d70  ay()+">",color=p
-00015210: 726f 6365 7373 5f63 6f6c 6f72 2c74 696d  rocess_color,tim
-00015220: 653d 7469 6d65 2e74 696d 6528 292d 7330  e=time.time()-s0
-00015230: 3029 2023 350d 0a20 2020 2023 3a3a 3a3a  0) #5..    #::::
+00014bf0: 0d0a 2020 2020 233a 3a3a 3a3a 2020 2020  ..    #:::::    
+00014c00: 2020 5354 4550 2033 202d 2052 4543 4f4e    STEP 3 - RECON
+00014c10: 5354 5255 4354 2055 2c20 ce9b 2c20 616e  STRUCT U, .., an
+00014c20: 6420 5620 4153 2047 5241 5353 4d41 4e4e  d V AS GRASSMANN
+00014c30: 2054 454e 534f 5253 2020 2020 2020 2020   TENSORS        
+00014c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c50: 2020 203a 3a3a 3a3a 0d0a 2020 2020 233a     :::::..    #:
+00014c60: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014c70: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014c80: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014c90: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014ca0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00014cb0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a0d  :::::::::::::::.
+00014cc0: 0a0d 0a20 2020 2073 6b69 705f 706f 7765  ...    skip_powe
+00014cd0: 725f 6f66 5f74 776f 5f63 6865 636b 203d  r_of_two_check =
+00014ce0: 2054 7275 650d 0a0d 0a20 2020 2023 7468   True....    #th
+00014cf0: 6520 6669 7273 7420 7761 7920 6973 2074  e first way is t
+00014d00: 6f20 666f 726d 2074 6865 2074 656e 736f  o form the tenso
+00014d10: 7220 6669 7273 742c 2074 6865 6e20 7370  r first, then sp
+00014d20: 6c69 740d 0a20 2020 20ce 9b73 7461 746c  lit..    ..statl
+00014d30: 6566 7420 3d20 2d31 0d0a 2020 2020 ce9b  eft = -1..    ..
+00014d40: 7374 6174 7269 6768 7420 3d20 2b31 0d0a  statright = +1..
+00014d50: 2020 2020 0d0a 2020 2020 6966 204f 626a      ..    if Obj
+00014d60: 2e73 7461 7469 7374 6963 5b30 5d3d 3d30  .statistic[0]==0
+00014d70: 3a0d 0a20 2020 2020 2020 2055 203d 2064  :..        U = d
+00014d80: 656e 7365 2855 2c65 6e63 6f64 6572 3d22  ense(U,encoder="
+00014d90: 7061 7269 7479 2d70 7265 7365 7276 696e  parity-preservin
+00014da0: 6722 2c66 6f72 6d61 743d 226d 6174 7269  g",format="matri
+00014db0: 7822 2c73 7461 7469 7374 6963 3d28 302c  x",statistic=(0,
+00014dc0: 3029 290d 0a20 2020 2020 2020 20ce 9b20  0))..        .. 
+00014dd0: 3d20 6465 6e73 6528 ce9b 2c65 6e63 6f64  = dense(..,encod
+00014de0: 6572 3d22 7061 7269 7479 2d70 7265 7365  er="parity-prese
+00014df0: 7276 696e 6722 2c66 6f72 6d61 743d 226d  rving",format="m
+00014e00: 6174 7269 7822 2c73 7461 7469 7374 6963  atrix",statistic
+00014e10: 3d28 302c 3029 290d 0a20 2020 2020 2020  =(0,0))..       
+00014e20: 2056 203d 2064 656e 7365 2856 2c65 6e63   V = dense(V,enc
+00014e30: 6f64 6572 3d22 7061 7269 7479 2d70 7265  oder="parity-pre
+00014e40: 7365 7276 696e 6722 2c66 6f72 6d61 743d  serving",format=
+00014e50: 226d 6174 7269 7822 2c73 7461 7469 7374  "matrix",statist
+00014e60: 6963 3d28 302c 4f62 6a2e 7374 6174 6973  ic=(0,Obj.statis
+00014e70: 7469 635b 315d 2929 0d0a 2020 2020 2020  tic[1]))..      
+00014e80: 2020 ce9b 7374 6174 6c65 6674 203d 2030    ..statleft = 0
+00014e90: 0d0a 2020 2020 2020 2020 ce9b 7374 6174  ..        ..stat
+00014ea0: 7269 6768 7420 3d20 300d 0a20 2020 2065  right = 0..    e
+00014eb0: 6c69 6620 4f62 6a2e 7374 6174 6973 7469  lif Obj.statisti
+00014ec0: 635b 315d 3d3d 303a 0d0a 2020 2020 2020  c[1]==0:..      
+00014ed0: 2020 5520 3d20 6465 6e73 6528 552c 656e    U = dense(U,en
+00014ee0: 636f 6465 723d 2270 6172 6974 792d 7072  coder="parity-pr
+00014ef0: 6573 6572 7669 6e67 222c 666f 726d 6174  eserving",format
+00014f00: 3d22 6d61 7472 6978 222c 7374 6174 6973  ="matrix",statis
+00014f10: 7469 633d 284f 626a 2e73 7461 7469 7374  tic=(Obj.statist
+00014f20: 6963 5b30 5d2c 3029 290d 0a20 2020 2020  ic[0],0))..     
+00014f30: 2020 20ce 9b20 3d20 6465 6e73 6528 ce9b     .. = dense(..
+00014f40: 2c65 6e63 6f64 6572 3d22 7061 7269 7479  ,encoder="parity
+00014f50: 2d70 7265 7365 7276 696e 6722 2c66 6f72  -preserving",for
+00014f60: 6d61 743d 226d 6174 7269 7822 2c73 7461  mat="matrix",sta
+00014f70: 7469 7374 6963 3d28 302c 3029 290d 0a20  tistic=(0,0)).. 
+00014f80: 2020 2020 2020 2056 203d 2064 656e 7365         V = dense
+00014f90: 2856 2c65 6e63 6f64 6572 3d22 7061 7269  (V,encoder="pari
+00014fa0: 7479 2d70 7265 7365 7276 696e 6722 2c66  ty-preserving",f
+00014fb0: 6f72 6d61 743d 226d 6174 7269 7822 2c73  ormat="matrix",s
+00014fc0: 7461 7469 7374 6963 3d28 302c 3029 290d  tatistic=(0,0)).
+00014fd0: 0a20 2020 2020 2020 20ce 9b73 7461 746c  .        ..statl
+00014fe0: 6566 7420 3d20 300d 0a20 2020 2020 2020  eft = 0..       
+00014ff0: 20ce 9b73 7461 7472 6967 6874 203d 2030   ..statright = 0
+00015000: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
+00015010: 2020 2020 2055 203d 2064 656e 7365 2855       U = dense(U
+00015020: 2c65 6e63 6f64 6572 3d22 7061 7269 7479  ,encoder="parity
+00015030: 2d70 7265 7365 7276 696e 6722 2c66 6f72  -preserving",for
+00015040: 6d61 743d 226d 6174 7269 7822 2c73 7461  mat="matrix",sta
+00015050: 7469 7374 6963 3d28 4f62 6a2e 7374 6174  tistic=(Obj.stat
+00015060: 6973 7469 635b 305d 2c31 2929 0d0a 2020  istic[0],1))..  
+00015070: 2020 2020 2020 ce9b 203d 2064 656e 7365        .. = dense
+00015080: 28ce 9b2c 656e 636f 6465 723d 2270 6172  (..,encoder="par
+00015090: 6974 792d 7072 6573 6572 7669 6e67 222c  ity-preserving",
+000150a0: 666f 726d 6174 3d22 6d61 7472 6978 222c  format="matrix",
+000150b0: 7374 6174 6973 7469 633d 282d 312c 3129  statistic=(-1,1)
+000150c0: 290d 0a20 2020 2020 2020 2056 203d 2064  )..        V = d
+000150d0: 656e 7365 2856 2c65 6e63 6f64 6572 3d22  ense(V,encoder="
+000150e0: 7061 7269 7479 2d70 7265 7365 7276 696e  parity-preservin
+000150f0: 6722 2c66 6f72 6d61 743d 226d 6174 7269  g",format="matri
+00015100: 7822 2c73 7461 7469 7374 6963 3d28 2d31  x",statistic=(-1
+00015110: 2c4f 626a 2e73 7461 7469 7374 6963 5b31  ,Obj.statistic[1
+00015120: 5d29 290d 0a20 2020 2064 ce9b 203d 20ce  ]))..    d.. = .
+00015130: 9b2e 7368 6170 655b 305d 0d0a 0d0a 2020  ..shape[0]....  
+00015140: 2020 736b 6970 5f70 6f77 6572 5f6f 665f    skip_power_of_
+00015150: 7477 6f5f 6368 6563 6b20 3d20 4661 6c73  two_check = Fals
+00015160: 650d 0a20 2020 2073 7465 7020 3d20 7368  e..    step = sh
+00015170: 6f77 5f70 726f 6772 6573 7328 7374 6570  ow_progress(step
+00015180: 2c70 726f 6365 7373 5f6c 656e 6774 682c  ,process_length,
+00015190: 7072 6f63 6573 735f 6e61 6d65 2b22 2022  process_name+" "
+000151a0: 2b22 3c22 2b63 7572 7265 6e74 5f6d 656d  +"<"+current_mem
+000151b0: 6f72 795f 6469 7370 6c61 7928 292b 223e  ory_display()+">
+000151c0: 222c 636f 6c6f 723d 7072 6f63 6573 735f  ",color=process_
+000151d0: 636f 6c6f 722c 7469 6d65 3d74 696d 652e  color,time=time.
+000151e0: 7469 6d65 2829 2d73 3030 2920 2335 0d0a  time()-s00) #5..
+000151f0: 2020 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a      #:::::::::::
+00015200: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00015210: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00015220: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00015230: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00015240: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00015250: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00015260: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00015270: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00015280: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00015290: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a 2020  ::::::::::::..  
-000152a0: 2020 233a 3a3a 3a3a 2020 2020 2020 5354    #:::::      ST
-000152b0: 4550 2034 202d 2053 706c 6974 2074 6865  EP 4 - Split the
-000152c0: 206c 6567 7320 2020 2020 2020 2020 2020   legs           
-000152d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000152e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000152f0: 2020 2020 2020 2020 2020 2020 2020 3a3a                ::
-00015300: 3a3a 3a0d 0a20 2020 2023 3a3a 3a3a 3a3a  :::..    #::::::
+00015250: 3a3a 3a3a 3a0d 0a20 2020 2023 3a3a 3a3a  :::::..    #::::
+00015260: 3a20 2020 2020 2053 5445 5020 3420 2d20  :      STEP 4 - 
+00015270: 5370 6c69 7420 7468 6520 6c65 6773 2020  Split the legs  
+00015280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152b0: 2020 2020 2020 203a 3a3a 3a3a 0d0a 2020         :::::..  
+000152c0: 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a    #:::::::::::::
+000152d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000152e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000152f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00015300: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
 00015310: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00015320: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00015330: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00015340: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00015350: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00015360: 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a 0d0a 2020  ::::::::::....  
-00015370: 2020 2320 636f 756e 7420 7468 6520 6e75    # count the nu
-00015380: 6d62 6572 206f 6620 696e 6469 6365 7320  mber of indices 
-00015390: 696e 2074 6865 2074 776f 2067 726f 7570  in the two group
-000153a0: 730d 0a20 2020 2055 696e 6420 3d20 2222  s..    Uind = ""
-000153b0: 0d0a 2020 2020 5669 6e64 203d 2022 220d  ..    Vind = "".
-000153c0: 0a20 2020 2055 7374 6174 7320 3d20 5b5d  .    Ustats = []
-000153d0: 0d0a 2020 2020 5673 7461 7473 203d 205b  ..    Vstats = [
-000153e0: 5d0d 0a20 2020 2055 7368 6170 6520 3d20  ]..    Ushape = 
-000153f0: 5b5d 0d0a 2020 2020 5673 6861 7065 203d  []..    Vshape =
-00015400: 205b 5d0d 0a20 2020 2070 6172 7469 7469   []..    partiti
-00015410: 6f6e 5f66 6f75 6e64 203d 2046 616c 7365  on_found = False
-00015420: 0d0a 2020 2020 666f 7220 692c 6368 6172  ..    for i,char
-00015430: 2069 6e20 656e 756d 6572 6174 6528 7374   in enumerate(st
-00015440: 7269 6e67 293a 0d0a 2020 2020 2020 2020  ring):..        
-00015450: 6966 2063 6861 7220 696e 2073 6570 6172  if char in separ
-00015460: 6174 6f72 5f6c 6973 7420 3a0d 0a20 2020  ator_list :..   
-00015470: 2020 2020 2020 2020 2070 6172 7469 7469           partiti
-00015480: 6f6e 5f66 6f75 6e64 203d 2054 7275 650d  on_found = True.
-00015490: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-000154a0: 7469 6e75 650d 0a20 2020 2020 2020 2069  tinue..        i
-000154b0: 6628 7061 7274 6974 696f 6e5f 666f 756e  f(partition_foun
-000154c0: 6429 3a0d 0a20 2020 2020 2020 2020 2020  d):..           
-000154d0: 2056 696e 642b 3d63 6861 720d 0a20 2020   Vind+=char..   
-000154e0: 2020 2020 2020 2020 2056 7374 6174 732b           Vstats+
-000154f0: 3d5b 584f 626a 5f73 7461 7473 5b69 2d31  =[XObj_stats[i-1
-00015500: 5d5d 0d0a 2020 2020 2020 2020 2020 2020  ]]..            
-00015510: 5673 6861 7065 2b3d 5b58 4f62 6a5f 7368  Vshape+=[XObj_sh
-00015520: 6170 655b 692d 315d 5d0d 0a20 2020 2020  ape[i-1]]..     
-00015530: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00015540: 2020 2020 2020 5569 6e64 2b3d 6368 6172        Uind+=char
-00015550: 0d0a 2020 2020 2020 2020 2020 2020 5573  ..            Us
-00015560: 7461 7473 2b3d 5b58 4f62 6a5f 7374 6174  tats+=[XObj_stat
-00015570: 735b 695d 5d0d 0a20 2020 2020 2020 2020  s[i]]..         
-00015580: 2020 2055 7368 6170 652b 3d5b 584f 626a     Ushape+=[XObj
-00015590: 5f73 6861 7065 5b69 5d5d 0d0a 0d0a 2020  _shape[i]]....  
-000155a0: 2020 6e65 775f 696e 6431 203d 2022 220d    new_ind1 = "".
-000155b0: 0a20 2020 2066 6f72 2063 6861 7220 696e  .    for char in
-000155c0: 2063 6861 725f 6c69 7374 3a0d 0a20 2020   char_list:..   
-000155d0: 2020 2020 2069 6620 6368 6172 206e 6f74       if char not
-000155e0: 2069 6e20 5569 6e64 2b56 696e 643a 0d0a   in Uind+Vind:..
-000155f0: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-00015600: 696e 6431 203d 2063 6861 720d 0a20 2020  ind1 = char..   
-00015610: 2020 2020 2020 2020 2062 7265 616b 0d0a           break..
-00015620: 0d0a 2020 2020 5569 6e64 2020 203d 2022  ..    Uind   = "
-00015630: 2822 2b55 696e 642b 2229 2220 2b20 6e65  ("+Uind+")" + ne
-00015640: 775f 696e 6431 0d0a 2020 2020 5669 6e64  w_ind1..    Vind
-00015650: 2020 203d 206e 6577 5f69 6e64 3120 2b20     = new_ind1 + 
-00015660: 2228 222b 5669 6e64 2b22 2922 0d0a 2020  "("+Vind+")"..  
-00015670: 2020 5573 7461 7473 203d 2074 7570 6c65    Ustats = tuple
-00015680: 2855 7374 6174 7320 2b20 5b2d ce9b 7374  (Ustats + [-..st
-00015690: 6174 6c65 6674 5d29 0d0a 2020 2020 5673  atleft])..    Vs
-000156a0: 7461 7473 203d 2074 7570 6c65 285b 2dce  tats = tuple([-.
-000156b0: 9b73 7461 7472 6967 6874 5d20 2b20 5673  .statright] + Vs
-000156c0: 7461 7473 290d 0a20 2020 2055 7368 6170  tats)..    Ushap
-000156d0: 6520 3d20 7475 706c 6528 5573 6861 7065  e = tuple(Ushape
-000156e0: 202b 205b 64ce 9b5d 290d 0a20 2020 2056   + [d..])..    V
-000156f0: 7368 6170 6520 3d20 7475 706c 6528 5b64  shape = tuple([d
-00015700: ce9b 5d20 2b20 5673 6861 7065 290d 0a20  ..] + Vshape).. 
-00015710: 2020 200d 0a20 2020 2073 7465 7020 3d20     ..    step = 
-00015720: 7368 6f77 5f70 726f 6772 6573 7328 7374  show_progress(st
-00015730: 6570 2c70 726f 6365 7373 5f6c 656e 6774  ep,process_lengt
-00015740: 682c 7072 6f63 6573 735f 6e61 6d65 2b22  h,process_name+"
-00015750: 2022 2b22 3c22 2b63 7572 7265 6e74 5f6d   "+"<"+current_m
-00015760: 656d 6f72 795f 6469 7370 6c61 7928 292b  emory_display()+
-00015770: 223e 222c 636f 6c6f 723d 7072 6f63 6573  ">",color=proces
-00015780: 735f 636f 6c6f 722c 7469 6d65 3d74 696d  s_color,time=tim
-00015790: 652e 7469 6d65 2829 2d73 3030 2920 2336  e.time()-s00) #6
-000157a0: 0d0a 2020 2020 5520 3d20 552e 7370 6c69  ..    U = U.spli
-000157b0: 745f 6c65 6773 2855 696e 642c 5573 7461  t_legs(Uind,Usta
-000157c0: 7473 2c55 7368 6170 652c 7361 7665 5f6d  ts,Ushape,save_m
-000157d0: 656d 6f72 793d 5472 7565 290d 0a20 2020  emory=True)..   
-000157e0: 20ce 9b20 3d20 ce9b 2e73 7769 7463 685f   .. = ...switch_
-000157f0: 656e 636f 6465 7228 7361 7665 5f6d 656d  encoder(save_mem
-00015800: 6f72 793d 5472 7565 290d 0a20 2020 2056  ory=True)..    V
-00015810: 203d 2056 2e73 706c 6974 5f6c 6567 7328   = V.split_legs(
-00015820: 5669 6e64 2c56 7374 6174 732c 5673 6861  Vind,Vstats,Vsha
-00015830: 7065 2c73 6176 655f 6d65 6d6f 7279 3d54  pe,save_memory=T
-00015840: 7275 6529 0d0a 2020 2020 0d0a 2020 2020  rue)..    ..    
-00015850: 6966 2874 6869 735f 666f 726d 6174 203d  if(this_format =
-00015860: 3d20 2773 7461 6e64 6172 6427 293a 0d0a  = 'standard'):..
-00015870: 2020 2020 2020 2020 5520 3d20 552e 7377          U = U.sw
-00015880: 6974 6368 5f66 6f72 6d61 7428 7361 7665  itch_format(save
-00015890: 5f6d 656d 6f72 793d 5472 7565 290d 0a20  _memory=True).. 
-000158a0: 2020 2020 2020 20ce 9b20 3d20 ce9b 2e73         .. = ...s
-000158b0: 7769 7463 685f 666f 726d 6174 2873 6176  witch_format(sav
-000158c0: 655f 6d65 6d6f 7279 3d54 7275 6529 0d0a  e_memory=True)..
-000158d0: 2020 2020 2020 2020 5620 3d20 562e 7377          V = V.sw
-000158e0: 6974 6368 5f66 6f72 6d61 7428 7361 7665  itch_format(save
-000158f0: 5f6d 656d 6f72 793d 5472 7565 290d 0a0d  _memory=True)...
-00015900: 0a20 2020 2069 6628 7468 6973 5f65 6e63  .    if(this_enc
-00015910: 6f64 6572 203d 3d20 2770 6172 6974 792d  oder == 'parity-
-00015920: 7072 6573 6572 7669 6e67 2729 3a0d 0a20  preserving'):.. 
-00015930: 2020 2020 2020 2055 203d 2055 2e73 7769         U = U.swi
-00015940: 7463 685f 656e 636f 6465 7228 7361 7665  tch_encoder(save
-00015950: 5f6d 656d 6f72 793d 5472 7565 290d 0a20  _memory=True).. 
-00015960: 2020 2020 2020 20ce 9b20 3d20 ce9b 2e73         .. = ...s
-00015970: 7769 7463 685f 656e 636f 6465 7228 7361  witch_encoder(sa
-00015980: 7665 5f6d 656d 6f72 793d 5472 7565 290d  ve_memory=True).
-00015990: 0a20 2020 2020 2020 2056 203d 2056 2e73  .        V = V.s
-000159a0: 7769 7463 685f 656e 636f 6465 7228 7361  witch_encoder(sa
-000159b0: 7665 5f6d 656d 6f72 793d 5472 7565 290d  ve_memory=True).
-000159c0: 0a0d 0a20 2020 2069 6628 7468 6973 5f74  ...    if(this_t
-000159d0: 7970 653d 3d73 7061 7273 6529 3a0d 0a20  ype==sparse):.. 
-000159e0: 2020 2020 2020 2055 203d 2073 7061 7273         U = spars
-000159f0: 6528 5529 0d0a 2020 2020 2020 2020 ce9b  e(U)..        ..
-00015a00: 203d 2073 7061 7273 6528 ce9b 290d 0a20   = sparse(..).. 
-00015a10: 2020 2020 2020 2056 203d 2073 7061 7273         V = spars
-00015a20: 6528 5629 0d0a 0d0a 2020 2020 636c 6561  e(V)....    clea
-00015a30: 725f 7072 6f67 7265 7373 2829 0d0a 2020  r_progress()..  
-00015a40: 2020 7379 732e 7374 646f 7574 2e77 7269    sys.stdout.wri
-00015a50: 7465 2822 5c30 3333 5b46 2229 0d0a 0d0a  te("\033[F")....
-00015a60: 2020 2020 7265 7475 726e 2055 2c20 ce9b      return U, ..
-00015a70: 2c20 560d 0a0d 0a23 2323 2323 2323 2323  , V....#########
-00015a80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015320: 3a3a 3a0d 0a0d 0a20 2020 2023 2063 6f75  :::....    # cou
+00015330: 6e74 2074 6865 206e 756d 6265 7220 6f66  nt the number of
+00015340: 2069 6e64 6963 6573 2069 6e20 7468 6520   indices in the 
+00015350: 7477 6f20 6772 6f75 7073 0d0a 2020 2020  two groups..    
+00015360: 5569 6e64 203d 2022 220d 0a20 2020 2056  Uind = ""..    V
+00015370: 696e 6420 3d20 2222 0d0a 2020 2020 5573  ind = ""..    Us
+00015380: 7461 7473 203d 205b 5d0d 0a20 2020 2056  tats = []..    V
+00015390: 7374 6174 7320 3d20 5b5d 0d0a 2020 2020  stats = []..    
+000153a0: 5573 6861 7065 203d 205b 5d0d 0a20 2020  Ushape = []..   
+000153b0: 2056 7368 6170 6520 3d20 5b5d 0d0a 2020   Vshape = []..  
+000153c0: 2020 7061 7274 6974 696f 6e5f 666f 756e    partition_foun
+000153d0: 6420 3d20 4661 6c73 650d 0a20 2020 2066  d = False..    f
+000153e0: 6f72 2069 2c63 6861 7220 696e 2065 6e75  or i,char in enu
+000153f0: 6d65 7261 7465 2873 7472 696e 6729 3a0d  merate(string):.
+00015400: 0a20 2020 2020 2020 2069 6620 6368 6172  .        if char
+00015410: 2069 6e20 7365 7061 7261 746f 725f 6c69   in separator_li
+00015420: 7374 203a 0d0a 2020 2020 2020 2020 2020  st :..          
+00015430: 2020 7061 7274 6974 696f 6e5f 666f 756e    partition_foun
+00015440: 6420 3d20 5472 7565 0d0a 2020 2020 2020  d = True..      
+00015450: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
+00015460: 2020 2020 2020 2020 6966 2870 6172 7469          if(parti
+00015470: 7469 6f6e 5f66 6f75 6e64 293a 0d0a 2020  tion_found):..  
+00015480: 2020 2020 2020 2020 2020 5669 6e64 2b3d            Vind+=
+00015490: 6368 6172 0d0a 2020 2020 2020 2020 2020  char..          
+000154a0: 2020 5673 7461 7473 2b3d 5b58 4f62 6a5f    Vstats+=[XObj_
+000154b0: 7374 6174 735b 692d 315d 5d0d 0a20 2020  stats[i-1]]..   
+000154c0: 2020 2020 2020 2020 2056 7368 6170 652b           Vshape+
+000154d0: 3d5b 584f 626a 5f73 6861 7065 5b69 2d31  =[XObj_shape[i-1
+000154e0: 5d5d 0d0a 2020 2020 2020 2020 656c 7365  ]]..        else
+000154f0: 3a0d 0a20 2020 2020 2020 2020 2020 2055  :..            U
+00015500: 696e 642b 3d63 6861 720d 0a20 2020 2020  ind+=char..     
+00015510: 2020 2020 2020 2055 7374 6174 732b 3d5b         Ustats+=[
+00015520: 584f 626a 5f73 7461 7473 5b69 5d5d 0d0a  XObj_stats[i]]..
+00015530: 2020 2020 2020 2020 2020 2020 5573 6861              Usha
+00015540: 7065 2b3d 5b58 4f62 6a5f 7368 6170 655b  pe+=[XObj_shape[
+00015550: 695d 5d0d 0a0d 0a20 2020 206e 6577 5f69  i]]....    new_i
+00015560: 6e64 3120 3d20 2222 0d0a 2020 2020 666f  nd1 = ""..    fo
+00015570: 7220 6368 6172 2069 6e20 6368 6172 5f6c  r char in char_l
+00015580: 6973 743a 0d0a 2020 2020 2020 2020 6966  ist:..        if
+00015590: 2063 6861 7220 6e6f 7420 696e 2055 696e   char not in Uin
+000155a0: 642b 5669 6e64 3a0d 0a20 2020 2020 2020  d+Vind:..       
+000155b0: 2020 2020 206e 6577 5f69 6e64 3120 3d20       new_ind1 = 
+000155c0: 6368 6172 0d0a 2020 2020 2020 2020 2020  char..          
+000155d0: 2020 6272 6561 6b0d 0a0d 0a20 2020 2055    break....    U
+000155e0: 696e 6420 2020 3d20 2228 222b 5569 6e64  ind   = "("+Uind
+000155f0: 2b22 2922 202b 206e 6577 5f69 6e64 310d  +")" + new_ind1.
+00015600: 0a20 2020 2056 696e 6420 2020 3d20 6e65  .    Vind   = ne
+00015610: 775f 696e 6431 202b 2022 2822 2b56 696e  w_ind1 + "("+Vin
+00015620: 642b 2229 220d 0a20 2020 2055 7374 6174  d+")"..    Ustat
+00015630: 7320 3d20 7475 706c 6528 5573 7461 7473  s = tuple(Ustats
+00015640: 202b 205b 2dce 9b73 7461 746c 6566 745d   + [-..statleft]
+00015650: 290d 0a20 2020 2056 7374 6174 7320 3d20  )..    Vstats = 
+00015660: 7475 706c 6528 5b2d ce9b 7374 6174 7269  tuple([-..statri
+00015670: 6768 745d 202b 2056 7374 6174 7329 0d0a  ght] + Vstats)..
+00015680: 2020 2020 5573 6861 7065 203d 2074 7570      Ushape = tup
+00015690: 6c65 2855 7368 6170 6520 2b20 5b64 ce9b  le(Ushape + [d..
+000156a0: 5d29 0d0a 2020 2020 5673 6861 7065 203d  ])..    Vshape =
+000156b0: 2074 7570 6c65 285b 64ce 9b5d 202b 2056   tuple([d..] + V
+000156c0: 7368 6170 6529 0d0a 2020 2020 0d0a 2020  shape)..    ..  
+000156d0: 2020 7374 6570 203d 2073 686f 775f 7072    step = show_pr
+000156e0: 6f67 7265 7373 2873 7465 702c 7072 6f63  ogress(step,proc
+000156f0: 6573 735f 6c65 6e67 7468 2c70 726f 6365  ess_length,proce
+00015700: 7373 5f6e 616d 652b 2220 222b 223c 222b  ss_name+" "+"<"+
+00015710: 6375 7272 656e 745f 6d65 6d6f 7279 5f64  current_memory_d
+00015720: 6973 706c 6179 2829 2b22 3e22 2c63 6f6c  isplay()+">",col
+00015730: 6f72 3d70 726f 6365 7373 5f63 6f6c 6f72  or=process_color
+00015740: 2c74 696d 653d 7469 6d65 2e74 696d 6528  ,time=time.time(
+00015750: 292d 7330 3029 2023 360d 0a20 2020 2055  )-s00) #6..    U
+00015760: 203d 2055 2e73 706c 6974 5f6c 6567 7328   = U.split_legs(
+00015770: 5569 6e64 2c55 7374 6174 732c 5573 6861  Uind,Ustats,Usha
+00015780: 7065 2c73 6176 655f 6d65 6d6f 7279 3d54  pe,save_memory=T
+00015790: 7275 6529 0d0a 2020 2020 ce9b 203d 20ce  rue)..    .. = .
+000157a0: 9b2e 7377 6974 6368 5f65 6e63 6f64 6572  ..switch_encoder
+000157b0: 2873 6176 655f 6d65 6d6f 7279 3d54 7275  (save_memory=Tru
+000157c0: 6529 0d0a 2020 2020 5620 3d20 562e 7370  e)..    V = V.sp
+000157d0: 6c69 745f 6c65 6773 2856 696e 642c 5673  lit_legs(Vind,Vs
+000157e0: 7461 7473 2c56 7368 6170 652c 7361 7665  tats,Vshape,save
+000157f0: 5f6d 656d 6f72 793d 5472 7565 290d 0a20  _memory=True).. 
+00015800: 2020 200d 0a20 2020 2069 6628 7468 6973     ..    if(this
+00015810: 5f66 6f72 6d61 7420 3d3d 2027 7374 616e  _format == 'stan
+00015820: 6461 7264 2729 3a0d 0a20 2020 2020 2020  dard'):..       
+00015830: 2055 203d 2055 2e73 7769 7463 685f 666f   U = U.switch_fo
+00015840: 726d 6174 2873 6176 655f 6d65 6d6f 7279  rmat(save_memory
+00015850: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00015860: ce9b 203d 20ce 9b2e 7377 6974 6368 5f66  .. = ...switch_f
+00015870: 6f72 6d61 7428 7361 7665 5f6d 656d 6f72  ormat(save_memor
+00015880: 793d 5472 7565 290d 0a20 2020 2020 2020  y=True)..       
+00015890: 2056 203d 2056 2e73 7769 7463 685f 666f   V = V.switch_fo
+000158a0: 726d 6174 2873 6176 655f 6d65 6d6f 7279  rmat(save_memory
+000158b0: 3d54 7275 6529 0d0a 0d0a 2020 2020 6966  =True)....    if
+000158c0: 2874 6869 735f 656e 636f 6465 7220 3d3d  (this_encoder ==
+000158d0: 2027 7061 7269 7479 2d70 7265 7365 7276   'parity-preserv
+000158e0: 696e 6727 293a 0d0a 2020 2020 2020 2020  ing'):..        
+000158f0: 5520 3d20 552e 7377 6974 6368 5f65 6e63  U = U.switch_enc
+00015900: 6f64 6572 2873 6176 655f 6d65 6d6f 7279  oder(save_memory
+00015910: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00015920: ce9b 203d 20ce 9b2e 7377 6974 6368 5f65  .. = ...switch_e
+00015930: 6e63 6f64 6572 2873 6176 655f 6d65 6d6f  ncoder(save_memo
+00015940: 7279 3d54 7275 6529 0d0a 2020 2020 2020  ry=True)..      
+00015950: 2020 5620 3d20 562e 7377 6974 6368 5f65    V = V.switch_e
+00015960: 6e63 6f64 6572 2873 6176 655f 6d65 6d6f  ncoder(save_memo
+00015970: 7279 3d54 7275 6529 0d0a 0d0a 2020 2020  ry=True)....    
+00015980: 6966 2874 6869 735f 7479 7065 3d3d 7370  if(this_type==sp
+00015990: 6172 7365 293a 0d0a 2020 2020 2020 2020  arse):..        
+000159a0: 5520 3d20 7370 6172 7365 2855 290d 0a20  U = sparse(U).. 
+000159b0: 2020 2020 2020 20ce 9b20 3d20 7370 6172         .. = spar
+000159c0: 7365 28ce 9b29 0d0a 2020 2020 2020 2020  se(..)..        
+000159d0: 5620 3d20 7370 6172 7365 2856 290d 0a0d  V = sparse(V)...
+000159e0: 0a20 2020 2063 6c65 6172 5f70 726f 6772  .    clear_progr
+000159f0: 6573 7328 290d 0a20 2020 2074 6162 5f75  ess()..    tab_u
+00015a00: 7028 290d 0a0d 0a20 2020 2072 6574 7572  p()....    retur
+00015a10: 6e20 552c 20ce 9b2c 2056 0d0a 0d0a 2323  n U, .., V....##
+00015a20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015a30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015a40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015a50: 2323 0d0a 2323 2020 2020 2020 2020 2020  ##..##          
+00015a60: 2020 4569 6765 6e20 7661 6c75 6520 6465    Eigen value de
+00015a70: 636f 6d70 6f73 6974 696f 6e20 2020 2020  composition     
+00015a80: 2020 2020 2020 2323 0d0a 2323 2323 2323        ##..######
 00015a90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015aa0: 2323 2323 2323 2323 2323 230d 0a23 2320  ###########..## 
-00015ab0: 2020 2020 2020 2020 2020 2045 6967 656e             Eigen
-00015ac0: 2076 616c 7565 2064 6563 6f6d 706f 7369   value decomposi
-00015ad0: 7469 6f6e 2020 2020 2020 2020 2020 2023  tion           #
-00015ae0: 230d 0a23 2323 2323 2323 2323 2323 2323  #..#############
-00015af0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015b00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00015b10: 2323 2323 2323 230d 0a0d 0a64 6566 2053  #######....def S
-00015b20: 6f72 7465 6445 6967 284d 2c63 7574 6f66  ortedEig(M,cutof
-00015b30: 663d 4e6f 6e65 2c64 6562 7567 5f6d 6f64  f=None,debug_mod
-00015b40: 653d 4661 6c73 6529 3a0d 0a0d 0a20 2020  e=False):....   
-00015b50: 204e 6f6e 4865 7269 7469 616e 4e6f 726d   NonHeritianNorm
-00015b60: 203d 206e 702e 6c69 6e61 6c67 2e6e 6f72   = np.linalg.nor
-00015b70: 6d28 4d2d 6e70 2e63 6f6e 6a75 6761 7465  m(M-np.conjugate
-00015b80: 286e 702e 7472 616e 7370 6f73 6528 4d29  (np.transpose(M)
-00015b90: 2929 2f6e 702e 6c69 6e61 6c67 2e6e 6f72  ))/np.linalg.nor
-00015ba0: 6d28 4d29 0d0a 2020 2020 6966 204e 6f6e  m(M)..    if Non
-00015bb0: 4865 7269 7469 616e 4e6f 726d 3e6e 756d  HeritianNorm>num
-00015bc0: 6572 5f63 7574 6f66 6620 3a0d 0a20 2020  er_cutoff :..   
-00015bd0: 2020 2020 2065 7272 6f72 2822 4572 726f       error("Erro
-00015be0: 725b 536f 7274 6564 4569 675d 3a20 5468  r[SortedEig]: Th
-00015bf0: 6520 696e 7075 7420 6d61 7472 6978 2069  e input matrix i
-00015c00: 7320 6e6f 7420 4865 726d 6974 6961 6e21  s not Hermitian!
-00015c10: 2229 0d0a 0d0a 2020 2020 552c 20ce 9b2c  ")....    U, ..,
-00015c20: 2056 203d 206e 702e 6c69 6e61 6c67 2e73   V = np.linalg.s
-00015c30: 7664 284d 2c20 6675 6c6c 5f6d 6174 7269  vd(M, full_matri
-00015c40: 6365 733d 4661 6c73 6529 0d0a 0d0a 2020  ces=False)....  
-00015c50: 2020 6e6e 7a20 3d20 300d 0a20 2020 2023    nnz = 0..    #
-00015c60: 6966 206e 702e 6162 7328 ce9b 5b30 5d29  if np.abs(..[0])
-00015c70: 203c 206e 756d 6572 5f63 7574 6f66 663a   < numer_cutoff:
-00015c80: 0d0a 2020 2020 2320 2020 2065 7272 6f72  ..    #    error
-00015c90: 2822 4572 726f 725b 536f 7274 6564 5356  ("Error[SortedSV
-00015ca0: 445d 3a20 6e70 2e6c 696e 616c 672e 7376  D]: np.linalg.sv
-00015cb0: 6428 2920 7265 7475 726e 7320 7a65 726f  d() returns zero
-00015cc0: 2073 696e 6775 6c61 7220 7661 6c75 6520   singular value 
-00015cd0: 7665 6374 6f72 2122 290d 0a0d 0a20 2020  vector!")....   
-00015ce0: 2066 6f72 2069 2c73 2069 6e20 656e 756d   for i,s in enum
-00015cf0: 6572 6174 6528 ce9b 293a 0d0a 2020 2020  erate(..):..    
-00015d00: 2020 2020 6966 206e 702e 6162 7328 732f      if np.abs(s/
-00015d10: ce9b 5b30 5d29 203e 206e 756d 6572 5f63  ..[0]) > numer_c
-00015d20: 7574 6f66 663a 0d0a 2020 2020 2020 2020  utoff:..        
-00015d30: 2020 2020 6e6e 7a2b 3d31 0d0a 0d0a 2020      nnz+=1....  
-00015d40: 2020 6966 2063 7574 6f66 6621 3d4e 6f6e    if cutoff!=Non
-00015d50: 6520 616e 6420 6375 746f 6666 203c 206e  e and cutoff < n
-00015d60: 6e7a 3a0d 0a20 2020 2020 2020 206e 6e7a  nz:..        nnz
-00015d70: 203d 2063 7574 6f66 660d 0a0d 0a20 2020   = cutoff....   
-00015d80: 20ce 9b20 3d20 ce9b 5b3a 6e6e 7a5d 0d0a   .. = ..[:nnz]..
-00015d90: 2020 2020 5520 3d20 555b 3a2c 3a6e 6e7a      U = U[:,:nnz
-00015da0: 5d0d 0a20 2020 2056 203d 2056 5b3a 6e6e  ]..    V = V[:nn
-00015db0: 7a2c 3a5d 0d0a 2020 2020 6355 203d 206e  z,:]..    cU = n
-00015dc0: 702e 636f 6e6a 7567 6174 6528 6e70 2e74  p.conjugate(np.t
-00015dd0: 7261 6e73 706f 7365 2855 2929 0d0a 2020  ranspose(U))..  
-00015de0: 2020 ce9b 5655 203d 206e 702e 6569 6e73    ..VU = np.eins
-00015df0: 756d 2827 692c 696a 2c6a 6b2d 3e69 6b27  um('i,ij,jk->ik'
-00015e00: 2cce 9b2c 562c 5529 0d0a 2020 2020 ce9b  ,..,V,U)..    ..
-00015e10: 203d 206e 702e 6569 6e73 756d 2827 692c   = np.einsum('i,
-00015e20: 696a 2c6a 6b2d 3e6b 272c ce9b 2c56 2c55  ij,jk->k',..,V,U
-00015e30: 290d 0a0d 0a20 2020 2072 6574 7572 6e20  )....    return 
-00015e40: 552c 20ce 9b2c 2063 550d 0a23 2049 203d  U, .., cU..# I =
-00015e50: 2063 5555 0d0a 6465 6620 426c 6f63 6b45   cUU..def BlockE
-00015e60: 6967 284f 626a 2c63 7574 6f66 663d 4e6f  ig(Obj,cutoff=No
-00015e70: 6e65 2c64 6562 7567 5f6d 6f64 653d 4661  ne,debug_mode=Fa
-00015e80: 6c73 6529 3a0d 0a20 2020 200d 0a20 2020  lse):..    ..   
-00015e90: 2023 2070 6572 666f 726d 696e 6720 616e   # performing an
-00015ea0: 2073 7664 206f 6620 6120 6d61 7472 6978   svd of a matrix
-00015eb0: 2062 6c6f 636b 2062 7920 626c 6f63 6b0d   block by block.
-00015ec0: 0a0d 0a20 2020 2069 6628 7479 7065 284f  ...    if(type(O
-00015ed0: 626a 2921 3d6e 702e 6172 7261 7920 616e  bj)!=np.array an
-00015ee0: 6420 7479 7065 284f 626a 2921 3d6e 702e  d type(Obj)!=np.
-00015ef0: 6e64 6172 7261 7929 3a0d 0a20 2020 2020  ndarray):..     
-00015f00: 2020 2065 7272 6f72 2822 4572 726f 725b     error("Error[
-00015f10: 426c 6f63 6b45 6967 5d3a 2041 6e20 696e  BlockEig]: An in
-00015f20: 7075 7420 6d75 7374 2062 6520 6f66 2074  put must be of t
-00015f30: 7970 6520 6e75 6d70 792e 6172 7261 7920  ype numpy.array 
-00015f40: 6f72 206e 756d 7079 2e6e 6461 7272 6179  or numpy.ndarray
-00015f50: 206f 6e6c 7921 2229 0d0a 2020 2020 2020   only!")..      
-00015f60: 2020 0d0a 0d0a 2020 2020 6966 284f 626a    ....    if(Obj
-00015f70: 2e6e 6469 6d21 3d32 293a 0d0a 2020 2020  .ndim!=2):..    
-00015f80: 2020 2020 6572 726f 7228 2245 7272 6f72      error("Error
-00015f90: 5b42 6c6f 636b 4569 675d 3a20 416e 2069  [BlockEig]: An i
-00015fa0: 6e70 7574 206d 7573 7420 6265 2061 206d  nput must be a m
-00015fb0: 6174 7269 7820 6f6e 6c79 2122 290d 0a20  atrix only!").. 
-00015fc0: 2020 2020 2020 200d 0a0d 0a20 2020 206d         ....    m
-00015fd0: 203d 204f 626a 2e73 6861 7065 5b30 5d0d   = Obj.shape[0].
-00015fe0: 0a20 2020 206e 203d 204f 626a 2e73 6861  .    n = Obj.sha
-00015ff0: 7065 5b31 5d0d 0a0d 0a20 2020 2069 6628  pe[1]....    if(
-00016000: 6d25 3221 3d30 2061 6e64 206e 2532 213d  m%2!=0 and n%2!=
-00016010: 3029 3a0d 0a20 2020 2020 2020 2065 7272  0):..        err
-00016020: 6f72 2822 4572 726f 725b 426c 6f63 6b45  or("Error[BlockE
-00016030: 6967 5d3a 2054 6865 206d 6174 7269 7820  ig]: The matrix 
-00016040: 6469 6d65 6e73 696f 6e73 206d 7573 7420  dimensions must 
-00016050: 6265 2065 7665 6e21 2229 0d0a 2020 2020  be even!")..    
-00016060: 2020 2020 0d0a 0d0a 0d0a 2020 2020 6966      ......    if
-00016070: 286d 3d3d 3020 616e 6420 6e3d 3d30 293a  (m==0 and n==0):
-00016080: 0d0a 2020 2020 2020 2020 6572 726f 7228  ..        error(
-00016090: 2245 7272 6f72 5b42 6c6f 636b 4569 675d  "Error[BlockEig]
-000160a0: 3a20 5468 6520 6d61 7472 6978 2064 696d  : The matrix dim
-000160b0: 656e 7369 6f6e 7320 6d75 7374 2062 6520  ensions must be 
-000160c0: 6174 206c 6561 7374 2032 2122 290d 0a20  at least 2!").. 
-000160d0: 2020 2020 2020 200d 0a0d 0a20 2020 2070         ....    p
-000160e0: 6172 6974 795f 6e6f 726d 203d 2030 0d0a  arity_norm = 0..
-000160f0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00016100: 6765 286d 293a 0d0a 2020 2020 2020 2020  ge(m):..        
-00016110: 666f 7220 6a20 696e 2072 616e 6765 286e  for j in range(n
-00016120: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00016130: 6966 2028 692b 6a29 2532 213d 303a 0d0a  if (i+j)%2!=0:..
-00016140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016150: 7061 7269 7479 5f6e 6f72 6d20 2b3d 206e  parity_norm += n
-00016160: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 4f62  p.linalg.norm(Ob
-00016170: 6a5b 692c 6a5d 290d 0a20 2020 2069 6628  j[i,j])..    if(
-00016180: 2028 6e6f 7420 736b 6970 5f70 6172 6974   (not skip_parit
-00016190: 795f 626c 6f63 6b69 6e67 5f63 6865 636b  y_blocking_check
-000161a0: 2920 616e 6420 7061 7269 7479 5f6e 6f72  ) and parity_nor
-000161b0: 6d2f 286d 2a6e 2f32 293e 312e 3065 2d31  m/(m*n/2)>1.0e-1
-000161c0: 3429 3a0d 0a20 2020 2020 2020 2065 7272  4):..        err
-000161d0: 6f72 2822 4572 726f 725b 426c 6f63 6b45  or("Error[BlockE
-000161e0: 6967 5d3a 2054 6869 7320 6d61 7472 6978  ig]: This matrix
-000161f0: 2069 7320 6e6f 7420 636f 6e73 7472 7563   is not construc
-00016200: 7465 6420 6672 6f6d 2061 2047 7261 7373  ted from a Grass
-00016210: 6d61 6e6e 2d65 7665 6e20 7465 6e73 6f72  mann-even tensor
-00016220: 2e22 290d 0a20 2020 2020 2020 2070 7269  .")..        pri
-00016230: 6e74 2822 2020 2020 2020 2020 2020 2020  nt("            
-00016240: 2020 2020 2028 4f72 2074 6861 7420 6f6e       (Or that on
-00016250: 6520 6f66 2074 6865 2069 6e64 6963 6573  e of the indices
-00016260: 2061 7265 206e 6f6e 2d66 6572 6d69 6f6e   are non-fermion
-00016270: 6963 2e29 2229 0d0a 2020 2020 2020 2020  ic.)")..        
-00016280: 0d0a 0d0a 2020 2020 2320 4174 2074 6869  ....    # At thi
-00016290: 7320 706f 696e 7420 7468 6520 6d61 7472  s point the matr
-000162a0: 6978 2069 7320 7765 6c6c 2d62 6568 6176  ix is well-behav
-000162b0: 6564 0d0a 0d0a 2020 2020 2320 7469 6d65  ed....    # time
-000162c0: 2074 6f20 7365 7061 7261 7465 2074 6865   to separate the
-000162d0: 2062 6c6f 636b 730d 0a20 2020 204d 4520   blocks..    ME 
-000162e0: 3d20 6e70 2e7a 6572 6f73 285b 696e 7428  = np.zeros([int(
-000162f0: 6d2f 3229 2c69 6e74 286e 2f32 295d 2c64  m/2),int(n/2)],d
-00016300: 7479 7065 3d74 7970 6528 4f62 6a5b 305d  type=type(Obj[0]
-00016310: 5b30 5d29 290d 0a20 2020 204d 4f20 3d20  [0]))..    MO = 
-00016320: 6e70 2e7a 6572 6f73 285b 696e 7428 6d2f  np.zeros([int(m/
-00016330: 3229 2c69 6e74 286e 2f32 295d 2c64 7479  2),int(n/2)],dty
-00016340: 7065 3d74 7970 6528 4f62 6a5b 305d 5b30  pe=type(Obj[0][0
-00016350: 5d29 290d 0a0d 0a20 2020 2066 6f72 2069  ]))....    for i
-00016360: 2069 6e20 7261 6e67 6528 696e 7428 6d2f   in range(int(m/
-00016370: 3229 293a 0d0a 2020 2020 2020 2020 666f  2)):..        fo
-00016380: 7220 6a20 696e 2072 616e 6765 2869 6e74  r j in range(int
-00016390: 286e 2f32 2929 3a0d 0a20 2020 2020 2020  (n/2)):..       
-000163a0: 2020 2020 204d 455b 692c 6a5d 203d 204f       ME[i,j] = O
-000163b0: 626a 5b32 2a69 2c32 2a6a 5d0d 0a20 2020  bj[2*i,2*j]..   
-000163c0: 2020 2020 2020 2020 204d 4f5b 692c 6a5d           MO[i,j]
-000163d0: 203d 204f 626a 5b32 2a69 2b31 2c32 2a6a   = Obj[2*i+1,2*j
-000163e0: 2b31 5d0d 0a0d 0a20 2020 2068 616c 6663  +1]....    halfc
-000163f0: 7574 6f66 6620 3d20 4e6f 6e65 0d0a 2020  utoff = None..  
-00016400: 2020 6966 2063 7574 6f66 6621 3d4e 6f6e    if cutoff!=Non
-00016410: 6520 3a0d 0a20 2020 2020 2020 2068 616c  e :..        hal
-00016420: 6663 7574 6f66 6620 3d20 696e 7428 6375  fcutoff = int(cu
-00016430: 746f 6666 2f32 290d 0a0d 0a20 2020 2055  toff/2)....    U
-00016440: 452c 20ce 9b45 2c20 6355 4520 3d20 536f  E, ..E, cUE = So
-00016450: 7274 6564 4569 6728 4d45 2c68 616c 6663  rtedEig(ME,halfc
-00016460: 7574 6f66 662c 6465 6275 675f 6d6f 6465  utoff,debug_mode
-00016470: 290d 0a20 2020 2055 4f2c 20ce 9b4f 2c20  )..    UO, ..O, 
-00016480: 6355 4f20 3d20 536f 7274 6564 4569 6728  cUO = SortedEig(
-00016490: 4d4f 2c68 616c 6663 7574 6f66 662c 6465  MO,halfcutoff,de
-000164a0: 6275 675f 6d6f 6465 290d 0a0d 0a20 2020  bug_mode)....   
-000164b0: 2064 203d 206d 6178 286c 656e 28ce 9b45   d = max(len(..E
-000164c0: 292c 6c65 6e28 ce9b 4f29 290d 0a20 2020  ),len(..O))..   
-000164d0: 2064 203d 2069 6e74 2832 2a2a 6d61 7468   d = int(2**math
-000164e0: 2e63 6569 6c28 6e70 2e6c 6f67 3228 6429  .ceil(np.log2(d)
-000164f0: 2929 0d0a 0d0a 2020 2020 6465 6620 7061  ))....    def pa
-00016500: 6464 696e 6728 5578 2c20 ce9b 782c 2063  dding(Ux, ..x, c
-00016510: 5578 2c20 7061 6464 696e 675f 6469 6d65  Ux, padding_dime
-00016520: 6e73 696f 6e29 3a0d 0a20 2020 2020 2020  nsion):..       
-00016530: 2055 7820 3d20 6e70 2e70 6164 2855 782c   Ux = np.pad(Ux,
-00016540: 2828 302c 3029 2c28 302c 7061 6464 696e  ((0,0),(0,paddin
-00016550: 675f 6469 6d65 6e73 696f 6e29 292c 2763  g_dimension)),'c
-00016560: 6f6e 7374 616e 7427 2c63 6f6e 7374 616e  onstant',constan
-00016570: 745f 7661 6c75 6573 3d28 2830 2c30 292c  t_values=((0,0),
-00016580: 2830 2c30 2929 290d 0a20 2020 2020 2020  (0,0)))..       
-00016590: 20ce 9b78 203d 206e 702e 6469 6167 286e   ..x = np.diag(n
-000165a0: 702e 7061 6428 ce9b 782c 2830 2c70 6164  p.pad(..x,(0,pad
-000165b0: 6469 6e67 5f64 696d 656e 7369 6f6e 292c  ding_dimension),
-000165c0: 2763 6f6e 7374 616e 7427 2c63 6f6e 7374  'constant',const
-000165d0: 616e 745f 7661 6c75 6573 3d28 302c 3029  ant_values=(0,0)
-000165e0: 2020 2020 2020 2029 290d 0a20 2020 2020         ))..     
-000165f0: 2020 2063 5578 203d 206e 702e 7061 6428     cUx = np.pad(
-00016600: 6355 782c 2828 302c 7061 6464 696e 675f  cUx,((0,padding_
-00016610: 6469 6d65 6e73 696f 6e29 2c28 302c 3029  dimension),(0,0)
-00016620: 292c 2763 6f6e 7374 616e 7427 2c63 6f6e  ),'constant',con
-00016630: 7374 616e 745f 7661 6c75 6573 3d28 2830  stant_values=((0
-00016640: 2c30 292c 2830 2c30 2929 290d 0a20 2020  ,0),(0,0)))..   
-00016650: 2020 2020 2072 6574 7572 6e20 5578 2c20       return Ux, 
-00016660: ce9b 782c 2063 5578 0d0a 0d0a 2020 2020  ..x, cUx....    
-00016670: 5545 2c20 ce9b 452c 2063 5545 203d 2070  UE, ..E, cUE = p
-00016680: 6164 6469 6e67 2855 452c 20ce 9b45 2c20  adding(UE, ..E, 
-00016690: 6355 452c 2064 2d6c 656e 28ce 9b45 2929  cUE, d-len(..E))
-000166a0: 0d0a 2020 2020 554f 2c20 ce9b 4f2c 2063  ..    UO, ..O, c
-000166b0: 554f 203d 2070 6164 6469 6e67 2855 4f2c  UO = padding(UO,
-000166c0: 20ce 9b4f 2c20 6355 4f2c 2064 2d6c 656e   ..O, cUO, d-len
-000166d0: 28ce 9b4f 2929 0d0a 0d0a 2020 2020 2370  (..O))....    #p
-000166e0: 7269 6e74 2829 0d0a 2020 2020 2370 7269  rint()..    #pri
-000166f0: 6e74 2822 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  nt("------------
-00016700: 2d2d 2d2d 2d2d 2d2d 2229 0d0a 2020 2020  --------")..    
-00016710: 2366 6f72 2069 2c73 2069 6e20 656e 756d  #for i,s in enum
-00016720: 6572 6174 6528 6e70 2e64 6961 6728 ce9b  erate(np.diag(..
-00016730: 4529 293a 0d0a 2020 2020 2320 2020 2070  E)):..    #    p
-00016740: 7269 6e74 2822 2065 7665 6e3a 222c 636c  rint(" even:",cl
-00016750: 6561 6e5f 666f 726d 6174 2873 2929 0d0a  ean_format(s))..
-00016760: 2020 2020 2370 7269 6e74 2829 0d0a 2020      #print()..  
-00016770: 2020 2366 6f72 2069 2c73 2069 6e20 656e    #for i,s in en
-00016780: 756d 6572 6174 6528 6e70 2e64 6961 6728  umerate(np.diag(
-00016790: ce9b 4f29 293a 0d0a 2020 2020 2320 2020  ..O)):..    #   
-000167a0: 2070 7269 6e74 2822 2020 6f64 643a 222c   print("  odd:",
-000167b0: 636c 6561 6e5f 666f 726d 6174 2873 2929  clean_format(s))
-000167c0: 0d0a 2020 2020 2370 7269 6e74 2822 2d2d  ..    #print("--
-000167d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000167e0: 2d2d 2229 0d0a 2020 2020 2370 7269 6e74  --")..    #print
-000167f0: 2829 0d0a 0d0a 2020 2020 6465 6620 6765  ()....    def ge
-00016800: 745f 6675 6c6c 5f6d 6174 7269 7828 4145  t_full_matrix(AE
-00016810: 2c20 414f 293a 0d0a 2020 2020 2020 2020  , AO):..        
-00016820: 6d68 616c 662c 6e68 616c 6620 3d20 4145  mhalf,nhalf = AE
-00016830: 2e73 6861 7065 0d0a 2020 2020 2020 2020  .shape..        
-00016840: 4120 3d20 6e70 2e7a 6572 6f73 285b 322a  A = np.zeros([2*
-00016850: 6d68 616c 662c 322a 6e68 616c 665d 2c64  mhalf,2*nhalf],d
-00016860: 7479 7065 3d74 7970 6528 4145 5b30 5d5b  type=type(AE[0][
-00016870: 305d 2929 0d0a 2020 2020 2020 2020 666f  0]))..        fo
-00016880: 7220 6920 696e 2072 616e 6765 286d 6861  r i in range(mha
-00016890: 6c66 293a 0d0a 2020 2020 2020 2020 2020  lf):..          
-000168a0: 2020 666f 7220 6a20 696e 2072 616e 6765    for j in range
-000168b0: 286e 6861 6c66 293a 0d0a 2020 2020 2020  (nhalf):..      
-000168c0: 2020 2020 2020 2020 2020 415b 322a 692c            A[2*i,
-000168d0: 322a 6a5d 203d 2041 455b 692c 6a5d 0d0a  2*j] = AE[i,j]..
-000168e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000168f0: 415b 322a 692b 312c 322a 6a2b 315d 203d  A[2*i+1,2*j+1] =
-00016900: 2041 4f5b 692c 6a5d 0d0a 2020 2020 2020   AO[i,j]..      
-00016910: 2020 7265 7475 726e 2041 0d0a 0d0a 2020    return A....  
-00016920: 2020 5520 3d20 6765 745f 6675 6c6c 5f6d    U = get_full_m
-00016930: 6174 7269 7828 5545 2c55 4f29 0d0a 2020  atrix(UE,UO)..  
-00016940: 2020 ce9b 203d 2067 6574 5f66 756c 6c5f    .. = get_full_
-00016950: 6d61 7472 6978 28ce 9b45 2cce 9b4f 290d  matrix(..E,..O).
-00016960: 0a20 2020 2063 5520 3d20 6765 745f 6675  .    cU = get_fu
-00016970: 6c6c 5f6d 6174 7269 7828 6355 452c 6355  ll_matrix(cUE,cU
-00016980: 4f29 0d0a 2020 2020 0d0a 0d0a 2020 2020  O)..    ....    
-00016990: 7265 7475 726e 2055 2c20 ce9b 2c20 6355  return U, .., cU
-000169a0: 0d0a 0d0a 6465 6620 6569 6728 496e 704f  ....def eig(InpO
-000169b0: 626a 2c73 7472 696e 672c 6375 746f 6666  bj,string,cutoff
-000169c0: 3d4e 6f6e 652c 6465 6275 675f 6d6f 6465  =None,debug_mode
-000169d0: 3d46 616c 7365 2c73 6176 655f 6d65 6d6f  =False,save_memo
-000169e0: 7279 3d46 616c 7365 293a 0d0a 0d0a 2020  ry=False):....  
-000169f0: 2020 7072 6f63 6573 735f 6e61 6d65 203d    process_name =
-00016a00: 2022 6569 6722 0d0a 2020 2020 7072 6f63   "eig"..    proc
-00016a10: 6573 735f 636f 6c6f 7220 3d20 2279 656c  ess_color = "yel
-00016a20: 6c6f 7722 0d0a 2020 2020 7072 6f63 6573  low"..    proces
-00016a30: 735f 6c65 6e67 7468 203d 2036 0d0a 2020  s_length = 6..  
-00016a40: 2020 7374 6570 203d 2031 0d0a 2020 2020    step = 1..    
-00016a50: 7330 3020 3d20 7469 6d65 2e74 696d 6528  s00 = time.time(
-00016a60: 290d 0a20 2020 2070 7269 6e74 2829 0d0a  )..    print()..
-00016a70: 0d0a 2020 2020 676c 6f62 616c 2073 6b69  ..    global ski
-00016a80: 705f 706f 7765 725f 6f66 5f74 776f 5f63  p_power_of_two_c
-00016a90: 6865 636b 0d0a 0d0a 2020 2020 2320 7468  heck....    # th
-00016aa0: 6520 7374 7269 6e67 2069 7320 6f66 2074  e string is of t
-00016ab0: 6865 2066 6f72 6d20 6161 6161 7c62 6262  he form aaaa|bbb
-00016ac0: 0d0a 0d0a 2020 2020 7374 7269 6e67 203d  ....    string =
-00016ad0: 2064 656e 756d 6572 6174 6528 7374 7269   denumerate(stri
-00016ae0: 6e67 290d 0a0d 0a20 2020 200d 0a20 2020  ng)....    ..   
-00016af0: 204f 626a 203d 2049 6e70 4f62 6a2e 636f   Obj = InpObj.co
-00016b00: 7079 2829 0d0a 2020 2020 7468 6973 5f74  py()..    this_t
-00016b10: 7970 6520 3d20 7479 7065 284f 626a 290d  ype = type(Obj).
-00016b20: 0a20 2020 2074 6869 735f 666f 726d 6174  .    this_format
-00016b30: 203d 204f 626a 2e66 6f72 6d61 740d 0a20   = Obj.format.. 
-00016b40: 2020 2074 6869 735f 656e 636f 6465 7220     this_encoder 
-00016b50: 3d20 4f62 6a2e 656e 636f 6465 720d 0a20  = Obj.encoder.. 
-00016b60: 2020 2058 4f62 6a5f 7374 6174 7320 3d20     XObj_stats = 
-00016b70: 4f62 6a2e 7374 6174 6973 7469 630d 0a20  Obj.statistic.. 
-00016b80: 2020 2058 4f62 6a5f 7368 6170 6520 3d20     XObj_shape = 
-00016b90: 4f62 6a2e 7368 6170 650d 0a0d 0a20 2020  Obj.shape....   
-00016ba0: 2069 6620 7361 7665 5f6d 656d 6f72 7920   if save_memory 
-00016bb0: 3a0d 0a20 2020 2020 2020 2064 656c 2049  :..        del I
-00016bc0: 6e70 4f62 6a2e 6461 7461 0d0a 2020 2020  npObj.data..    
-00016bd0: 2020 2020 6465 6c20 496e 704f 626a 0d0a      del InpObj..
-00016be0: 2020 2020 2020 2020 6763 2e63 6f6c 6c65          gc.colle
-00016bf0: 6374 2829 0d0a 2020 2020 2020 2020 0d0a  ct()..        ..
-00016c00: 2020 2020 2020 2020 0d0a 2020 2020 6966          ..    if
-00016c10: 2874 6869 735f 7479 7065 3d3d 7370 6172  (this_type==spar
-00016c20: 7365 293a 0d0a 2020 2020 2020 2020 4f62  se):..        Ob
-00016c30: 6a20 3d20 6465 6e73 6528 4f62 6a29 0d0a  j = dense(Obj)..
-00016c40: 2020 2020 6966 2874 6869 735f 7479 7065      if(this_type
-00016c50: 206e 6f74 2069 6e20 5b64 656e 7365 2c73   not in [dense,s
-00016c60: 7061 7273 655d 293a 0d0a 2020 2020 2020  parse]):..      
-00016c70: 2020 6572 726f 7228 2245 7272 6f72 5b65    error("Error[e
-00016c80: 6967 5d3a 204f 626a 6563 7420 7479 7065  ig]: Object type
-00016c90: 206d 7573 7420 6f6e 6c79 2062 6520 6465   must only be de
-00016ca0: 6e73 6520 6f72 2073 7061 7273 6521 2229  nse or sparse!")
-00016cb0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00016cc0: 2320 6368 6563 6b20 6966 204f 626a 2e73  # check if Obj.s
-00016cd0: 7461 7469 7374 6963 206f 7220 6669 6e61  tatistic or fina
-00016ce0: 6c5f 7374 6174 6973 7469 6320 6973 2077  l_statistic is w
-00016cf0: 6569 7264 206f 7220 6e6f 740d 0a20 2020  eird or not..   
-00016d00: 2066 6f72 2073 7461 7420 696e 204f 626a   for stat in Obj
-00016d10: 2e73 7461 7469 7374 6963 3a0d 0a20 2020  .statistic:..   
-00016d20: 2020 2020 2069 6628 7374 6174 206e 6f74       if(stat not
-00016d30: 2069 6e20 616c 6c6f 7765 645f 7374 6174   in allowed_stat
-00016d40: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00016d50: 6572 726f 7228 2245 7272 6f72 5b65 6967  error("Error[eig
-00016d60: 5d3a 2054 6865 2069 6e70 7574 206f 626a  ]: The input obj
-00016d70: 6563 7420 636f 6e74 6169 6e73 2069 6c6c  ect contains ill
-00016d80: 6567 616c 2073 7461 7469 7374 6963 2e20  egal statistic. 
-00016d90: 2830 2c20 312c 202d 312c 206f 7220 222b  (0, 1, -1, or "+
-00016da0: 6879 6272 6964 5f73 796d 626f 6c2b 2220  hybrid_symbol+" 
-00016db0: 6f6e 6c79 2922 290d 0a0d 0a20 2020 2069  only)")....    i
-00016dc0: 6620 7374 7269 6e67 2e63 6f75 6e74 2822  f string.count("
-00016dd0: 2822 293d 3d73 7472 696e 672e 636f 756e  (")==string.coun
-00016de0: 7428 2229 2229 2061 6e64 2073 7472 696e  t(")") and strin
-00016df0: 672e 636f 756e 7428 2228 2229 3e30 3a0d  g.count("(")>0:.
-00016e00: 0a20 2020 2020 2020 2073 7472 696e 6720  .        string 
-00016e10: 3d20 7374 7269 6e67 2e72 6570 6c61 6365  = string.replace
-00016e20: 2822 2022 2c22 2229 0d0a 2020 2020 2020  (" ","")..      
-00016e30: 2020 7374 7269 6e67 203d 2073 7472 696e    string = strin
-00016e40: 672e 7265 706c 6163 6528 2229 2822 2c22  g.replace(")(","
-00016e50: 2022 290d 0a20 2020 2020 2020 2069 6620   ")..        if 
-00016e60: 7374 7269 6e67 2e63 6f75 6e74 2822 2822  string.count("("
-00016e70: 293e 3120 6f72 2073 7472 696e 672e 636f  )>1 or string.co
-00016e80: 756e 7428 2229 2229 3c31 3a0d 0a20 2020  unt(")")<1:..   
-00016e90: 2020 2020 2020 2020 2065 7272 6f72 2822           error("
-00016ea0: 4572 726f 725b 6569 675d 3a20 5061 7265  Error[eig]: Pare
-00016eb0: 6e74 6865 7365 7320 646f 6e27 7420 6d61  ntheses don't ma
-00016ec0: 7463 6822 290d 0a20 2020 2020 2020 2073  tch")..        s
-00016ed0: 7472 696e 6720 3d20 7374 7269 6e67 2e72  tring = string.r
-00016ee0: 6570 6c61 6365 2822 2922 2c22 2229 0d0a  eplace(")","")..
-00016ef0: 2020 2020 2020 2020 7374 7269 6e67 203d          string =
-00016f00: 2073 7472 696e 672e 7265 706c 6163 6528   string.replace(
-00016f10: 2228 222c 2222 290d 0a0d 0a20 2020 2070  "(","")....    p
-00016f20: 6172 7469 7469 6f6e 5f63 6f75 6e74 203d  artition_count =
-00016f30: 2030 0d0a 2020 2020 666f 7220 7061 7274   0..    for part
-00016f40: 6974 696f 6e20 696e 2073 6570 6172 6174  ition in separat
-00016f50: 6f72 5f6c 6973 743a 0d0a 2020 2020 2020  or_list:..      
-00016f60: 2020 7061 7274 6974 696f 6e5f 636f 756e    partition_coun
-00016f70: 7420 2b3d 2073 7472 696e 672e 636f 756e  t += string.coun
-00016f80: 7428 7061 7274 6974 696f 6e29 0d0a 2020  t(partition)..  
-00016f90: 2020 6966 2870 6172 7469 7469 6f6e 5f63    if(partition_c
-00016fa0: 6f75 6e74 213d 3129 3a0d 0a20 2020 2020  ount!=1):..     
-00016fb0: 2020 2070 6172 7469 7469 6f6e 5f73 7472     partition_str
-00016fc0: 696e 6720 3d20 2222 0d0a 2020 2020 2020  ing = ""..      
-00016fd0: 2020 666f 7220 692c 2070 6172 7469 7469    for i, partiti
-00016fe0: 6f6e 2069 6e20 656e 756d 6572 6174 6528  on in enumerate(
-00016ff0: 7365 7061 7261 746f 725f 6c69 7374 293a  separator_list):
-00017000: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00017010: 2869 3d3d 3029 3a0d 0a20 2020 2020 2020  (i==0):..       
-00017020: 2020 2020 2020 2020 2070 6172 7469 7469           partiti
-00017030: 6f6e 5f73 7472 696e 6720 2b3d 2022 2820  on_string += "( 
-00017040: 220d 0a20 2020 2020 2020 2020 2020 2065  "..            e
-00017050: 6c69 6628 693d 3d6c 656e 2873 6570 6172  lif(i==len(separ
-00017060: 6174 6f72 5f6c 6973 7429 2d31 293a 0d0a  ator_list)-1):..
-00017070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017080: 7061 7274 6974 696f 6e5f 7374 7269 6e67  partition_string
-00017090: 202b 3d20 222c 206f 7220 220d 0a20 2020   += ", or "..   
-000170a0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-000170b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170c0: 7061 7274 6974 696f 6e5f 7374 7269 6e67  partition_string
-000170d0: 202b 3d20 222c 2022 0d0a 0d0a 2020 2020   += ", "....    
-000170e0: 2020 2020 2020 2020 7061 7274 6974 696f          partitio
-000170f0: 6e5f 7374 7269 6e67 202b 3d20 2227 222b  n_string += "'"+
-00017100: 7061 7274 6974 696f 6e2b 2227 220d 0a0d  partition+"'"...
-00017110: 0a20 2020 2020 2020 2020 2020 2069 6628  .            if(
-00017120: 693d 3d6c 656e 2873 6570 6172 6174 6f72  i==len(separator
-00017130: 5f6c 6973 7429 2d31 293a 0d0a 2020 2020  _list)-1):..    
-00017140: 2020 2020 2020 2020 2020 2020 7061 7274              part
-00017150: 6974 696f 6e5f 7374 7269 6e67 202b 3d20  ition_string += 
-00017160: 2220 2922 0d0a 0d0a 2020 2020 2020 2020  " )"....        
-00017170: 6572 726f 7228 2245 7272 6f72 5b65 6967  error("Error[eig
-00017180: 5d3a 2054 6865 2069 6e70 7574 2073 7472  ]: The input str
-00017190: 696e 6720 6d75 7374 2063 6f6e 7461 696e  ing must contain
-000171a0: 206f 6e65 2061 6e64 206f 6e6c 7920 6f6e   one and only on
-000171b0: 6520 7061 7274 6974 696f 6e20 222b 7061  e partition "+pa
-000171c0: 7274 6974 696f 6e5f 7374 7269 6e67 2b22  rtition_string+"
-000171d0: 2069 6e20 6974 2e22 290d 0a20 2020 200d   in it.")..    .
-000171e0: 0a20 2020 2073 7465 7020 3d20 7368 6f77  .    step = show
-000171f0: 5f70 726f 6772 6573 7328 7374 6570 2c70  _progress(step,p
-00017200: 726f 6365 7373 5f6c 656e 6774 682c 7072  rocess_length,pr
-00017210: 6f63 6573 735f 6e61 6d65 2b22 2022 2b22  ocess_name+" "+"
-00017220: 3c22 2b63 7572 7265 6e74 5f6d 656d 6f72  <"+current_memor
-00017230: 795f 6469 7370 6c61 7928 292b 223e 222c  y_display()+">",
-00017240: 636f 6c6f 723d 7072 6f63 6573 735f 636f  color=process_co
-00017250: 6c6f 722c 7469 6d65 3d74 696d 652e 7469  lor,time=time.ti
-00017260: 6d65 2829 2d73 3030 2920 2331 0d0a 2020  me()-s00) #1..  
-00017270: 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a    #:::::::::::::
-00017280: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017290: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000172a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000172b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000172c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000172d0: 3a3a 3a0d 0a20 2020 2023 3a3a 3a3a 3a20  :::..    #::::: 
-000172e0: 2020 2020 2053 5445 5020 3120 2d20 4a4f       STEP 1 - JO
-000172f0: 494e 204c 4547 5320 4241 4553 4420 4f4e  IN LEGS BAESD ON
-00017300: 2054 4845 2047 524f 5550 494e 4753 2020   THE GROUPINGS  
-00017310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017330: 2020 2020 203a 3a3a 3a3a 0d0a 2020 2020       :::::..    
-00017340: 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  #:::::::::::::::
-00017350: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017360: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017370: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017380: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017390: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000173a0: 3a0d 0a0d 0a20 2020 2023 2063 6f75 6e74  :....    # count
-000173b0: 2074 6865 206e 756d 6265 7220 6f66 2069   the number of i
-000173c0: 6e64 6963 6573 2069 6e20 7468 6520 7477  ndices in the tw
-000173d0: 6f20 6772 6f75 7073 0d0a 2020 2020 6e5f  o groups..    n_
-000173e0: 6c65 6674 203d 2030 0d0a 2020 2020 6e5f  left = 0..    n_
-000173f0: 7269 6768 7420 3d20 300d 0a20 2020 2070  right = 0..    p
-00017400: 6172 7469 7469 6f6e 5f66 6f75 6e64 203d  artition_found =
-00017410: 2046 616c 7365 0d0a 2020 2020 666f 7220   False..    for 
-00017420: 6368 6172 2069 6e20 7374 7269 6e67 3a0d  char in string:.
-00017430: 0a20 2020 2020 2020 2069 6620 6368 6172  .        if char
-00017440: 2069 6e20 7365 7061 7261 746f 725f 6c69   in separator_li
-00017450: 7374 203a 0d0a 2020 2020 2020 2020 2020  st :..          
-00017460: 2020 7061 7274 6974 696f 6e5f 666f 756e    partition_foun
-00017470: 6420 3d20 5472 7565 0d0a 2020 2020 2020  d = True..      
-00017480: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
-00017490: 2020 2020 2020 2020 6966 2870 6172 7469          if(parti
-000174a0: 7469 6f6e 5f66 6f75 6e64 293a 0d0a 2020  tion_found):..  
-000174b0: 2020 2020 2020 2020 2020 6e5f 7269 6768            n_righ
-000174c0: 742b 3d31 0d0a 2020 2020 2020 2020 656c  t+=1..        el
-000174d0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-000174e0: 206e 5f6c 6566 742b 3d31 0d0a 0d0a 2020   n_left+=1....  
-000174f0: 2020 6a6f 696e 5f6c 6567 735f 7374 7269    join_legs_stri
-00017500: 6e67 5f69 6e70 7574 203d 2073 7472 696e  ng_input = strin
-00017510: 670d 0a20 2020 2066 6f72 2070 6172 7469  g..    for parti
-00017520: 7469 6f6e 2069 6e20 7365 7061 7261 746f  tion in separato
-00017530: 725f 6c69 7374 3a0d 0a20 2020 2020 2020  r_list:..       
-00017540: 206a 6f69 6e5f 6c65 6773 5f73 7472 696e   join_legs_strin
-00017550: 675f 696e 7075 7420 3d20 6a6f 696e 5f6c  g_input = join_l
-00017560: 6567 735f 7374 7269 6e67 5f69 6e70 7574  egs_string_input
-00017570: 2e72 6570 6c61 6365 2870 6172 7469 7469  .replace(partiti
-00017580: 6f6e 2c22 2928 2229 0d0a 2020 2020 6a6f  on,")(")..    jo
-00017590: 696e 5f6c 6567 735f 7374 7269 6e67 5f69  in_legs_string_i
-000175a0: 6e70 7574 203d 2022 2822 2b6a 6f69 6e5f  nput = "("+join_
-000175b0: 6c65 6773 5f73 7472 696e 675f 696e 7075  legs_string_inpu
-000175c0: 742b 2229 220d 0a0d 0a20 2020 2073 6861  t+")"....    sha
-000175d0: 7065 5f6c 6566 7420 203d 204f 626a 2e73  pe_left  = Obj.s
-000175e0: 6861 7065 5b3a 6e5f 6c65 6674 5d0d 0a20  hape[:n_left].. 
-000175f0: 2020 2073 7461 7473 5f6c 6566 7420 203d     stats_left  =
-00017600: 204f 626a 2e73 7461 7469 7374 6963 5b3a   Obj.statistic[:
-00017610: 6e5f 6c65 6674 5d0d 0a20 2020 2073 6861  n_left]..    sha
-00017620: 7065 5f72 6967 6874 203d 204f 626a 2e73  pe_right = Obj.s
-00017630: 6861 7065 5b6e 5f6c 6566 743a 5d0d 0a20  hape[n_left:].. 
-00017640: 2020 2073 7461 7473 5f72 6967 6874 203d     stats_right =
-00017650: 204f 626a 2e73 7461 7469 7374 6963 5b6e   Obj.statistic[n
-00017660: 5f6c 6566 743a 5d0d 0a0d 0a20 2020 2064  _left:]....    d
-00017670: 6566 207a 6572 6f5f 6f72 5f65 6c73 6528  ef zero_or_else(
-00017680: 7665 6374 6f72 2c76 616c 7565 293a 0d0a  vector,value):..
-00017690: 2020 2020 2020 2020 666f 7220 656c 656d          for elem
-000176a0: 2069 6e20 7665 6374 6f72 3a0d 0a20 2020   in vector:..   
-000176b0: 2020 2020 2020 2020 2069 6620 656c 656d           if elem
-000176c0: 213d 303a 0d0a 2020 2020 2020 2020 2020  !=0:..          
-000176d0: 2020 2020 2020 7265 7475 726e 2076 616c        return val
-000176e0: 7565 0d0a 2020 2020 2020 2020 7265 7475  ue..        retu
-000176f0: 726e 2030 0d0a 2020 2020 6465 6620 6765  rn 0..    def ge
-00017700: 745f 7374 6174 2876 6563 746f 722c 7072  t_stat(vector,pr
-00017710: 6566 6572 3d4e 6f6e 6529 3a0d 0a20 2020  efer=None):..   
-00017720: 2020 2020 2062 6f73 6f6e 5f63 6f75 6e74       boson_count
-00017730: 203d 2030 0d0a 2020 2020 2020 2020 6665   = 0..        fe
-00017740: 726d 695f 636f 756e 7420 3d20 300d 0a20  rmi_count = 0.. 
-00017750: 2020 2020 2020 2066 6f72 2065 6c65 6d20         for elem 
-00017760: 696e 2076 6563 746f 723a 0d0a 2020 2020  in vector:..    
-00017770: 2020 2020 2020 2020 6966 2065 6c65 6d20          if elem 
-00017780: 696e 2062 6f73 655f 7479 7065 203a 0d0a  in bose_type :..
-00017790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177a0: 626f 736f 6e5f 636f 756e 7420 2b3d 2031  boson_count += 1
-000177b0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000177c0: 2065 6c65 6d20 696e 2066 6572 6d69 5f74   elem in fermi_t
-000177d0: 7970 6520 3a0d 0a20 2020 2020 2020 2020  ype :..         
-000177e0: 2020 2020 2020 2066 6572 6d69 5f63 6f75         fermi_cou
-000177f0: 6e74 202b 3d20 310d 0a0d 0a20 2020 2020  nt += 1....     
-00017800: 2020 2069 6628 626f 736f 6e5f 636f 756e     if(boson_coun
-00017810: 743d 3d30 2061 6e64 2066 6572 6d69 5f63  t==0 and fermi_c
-00017820: 6f75 6e74 3e30 293a 0d0a 2020 2020 2020  ount>0):..      
-00017830: 2020 2020 2020 6966 2070 7265 6665 7220        if prefer 
-00017840: 213d 204e 6f6e 653a 0d0a 2020 2020 2020  != None:..      
-00017850: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00017860: 2070 7265 6665 720d 0a20 2020 2020 2020   prefer..       
-00017870: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00017880: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00017890: 726e 2031 0d0a 2020 2020 2020 2020 656c  rn 1..        el
-000178a0: 6966 2862 6f73 6f6e 5f63 6f75 6e74 3e30  if(boson_count>0
-000178b0: 2061 6e64 2066 6572 6d69 5f63 6f75 6e74   and fermi_count
-000178c0: 3d3d 3029 3a0d 0a20 2020 2020 2020 2020  ==0):..         
-000178d0: 2020 2069 6620 7072 6566 6572 2021 3d20     if prefer != 
-000178e0: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-000178f0: 2020 2020 2020 2072 6574 7572 6e20 7072         return pr
-00017900: 6566 6572 0d0a 2020 2020 2020 2020 2020  efer..          
-00017910: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00017920: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00017930: 300d 0a20 2020 2020 2020 2065 6c69 6628  0..        elif(
-00017940: 626f 736f 6e5f 636f 756e 743e 3020 616e  boson_count>0 an
-00017950: 6420 6665 726d 695f 636f 756e 743e 3029  d fermi_count>0)
-00017960: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00017970: 6574 7572 6e20 6879 6272 6964 5f73 796d  eturn hybrid_sym
-00017980: 626f 6c0d 0a20 2020 200d 0a20 2020 2073  bol..    ..    s
-00017990: 7465 7020 3d20 7368 6f77 5f70 726f 6772  tep = show_progr
-000179a0: 6573 7328 7374 6570 2c70 726f 6365 7373  ess(step,process
-000179b0: 5f6c 656e 6774 682c 7072 6f63 6573 735f  _length,process_
-000179c0: 6e61 6d65 2b22 2022 2b22 3c22 2b63 7572  name+" "+"<"+cur
-000179d0: 7265 6e74 5f6d 656d 6f72 795f 6469 7370  rent_memory_disp
-000179e0: 6c61 7928 292b 223e 222c 636f 6c6f 723d  lay()+">",color=
-000179f0: 7072 6f63 6573 735f 636f 6c6f 722c 7469  process_color,ti
-00017a00: 6d65 3d74 696d 652e 7469 6d65 2829 2d73  me=time.time()-s
-00017a10: 3030 2920 2332 0d0a 2020 2020 696e 7465  00) #2..    inte
-00017a20: 726d 6564 6961 7465 5f73 7461 7420 3d20  rmediate_stat = 
-00017a30: 2820 7a65 726f 5f6f 725f 656c 7365 2873  ( zero_or_else(s
-00017a40: 7461 7473 5f6c 6566 742c 2d31 292c 7a65  tats_left,-1),ze
-00017a50: 726f 5f6f 725f 656c 7365 2873 7461 7473  ro_or_else(stats
-00017a60: 5f72 6967 6874 2c31 2920 290d 0a20 2020  _right,1) )..   
-00017a70: 204f 626a 203d 204f 626a 2e6a 6f69 6e5f   Obj = Obj.join_
-00017a80: 6c65 6773 286a 6f69 6e5f 6c65 6773 5f73  legs(join_legs_s
-00017a90: 7472 696e 675f 696e 7075 742c 226d 6174  tring_input,"mat
-00017aa0: 7269 7822 2c69 6e74 6572 6d65 6469 6174  rix",intermediat
-00017ab0: 655f 7374 6174 3d69 6e74 6572 6d65 6469  e_stat=intermedi
-00017ac0: 6174 655f 7374 6174 2c73 6176 655f 6d65  ate_stat,save_me
-00017ad0: 6d6f 7279 3d54 7275 6529 0d0a 0d0a 2020  mory=True)....  
-00017ae0: 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a    #:::::::::::::
-00017af0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017b00: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017b10: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017b20: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017b30: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017b40: 3a3a 3a0d 0a20 2020 2023 3a3a 3a3a 3a20  :::..    #::::: 
-00017b50: 2020 2020 2053 5445 5020 3220 2d20 424c       STEP 2 - BL
-00017b60: 4f43 4b20 5356 4420 284d 414b 4520 5355  OCK SVD (MAKE SU
-00017b70: 5245 2049 5427 5320 5041 5249 5459 2d50  RE IT'S PARITY-P
-00017b80: 5245 5345 5256 494e 4721 2920 2020 2020  RESERVING!)     
-00017b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ba0: 2020 2020 203a 3a3a 3a3a 0d0a 2020 2020       :::::..    
-00017bb0: 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  #:::::::::::::::
-00017bc0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017bd0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017be0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017bf0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017c00: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017c10: 3a0d 0a0d 0a20 2020 2073 7465 7020 3d20  :....    step = 
-00017c20: 7368 6f77 5f70 726f 6772 6573 7328 7374  show_progress(st
-00017c30: 6570 2c70 726f 6365 7373 5f6c 656e 6774  ep,process_lengt
-00017c40: 682c 7072 6f63 6573 735f 6e61 6d65 2b22  h,process_name+"
-00017c50: 2022 2b22 3c22 2b63 7572 7265 6e74 5f6d   "+"<"+current_m
-00017c60: 656d 6f72 795f 6469 7370 6c61 7928 292b  emory_display()+
-00017c70: 223e 222c 636f 6c6f 723d 7072 6f63 6573  ">",color=proces
-00017c80: 735f 636f 6c6f 722c 7469 6d65 3d74 696d  s_color,time=tim
-00017c90: 652e 7469 6d65 2829 2d73 3030 2920 2333  e.time()-s00) #3
-00017ca0: 0d0a 2020 2020 6966 204f 626a 2e73 7461  ..    if Obj.sta
-00017cb0: 7469 7374 6963 5b30 5d3d 3d30 206f 7220  tistic[0]==0 or 
-00017cc0: 4f62 6a2e 7374 6174 6973 7469 635b 315d  Obj.statistic[1]
-00017cd0: 3d3d 303a 0d0a 2020 2020 2020 2020 552c  ==0:..        U,
-00017ce0: 20ce 9b2c 2056 203d 2053 6f72 7465 6445   .., V = SortedE
-00017cf0: 6967 284f 626a 2e64 6174 612c 6375 746f  ig(Obj.data,cuto
-00017d00: 6666 2c64 6562 7567 5f6d 6f64 6529 0d0a  ff,debug_mode)..
-00017d10: 2020 2020 2020 2020 ce9b 203d 206e 702e          .. = np.
-00017d20: 6469 6167 28ce 9b29 0d0a 2020 2020 656c  diag(..)..    el
-00017d30: 7365 3a0d 0a20 2020 2020 2020 2055 2c20  se:..        U, 
-00017d40: ce9b 2c20 5620 3d20 426c 6f63 6b45 6967  .., V = BlockEig
-00017d50: 284f 626a 2e64 6174 612c 6375 746f 6666  (Obj.data,cutoff
-00017d60: 2c64 6562 7567 5f6d 6f64 6529 0d0a 0d0a  ,debug_mode)....
-00017d70: 2020 2020 7374 6570 203d 2073 686f 775f      step = show_
-00017d80: 7072 6f67 7265 7373 2873 7465 702c 7072  progress(step,pr
-00017d90: 6f63 6573 735f 6c65 6e67 7468 2c70 726f  ocess_length,pro
-00017da0: 6365 7373 5f6e 616d 652b 2220 222b 223c  cess_name+" "+"<
-00017db0: 222b 6375 7272 656e 745f 6d65 6d6f 7279  "+current_memory
-00017dc0: 5f64 6973 706c 6179 2829 2b22 3e22 2c63  _display()+">",c
-00017dd0: 6f6c 6f72 3d70 726f 6365 7373 5f63 6f6c  olor=process_col
-00017de0: 6f72 2c74 696d 653d 7469 6d65 2e74 696d  or,time=time.tim
-00017df0: 6528 292d 7330 3029 2023 340d 0a20 2020  e()-s00) #4..   
-00017e00: 2023 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a   #::::::::::::::
-00017e10: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017e20: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017e30: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017e40: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017e50: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017e60: 3a3a 0d0a 2020 2020 233a 3a3a 3a3a 2020  ::..    #:::::  
-00017e70: 2020 2020 5354 4550 2033 202d 2052 4543      STEP 3 - REC
-00017e80: 4f4e 5354 5255 4354 2055 2c20 ce9b 2c20  ONSTRUCT U, .., 
-00017e90: 616e 6420 5620 4153 2047 5241 5353 4d41  and V AS GRASSMA
-00017ea0: 4e4e 2054 454e 534f 5253 2020 2020 2020  NN TENSORS      
-00017eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ec0: 2020 2020 203a 3a3a 3a3a 0d0a 2020 2020       :::::..    
-00017ed0: 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  #:::::::::::::::
-00017ee0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017ef0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017f00: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017f10: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017f20: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00017f30: 3a0d 0a0d 0a20 2020 2073 6b69 705f 706f  :....    skip_po
-00017f40: 7765 725f 6f66 5f74 776f 5f63 6865 636b  wer_of_two_check
-00017f50: 203d 2054 7275 650d 0a0d 0a20 2020 2023   = True....    #
-00017f60: 7468 6520 6669 7273 7420 7761 7920 6973  the first way is
-00017f70: 2074 6f20 666f 726d 2074 6865 2074 656e   to form the ten
-00017f80: 736f 7220 6669 7273 742c 2074 6865 6e20  sor first, then 
-00017f90: 7370 6c69 740d 0a20 2020 20ce 9b73 7461  split..    ..sta
-00017fa0: 746c 6566 7420 3d20 2d31 0d0a 2020 2020  tleft = -1..    
-00017fb0: ce9b 7374 6174 7269 6768 7420 3d20 2b31  ..statright = +1
-00017fc0: 0d0a 2020 2020 0d0a 2020 2020 6966 204f  ..    ..    if O
-00017fd0: 626a 2e73 7461 7469 7374 6963 5b30 5d3d  bj.statistic[0]=
-00017fe0: 3d30 3a0d 0a20 2020 2020 2020 2055 203d  =0:..        U =
-00017ff0: 2064 656e 7365 2855 2c65 6e63 6f64 6572   dense(U,encoder
-00018000: 3d22 7061 7269 7479 2d70 7265 7365 7276  ="parity-preserv
-00018010: 696e 6722 2c66 6f72 6d61 743d 226d 6174  ing",format="mat
-00018020: 7269 7822 2c73 7461 7469 7374 6963 3d28  rix",statistic=(
-00018030: 302c 3029 290d 0a20 2020 2020 2020 20ce  0,0))..        .
-00018040: 9b20 3d20 6465 6e73 6528 ce9b 2c65 6e63  . = dense(..,enc
-00018050: 6f64 6572 3d22 7061 7269 7479 2d70 7265  oder="parity-pre
-00018060: 7365 7276 696e 6722 2c66 6f72 6d61 743d  serving",format=
-00018070: 226d 6174 7269 7822 2c73 7461 7469 7374  "matrix",statist
-00018080: 6963 3d28 302c 3029 290d 0a20 2020 2020  ic=(0,0))..     
-00018090: 2020 2056 203d 2064 656e 7365 2856 2c65     V = dense(V,e
-000180a0: 6e63 6f64 6572 3d22 7061 7269 7479 2d70  ncoder="parity-p
-000180b0: 7265 7365 7276 696e 6722 2c66 6f72 6d61  reserving",forma
-000180c0: 743d 226d 6174 7269 7822 2c73 7461 7469  t="matrix",stati
-000180d0: 7374 6963 3d28 302c 4f62 6a2e 7374 6174  stic=(0,Obj.stat
-000180e0: 6973 7469 635b 315d 2929 0d0a 2020 2020  istic[1]))..    
-000180f0: 2020 2020 ce9b 7374 6174 6c65 6674 203d      ..statleft =
-00018100: 2030 0d0a 2020 2020 2020 2020 ce9b 7374   0..        ..st
-00018110: 6174 7269 6768 7420 3d20 300d 0a20 2020  atright = 0..   
-00018120: 2065 6c69 6620 4f62 6a2e 7374 6174 6973   elif Obj.statis
-00018130: 7469 635b 315d 3d3d 303a 0d0a 2020 2020  tic[1]==0:..    
-00018140: 2020 2020 5520 3d20 6465 6e73 6528 552c      U = dense(U,
-00018150: 656e 636f 6465 723d 2270 6172 6974 792d  encoder="parity-
-00018160: 7072 6573 6572 7669 6e67 222c 666f 726d  preserving",form
-00018170: 6174 3d22 6d61 7472 6978 222c 7374 6174  at="matrix",stat
-00018180: 6973 7469 633d 284f 626a 2e73 7461 7469  istic=(Obj.stati
-00018190: 7374 6963 5b30 5d2c 3029 290d 0a20 2020  stic[0],0))..   
-000181a0: 2020 2020 20ce 9b20 3d20 6465 6e73 6528       .. = dense(
-000181b0: ce9b 2c65 6e63 6f64 6572 3d22 7061 7269  ..,encoder="pari
-000181c0: 7479 2d70 7265 7365 7276 696e 6722 2c66  ty-preserving",f
-000181d0: 6f72 6d61 743d 226d 6174 7269 7822 2c73  ormat="matrix",s
-000181e0: 7461 7469 7374 6963 3d28 302c 3029 290d  tatistic=(0,0)).
-000181f0: 0a20 2020 2020 2020 2056 203d 2064 656e  .        V = den
-00018200: 7365 2856 2c65 6e63 6f64 6572 3d22 7061  se(V,encoder="pa
-00018210: 7269 7479 2d70 7265 7365 7276 696e 6722  rity-preserving"
-00018220: 2c66 6f72 6d61 743d 226d 6174 7269 7822  ,format="matrix"
-00018230: 2c73 7461 7469 7374 6963 3d28 302c 3029  ,statistic=(0,0)
-00018240: 290d 0a20 2020 2020 2020 20ce 9b73 7461  )..        ..sta
-00018250: 746c 6566 7420 3d20 300d 0a20 2020 2020  tleft = 0..     
-00018260: 2020 20ce 9b73 7461 7472 6967 6874 203d     ..statright =
-00018270: 2030 0d0a 2020 2020 656c 7365 3a0d 0a20   0..    else:.. 
-00018280: 2020 2020 2020 2055 203d 2064 656e 7365         U = dense
-00018290: 2855 2c65 6e63 6f64 6572 3d22 7061 7269  (U,encoder="pari
-000182a0: 7479 2d70 7265 7365 7276 696e 6722 2c66  ty-preserving",f
-000182b0: 6f72 6d61 743d 226d 6174 7269 7822 2c73  ormat="matrix",s
-000182c0: 7461 7469 7374 6963 3d28 4f62 6a2e 7374  tatistic=(Obj.st
-000182d0: 6174 6973 7469 635b 305d 2c31 2929 0d0a  atistic[0],1))..
-000182e0: 2020 2020 2020 2020 ce9b 203d 2064 656e          .. = den
-000182f0: 7365 28ce 9b2c 656e 636f 6465 723d 2270  se(..,encoder="p
-00018300: 6172 6974 792d 7072 6573 6572 7669 6e67  arity-preserving
-00018310: 222c 666f 726d 6174 3d22 6d61 7472 6978  ",format="matrix
-00018320: 222c 7374 6174 6973 7469 633d 282d 312c  ",statistic=(-1,
-00018330: 3129 290d 0a20 2020 2020 2020 2056 203d  1))..        V =
-00018340: 2064 656e 7365 2856 2c65 6e63 6f64 6572   dense(V,encoder
-00018350: 3d22 7061 7269 7479 2d70 7265 7365 7276  ="parity-preserv
-00018360: 696e 6722 2c66 6f72 6d61 743d 226d 6174  ing",format="mat
-00018370: 7269 7822 2c73 7461 7469 7374 6963 3d28  rix",statistic=(
-00018380: 2d31 2c4f 626a 2e73 7461 7469 7374 6963  -1,Obj.statistic
-00018390: 5b31 5d29 290d 0a20 2020 2064 ce9b 203d  [1]))..    d.. =
-000183a0: 20ce 9b2e 7368 6170 655b 305d 0d0a 0d0a   ...shape[0]....
-000183b0: 2020 2020 7374 6570 203d 2073 686f 775f      step = show_
-000183c0: 7072 6f67 7265 7373 2873 7465 702c 7072  progress(step,pr
-000183d0: 6f63 6573 735f 6c65 6e67 7468 2c70 726f  ocess_length,pro
-000183e0: 6365 7373 5f6e 616d 652b 2220 222b 223c  cess_name+" "+"<
-000183f0: 222b 6375 7272 656e 745f 6d65 6d6f 7279  "+current_memory
-00018400: 5f64 6973 706c 6179 2829 2b22 3e22 2c63  _display()+">",c
-00018410: 6f6c 6f72 3d70 726f 6365 7373 5f63 6f6c  olor=process_col
-00018420: 6f72 2c74 696d 653d 7469 6d65 2e74 696d  or,time=time.tim
-00018430: 6528 292d 7330 3029 2023 350d 0a20 2020  e()-s00) #5..   
-00018440: 2073 6b69 705f 706f 7765 725f 6f66 5f74   skip_power_of_t
-00018450: 776f 5f63 6865 636b 203d 2046 616c 7365  wo_check = False
-00018460: 0d0a 2020 2020 233a 3a3a 3a3a 3a3a 3a3a  ..    #:::::::::
-00018470: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00018480: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00018490: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000184a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000184b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-000184c0: 3a3a 3a3a 3a3a 3a0d 0a20 2020 2023 3a3a  :::::::..    #::
-000184d0: 3a3a 3a20 2020 2020 2053 5445 5020 3420  :::      STEP 4 
-000184e0: 2d20 5370 6c69 7420 7468 6520 6c65 6773  - Split the legs
-000184f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018520: 2020 2020 2020 2020 203a 3a3a 3a3a 0d0a           :::::..
-00018530: 2020 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a      #:::::::::::
-00018540: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00018550: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00018560: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00018570: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00018580: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00018590: 3a3a 3a3a 3a0d 0a0d 0a20 2020 2023 2063  :::::....    # c
-000185a0: 6f75 6e74 2074 6865 206e 756d 6265 7220  ount the number 
-000185b0: 6f66 2069 6e64 6963 6573 2069 6e20 7468  of indices in th
-000185c0: 6520 7477 6f20 6772 6f75 7073 0d0a 2020  e two groups..  
-000185d0: 2020 5569 6e64 203d 2022 220d 0a20 2020    Uind = ""..   
-000185e0: 2056 696e 6420 3d20 2222 0d0a 2020 2020   Vind = ""..    
-000185f0: 5573 7461 7473 203d 205b 5d0d 0a20 2020  Ustats = []..   
-00018600: 2056 7374 6174 7320 3d20 5b5d 0d0a 2020   Vstats = []..  
-00018610: 2020 5573 6861 7065 203d 205b 5d0d 0a20    Ushape = [].. 
-00018620: 2020 2056 7368 6170 6520 3d20 5b5d 0d0a     Vshape = []..
-00018630: 2020 2020 7061 7274 6974 696f 6e5f 666f      partition_fo
-00018640: 756e 6420 3d20 4661 6c73 650d 0a20 2020  und = False..   
-00018650: 2066 6f72 2069 2c63 6861 7220 696e 2065   for i,char in e
-00018660: 6e75 6d65 7261 7465 2873 7472 696e 6729  numerate(string)
-00018670: 3a0d 0a20 2020 2020 2020 2069 6620 6368  :..        if ch
-00018680: 6172 2069 6e20 7365 7061 7261 746f 725f  ar in separator_
-00018690: 6c69 7374 203a 0d0a 2020 2020 2020 2020  list :..        
-000186a0: 2020 2020 7061 7274 6974 696f 6e5f 666f      partition_fo
-000186b0: 756e 6420 3d20 5472 7565 0d0a 2020 2020  und = True..    
-000186c0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-000186d0: 0d0a 2020 2020 2020 2020 6966 2870 6172  ..        if(par
-000186e0: 7469 7469 6f6e 5f66 6f75 6e64 293a 0d0a  tition_found):..
-000186f0: 2020 2020 2020 2020 2020 2020 5669 6e64              Vind
-00018700: 2b3d 6368 6172 0d0a 2020 2020 2020 2020  +=char..        
-00018710: 2020 2020 5673 7461 7473 2b3d 5b58 4f62      Vstats+=[XOb
-00018720: 6a5f 7374 6174 735b 692d 315d 5d0d 0a20  j_stats[i-1]].. 
-00018730: 2020 2020 2020 2020 2020 2056 7368 6170             Vshap
-00018740: 652b 3d5b 584f 626a 5f73 6861 7065 5b69  e+=[XObj_shape[i
-00018750: 2d31 5d5d 0d0a 2020 2020 2020 2020 656c  -1]]..        el
-00018760: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00018770: 2055 696e 642b 3d63 6861 720d 0a20 2020   Uind+=char..   
-00018780: 2020 2020 2020 2020 2055 7374 6174 732b           Ustats+
-00018790: 3d5b 584f 626a 5f73 7461 7473 5b69 5d5d  =[XObj_stats[i]]
-000187a0: 0d0a 2020 2020 2020 2020 2020 2020 5573  ..            Us
-000187b0: 6861 7065 2b3d 5b58 4f62 6a5f 7368 6170  hape+=[XObj_shap
-000187c0: 655b 695d 5d0d 0a0d 0a20 2020 206e 6577  e[i]]....    new
-000187d0: 5f69 6e64 3120 3d20 2222 0d0a 2020 2020  _ind1 = ""..    
-000187e0: 666f 7220 6368 6172 2069 6e20 6368 6172  for char in char
-000187f0: 5f6c 6973 743a 0d0a 2020 2020 2020 2020  _list:..        
-00018800: 6966 2063 6861 7220 6e6f 7420 696e 2055  if char not in U
-00018810: 696e 642b 5669 6e64 3a0d 0a20 2020 2020  ind+Vind:..     
-00018820: 2020 2020 2020 206e 6577 5f69 6e64 3120         new_ind1 
-00018830: 3d20 6368 6172 0d0a 2020 2020 2020 2020  = char..        
-00018840: 2020 2020 6272 6561 6b0d 0a0d 0a20 2020      break....   
-00018850: 2055 696e 6420 2020 3d20 2228 222b 5569   Uind   = "("+Ui
-00018860: 6e64 2b22 2922 202b 206e 6577 5f69 6e64  nd+")" + new_ind
-00018870: 310d 0a20 2020 2056 696e 6420 2020 3d20  1..    Vind   = 
-00018880: 6e65 775f 696e 6431 202b 2022 2822 2b56  new_ind1 + "("+V
-00018890: 696e 642b 2229 220d 0a20 2020 2055 7374  ind+")"..    Ust
-000188a0: 6174 7320 3d20 7475 706c 6528 5573 7461  ats = tuple(Usta
-000188b0: 7473 202b 205b 2dce 9b73 7461 746c 6566  ts + [-..statlef
-000188c0: 745d 290d 0a20 2020 2056 7374 6174 7320  t])..    Vstats 
-000188d0: 3d20 7475 706c 6528 5b2d ce9b 7374 6174  = tuple([-..stat
-000188e0: 7269 6768 745d 202b 2056 7374 6174 7329  right] + Vstats)
-000188f0: 0d0a 2020 2020 5573 6861 7065 203d 2074  ..    Ushape = t
-00018900: 7570 6c65 2855 7368 6170 6520 2b20 5b64  uple(Ushape + [d
-00018910: ce9b 5d29 0d0a 2020 2020 5673 6861 7065  ..])..    Vshape
-00018920: 203d 2074 7570 6c65 285b 64ce 9b5d 202b   = tuple([d..] +
-00018930: 2056 7368 6170 6529 0d0a 2020 2020 0d0a   Vshape)..    ..
-00018940: 2020 2020 7374 6570 203d 2073 686f 775f      step = show_
-00018950: 7072 6f67 7265 7373 2873 7465 702c 7072  progress(step,pr
-00018960: 6f63 6573 735f 6c65 6e67 7468 2c70 726f  ocess_length,pro
-00018970: 6365 7373 5f6e 616d 652b 2220 222b 223c  cess_name+" "+"<
-00018980: 222b 6375 7272 656e 745f 6d65 6d6f 7279  "+current_memory
-00018990: 5f64 6973 706c 6179 2829 2b22 3e22 2c63  _display()+">",c
-000189a0: 6f6c 6f72 3d70 726f 6365 7373 5f63 6f6c  olor=process_col
-000189b0: 6f72 2c74 696d 653d 7469 6d65 2e74 696d  or,time=time.tim
-000189c0: 6528 292d 7330 3029 2023 360d 0a20 2020  e()-s00) #6..   
-000189d0: 2055 203d 2055 2e73 706c 6974 5f6c 6567   U = U.split_leg
-000189e0: 7328 5569 6e64 2c55 7374 6174 732c 5573  s(Uind,Ustats,Us
-000189f0: 6861 7065 2c73 6176 655f 6d65 6d6f 7279  hape,save_memory
-00018a00: 3d54 7275 6529 0d0a 2020 2020 ce9b 203d  =True)..    .. =
-00018a10: 20ce 9b2e 7377 6974 6368 5f65 6e63 6f64   ...switch_encod
-00018a20: 6572 2873 6176 655f 6d65 6d6f 7279 3d54  er(save_memory=T
-00018a30: 7275 6529 0d0a 2020 2020 5620 3d20 562e  rue)..    V = V.
-00018a40: 7370 6c69 745f 6c65 6773 2856 696e 642c  split_legs(Vind,
-00018a50: 5673 7461 7473 2c56 7368 6170 652c 7361  Vstats,Vshape,sa
-00018a60: 7665 5f6d 656d 6f72 793d 5472 7565 290d  ve_memory=True).
-00018a70: 0a20 2020 200d 0a20 2020 2069 6628 7468  .    ..    if(th
-00018a80: 6973 5f66 6f72 6d61 7420 3d3d 2027 7374  is_format == 'st
-00018a90: 616e 6461 7264 2729 3a0d 0a20 2020 2020  andard'):..     
-00018aa0: 2020 2055 203d 2055 2e73 7769 7463 685f     U = U.switch_
-00018ab0: 666f 726d 6174 2873 6176 655f 6d65 6d6f  format(save_memo
-00018ac0: 7279 3d54 7275 6529 0d0a 2020 2020 2020  ry=True)..      
-00018ad0: 2020 ce9b 203d 20ce 9b2e 7377 6974 6368    .. = ...switch
-00018ae0: 5f66 6f72 6d61 7428 7361 7665 5f6d 656d  _format(save_mem
-00018af0: 6f72 793d 5472 7565 290d 0a20 2020 2020  ory=True)..     
-00018b00: 2020 2056 203d 2056 2e73 7769 7463 685f     V = V.switch_
-00018b10: 666f 726d 6174 2873 6176 655f 6d65 6d6f  format(save_memo
-00018b20: 7279 3d54 7275 6529 0d0a 0d0a 2020 2020  ry=True)....    
-00018b30: 6966 2874 6869 735f 656e 636f 6465 7220  if(this_encoder 
-00018b40: 3d3d 2027 7061 7269 7479 2d70 7265 7365  == 'parity-prese
-00018b50: 7276 696e 6727 293a 0d0a 2020 2020 2020  rving'):..      
-00018b60: 2020 5520 3d20 552e 7377 6974 6368 5f65    U = U.switch_e
-00018b70: 6e63 6f64 6572 2873 6176 655f 6d65 6d6f  ncoder(save_memo
-00018b80: 7279 3d54 7275 6529 0d0a 2020 2020 2020  ry=True)..      
-00018b90: 2020 ce9b 203d 20ce 9b2e 7377 6974 6368    .. = ...switch
-00018ba0: 5f65 6e63 6f64 6572 2873 6176 655f 6d65  _encoder(save_me
-00018bb0: 6d6f 7279 3d54 7275 6529 0d0a 2020 2020  mory=True)..    
-00018bc0: 2020 2020 5620 3d20 562e 7377 6974 6368      V = V.switch
-00018bd0: 5f65 6e63 6f64 6572 2873 6176 655f 6d65  _encoder(save_me
-00018be0: 6d6f 7279 3d54 7275 6529 0d0a 0d0a 2020  mory=True)....  
-00018bf0: 2020 6966 2874 6869 735f 7479 7065 3d3d    if(this_type==
-00018c00: 7370 6172 7365 293a 0d0a 2020 2020 2020  sparse):..      
-00018c10: 2020 5520 3d20 7370 6172 7365 2855 290d    U = sparse(U).
-00018c20: 0a20 2020 2020 2020 20ce 9b20 3d20 7370  .        .. = sp
-00018c30: 6172 7365 28ce 9b29 0d0a 2020 2020 2020  arse(..)..      
-00018c40: 2020 5620 3d20 7370 6172 7365 2856 290d    V = sparse(V).
-00018c50: 0a0d 0a20 2020 2063 6c65 6172 5f70 726f  ...    clear_pro
-00018c60: 6772 6573 7328 290d 0a20 2020 2073 7973  gress()..    sys
-00018c70: 2e73 7464 6f75 742e 7772 6974 6528 225c  .stdout.write("\
-00018c80: 3033 335b 4622 290d 0a20 2020 200d 0a20  033[F")..    .. 
-00018c90: 2020 2072 6574 7572 6e20 552c 20ce 9b2c     return U, ..,
-00018ca0: 2056 0d0a 0d0a 2323 2323 2323 2323 2323   V....##########
-00018cb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018cc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018cd0: 2323 2323 2323 2323 2323 0d0a 2323 2020  ##########..##  
-00018ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cf0: 2043 6f6e 6a75 6761 7469 6f6e 2020 2020   Conjugation    
-00018d00: 2020 2020 2020 2020 2020 2020 2020 2323                ##
-00018d10: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
-00018d20: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018d30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018d40: 2323 2323 2323 0d0a 0d0a 6465 6620 6863  ######....def hc
-00018d50: 6f6e 6a75 6761 7465 2849 6e70 4f62 6a2c  onjugate(InpObj,
-00018d60: 7374 7269 6e67 2c73 6176 655f 6d65 6d6f  string,save_memo
-00018d70: 7279 3d46 616c 7365 293a 0d0a 0d0a 2020  ry=False):....  
-00018d80: 2020 7072 6f63 6573 735f 6e61 6d65 203d    process_name =
-00018d90: 2022 6863 6f6e 6a75 6761 7465 220d 0a20   "hconjugate".. 
-00018da0: 2020 2070 726f 6365 7373 5f6c 656e 6774     process_lengt
-00018db0: 6820 3d20 360d 0a20 2020 2070 726f 6365  h = 6..    proce
-00018dc0: 7373 5f63 6f6c 6f72 3d22 7965 6c6c 6f77  ss_color="yellow
-00018dd0: 220d 0a20 2020 2073 7465 7020 3d20 310d  "..    step = 1.
-00018de0: 0a20 2020 2073 3030 203d 2074 696d 652e  .    s00 = time.
-00018df0: 7469 6d65 2829 0d0a 2020 2020 7072 696e  time()..    prin
-00018e00: 7428 2920 2320 3c3c 2044 6f6e 2774 2072  t() # << Don't r
-00018e10: 656d 6f76 6520 7468 6973 2e20 5468 6973  emove this. This
-00018e20: 2069 7320 666f 7220 7468 6520 7368 6f77   is for the show
-00018e30: 5f70 726f 6772 6573 7321 0d0a 0d0a 2020  _progress!....  
-00018e40: 2020 7374 7269 6e67 203d 2064 656e 756d    string = denum
-00018e50: 6572 6174 6528 7374 7269 6e67 290d 0a20  erate(string).. 
-00018e60: 2020 200d 0a20 2020 2069 6620 7374 7269     ..    if stri
-00018e70: 6e67 2e63 6f75 6e74 2822 2822 293d 3d73  ng.count("(")==s
-00018e80: 7472 696e 672e 636f 756e 7428 2229 2229  tring.count(")")
-00018e90: 2061 6e64 2073 7472 696e 672e 636f 756e   and string.coun
-00018ea0: 7428 2228 2229 3e30 3a0d 0a20 2020 2020  t("(")>0:..     
-00018eb0: 2020 2073 7472 696e 6720 3d20 7374 7269     string = stri
-00018ec0: 6e67 2e72 6570 6c61 6365 2822 2022 2c22  ng.replace(" ","
-00018ed0: 2229 0d0a 2020 2020 2020 2020 7374 7269  ")..        stri
-00018ee0: 6e67 203d 2073 7472 696e 672e 7265 706c  ng = string.repl
-00018ef0: 6163 6528 2229 2822 2c22 2022 290d 0a20  ace(")("," ").. 
-00018f00: 2020 2020 2020 2069 6620 7374 7269 6e67         if string
-00018f10: 2e63 6f75 6e74 2822 2822 293e 3120 6f72  .count("(")>1 or
-00018f20: 2073 7472 696e 672e 636f 756e 7428 2229   string.count(")
-00018f30: 2229 3c31 3a0d 0a20 2020 2020 2020 2020  ")<1:..         
-00018f40: 2020 2065 7272 6f72 2822 4572 726f 725b     error("Error[
-00018f50: 6863 6f6e 6a75 6761 7465 5d3a 2050 6172  hconjugate]: Par
-00018f60: 656e 7468 6573 6573 2064 6f6e 2774 206d  entheses don't m
-00018f70: 6174 6368 2229 0d0a 2020 2020 2020 2020  atch")..        
-00018f80: 7374 7269 6e67 203d 2073 7472 696e 672e  string = string.
-00018f90: 7265 706c 6163 6528 2229 222c 2222 290d  replace(")","").
-00018fa0: 0a20 2020 2020 2020 2073 7472 696e 6720  .        string 
-00018fb0: 3d20 7374 7269 6e67 2e72 6570 6c61 6365  = string.replace
-00018fc0: 2822 2822 2c22 2229 0d0a 0d0a 0d0a 2020  ("(","")......  
-00018fd0: 2020 2320 7468 6520 7374 7269 6e67 2069    # the string i
-00018fe0: 7320 6f66 2074 6865 2066 6f72 6d20 6161  s of the form aa
-00018ff0: 6161 7c62 6262 0d0a 0d0a 2020 2020 4f62  aa|bbb....    Ob
-00019000: 6a20 3d20 496e 704f 626a 2e63 6f70 7928  j = InpObj.copy(
-00019010: 290d 0a20 2020 2074 6869 735f 7479 7065  )..    this_type
-00019020: 203d 2074 7970 6528 4f62 6a29 0d0a 2020   = type(Obj)..  
-00019030: 2020 7468 6973 5f66 6f72 6d61 7420 3d20    this_format = 
-00019040: 4f62 6a2e 666f 726d 6174 0d0a 2020 2020  Obj.format..    
-00019050: 7468 6973 5f65 6e63 6f64 6572 203d 204f  this_encoder = O
-00019060: 626a 2e65 6e63 6f64 6572 0d0a 2020 2020  bj.encoder..    
-00019070: 584f 626a 5f73 7461 7473 203d 204f 626a  XObj_stats = Obj
-00019080: 2e73 7461 7469 7374 6963 0d0a 2020 2020  .statistic..    
-00019090: 584f 626a 5f73 6861 7065 203d 204f 626a  XObj_shape = Obj
-000190a0: 2e73 6861 7065 0d0a 0d0a 2020 2020 6966  .shape....    if
-000190b0: 2073 6176 655f 6d65 6d6f 7279 203a 0d0a   save_memory :..
-000190c0: 2020 2020 2020 2020 6465 6c20 496e 704f          del InpO
-000190d0: 626a 2e64 6174 610d 0a20 2020 2020 2020  bj.data..       
-000190e0: 2064 656c 2049 6e70 4f62 6a0d 0a20 2020   del InpObj..   
-000190f0: 2020 2020 2067 632e 636f 6c6c 6563 7428       gc.collect(
-00019100: 290d 0a0d 0a20 2020 2023 6966 2074 6869  )....    #if thi
-00019110: 735f 7479 7065 3d3d 7370 6172 7365 203a  s_type==sparse :
-00019120: 0d0a 2020 2020 2320 2020 204f 626a 203d  ..    #    Obj =
-00019130: 2064 656e 7365 284f 626a 290d 0a20 2020   dense(Obj)..   
-00019140: 2069 6620 7468 6973 5f74 7970 6520 6e6f   if this_type no
-00019150: 7420 696e 205b 6465 6e73 652c 7370 6172  t in [dense,spar
-00019160: 7365 5d20 3a0d 0a20 2020 2020 2020 2065  se] :..        e
-00019170: 7272 6f72 2822 4572 726f 725b 6863 6f6e  rror("Error[hcon
-00019180: 6a75 6761 7465 5d3a 204f 626a 6563 7420  jugate]: Object 
-00019190: 7479 7065 206d 7573 7420 6f6e 6c79 2062  type must only b
-000191a0: 6520 6465 6e73 6520 6f72 2073 7061 7273  e dense or spars
-000191b0: 6521 2229 0d0a 2020 2020 2020 2020 0d0a  e!")..        ..
-000191c0: 2020 2020 2320 6368 6563 6b20 6966 204f      # check if O
-000191d0: 626a 2e73 7461 7469 7374 6963 206f 7220  bj.statistic or 
-000191e0: 6669 6e61 6c5f 7374 6174 6973 7469 6320  final_statistic 
-000191f0: 6973 2077 6569 7264 206f 7220 6e6f 740d  is weird or not.
-00019200: 0a20 2020 2066 6f72 2073 7461 7420 696e  .    for stat in
-00019210: 204f 626a 2e73 7461 7469 7374 6963 3a0d   Obj.statistic:.
-00019220: 0a20 2020 2020 2020 2069 6628 7374 6174  .        if(stat
-00019230: 206e 6f74 2069 6e20 616c 6c6f 7765 645f   not in allowed_
-00019240: 7374 6174 293a 0d0a 2020 2020 2020 2020  stat):..        
-00019250: 2020 2020 6572 726f 7228 2245 7272 6f72      error("Error
-00019260: 5b68 636f 6e6a 7567 6174 655d 3a20 5468  [hconjugate]: Th
-00019270: 6520 696e 7075 7420 6f62 6a65 6374 2063  e input object c
-00019280: 6f6e 7461 696e 7320 696c 6c65 6761 6c20  ontains illegal 
-00019290: 7374 6174 6973 7469 632e 2028 302c 2031  statistic. (0, 1
-000192a0: 2c20 2d31 2c20 6f72 2022 2b68 7962 7269  , -1, or "+hybri
-000192b0: 645f 7379 6d62 6f6c 2b22 206f 6e6c 7929  d_symbol+" only)
-000192c0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-000192d0: 0d0a 2020 2020 7061 7274 6974 696f 6e5f  ..    partition_
-000192e0: 636f 756e 7420 3d20 300d 0a20 2020 2066  count = 0..    f
-000192f0: 6f72 2070 6172 7469 7469 6f6e 2069 6e20  or partition in 
-00019300: 7365 7061 7261 746f 725f 6c69 7374 3a0d  separator_list:.
-00019310: 0a20 2020 2020 2020 2070 6172 7469 7469  .        partiti
-00019320: 6f6e 5f63 6f75 6e74 202b 3d20 7374 7269  on_count += stri
-00019330: 6e67 2e63 6f75 6e74 2870 6172 7469 7469  ng.count(partiti
-00019340: 6f6e 290d 0a20 2020 2069 6628 7061 7274  on)..    if(part
-00019350: 6974 696f 6e5f 636f 756e 7421 3d31 293a  ition_count!=1):
-00019360: 0d0a 2020 2020 2020 2020 7061 7274 6974  ..        partit
-00019370: 696f 6e5f 7374 7269 6e67 203d 2022 220d  ion_string = "".
-00019380: 0a20 2020 2020 2020 2066 6f72 2069 2c20  .        for i, 
-00019390: 7061 7274 6974 696f 6e20 696e 2065 6e75  partition in enu
-000193a0: 6d65 7261 7465 2873 6570 6172 6174 6f72  merate(separator
-000193b0: 5f6c 6973 7429 3a0d 0a20 2020 2020 2020  _list):..       
-000193c0: 2020 2020 2069 6628 693d 3d30 293a 0d0a       if(i==0):..
-000193d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193e0: 7061 7274 6974 696f 6e5f 7374 7269 6e67  partition_string
-000193f0: 202b 3d20 2228 2022 0d0a 2020 2020 2020   += "( "..      
-00019400: 2020 2020 2020 656c 6966 2869 3d3d 6c65        elif(i==le
-00019410: 6e28 7365 7061 7261 746f 725f 6c69 7374  n(separator_list
-00019420: 292d 3129 3a0d 0a20 2020 2020 2020 2020  )-1):..         
-00019430: 2020 2020 2020 2070 6172 7469 7469 6f6e         partition
-00019440: 5f73 7472 696e 6720 2b3d 2022 2c20 6f72  _string += ", or
-00019450: 2022 0d0a 2020 2020 2020 2020 2020 2020   "..            
-00019460: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00019470: 2020 2020 2020 2070 6172 7469 7469 6f6e         partition
-00019480: 5f73 7472 696e 6720 2b3d 2022 2c20 220d  _string += ", ".
-00019490: 0a0d 0a20 2020 2020 2020 2020 2020 2070  ...            p
-000194a0: 6172 7469 7469 6f6e 5f73 7472 696e 6720  artition_string 
-000194b0: 2b3d 2022 2722 2b70 6172 7469 7469 6f6e  += "'"+partition
-000194c0: 2b22 2722 0d0a 0d0a 2020 2020 2020 2020  +"'"....        
-000194d0: 2020 2020 6966 2869 3d3d 6c65 6e28 7365      if(i==len(se
-000194e0: 7061 7261 746f 725f 6c69 7374 292d 3129  parator_list)-1)
-000194f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00019500: 2020 2070 6172 7469 7469 6f6e 5f73 7472     partition_str
-00019510: 696e 6720 2b3d 2022 2029 220d 0a0d 0a20  ing += " )".... 
-00019520: 2020 2020 2020 2065 7272 6f72 2822 4572         error("Er
-00019530: 726f 725b 6863 6f6e 6a75 6761 7465 5d3a  ror[hconjugate]:
-00019540: 2054 6865 2069 6e70 7574 2073 7472 696e   The input strin
-00019550: 6720 6d75 7374 2063 6f6e 7461 696e 206f  g must contain o
-00019560: 6e65 2061 6e64 206f 6e6c 7920 6f6e 6520  ne and only one 
-00019570: 7061 7274 6974 696f 6e20 222b 7061 7274  partition "+part
-00019580: 6974 696f 6e5f 7374 7269 6e67 2b22 2069  ition_string+" i
-00019590: 6e20 6974 2e22 290d 0a20 2020 200d 0a20  n it.")..    .. 
-000195a0: 2020 2073 7465 7020 3d20 7368 6f77 5f70     step = show_p
-000195b0: 726f 6772 6573 7328 7374 6570 2c70 726f  rogress(step,pro
-000195c0: 6365 7373 5f6c 656e 6774 682c 7072 6f63  cess_length,proc
-000195d0: 6573 735f 6e61 6d65 2b22 2022 2b22 3c22  ess_name+" "+"<"
-000195e0: 2b63 7572 7265 6e74 5f6d 656d 6f72 795f  +current_memory_
-000195f0: 6469 7370 6c61 7928 292b 223e 222c 636f  display()+">",co
-00019600: 6c6f 723d 7072 6f63 6573 735f 636f 6c6f  lor=process_colo
-00019610: 722c 7469 6d65 3d74 696d 652e 7469 6d65  r,time=time.time
-00019620: 2829 2d73 3030 290d 0a20 2020 2023 3a3a  ()-s00)..    #::
-00019630: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019640: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019650: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019660: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019670: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019680: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a  ::::::::::::::..
-00019690: 2020 2020 233a 3a3a 3a3a 2020 2020 2020      #:::::      
-000196a0: 5354 4550 2031 202d 204a 4f49 4e20 4c45  STEP 1 - JOIN LE
-000196b0: 4753 2042 4145 5344 204f 4e20 5448 4520  GS BAESD ON THE 
-000196c0: 4752 4f55 5049 4e47 5320 2020 2020 2020  GROUPINGS       
-000196d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196f0: 3a3a 3a3a 3a0d 0a20 2020 2023 3a3a 3a3a  :::::..    #::::
-00019700: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019710: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019720: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019730: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019740: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019750: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a 0d0a  ::::::::::::....
-00019760: 2020 2020 2320 636f 756e 7420 7468 6520      # count the 
-00019770: 6e75 6d62 6572 206f 6620 696e 6469 6365  number of indice
-00019780: 7320 696e 2074 6865 2074 776f 2067 726f  s in the two gro
-00019790: 7570 730d 0a20 2020 206e 5f6c 6566 7420  ups..    n_left 
-000197a0: 3d20 300d 0a20 2020 206e 5f72 6967 6874  = 0..    n_right
-000197b0: 203d 2030 0d0a 2020 2020 7061 7274 6974   = 0..    partit
-000197c0: 696f 6e5f 666f 756e 6420 3d20 4661 6c73  ion_found = Fals
-000197d0: 650d 0a20 2020 2066 6f72 2063 6861 7220  e..    for char 
-000197e0: 696e 2073 7472 696e 673a 0d0a 2020 2020  in string:..    
-000197f0: 2020 2020 6966 2063 6861 7220 696e 2073      if char in s
-00019800: 6570 6172 6174 6f72 5f6c 6973 7420 3a0d  eparator_list :.
-00019810: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-00019820: 7469 7469 6f6e 5f66 6f75 6e64 203d 2054  tition_found = T
-00019830: 7275 650d 0a20 2020 2020 2020 2020 2020  rue..           
-00019840: 2063 6f6e 7469 6e75 650d 0a20 2020 2020   continue..     
-00019850: 2020 2069 6628 7061 7274 6974 696f 6e5f     if(partition_
-00019860: 666f 756e 6429 3a0d 0a20 2020 2020 2020  found):..       
-00019870: 2020 2020 206e 5f72 6967 6874 2b3d 310d       n_right+=1.
-00019880: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00019890: 2020 2020 2020 2020 2020 2020 6e5f 6c65              n_le
-000198a0: 6674 2b3d 310d 0a0d 0a20 2020 206a 6f69  ft+=1....    joi
-000198b0: 6e5f 6c65 6773 5f73 7472 696e 675f 696e  n_legs_string_in
-000198c0: 7075 7420 3d20 7374 7269 6e67 0d0a 2020  put = string..  
-000198d0: 2020 666f 7220 7061 7274 6974 696f 6e20    for partition 
-000198e0: 696e 2073 6570 6172 6174 6f72 5f6c 6973  in separator_lis
-000198f0: 743a 0d0a 2020 2020 2020 2020 6a6f 696e  t:..        join
-00019900: 5f6c 6567 735f 7374 7269 6e67 5f69 6e70  _legs_string_inp
-00019910: 7574 203d 206a 6f69 6e5f 6c65 6773 5f73  ut = join_legs_s
-00019920: 7472 696e 675f 696e 7075 742e 7265 706c  tring_input.repl
-00019930: 6163 6528 7061 7274 6974 696f 6e2c 2229  ace(partition,")
-00019940: 2822 290d 0a20 2020 206a 6f69 6e5f 6c65  (")..    join_le
-00019950: 6773 5f73 7472 696e 675f 696e 7075 7420  gs_string_input 
-00019960: 3d20 2228 222b 6a6f 696e 5f6c 6567 735f  = "("+join_legs_
-00019970: 7374 7269 6e67 5f69 6e70 7574 2b22 2922  string_input+")"
-00019980: 0d0a 0d0a 2020 2020 7368 6170 655f 6c65  ....    shape_le
-00019990: 6674 2020 3d20 4f62 6a2e 7368 6170 655b  ft  = Obj.shape[
-000199a0: 3a6e 5f6c 6566 745d 0d0a 2020 2020 7374  :n_left]..    st
-000199b0: 6174 735f 6c65 6674 2020 3d20 4f62 6a2e  ats_left  = Obj.
-000199c0: 7374 6174 6973 7469 635b 3a6e 5f6c 6566  statistic[:n_lef
-000199d0: 745d 0d0a 2020 2020 7368 6170 655f 7269  t]..    shape_ri
-000199e0: 6768 7420 3d20 4f62 6a2e 7368 6170 655b  ght = Obj.shape[
-000199f0: 6e5f 6c65 6674 3a5d 0d0a 2020 2020 7374  n_left:]..    st
-00019a00: 6174 735f 7269 6768 7420 3d20 4f62 6a2e  ats_right = Obj.
-00019a10: 7374 6174 6973 7469 635b 6e5f 6c65 6674  statistic[n_left
-00019a20: 3a5d 0d0a 2020 2020 6465 6620 7072 6f64  :]..    def prod
-00019a30: 2876 6563 746f 7229 3a0d 0a20 2020 2020  (vector):..     
-00019a40: 2020 2072 6574 203d 2031 0d0a 2020 2020     ret = 1..    
-00019a50: 2020 2020 666f 7220 656c 656d 2069 6e20      for elem in 
-00019a60: 7665 6374 6f72 3a0d 0a20 2020 2020 2020  vector:..       
-00019a70: 2020 2020 2072 6574 202a 3d20 656c 656d       ret *= elem
-00019a80: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00019a90: 2072 6574 0d0a 2020 2020 6465 6620 6765   ret..    def ge
-00019aa0: 745f 7374 6174 2876 6563 746f 722c 7072  t_stat(vector,pr
-00019ab0: 6566 6572 3d4e 6f6e 6529 3a0d 0a20 2020  efer=None):..   
-00019ac0: 2020 2020 2062 6f73 6f6e 5f63 6f75 6e74       boson_count
-00019ad0: 203d 2030 0d0a 2020 2020 2020 2020 6665   = 0..        fe
-00019ae0: 726d 695f 636f 756e 7420 3d20 300d 0a20  rmi_count = 0.. 
-00019af0: 2020 2020 2020 2066 6f72 2065 6c65 6d20         for elem 
-00019b00: 696e 2076 6563 746f 723a 0d0a 2020 2020  in vector:..    
-00019b10: 2020 2020 2020 2020 6966 2065 6c65 6d20          if elem 
-00019b20: 696e 2062 6f73 655f 7479 7065 203a 0d0a  in bose_type :..
-00019b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b40: 626f 736f 6e5f 636f 756e 7420 2b3d 2031  boson_count += 1
-00019b50: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00019b60: 2065 6c65 6d20 696e 2066 6572 6d69 5f74   elem in fermi_t
-00019b70: 7970 6520 3a0d 0a20 2020 2020 2020 2020  ype :..         
-00019b80: 2020 2020 2020 2066 6572 6d69 5f63 6f75         fermi_cou
-00019b90: 6e74 202b 3d20 310d 0a0d 0a20 2020 2020  nt += 1....     
-00019ba0: 2020 2069 6628 626f 736f 6e5f 636f 756e     if(boson_coun
-00019bb0: 743d 3d30 2061 6e64 2066 6572 6d69 5f63  t==0 and fermi_c
-00019bc0: 6f75 6e74 3e30 293a 0d0a 2020 2020 2020  ount>0):..      
-00019bd0: 2020 2020 2020 6966 2070 7265 6665 7220        if prefer 
-00019be0: 213d 204e 6f6e 653a 0d0a 2020 2020 2020  != None:..      
-00019bf0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00019c00: 2070 7265 6665 720d 0a20 2020 2020 2020   prefer..       
-00019c10: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-00019c20: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00019c30: 726e 2031 0d0a 2020 2020 2020 2020 656c  rn 1..        el
-00019c40: 6966 2862 6f73 6f6e 5f63 6f75 6e74 3e30  if(boson_count>0
-00019c50: 2061 6e64 2066 6572 6d69 5f63 6f75 6e74   and fermi_count
-00019c60: 3d3d 3029 3a0d 0a20 2020 2020 2020 2020  ==0):..         
-00019c70: 2020 2069 6620 7072 6566 6572 2021 3d20     if prefer != 
-00019c80: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00019c90: 2020 2020 2020 2072 6574 7572 6e20 7072         return pr
-00019ca0: 6566 6572 0d0a 2020 2020 2020 2020 2020  efer..          
-00019cb0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00019cc0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00019cd0: 300d 0a20 2020 2020 2020 2065 6c69 6628  0..        elif(
-00019ce0: 626f 736f 6e5f 636f 756e 743e 3020 616e  boson_count>0 an
-00019cf0: 6420 6665 726d 695f 636f 756e 743e 3029  d fermi_count>0)
-00019d00: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00019d10: 6574 7572 6e20 6879 6272 6964 5f73 796d  eturn hybrid_sym
-00019d20: 626f 6c0d 0a20 2020 2073 7465 7020 3d20  bol..    step = 
-00019d30: 7368 6f77 5f70 726f 6772 6573 7328 7374  show_progress(st
-00019d40: 6570 2c70 726f 6365 7373 5f6c 656e 6774  ep,process_lengt
-00019d50: 682c 7072 6f63 6573 735f 6e61 6d65 2b22  h,process_name+"
-00019d60: 2022 2b22 3c22 2b63 7572 7265 6e74 5f6d   "+"<"+current_m
-00019d70: 656d 6f72 795f 6469 7370 6c61 7928 292b  emory_display()+
-00019d80: 223e 222c 636f 6c6f 723d 7072 6f63 6573  ">",color=proces
-00019d90: 735f 636f 6c6f 722c 7469 6d65 3d74 696d  s_color,time=tim
-00019da0: 652e 7469 6d65 2829 2d73 3030 290d 0a20  e.time()-s00).. 
-00019db0: 2020 204f 626a 203d 204f 626a 2e6a 6f69     Obj = Obj.joi
-00019dc0: 6e5f 6c65 6773 286a 6f69 6e5f 6c65 6773  n_legs(join_legs
-00019dd0: 5f73 7472 696e 675f 696e 7075 742c 226d  _string_input,"m
-00019de0: 6174 7269 7822 2c73 6176 655f 6d65 6d6f  atrix",save_memo
-00019df0: 7279 3d54 7275 6529 0d0a 2020 2020 0d0a  ry=True)..    ..
-00019e00: 2020 2020 7374 6570 203d 2073 686f 775f      step = show_
-00019e10: 7072 6f67 7265 7373 2873 7465 702c 7072  progress(step,pr
-00019e20: 6f63 6573 735f 6c65 6e67 7468 2c70 726f  ocess_length,pro
-00019e30: 6365 7373 5f6e 616d 652b 2220 222b 223c  cess_name+" "+"<
-00019e40: 222b 6375 7272 656e 745f 6d65 6d6f 7279  "+current_memory
-00019e50: 5f64 6973 706c 6179 2829 2b22 3e22 2c63  _display()+">",c
-00019e60: 6f6c 6f72 3d70 726f 6365 7373 5f63 6f6c  olor=process_col
-00019e70: 6f72 2c74 696d 653d 7469 6d65 2e74 696d  or,time=time.tim
-00019e80: 6528 292d 7330 3029 0d0a 2020 2020 233a  e()-s00)..    #:
-00019e90: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019ea0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019eb0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019ec0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019ed0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019ee0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a0d  :::::::::::::::.
-00019ef0: 0a20 2020 2023 3a3a 3a3a 3a20 2020 2020  .    #:::::     
-00019f00: 2053 5445 5020 3220 2d20 5065 7266 6f72   STEP 2 - Perfor
-00019f10: 6d20 4865 726d 6974 6961 6e20 436f 6e6a  m Hermitian Conj
-00019f20: 7567 6174 696f 6e20 2020 2020 2020 2020  ugation         
-00019f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019f50: 203a 3a3a 3a3a 0d0a 2020 2020 233a 3a3a   :::::..    #:::
-00019f60: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019f70: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019f80: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019f90: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019fa0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-00019fb0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a0d 0a0d  :::::::::::::...
-00019fc0: 0a20 2020 204f 626a 2e64 6174 6120 3d20  .    Obj.data = 
-00019fd0: 6e70 2e63 6f6e 6a75 6761 7465 286f 652e  np.conjugate(oe.
-00019fe0: 636f 6e74 7261 6374 2827 696a 2d3e 6a69  contract('ij->ji
-00019ff0: 272c 4f62 6a2e 6461 7461 2929 0d0a 2020  ',Obj.data))..  
-0001a000: 2020 0d0a 2020 2020 6e65 775f 7374 6174    ..    new_stat
-0001a010: 203d 205b 312c 315d 0d0a 2020 2020 0d0a   = [1,1]..    ..
-0001a020: 2020 2020 6966 204f 626a 2e73 7461 7469      if Obj.stati
-0001a030: 7374 6963 5b30 5d20 696e 2066 6572 6d69  stic[0] in fermi
-0001a040: 5f74 7970 6520 3a0d 0a20 2020 2020 2020  _type :..       
-0001a050: 206e 6577 5f73 7461 745b 315d 203d 202d   new_stat[1] = -
-0001a060: 4f62 6a2e 7374 6174 6973 7469 635b 305d  Obj.statistic[0]
-0001a070: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
-0001a080: 2020 2020 206e 6577 5f73 7461 745b 315d       new_stat[1]
-0001a090: 203d 204f 626a 2e73 7461 7469 7374 6963   = Obj.statistic
-0001a0a0: 5b30 5d0d 0a20 2020 2020 2020 200d 0a20  [0]..        .. 
-0001a0b0: 2020 2069 6620 4f62 6a2e 7374 6174 6973     if Obj.statis
-0001a0c0: 7469 635b 315d 2069 6e20 6665 726d 695f  tic[1] in fermi_
-0001a0d0: 7479 7065 203a 0d0a 2020 2020 2020 2020  type :..        
-0001a0e0: 6e65 775f 7374 6174 5b30 5d20 3d20 2d4f  new_stat[0] = -O
-0001a0f0: 626a 2e73 7461 7469 7374 6963 5b31 5d0d  bj.statistic[1].
-0001a100: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
-0001a110: 2020 2020 6e65 775f 7374 6174 5b30 5d20      new_stat[0] 
-0001a120: 3d20 4f62 6a2e 7374 6174 6973 7469 635b  = Obj.statistic[
-0001a130: 315d 0d0a 2020 2020 0d0a 2020 2020 6e65  1]..    ..    ne
-0001a140: 775f 7374 6174 203d 206d 616b 655f 7475  w_stat = make_tu
-0001a150: 706c 6528 6e65 775f 7374 6174 290d 0a20  ple(new_stat).. 
-0001a160: 2020 200d 0a20 2020 204f 626a 2e73 7461     ..    Obj.sta
-0001a170: 7469 7374 6963 203d 206e 6577 5f73 7461  tistic = new_sta
-0001a180: 740d 0a20 2020 200d 0a20 2020 2073 7465  t..    ..    ste
-0001a190: 7020 3d20 7368 6f77 5f70 726f 6772 6573  p = show_progres
-0001a1a0: 7328 7374 6570 2c70 726f 6365 7373 5f6c  s(step,process_l
-0001a1b0: 656e 6774 682c 7072 6f63 6573 735f 6e61  ength,process_na
-0001a1c0: 6d65 2b22 2022 2b22 3c22 2b63 7572 7265  me+" "+"<"+curre
-0001a1d0: 6e74 5f6d 656d 6f72 795f 6469 7370 6c61  nt_memory_displa
-0001a1e0: 7928 292b 223e 222c 636f 6c6f 723d 7072  y()+">",color=pr
-0001a1f0: 6f63 6573 735f 636f 6c6f 722c 7469 6d65  ocess_color,time
-0001a200: 3d74 696d 652e 7469 6d65 2829 2d73 3030  =time.time()-s00
-0001a210: 290d 0a20 2020 2023 3a3a 3a3a 3a3a 3a3a  )..    #::::::::
-0001a220: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0001a230: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0001a240: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0001a250: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0001a260: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0001a270: 3a3a 3a3a 3a3a 3a3a 0d0a 2020 2020 233a  ::::::::..    #:
-0001a280: 3a3a 3a3a 2020 2020 2020 5354 4550 2033  ::::      STEP 3
-0001a290: 202d 2053 706c 6974 206c 6567 7320 2020   - Split legs   
-0001a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a2d0: 2020 2020 2020 2020 2020 3a3a 3a3a 3a0d            :::::.
-0001a2e0: 0a20 2020 2023 3a3a 3a3a 3a3a 3a3a 3a3a  .    #::::::::::
-0001a2f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0001a300: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0001a310: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0001a320: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0001a330: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
-0001a340: 3a3a 3a3a 3a3a 0d0a 2020 2020 0d0a 2020  ::::::..    ..  
-0001a350: 2020 0d0a 2020 2020 2320 636f 756e 7420    ..    # count 
-0001a360: 7468 6520 6e75 6d62 6572 206f 6620 696e  the number of in
-0001a370: 6469 6365 7320 696e 2074 6865 2074 776f  dices in the two
-0001a380: 2067 726f 7570 730d 0a20 2020 2055 696e   groups..    Uin
-0001a390: 6420 3d20 2222 0d0a 2020 2020 5669 6e64  d = ""..    Vind
-0001a3a0: 203d 2022 220d 0a20 2020 2055 7374 6174   = ""..    Ustat
-0001a3b0: 7320 3d20 5b5d 0d0a 2020 2020 5673 7461  s = []..    Vsta
-0001a3c0: 7473 203d 205b 5d0d 0a20 2020 2055 7368  ts = []..    Ush
-0001a3d0: 6170 6520 3d20 5b5d 0d0a 2020 2020 5673  ape = []..    Vs
-0001a3e0: 6861 7065 203d 205b 5d0d 0a20 2020 2070  hape = []..    p
-0001a3f0: 6172 7469 7469 6f6e 5f66 6f75 6e64 203d  artition_found =
-0001a400: 2046 616c 7365 0d0a 2020 2020 666f 7220   False..    for 
-0001a410: 692c 6368 6172 2069 6e20 656e 756d 6572  i,char in enumer
-0001a420: 6174 6528 7374 7269 6e67 293a 0d0a 2020  ate(string):..  
-0001a430: 2020 2020 2020 6966 2063 6861 7220 696e        if char in
-0001a440: 2073 6570 6172 6174 6f72 5f6c 6973 7420   separator_list 
-0001a450: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-0001a460: 6172 7469 7469 6f6e 5f66 6f75 6e64 203d  artition_found =
-0001a470: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
-0001a480: 2020 2063 6f6e 7469 6e75 650d 0a20 2020     continue..   
-0001a490: 2020 2020 2069 6628 7061 7274 6974 696f       if(partitio
-0001a4a0: 6e5f 666f 756e 6429 3a0d 0a20 2020 2020  n_found):..     
-0001a4b0: 2020 2020 2020 2056 696e 642b 3d63 6861         Vind+=cha
-0001a4c0: 720d 0a20 2020 2020 2020 2020 2020 2056  r..            V
-0001a4d0: 7374 6174 732b 3d5b 584f 626a 5f73 7461  stats+=[XObj_sta
-0001a4e0: 7473 5b69 2d31 5d5d 0d0a 2020 2020 2020  ts[i-1]]..      
-0001a4f0: 2020 2020 2020 5673 6861 7065 2b3d 5b58        Vshape+=[X
-0001a500: 4f62 6a5f 7368 6170 655b 692d 315d 5d0d  Obj_shape[i-1]].
-0001a510: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-0001a520: 2020 2020 2020 2020 2020 2020 5569 6e64              Uind
-0001a530: 2b3d 6368 6172 0d0a 2020 2020 2020 2020  +=char..        
-0001a540: 2020 2020 5573 7461 7473 2b3d 5b58 4f62      Ustats+=[XOb
-0001a550: 6a5f 7374 6174 735b 695d 5d0d 0a20 2020  j_stats[i]]..   
-0001a560: 2020 2020 2020 2020 2055 7368 6170 652b           Ushape+
-0001a570: 3d5b 584f 626a 5f73 6861 7065 5b69 5d5d  =[XObj_shape[i]]
-0001a580: 0d0a 2020 2020 0d0a 2020 2020 6e65 775f  ..    ..    new_
-0001a590: 696e 6420 3d20 2228 222b 5669 6e64 2b22  ind = "("+Vind+"
-0001a5a0: 2928 222b 5569 6e64 2b22 2922 0d0a 2020  )("+Uind+")"..  
-0001a5b0: 2020 6e65 775f 7374 6174 7320 3d20 5673    new_stats = Vs
-0001a5c0: 7461 7473 202b 2055 7374 6174 730d 0a20  tats + Ustats.. 
-0001a5d0: 2020 206e 6577 5f73 6861 7065 203d 206d     new_shape = m
-0001a5e0: 616b 655f 7475 706c 6528 5673 6861 7065  ake_tuple(Vshape
-0001a5f0: 202b 2055 7368 6170 6529 0d0a 2020 2020   + Ushape)..    
-0001a600: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-0001a610: 656e 286e 6577 5f73 7461 7473 2929 3a0d  en(new_stats)):.
-0001a620: 0a20 2020 2020 2020 2069 6620 6e65 775f  .        if new_
-0001a630: 7374 6174 735b 695d 2069 6e20 6665 726d  stats[i] in ferm
-0001a640: 695f 7479 7065 203a 0d0a 2020 2020 2020  i_type :..      
-0001a650: 2020 2020 2020 6e65 775f 7374 6174 735b        new_stats[
-0001a660: 695d 2a3d 2d31 0d0a 2020 2020 6e65 775f  i]*=-1..    new_
-0001a670: 7374 6174 7320 3d20 6d61 6b65 5f74 7570  stats = make_tup
-0001a680: 6c65 286e 6577 5f73 7461 7473 290d 0a20  le(new_stats).. 
-0001a690: 2020 2073 7465 7020 3d20 7368 6f77 5f70     step = show_p
-0001a6a0: 726f 6772 6573 7328 7374 6570 2c70 726f  rogress(step,pro
-0001a6b0: 6365 7373 5f6c 656e 6774 682c 7072 6f63  cess_length,proc
-0001a6c0: 6573 735f 6e61 6d65 2b22 2022 2b22 3c22  ess_name+" "+"<"
-0001a6d0: 2b63 7572 7265 6e74 5f6d 656d 6f72 795f  +current_memory_
-0001a6e0: 6469 7370 6c61 7928 292b 223e 222c 636f  display()+">",co
-0001a6f0: 6c6f 723d 7072 6f63 6573 735f 636f 6c6f  lor=process_colo
-0001a700: 722c 7469 6d65 3d74 696d 652e 7469 6d65  r,time=time.time
-0001a710: 2829 2d73 3030 290d 0a20 2020 204f 626a  ()-s00)..    Obj
-0001a720: 203d 204f 626a 2e73 706c 6974 5f6c 6567   = Obj.split_leg
-0001a730: 7328 6e65 775f 696e 642c 6e65 775f 7374  s(new_ind,new_st
-0001a740: 6174 732c 6e65 775f 7368 6170 652c 7361  ats,new_shape,sa
-0001a750: 7665 5f6d 656d 6f72 793d 5472 7565 290d  ve_memory=True).
-0001a760: 0a20 2020 200d 0a20 2020 2023 6966 2074  .    ..    #if t
-0001a770: 6869 735f 7479 7065 3d3d 7370 6172 7365  his_type==sparse
-0001a780: 203a 0d0a 2020 2020 2320 2020 204f 626a   :..    #    Obj
-0001a790: 203d 2073 7061 7273 6528 4f62 6a29 0d0a   = sparse(Obj)..
-0001a7a0: 2020 2020 6966 2074 6869 735f 666f 726d      if this_form
-0001a7b0: 6174 213d 4f62 6a2e 666f 726d 6174 203a  at!=Obj.format :
-0001a7c0: 0d0a 2020 2020 2020 2020 4f62 6a20 3d20  ..        Obj = 
-0001a7d0: 4f62 6a2e 7377 6974 6368 5f66 6f72 6d61  Obj.switch_forma
-0001a7e0: 7428 7361 7665 5f6d 656d 6f72 793d 5472  t(save_memory=Tr
-0001a7f0: 7565 290d 0a20 2020 2069 6620 7468 6973  ue)..    if this
-0001a800: 5f65 6e63 6f64 6572 213d 4f62 6a2e 656e  _encoder!=Obj.en
-0001a810: 636f 6465 7220 3a0d 0a20 2020 2020 2020  coder :..       
-0001a820: 204f 626a 203d 204f 626a 2e73 7769 7463   Obj = Obj.switc
-0001a830: 685f 656e 636f 6465 7228 7361 7665 5f6d  h_encoder(save_m
-0001a840: 656d 6f72 793d 5472 7565 290d 0a0d 0a20  emory=True).... 
-0001a850: 2020 2063 6c65 6172 5f70 726f 6772 6573     clear_progres
-0001a860: 7328 290d 0a20 2020 2073 7973 2e73 7464  s()..    sys.std
-0001a870: 6f75 742e 7772 6974 6528 225c 3033 335b  out.write("\033[
-0001a880: 4622 290d 0a0d 0a20 2020 2072 6574 7572  F")....    retur
-0001a890: 6e20 4f62 6a0d 0a0d 0a23 2323 2323 2323  n Obj....#######
-0001a8a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001a8b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001a8c0: 2323 2323 2323 2323 2323 2323 230d 0a23  #############..#
-0001a8d0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
-0001a8e0: 2020 2020 2055 7469 6c69 7469 6573 2020       Utilities  
-0001a8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a900: 2023 230d 0a23 2323 2323 2323 2323 2323   ##..###########
-0001a910: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001a920: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001a930: 2323 2323 2323 2323 230d 0a0d 0a64 6566  #########....def
-0001a940: 2072 616e 646f 6d28 7368 6170 652c 7374   random(shape,st
-0001a950: 6174 6973 7469 632c 7465 6e73 6f72 5f66  atistic,tensor_f
-0001a960: 6f72 6d61 743d 6465 6e73 652c 6474 7970  ormat=dense,dtyp
-0001a970: 653d 666c 6f61 742c 736b 6970 5f74 7269  e=float,skip_tri
-0001a980: 6d6d 696e 673d 4661 6c73 6529 3a0d 0a20  mming=False):.. 
-0001a990: 2020 2058 203d 206e 702e 7261 6e64 6f6d     X = np.random
-0001a9a0: 2e72 616e 6428 2a73 6861 7065 290d 0a20  .rand(*shape).. 
-0001a9b0: 2020 2069 6620 6474 7970 6520 3d3d 2063     if dtype == c
-0001a9c0: 6f6d 706c 6578 203a 0d0a 2020 2020 2020  omplex :..      
-0001a9d0: 2020 5820 3d20 636f 6d70 6c65 7828 312c    X = complex(1,
-0001a9e0: 3029 2a58 202b 2063 6f6d 706c 6578 2830  0)*X + complex(0
-0001a9f0: 2c31 292a 6e70 2e72 616e 646f 6d2e 7261  ,1)*np.random.ra
-0001aa00: 6e64 282a 7368 6170 6529 0d0a 2020 2020  nd(*shape)..    
-0001aa10: 4120 3d20 6465 6e73 6528 582c 2073 7461  A = dense(X, sta
-0001aa20: 7469 7374 6963 203d 2073 7461 7469 7374  tistic = statist
-0001aa30: 6963 290d 0a20 2020 2069 6620 6e6f 7420  ic)..    if not 
-0001aa40: 736b 6970 5f74 7269 6d6d 696e 673a 0d0a  skip_trimming:..
-0001aa50: 2020 2020 2020 2020 4120 3d20 7472 696d          A = trim
-0001aa60: 5f67 7261 7373 6d61 6e6e 5f6f 6464 2841  _grassmann_odd(A
-0001aa70: 290d 0a20 2020 2069 6620 7465 6e73 6f72  )..    if tensor
-0001aa80: 5f66 6f72 6d61 743d 3d73 7061 7273 653a  _format==sparse:
-0001aa90: 0d0a 2020 2020 2020 2020 4120 3d20 7370  ..        A = sp
-0001aaa0: 6172 7365 2841 290d 0a20 2020 2020 2020  arse(A)..       
-0001aab0: 2041 203d 2041 2e72 656d 6f76 655f 7a65   A = A.remove_ze
-0001aac0: 726f 7328 290d 0a20 2020 2072 6574 7572  ros()..    retur
-0001aad0: 6e20 410d 0a0d 0a64 6566 2070 6f77 6572  n A....def power
-0001aae0: 2854 2c70 293a 0d0a 2020 2020 7468 6973  (T,p):..    this
-0001aaf0: 5f74 7970 6520 3d20 7479 7065 2854 290d  _type = type(T).
-0001ab00: 0a20 2020 2074 6869 735f 666f 726d 6174  .    this_format
-0001ab10: 203d 2054 2e66 6f72 6d61 740d 0a20 2020   = T.format..   
-0001ab20: 2074 6869 735f 656e 636f 6465 7220 3d20   this_encoder = 
-0001ab30: 542e 656e 636f 6465 720d 0a20 2020 2054  T.encoder..    T
-0001ab40: 203d 2064 656e 7365 2854 292e 666f 7263   = dense(T).forc
-0001ab50: 655f 666f 726d 6174 2822 6d61 7472 6978  e_format("matrix
-0001ab60: 2229 2e66 6f72 6365 5f65 6e63 6f64 6572  ").force_encoder
-0001ab70: 2822 6361 6e6f 6e69 6361 6c22 290d 0a20  ("canonical").. 
-0001ab80: 2020 2054 2e64 6174 6120 3d20 6e70 2e70     T.data = np.p
-0001ab90: 6f77 6572 2854 2e64 6174 612c 7029 0d0a  ower(T.data,p)..
-0001aba0: 2020 2020 5420 3d20 542e 666f 7263 655f      T = T.force_
-0001abb0: 666f 726d 6174 2874 6869 735f 666f 726d  format(this_form
-0001abc0: 6174 292e 666f 7263 655f 656e 636f 6465  at).force_encode
-0001abd0: 7228 7468 6973 5f65 6e63 6f64 6572 290d  r(this_encoder).
-0001abe0: 0a20 2020 2069 6620 7468 6973 5f74 7970  .    if this_typ
-0001abf0: 653d 3d73 7061 7273 6520 3a0d 0a20 2020  e==sparse :..   
-0001ac00: 2020 2020 2054 203d 2073 7061 7273 6528       T = sparse(
-0001ac10: 5429 0d0a 2020 2020 7265 7475 726e 2054  T)..    return T
-0001ac20: 0d0a 0d0a 6465 6620 7371 7274 2854 293a  ....def sqrt(T):
-0001ac30: 0d0a 2020 2020 7265 7475 726e 2070 6f77  ..    return pow
-0001ac40: 6572 2854 2c30 2e35 290d 0a              er(T,0.5)..
+00015aa0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00015ab0: 2323 2323 2323 2323 2323 2323 2323 0d0a  ##############..
+00015ac0: 0d0a 6465 6620 536f 7274 6564 4569 6728  ..def SortedEig(
+00015ad0: 4d2c 6375 746f 6666 3d4e 6f6e 652c 6465  M,cutoff=None,de
+00015ae0: 6275 675f 6d6f 6465 3d46 616c 7365 293a  bug_mode=False):
+00015af0: 0d0a 0d0a 2020 2020 4e6f 6e48 6572 6974  ....    NonHerit
+00015b00: 6961 6e4e 6f72 6d20 3d20 6e70 2e6c 696e  ianNorm = np.lin
+00015b10: 616c 672e 6e6f 726d 284d 2d6e 702e 636f  alg.norm(M-np.co
+00015b20: 6e6a 7567 6174 6528 6e70 2e74 7261 6e73  njugate(np.trans
+00015b30: 706f 7365 284d 2929 292f 6e70 2e6c 696e  pose(M)))/np.lin
+00015b40: 616c 672e 6e6f 726d 284d 290d 0a20 2020  alg.norm(M)..   
+00015b50: 2069 6620 4e6f 6e48 6572 6974 6961 6e4e   if NonHeritianN
+00015b60: 6f72 6d3e 6e75 6d65 725f 6375 746f 6666  orm>numer_cutoff
+00015b70: 203a 0d0a 2020 2020 2020 2020 6572 726f   :..        erro
+00015b80: 7228 2245 7272 6f72 5b53 6f72 7465 6445  r("Error[SortedE
+00015b90: 6967 5d3a 2054 6865 2069 6e70 7574 206d  ig]: The input m
+00015ba0: 6174 7269 7820 6973 206e 6f74 2048 6572  atrix is not Her
+00015bb0: 6d69 7469 616e 2122 290d 0a0d 0a20 2020  mitian!")....   
+00015bc0: 2055 2c20 ce9b 2c20 5620 3d20 6e70 2e6c   U, .., V = np.l
+00015bd0: 696e 616c 672e 7376 6428 4d2c 2066 756c  inalg.svd(M, ful
+00015be0: 6c5f 6d61 7472 6963 6573 3d46 616c 7365  l_matrices=False
+00015bf0: 290d 0a0d 0a20 2020 206e 6e7a 203d 2030  )....    nnz = 0
+00015c00: 0d0a 2020 2020 2369 6620 6e70 2e61 6273  ..    #if np.abs
+00015c10: 28ce 9b5b 305d 2920 3c20 6e75 6d65 725f  (..[0]) < numer_
+00015c20: 6375 746f 6666 3a0d 0a20 2020 2023 2020  cutoff:..    #  
+00015c30: 2020 6572 726f 7228 2245 7272 6f72 5b53    error("Error[S
+00015c40: 6f72 7465 6453 5644 5d3a 206e 702e 6c69  ortedSVD]: np.li
+00015c50: 6e61 6c67 2e73 7664 2829 2072 6574 7572  nalg.svd() retur
+00015c60: 6e73 207a 6572 6f20 7369 6e67 756c 6172  ns zero singular
+00015c70: 2076 616c 7565 2076 6563 746f 7221 2229   value vector!")
+00015c80: 0d0a 0d0a 2020 2020 666f 7220 692c 7320  ....    for i,s 
+00015c90: 696e 2065 6e75 6d65 7261 7465 28ce 9b29  in enumerate(..)
+00015ca0: 3a0d 0a20 2020 2020 2020 2069 6620 6e70  :..        if np
+00015cb0: 2e61 6273 2873 2fce 9b5b 305d 2920 3e20  .abs(s/..[0]) > 
+00015cc0: 6e75 6d65 725f 6375 746f 6666 3a0d 0a20  numer_cutoff:.. 
+00015cd0: 2020 2020 2020 2020 2020 206e 6e7a 2b3d             nnz+=
+00015ce0: 310d 0a0d 0a20 2020 2069 6620 6375 746f  1....    if cuto
+00015cf0: 6666 213d 4e6f 6e65 2061 6e64 2063 7574  ff!=None and cut
+00015d00: 6f66 6620 3c20 6e6e 7a3a 0d0a 2020 2020  off < nnz:..    
+00015d10: 2020 2020 6e6e 7a20 3d20 6375 746f 6666      nnz = cutoff
+00015d20: 0d0a 0d0a 2020 2020 ce9b 203d 20ce 9b5b  ....    .. = ..[
+00015d30: 3a6e 6e7a 5d0d 0a20 2020 2055 203d 2055  :nnz]..    U = U
+00015d40: 5b3a 2c3a 6e6e 7a5d 0d0a 2020 2020 5620  [:,:nnz]..    V 
+00015d50: 3d20 565b 3a6e 6e7a 2c3a 5d0d 0a20 2020  = V[:nnz,:]..   
+00015d60: 2063 5520 3d20 6e70 2e63 6f6e 6a75 6761   cU = np.conjuga
+00015d70: 7465 286e 702e 7472 616e 7370 6f73 6528  te(np.transpose(
+00015d80: 5529 290d 0a20 2020 20ce 9b56 5520 3d20  U))..    ..VU = 
+00015d90: 6e70 2e65 696e 7375 6d28 2769 2c69 6a2c  np.einsum('i,ij,
+00015da0: 6a6b 2d3e 696b 272c ce9b 2c56 2c55 290d  jk->ik',..,V,U).
+00015db0: 0a20 2020 20ce 9b20 3d20 6e70 2e65 696e  .    .. = np.ein
+00015dc0: 7375 6d28 2769 2c69 6a2c 6a6b 2d3e 6b27  sum('i,ij,jk->k'
+00015dd0: 2cce 9b2c 562c 5529 0d0a 0d0a 2020 2020  ,..,V,U)....    
+00015de0: 7265 7475 726e 2055 2c20 ce9b 2c20 6355  return U, .., cU
+00015df0: 0d0a 2320 4920 3d20 6355 550d 0a64 6566  ..# I = cUU..def
+00015e00: 2042 6c6f 636b 4569 6728 4f62 6a2c 6375   BlockEig(Obj,cu
+00015e10: 746f 6666 3d4e 6f6e 652c 6465 6275 675f  toff=None,debug_
+00015e20: 6d6f 6465 3d46 616c 7365 293a 0d0a 2020  mode=False):..  
+00015e30: 2020 0d0a 2020 2020 2320 7065 7266 6f72    ..    # perfor
+00015e40: 6d69 6e67 2061 6e20 7376 6420 6f66 2061  ming an svd of a
+00015e50: 206d 6174 7269 7820 626c 6f63 6b20 6279   matrix block by
+00015e60: 2062 6c6f 636b 0d0a 0d0a 2020 2020 6966   block....    if
+00015e70: 2874 7970 6528 4f62 6a29 213d 6e70 2e61  (type(Obj)!=np.a
+00015e80: 7272 6179 2061 6e64 2074 7970 6528 4f62  rray and type(Ob
+00015e90: 6a29 213d 6e70 2e6e 6461 7272 6179 293a  j)!=np.ndarray):
+00015ea0: 0d0a 2020 2020 2020 2020 6572 726f 7228  ..        error(
+00015eb0: 2245 7272 6f72 5b42 6c6f 636b 4569 675d  "Error[BlockEig]
+00015ec0: 3a20 416e 2069 6e70 7574 206d 7573 7420  : An input must 
+00015ed0: 6265 206f 6620 7479 7065 206e 756d 7079  be of type numpy
+00015ee0: 2e61 7272 6179 206f 7220 6e75 6d70 792e  .array or numpy.
+00015ef0: 6e64 6172 7261 7920 6f6e 6c79 2122 290d  ndarray only!").
+00015f00: 0a20 2020 2020 2020 200d 0a0d 0a20 2020  .        ....   
+00015f10: 2069 6628 4f62 6a2e 6e64 696d 213d 3229   if(Obj.ndim!=2)
+00015f20: 3a0d 0a20 2020 2020 2020 2065 7272 6f72  :..        error
+00015f30: 2822 4572 726f 725b 426c 6f63 6b45 6967  ("Error[BlockEig
+00015f40: 5d3a 2041 6e20 696e 7075 7420 6d75 7374  ]: An input must
+00015f50: 2062 6520 6120 6d61 7472 6978 206f 6e6c   be a matrix onl
+00015f60: 7921 2229 0d0a 2020 2020 2020 2020 0d0a  y!")..        ..
+00015f70: 0d0a 2020 2020 6d20 3d20 4f62 6a2e 7368  ..    m = Obj.sh
+00015f80: 6170 655b 305d 0d0a 2020 2020 6e20 3d20  ape[0]..    n = 
+00015f90: 4f62 6a2e 7368 6170 655b 315d 0d0a 0d0a  Obj.shape[1]....
+00015fa0: 2020 2020 6966 286d 2532 213d 3020 616e      if(m%2!=0 an
+00015fb0: 6420 6e25 3221 3d30 293a 0d0a 2020 2020  d n%2!=0):..    
+00015fc0: 2020 2020 6572 726f 7228 2245 7272 6f72      error("Error
+00015fd0: 5b42 6c6f 636b 4569 675d 3a20 5468 6520  [BlockEig]: The 
+00015fe0: 6d61 7472 6978 2064 696d 656e 7369 6f6e  matrix dimension
+00015ff0: 7320 6d75 7374 2062 6520 6576 656e 2122  s must be even!"
+00016000: 290d 0a20 2020 2020 2020 200d 0a0d 0a0d  )..        .....
+00016010: 0a20 2020 2069 6628 6d3d 3d30 2061 6e64  .    if(m==0 and
+00016020: 206e 3d3d 3029 3a0d 0a20 2020 2020 2020   n==0):..       
+00016030: 2065 7272 6f72 2822 4572 726f 725b 426c   error("Error[Bl
+00016040: 6f63 6b45 6967 5d3a 2054 6865 206d 6174  ockEig]: The mat
+00016050: 7269 7820 6469 6d65 6e73 696f 6e73 206d  rix dimensions m
+00016060: 7573 7420 6265 2061 7420 6c65 6173 7420  ust be at least 
+00016070: 3221 2229 0d0a 2020 2020 2020 2020 0d0a  2!")..        ..
+00016080: 0d0a 2020 2020 7061 7269 7479 5f6e 6f72  ..    parity_nor
+00016090: 6d20 3d20 300d 0a20 2020 2066 6f72 2069  m = 0..    for i
+000160a0: 2069 6e20 7261 6e67 6528 6d29 3a0d 0a20   in range(m):.. 
+000160b0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+000160c0: 7261 6e67 6528 6e29 3a0d 0a20 2020 2020  range(n):..     
+000160d0: 2020 2020 2020 2069 6620 2869 2b6a 2925         if (i+j)%
+000160e0: 3221 3d30 3a0d 0a20 2020 2020 2020 2020  2!=0:..         
+000160f0: 2020 2020 2020 2070 6172 6974 795f 6e6f         parity_no
+00016100: 726d 202b 3d20 6e70 2e6c 696e 616c 672e  rm += np.linalg.
+00016110: 6e6f 726d 284f 626a 5b69 2c6a 5d29 0d0a  norm(Obj[i,j])..
+00016120: 2020 2020 6966 2820 286e 6f74 2073 6b69      if( (not ski
+00016130: 705f 7061 7269 7479 5f62 6c6f 636b 696e  p_parity_blockin
+00016140: 675f 6368 6563 6b29 2061 6e64 2070 6172  g_check) and par
+00016150: 6974 795f 6e6f 726d 2f28 6d2a 6e2f 3229  ity_norm/(m*n/2)
+00016160: 3e31 2e30 652d 3134 293a 0d0a 2020 2020  >1.0e-14):..    
+00016170: 2020 2020 6572 726f 7228 2245 7272 6f72      error("Error
+00016180: 5b42 6c6f 636b 4569 675d 3a20 5468 6973  [BlockEig]: This
+00016190: 206d 6174 7269 7820 6973 206e 6f74 2063   matrix is not c
+000161a0: 6f6e 7374 7275 6374 6564 2066 726f 6d20  onstructed from 
+000161b0: 6120 4772 6173 736d 616e 6e2d 6576 656e  a Grassmann-even
+000161c0: 2074 656e 736f 722e 2229 0d0a 2020 2020   tensor.")..    
+000161d0: 2020 2020 7072 696e 7428 2220 2020 2020      print("     
+000161e0: 2020 2020 2020 2020 2020 2020 284f 7220              (Or 
+000161f0: 7468 6174 206f 6e65 206f 6620 7468 6520  that one of the 
+00016200: 696e 6469 6365 7320 6172 6520 6e6f 6e2d  indices are non-
+00016210: 6665 726d 696f 6e69 632e 2922 290d 0a20  fermionic.)").. 
+00016220: 2020 2020 2020 200d 0a0d 0a20 2020 2023         ....    #
+00016230: 2041 7420 7468 6973 2070 6f69 6e74 2074   At this point t
+00016240: 6865 206d 6174 7269 7820 6973 2077 656c  he matrix is wel
+00016250: 6c2d 6265 6861 7665 640d 0a0d 0a20 2020  l-behaved....   
+00016260: 2023 2074 696d 6520 746f 2073 6570 6172   # time to separ
+00016270: 6174 6520 7468 6520 626c 6f63 6b73 0d0a  ate the blocks..
+00016280: 2020 2020 4d45 203d 206e 702e 7a65 726f      ME = np.zero
+00016290: 7328 5b69 6e74 286d 2f32 292c 696e 7428  s([int(m/2),int(
+000162a0: 6e2f 3229 5d2c 6474 7970 653d 7479 7065  n/2)],dtype=type
+000162b0: 284f 626a 5b30 5d5b 305d 2929 0d0a 2020  (Obj[0][0]))..  
+000162c0: 2020 4d4f 203d 206e 702e 7a65 726f 7328    MO = np.zeros(
+000162d0: 5b69 6e74 286d 2f32 292c 696e 7428 6e2f  [int(m/2),int(n/
+000162e0: 3229 5d2c 6474 7970 653d 7479 7065 284f  2)],dtype=type(O
+000162f0: 626a 5b30 5d5b 305d 2929 0d0a 0d0a 2020  bj[0][0]))....  
+00016300: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00016310: 2869 6e74 286d 2f32 2929 3a0d 0a20 2020  (int(m/2)):..   
+00016320: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
+00016330: 6e67 6528 696e 7428 6e2f 3229 293a 0d0a  nge(int(n/2)):..
+00016340: 2020 2020 2020 2020 2020 2020 4d45 5b69              ME[i
+00016350: 2c6a 5d20 3d20 4f62 6a5b 322a 692c 322a  ,j] = Obj[2*i,2*
+00016360: 6a5d 0d0a 2020 2020 2020 2020 2020 2020  j]..            
+00016370: 4d4f 5b69 2c6a 5d20 3d20 4f62 6a5b 322a  MO[i,j] = Obj[2*
+00016380: 692b 312c 322a 6a2b 315d 0d0a 0d0a 2020  i+1,2*j+1]....  
+00016390: 2020 6861 6c66 6375 746f 6666 203d 204e    halfcutoff = N
+000163a0: 6f6e 650d 0a20 2020 2069 6620 6375 746f  one..    if cuto
+000163b0: 6666 213d 4e6f 6e65 203a 0d0a 2020 2020  ff!=None :..    
+000163c0: 2020 2020 6861 6c66 6375 746f 6666 203d      halfcutoff =
+000163d0: 2069 6e74 2863 7574 6f66 662f 3229 0d0a   int(cutoff/2)..
+000163e0: 0d0a 2020 2020 5545 2c20 ce9b 452c 2063  ..    UE, ..E, c
+000163f0: 5545 203d 2053 6f72 7465 6445 6967 284d  UE = SortedEig(M
+00016400: 452c 6861 6c66 6375 746f 6666 2c64 6562  E,halfcutoff,deb
+00016410: 7567 5f6d 6f64 6529 0d0a 2020 2020 554f  ug_mode)..    UO
+00016420: 2c20 ce9b 4f2c 2063 554f 203d 2053 6f72  , ..O, cUO = Sor
+00016430: 7465 6445 6967 284d 4f2c 6861 6c66 6375  tedEig(MO,halfcu
+00016440: 746f 6666 2c64 6562 7567 5f6d 6f64 6529  toff,debug_mode)
+00016450: 0d0a 0d0a 2020 2020 6420 3d20 6d61 7828  ....    d = max(
+00016460: 6c65 6e28 ce9b 4529 2c6c 656e 28ce 9b4f  len(..E),len(..O
+00016470: 2929 0d0a 2020 2020 6420 3d20 696e 7428  ))..    d = int(
+00016480: 322a 2a6d 6174 682e 6365 696c 286e 702e  2**math.ceil(np.
+00016490: 6c6f 6732 2864 2929 290d 0a0d 0a20 2020  log2(d)))....   
+000164a0: 2064 6566 2070 6164 6469 6e67 2855 782c   def padding(Ux,
+000164b0: 20ce 9b78 2c20 6355 782c 2070 6164 6469   ..x, cUx, paddi
+000164c0: 6e67 5f64 696d 656e 7369 6f6e 293a 0d0a  ng_dimension):..
+000164d0: 2020 2020 2020 2020 5578 203d 206e 702e          Ux = np.
+000164e0: 7061 6428 5578 2c28 2830 2c30 292c 2830  pad(Ux,((0,0),(0
+000164f0: 2c70 6164 6469 6e67 5f64 696d 656e 7369  ,padding_dimensi
+00016500: 6f6e 2929 2c27 636f 6e73 7461 6e74 272c  on)),'constant',
+00016510: 636f 6e73 7461 6e74 5f76 616c 7565 733d  constant_values=
+00016520: 2828 302c 3029 2c28 302c 3029 2929 0d0a  ((0,0),(0,0)))..
+00016530: 2020 2020 2020 2020 ce9b 7820 3d20 6e70          ..x = np
+00016540: 2e64 6961 6728 6e70 2e70 6164 28ce 9b78  .diag(np.pad(..x
+00016550: 2c28 302c 7061 6464 696e 675f 6469 6d65  ,(0,padding_dime
+00016560: 6e73 696f 6e29 2c27 636f 6e73 7461 6e74  nsion),'constant
+00016570: 272c 636f 6e73 7461 6e74 5f76 616c 7565  ',constant_value
+00016580: 733d 2830 2c30 2920 2020 2020 2020 2929  s=(0,0)       ))
+00016590: 0d0a 2020 2020 2020 2020 6355 7820 3d20  ..        cUx = 
+000165a0: 6e70 2e70 6164 2863 5578 2c28 2830 2c70  np.pad(cUx,((0,p
+000165b0: 6164 6469 6e67 5f64 696d 656e 7369 6f6e  adding_dimension
+000165c0: 292c 2830 2c30 2929 2c27 636f 6e73 7461  ),(0,0)),'consta
+000165d0: 6e74 272c 636f 6e73 7461 6e74 5f76 616c  nt',constant_val
+000165e0: 7565 733d 2828 302c 3029 2c28 302c 3029  ues=((0,0),(0,0)
+000165f0: 2929 0d0a 2020 2020 2020 2020 7265 7475  ))..        retu
+00016600: 726e 2055 782c 20ce 9b78 2c20 6355 780d  rn Ux, ..x, cUx.
+00016610: 0a0d 0a20 2020 2055 452c 20ce 9b45 2c20  ...    UE, ..E, 
+00016620: 6355 4520 3d20 7061 6464 696e 6728 5545  cUE = padding(UE
+00016630: 2c20 ce9b 452c 2063 5545 2c20 642d 6c65  , ..E, cUE, d-le
+00016640: 6e28 ce9b 4529 290d 0a20 2020 2055 4f2c  n(..E))..    UO,
+00016650: 20ce 9b4f 2c20 6355 4f20 3d20 7061 6464   ..O, cUO = padd
+00016660: 696e 6728 554f 2c20 ce9b 4f2c 2063 554f  ing(UO, ..O, cUO
+00016670: 2c20 642d 6c65 6e28 ce9b 4f29 290d 0a0d  , d-len(..O))...
+00016680: 0a20 2020 2064 6566 2067 6574 5f66 756c  .    def get_ful
+00016690: 6c5f 6d61 7472 6978 2841 452c 2041 4f29  l_matrix(AE, AO)
+000166a0: 3a0d 0a20 2020 2020 2020 206d 6861 6c66  :..        mhalf
+000166b0: 2c6e 6861 6c66 203d 2041 452e 7368 6170  ,nhalf = AE.shap
+000166c0: 650d 0a20 2020 2020 2020 2041 203d 206e  e..        A = n
+000166d0: 702e 7a65 726f 7328 5b32 2a6d 6861 6c66  p.zeros([2*mhalf
+000166e0: 2c32 2a6e 6861 6c66 5d2c 6474 7970 653d  ,2*nhalf],dtype=
+000166f0: 7479 7065 2841 455b 305d 5b30 5d29 290d  type(AE[0][0])).
+00016700: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+00016710: 6e20 7261 6e67 6528 6d68 616c 6629 3a0d  n range(mhalf):.
+00016720: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00016730: 206a 2069 6e20 7261 6e67 6528 6e68 616c   j in range(nhal
+00016740: 6629 3a0d 0a20 2020 2020 2020 2020 2020  f):..           
+00016750: 2020 2020 2041 5b32 2a69 2c32 2a6a 5d20       A[2*i,2*j] 
+00016760: 3d20 4145 5b69 2c6a 5d0d 0a20 2020 2020  = AE[i,j]..     
+00016770: 2020 2020 2020 2020 2020 2041 5b32 2a69             A[2*i
+00016780: 2b31 2c32 2a6a 2b31 5d20 3d20 414f 5b69  +1,2*j+1] = AO[i
+00016790: 2c6a 5d0d 0a20 2020 2020 2020 2072 6574  ,j]..        ret
+000167a0: 7572 6e20 410d 0a0d 0a20 2020 2055 203d  urn A....    U =
+000167b0: 2067 6574 5f66 756c 6c5f 6d61 7472 6978   get_full_matrix
+000167c0: 2855 452c 554f 290d 0a20 2020 20ce 9b20  (UE,UO)..    .. 
+000167d0: 3d20 6765 745f 6675 6c6c 5f6d 6174 7269  = get_full_matri
+000167e0: 7828 ce9b 452c ce9b 4f29 0d0a 2020 2020  x(..E,..O)..    
+000167f0: 6355 203d 2067 6574 5f66 756c 6c5f 6d61  cU = get_full_ma
+00016800: 7472 6978 2863 5545 2c63 554f 290d 0a20  trix(cUE,cUO).. 
+00016810: 2020 200d 0a0d 0a20 2020 2072 6574 7572     ....    retur
+00016820: 6e20 552c 20ce 9b2c 2063 550d 0a0d 0a64  n U, .., cU....d
+00016830: 6566 2065 6967 2849 6e70 4f62 6a2c 7374  ef eig(InpObj,st
+00016840: 7269 6e67 2c63 7574 6f66 663d 4e6f 6e65  ring,cutoff=None
+00016850: 2c64 6562 7567 5f6d 6f64 653d 4661 6c73  ,debug_mode=Fals
+00016860: 652c 7361 7665 5f6d 656d 6f72 793d 4661  e,save_memory=Fa
+00016870: 6c73 6529 3a0d 0a0d 0a20 2020 2070 726f  lse):....    pro
+00016880: 6365 7373 5f6e 616d 6520 3d20 2265 6967  cess_name = "eig
+00016890: 220d 0a20 2020 2070 726f 6365 7373 5f63  "..    process_c
+000168a0: 6f6c 6f72 203d 2022 7965 6c6c 6f77 220d  olor = "yellow".
+000168b0: 0a20 2020 2070 726f 6365 7373 5f6c 656e  .    process_len
+000168c0: 6774 6820 3d20 360d 0a20 2020 2073 7465  gth = 6..    ste
+000168d0: 7020 3d20 310d 0a20 2020 2073 3030 203d  p = 1..    s00 =
+000168e0: 2074 696d 652e 7469 6d65 2829 0d0a 2020   time.time()..  
+000168f0: 2020 7072 6f67 7265 7373 5f73 7061 6365    progress_space
+00016900: 2829 0d0a 0d0a 2020 2020 676c 6f62 616c  ()....    global
+00016910: 2073 6b69 705f 706f 7765 725f 6f66 5f74   skip_power_of_t
+00016920: 776f 5f63 6865 636b 0d0a 0d0a 2020 2020  wo_check....    
+00016930: 2320 7468 6520 7374 7269 6e67 2069 7320  # the string is 
+00016940: 6f66 2074 6865 2066 6f72 6d20 6161 6161  of the form aaaa
+00016950: 7c62 6262 0d0a 0d0a 2020 2020 7374 7269  |bbb....    stri
+00016960: 6e67 203d 2064 656e 756d 6572 6174 6528  ng = denumerate(
+00016970: 7374 7269 6e67 290d 0a0d 0a20 2020 200d  string)....    .
+00016980: 0a20 2020 204f 626a 203d 2049 6e70 4f62  .    Obj = InpOb
+00016990: 6a2e 636f 7079 2829 0d0a 2020 2020 7468  j.copy()..    th
+000169a0: 6973 5f74 7970 6520 3d20 7479 7065 284f  is_type = type(O
+000169b0: 626a 290d 0a20 2020 2074 6869 735f 666f  bj)..    this_fo
+000169c0: 726d 6174 203d 204f 626a 2e66 6f72 6d61  rmat = Obj.forma
+000169d0: 740d 0a20 2020 2074 6869 735f 656e 636f  t..    this_enco
+000169e0: 6465 7220 3d20 4f62 6a2e 656e 636f 6465  der = Obj.encode
+000169f0: 720d 0a20 2020 2058 4f62 6a5f 7374 6174  r..    XObj_stat
+00016a00: 7320 3d20 4f62 6a2e 7374 6174 6973 7469  s = Obj.statisti
+00016a10: 630d 0a20 2020 2058 4f62 6a5f 7368 6170  c..    XObj_shap
+00016a20: 6520 3d20 4f62 6a2e 7368 6170 650d 0a0d  e = Obj.shape...
+00016a30: 0a20 2020 2069 6620 7361 7665 5f6d 656d  .    if save_mem
+00016a40: 6f72 7920 3a0d 0a20 2020 2020 2020 2064  ory :..        d
+00016a50: 656c 2049 6e70 4f62 6a2e 6461 7461 0d0a  el InpObj.data..
+00016a60: 2020 2020 2020 2020 6465 6c20 496e 704f          del InpO
+00016a70: 626a 0d0a 2020 2020 2020 2020 6763 2e63  bj..        gc.c
+00016a80: 6f6c 6c65 6374 2829 0d0a 2020 2020 2020  ollect()..      
+00016a90: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
+00016aa0: 2020 6966 2874 6869 735f 7479 7065 3d3d    if(this_type==
+00016ab0: 7370 6172 7365 293a 0d0a 2020 2020 2020  sparse):..      
+00016ac0: 2020 4f62 6a20 3d20 6465 6e73 6528 4f62    Obj = dense(Ob
+00016ad0: 6a29 0d0a 2020 2020 6966 2874 6869 735f  j)..    if(this_
+00016ae0: 7479 7065 206e 6f74 2069 6e20 5b64 656e  type not in [den
+00016af0: 7365 2c73 7061 7273 655d 293a 0d0a 2020  se,sparse]):..  
+00016b00: 2020 2020 2020 6572 726f 7228 2245 7272        error("Err
+00016b10: 6f72 5b65 6967 5d3a 204f 626a 6563 7420  or[eig]: Object 
+00016b20: 7479 7065 206d 7573 7420 6f6e 6c79 2062  type must only b
+00016b30: 6520 6465 6e73 6520 6f72 2073 7061 7273  e dense or spars
+00016b40: 6521 2229 0d0a 2020 2020 2020 2020 0d0a  e!")..        ..
+00016b50: 2020 2020 2320 6368 6563 6b20 6966 204f      # check if O
+00016b60: 626a 2e73 7461 7469 7374 6963 206f 7220  bj.statistic or 
+00016b70: 6669 6e61 6c5f 7374 6174 6973 7469 6320  final_statistic 
+00016b80: 6973 2077 6569 7264 206f 7220 6e6f 740d  is weird or not.
+00016b90: 0a20 2020 2066 6f72 2073 7461 7420 696e  .    for stat in
+00016ba0: 204f 626a 2e73 7461 7469 7374 6963 3a0d   Obj.statistic:.
+00016bb0: 0a20 2020 2020 2020 2069 6628 7374 6174  .        if(stat
+00016bc0: 206e 6f74 2069 6e20 616c 6c6f 7765 645f   not in allowed_
+00016bd0: 7374 6174 293a 0d0a 2020 2020 2020 2020  stat):..        
+00016be0: 2020 2020 6572 726f 7228 2245 7272 6f72      error("Error
+00016bf0: 5b65 6967 5d3a 2054 6865 2069 6e70 7574  [eig]: The input
+00016c00: 206f 626a 6563 7420 636f 6e74 6169 6e73   object contains
+00016c10: 2069 6c6c 6567 616c 2073 7461 7469 7374   illegal statist
+00016c20: 6963 2e20 2830 2c20 312c 202d 312c 206f  ic. (0, 1, -1, o
+00016c30: 7220 222b 6879 6272 6964 5f73 796d 626f  r "+hybrid_symbo
+00016c40: 6c2b 2220 6f6e 6c79 2922 290d 0a0d 0a20  l+" only)").... 
+00016c50: 2020 2069 6620 7374 7269 6e67 2e63 6f75     if string.cou
+00016c60: 6e74 2822 2822 293d 3d73 7472 696e 672e  nt("(")==string.
+00016c70: 636f 756e 7428 2229 2229 2061 6e64 2073  count(")") and s
+00016c80: 7472 696e 672e 636f 756e 7428 2228 2229  tring.count("(")
+00016c90: 3e30 3a0d 0a20 2020 2020 2020 2073 7472  >0:..        str
+00016ca0: 696e 6720 3d20 7374 7269 6e67 2e72 6570  ing = string.rep
+00016cb0: 6c61 6365 2822 2022 2c22 2229 0d0a 2020  lace(" ","")..  
+00016cc0: 2020 2020 2020 7374 7269 6e67 203d 2073        string = s
+00016cd0: 7472 696e 672e 7265 706c 6163 6528 2229  tring.replace(")
+00016ce0: 2822 2c22 2022 290d 0a20 2020 2020 2020  ("," ")..       
+00016cf0: 2069 6620 7374 7269 6e67 2e63 6f75 6e74   if string.count
+00016d00: 2822 2822 293e 3120 6f72 2073 7472 696e  ("(")>1 or strin
+00016d10: 672e 636f 756e 7428 2229 2229 3c31 3a0d  g.count(")")<1:.
+00016d20: 0a20 2020 2020 2020 2020 2020 2065 7272  .            err
+00016d30: 6f72 2822 4572 726f 725b 6569 675d 3a20  or("Error[eig]: 
+00016d40: 5061 7265 6e74 6865 7365 7320 646f 6e27  Parentheses don'
+00016d50: 7420 6d61 7463 6822 290d 0a20 2020 2020  t match")..     
+00016d60: 2020 2073 7472 696e 6720 3d20 7374 7269     string = stri
+00016d70: 6e67 2e72 6570 6c61 6365 2822 2922 2c22  ng.replace(")","
+00016d80: 2229 0d0a 2020 2020 2020 2020 7374 7269  ")..        stri
+00016d90: 6e67 203d 2073 7472 696e 672e 7265 706c  ng = string.repl
+00016da0: 6163 6528 2228 222c 2222 290d 0a0d 0a20  ace("(","").... 
+00016db0: 2020 2070 6172 7469 7469 6f6e 5f63 6f75     partition_cou
+00016dc0: 6e74 203d 2030 0d0a 2020 2020 666f 7220  nt = 0..    for 
+00016dd0: 7061 7274 6974 696f 6e20 696e 2073 6570  partition in sep
+00016de0: 6172 6174 6f72 5f6c 6973 743a 0d0a 2020  arator_list:..  
+00016df0: 2020 2020 2020 7061 7274 6974 696f 6e5f        partition_
+00016e00: 636f 756e 7420 2b3d 2073 7472 696e 672e  count += string.
+00016e10: 636f 756e 7428 7061 7274 6974 696f 6e29  count(partition)
+00016e20: 0d0a 2020 2020 6966 2870 6172 7469 7469  ..    if(partiti
+00016e30: 6f6e 5f63 6f75 6e74 213d 3129 3a0d 0a20  on_count!=1):.. 
+00016e40: 2020 2020 2020 2070 6172 7469 7469 6f6e         partition
+00016e50: 5f73 7472 696e 6720 3d20 2222 0d0a 2020  _string = ""..  
+00016e60: 2020 2020 2020 666f 7220 692c 2070 6172        for i, par
+00016e70: 7469 7469 6f6e 2069 6e20 656e 756d 6572  tition in enumer
+00016e80: 6174 6528 7365 7061 7261 746f 725f 6c69  ate(separator_li
+00016e90: 7374 293a 0d0a 2020 2020 2020 2020 2020  st):..          
+00016ea0: 2020 6966 2869 3d3d 3029 3a0d 0a20 2020    if(i==0):..   
+00016eb0: 2020 2020 2020 2020 2020 2020 2070 6172               par
+00016ec0: 7469 7469 6f6e 5f73 7472 696e 6720 2b3d  tition_string +=
+00016ed0: 2022 2820 220d 0a20 2020 2020 2020 2020   "( "..         
+00016ee0: 2020 2065 6c69 6628 693d 3d6c 656e 2873     elif(i==len(s
+00016ef0: 6570 6172 6174 6f72 5f6c 6973 7429 2d31  eparator_list)-1
+00016f00: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00016f10: 2020 2020 7061 7274 6974 696f 6e5f 7374      partition_st
+00016f20: 7269 6e67 202b 3d20 222c 206f 7220 220d  ring += ", or ".
+00016f30: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00016f40: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00016f50: 2020 2020 7061 7274 6974 696f 6e5f 7374      partition_st
+00016f60: 7269 6e67 202b 3d20 222c 2022 0d0a 0d0a  ring += ", "....
+00016f70: 2020 2020 2020 2020 2020 2020 7061 7274              part
+00016f80: 6974 696f 6e5f 7374 7269 6e67 202b 3d20  ition_string += 
+00016f90: 2227 222b 7061 7274 6974 696f 6e2b 2227  "'"+partition+"'
+00016fa0: 220d 0a0d 0a20 2020 2020 2020 2020 2020  "....           
+00016fb0: 2069 6628 693d 3d6c 656e 2873 6570 6172   if(i==len(separ
+00016fc0: 6174 6f72 5f6c 6973 7429 2d31 293a 0d0a  ator_list)-1):..
+00016fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fe0: 7061 7274 6974 696f 6e5f 7374 7269 6e67  partition_string
+00016ff0: 202b 3d20 2220 2922 0d0a 0d0a 2020 2020   += " )"....    
+00017000: 2020 2020 6572 726f 7228 2245 7272 6f72      error("Error
+00017010: 5b65 6967 5d3a 2054 6865 2069 6e70 7574  [eig]: The input
+00017020: 2073 7472 696e 6720 6d75 7374 2063 6f6e   string must con
+00017030: 7461 696e 206f 6e65 2061 6e64 206f 6e6c  tain one and onl
+00017040: 7920 6f6e 6520 7061 7274 6974 696f 6e20  y one partition 
+00017050: 222b 7061 7274 6974 696f 6e5f 7374 7269  "+partition_stri
+00017060: 6e67 2b22 2069 6e20 6974 2e22 290d 0a20  ng+" in it.").. 
+00017070: 2020 200d 0a20 2020 2073 7465 7020 3d20     ..    step = 
+00017080: 7368 6f77 5f70 726f 6772 6573 7328 7374  show_progress(st
+00017090: 6570 2c70 726f 6365 7373 5f6c 656e 6774  ep,process_lengt
+000170a0: 682c 7072 6f63 6573 735f 6e61 6d65 2b22  h,process_name+"
+000170b0: 2022 2b22 3c22 2b63 7572 7265 6e74 5f6d   "+"<"+current_m
+000170c0: 656d 6f72 795f 6469 7370 6c61 7928 292b  emory_display()+
+000170d0: 223e 222c 636f 6c6f 723d 7072 6f63 6573  ">",color=proces
+000170e0: 735f 636f 6c6f 722c 7469 6d65 3d74 696d  s_color,time=tim
+000170f0: 652e 7469 6d65 2829 2d73 3030 2920 2331  e.time()-s00) #1
+00017100: 0d0a 2020 2020 233a 3a3a 3a3a 3a3a 3a3a  ..    #:::::::::
+00017110: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017120: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017130: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017140: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017150: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017160: 3a3a 3a3a 3a3a 3a0d 0a20 2020 2023 3a3a  :::::::..    #::
+00017170: 3a3a 3a20 2020 2020 2053 5445 5020 3120  :::      STEP 1 
+00017180: 2d20 4a4f 494e 204c 4547 5320 4241 4553  - JOIN LEGS BAES
+00017190: 4420 4f4e 2054 4845 2047 524f 5550 494e  D ON THE GROUPIN
+000171a0: 4753 2020 2020 2020 2020 2020 2020 2020  GS              
+000171b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171c0: 2020 2020 2020 2020 203a 3a3a 3a3a 0d0a           :::::..
+000171d0: 2020 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a      #:::::::::::
+000171e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000171f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017200: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017210: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017220: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017230: 3a3a 3a3a 3a0d 0a0d 0a20 2020 2023 2063  :::::....    # c
+00017240: 6f75 6e74 2074 6865 206e 756d 6265 7220  ount the number 
+00017250: 6f66 2069 6e64 6963 6573 2069 6e20 7468  of indices in th
+00017260: 6520 7477 6f20 6772 6f75 7073 0d0a 2020  e two groups..  
+00017270: 2020 6e5f 6c65 6674 203d 2030 0d0a 2020    n_left = 0..  
+00017280: 2020 6e5f 7269 6768 7420 3d20 300d 0a20    n_right = 0.. 
+00017290: 2020 2070 6172 7469 7469 6f6e 5f66 6f75     partition_fou
+000172a0: 6e64 203d 2046 616c 7365 0d0a 2020 2020  nd = False..    
+000172b0: 666f 7220 6368 6172 2069 6e20 7374 7269  for char in stri
+000172c0: 6e67 3a0d 0a20 2020 2020 2020 2069 6620  ng:..        if 
+000172d0: 6368 6172 2069 6e20 7365 7061 7261 746f  char in separato
+000172e0: 725f 6c69 7374 203a 0d0a 2020 2020 2020  r_list :..      
+000172f0: 2020 2020 2020 7061 7274 6974 696f 6e5f        partition_
+00017300: 666f 756e 6420 3d20 5472 7565 0d0a 2020  found = True..  
+00017310: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00017320: 7565 0d0a 2020 2020 2020 2020 6966 2870  ue..        if(p
+00017330: 6172 7469 7469 6f6e 5f66 6f75 6e64 293a  artition_found):
+00017340: 0d0a 2020 2020 2020 2020 2020 2020 6e5f  ..            n_
+00017350: 7269 6768 742b 3d31 0d0a 2020 2020 2020  right+=1..      
+00017360: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00017370: 2020 2020 206e 5f6c 6566 742b 3d31 0d0a       n_left+=1..
+00017380: 0d0a 2020 2020 6a6f 696e 5f6c 6567 735f  ..    join_legs_
+00017390: 7374 7269 6e67 5f69 6e70 7574 203d 2073  string_input = s
+000173a0: 7472 696e 670d 0a20 2020 2066 6f72 2070  tring..    for p
+000173b0: 6172 7469 7469 6f6e 2069 6e20 7365 7061  artition in sepa
+000173c0: 7261 746f 725f 6c69 7374 3a0d 0a20 2020  rator_list:..   
+000173d0: 2020 2020 206a 6f69 6e5f 6c65 6773 5f73       join_legs_s
+000173e0: 7472 696e 675f 696e 7075 7420 3d20 6a6f  tring_input = jo
+000173f0: 696e 5f6c 6567 735f 7374 7269 6e67 5f69  in_legs_string_i
+00017400: 6e70 7574 2e72 6570 6c61 6365 2870 6172  nput.replace(par
+00017410: 7469 7469 6f6e 2c22 2928 2229 0d0a 2020  tition,")(")..  
+00017420: 2020 6a6f 696e 5f6c 6567 735f 7374 7269    join_legs_stri
+00017430: 6e67 5f69 6e70 7574 203d 2022 2822 2b6a  ng_input = "("+j
+00017440: 6f69 6e5f 6c65 6773 5f73 7472 696e 675f  oin_legs_string_
+00017450: 696e 7075 742b 2229 220d 0a0d 0a20 2020  input+")"....   
+00017460: 2073 6861 7065 5f6c 6566 7420 203d 204f   shape_left  = O
+00017470: 626a 2e73 6861 7065 5b3a 6e5f 6c65 6674  bj.shape[:n_left
+00017480: 5d0d 0a20 2020 2073 7461 7473 5f6c 6566  ]..    stats_lef
+00017490: 7420 203d 204f 626a 2e73 7461 7469 7374  t  = Obj.statist
+000174a0: 6963 5b3a 6e5f 6c65 6674 5d0d 0a20 2020  ic[:n_left]..   
+000174b0: 2073 6861 7065 5f72 6967 6874 203d 204f   shape_right = O
+000174c0: 626a 2e73 6861 7065 5b6e 5f6c 6566 743a  bj.shape[n_left:
+000174d0: 5d0d 0a20 2020 2073 7461 7473 5f72 6967  ]..    stats_rig
+000174e0: 6874 203d 204f 626a 2e73 7461 7469 7374  ht = Obj.statist
+000174f0: 6963 5b6e 5f6c 6566 743a 5d0d 0a0d 0a20  ic[n_left:].... 
+00017500: 2020 2064 6566 207a 6572 6f5f 6f72 5f65     def zero_or_e
+00017510: 6c73 6528 7665 6374 6f72 2c76 616c 7565  lse(vector,value
+00017520: 293a 0d0a 2020 2020 2020 2020 666f 7220  ):..        for 
+00017530: 656c 656d 2069 6e20 7665 6374 6f72 3a0d  elem in vector:.
+00017540: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00017550: 656c 656d 213d 303a 0d0a 2020 2020 2020  elem!=0:..      
+00017560: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00017570: 2076 616c 7565 0d0a 2020 2020 2020 2020   value..        
+00017580: 7265 7475 726e 2030 0d0a 2020 2020 6465  return 0..    de
+00017590: 6620 6765 745f 7374 6174 2876 6563 746f  f get_stat(vecto
+000175a0: 722c 7072 6566 6572 3d4e 6f6e 6529 3a0d  r,prefer=None):.
+000175b0: 0a20 2020 2020 2020 2062 6f73 6f6e 5f63  .        boson_c
+000175c0: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
+000175d0: 2020 6665 726d 695f 636f 756e 7420 3d20    fermi_count = 
+000175e0: 300d 0a20 2020 2020 2020 2066 6f72 2065  0..        for e
+000175f0: 6c65 6d20 696e 2076 6563 746f 723a 0d0a  lem in vector:..
+00017600: 2020 2020 2020 2020 2020 2020 6966 2065              if e
+00017610: 6c65 6d20 696e 2062 6f73 655f 7479 7065  lem in bose_type
+00017620: 203a 0d0a 2020 2020 2020 2020 2020 2020   :..            
+00017630: 2020 2020 626f 736f 6e5f 636f 756e 7420      boson_count 
+00017640: 2b3d 2031 0d0a 2020 2020 2020 2020 2020  += 1..          
+00017650: 2020 6966 2065 6c65 6d20 696e 2066 6572    if elem in fer
+00017660: 6d69 5f74 7970 6520 3a0d 0a20 2020 2020  mi_type :..     
+00017670: 2020 2020 2020 2020 2020 2066 6572 6d69             fermi
+00017680: 5f63 6f75 6e74 202b 3d20 310d 0a0d 0a20  _count += 1.... 
+00017690: 2020 2020 2020 2069 6628 626f 736f 6e5f         if(boson_
+000176a0: 636f 756e 743d 3d30 2061 6e64 2066 6572  count==0 and fer
+000176b0: 6d69 5f63 6f75 6e74 3e30 293a 0d0a 2020  mi_count>0):..  
+000176c0: 2020 2020 2020 2020 2020 6966 2070 7265            if pre
+000176d0: 6665 7220 213d 204e 6f6e 653a 0d0a 2020  fer != None:..  
+000176e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000176f0: 7475 726e 2070 7265 6665 720d 0a20 2020  turn prefer..   
+00017700: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
+00017710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017720: 7265 7475 726e 2031 0d0a 2020 2020 2020  return 1..      
+00017730: 2020 656c 6966 2862 6f73 6f6e 5f63 6f75    elif(boson_cou
+00017740: 6e74 3e30 2061 6e64 2066 6572 6d69 5f63  nt>0 and fermi_c
+00017750: 6f75 6e74 3d3d 3029 3a0d 0a20 2020 2020  ount==0):..     
+00017760: 2020 2020 2020 2069 6620 7072 6566 6572         if prefer
+00017770: 2021 3d20 4e6f 6e65 3a0d 0a20 2020 2020   != None:..     
+00017780: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00017790: 6e20 7072 6566 6572 0d0a 2020 2020 2020  n prefer..      
+000177a0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+000177b0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000177c0: 7572 6e20 300d 0a20 2020 2020 2020 2065  urn 0..        e
+000177d0: 6c69 6628 626f 736f 6e5f 636f 756e 743e  lif(boson_count>
+000177e0: 3020 616e 6420 6665 726d 695f 636f 756e  0 and fermi_coun
+000177f0: 743e 3029 3a0d 0a20 2020 2020 2020 2020  t>0):..         
+00017800: 2020 2072 6574 7572 6e20 6879 6272 6964     return hybrid
+00017810: 5f73 796d 626f 6c0d 0a20 2020 200d 0a20  _symbol..    .. 
+00017820: 2020 2073 7465 7020 3d20 7368 6f77 5f70     step = show_p
+00017830: 726f 6772 6573 7328 7374 6570 2c70 726f  rogress(step,pro
+00017840: 6365 7373 5f6c 656e 6774 682c 7072 6f63  cess_length,proc
+00017850: 6573 735f 6e61 6d65 2b22 2022 2b22 3c22  ess_name+" "+"<"
+00017860: 2b63 7572 7265 6e74 5f6d 656d 6f72 795f  +current_memory_
+00017870: 6469 7370 6c61 7928 292b 223e 222c 636f  display()+">",co
+00017880: 6c6f 723d 7072 6f63 6573 735f 636f 6c6f  lor=process_colo
+00017890: 722c 7469 6d65 3d74 696d 652e 7469 6d65  r,time=time.time
+000178a0: 2829 2d73 3030 2920 2332 0d0a 2020 2020  ()-s00) #2..    
+000178b0: 696e 7465 726d 6564 6961 7465 5f73 7461  intermediate_sta
+000178c0: 7420 3d20 2820 7a65 726f 5f6f 725f 656c  t = ( zero_or_el
+000178d0: 7365 2873 7461 7473 5f6c 6566 742c 2d31  se(stats_left,-1
+000178e0: 292c 7a65 726f 5f6f 725f 656c 7365 2873  ),zero_or_else(s
+000178f0: 7461 7473 5f72 6967 6874 2c31 2920 290d  tats_right,1) ).
+00017900: 0a20 2020 204f 626a 203d 204f 626a 2e6a  .    Obj = Obj.j
+00017910: 6f69 6e5f 6c65 6773 286a 6f69 6e5f 6c65  oin_legs(join_le
+00017920: 6773 5f73 7472 696e 675f 696e 7075 742c  gs_string_input,
+00017930: 226d 6174 7269 7822 2c69 6e74 6572 6d65  "matrix",interme
+00017940: 6469 6174 655f 7374 6174 3d69 6e74 6572  diate_stat=inter
+00017950: 6d65 6469 6174 655f 7374 6174 2c73 6176  mediate_stat,sav
+00017960: 655f 6d65 6d6f 7279 3d54 7275 6529 0d0a  e_memory=True)..
+00017970: 0d0a 2020 2020 233a 3a3a 3a3a 3a3a 3a3a  ..    #:::::::::
+00017980: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017990: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000179a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000179b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000179c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000179d0: 3a3a 3a3a 3a3a 3a0d 0a20 2020 2023 3a3a  :::::::..    #::
+000179e0: 3a3a 3a20 2020 2020 2053 5445 5020 3220  :::      STEP 2 
+000179f0: 2d20 424c 4f43 4b20 5356 4420 284d 414b  - BLOCK SVD (MAK
+00017a00: 4520 5355 5245 2049 5427 5320 5041 5249  E SURE IT'S PARI
+00017a10: 5459 2d50 5245 5345 5256 494e 4721 2920  TY-PRESERVING!) 
+00017a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a30: 2020 2020 2020 2020 203a 3a3a 3a3a 0d0a           :::::..
+00017a40: 2020 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a      #:::::::::::
+00017a50: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017a60: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017a70: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017a80: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017a90: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017aa0: 3a3a 3a3a 3a0d 0a0d 0a20 2020 2073 7465  :::::....    ste
+00017ab0: 7020 3d20 7368 6f77 5f70 726f 6772 6573  p = show_progres
+00017ac0: 7328 7374 6570 2c70 726f 6365 7373 5f6c  s(step,process_l
+00017ad0: 656e 6774 682c 7072 6f63 6573 735f 6e61  ength,process_na
+00017ae0: 6d65 2b22 2022 2b22 3c22 2b63 7572 7265  me+" "+"<"+curre
+00017af0: 6e74 5f6d 656d 6f72 795f 6469 7370 6c61  nt_memory_displa
+00017b00: 7928 292b 223e 222c 636f 6c6f 723d 7072  y()+">",color=pr
+00017b10: 6f63 6573 735f 636f 6c6f 722c 7469 6d65  ocess_color,time
+00017b20: 3d74 696d 652e 7469 6d65 2829 2d73 3030  =time.time()-s00
+00017b30: 2920 2333 0d0a 2020 2020 6966 204f 626a  ) #3..    if Obj
+00017b40: 2e73 7461 7469 7374 6963 5b30 5d3d 3d30  .statistic[0]==0
+00017b50: 206f 7220 4f62 6a2e 7374 6174 6973 7469   or Obj.statisti
+00017b60: 635b 315d 3d3d 303a 0d0a 2020 2020 2020  c[1]==0:..      
+00017b70: 2020 552c 20ce 9b2c 2056 203d 2053 6f72    U, .., V = Sor
+00017b80: 7465 6445 6967 284f 626a 2e64 6174 612c  tedEig(Obj.data,
+00017b90: 6375 746f 6666 2c64 6562 7567 5f6d 6f64  cutoff,debug_mod
+00017ba0: 6529 0d0a 2020 2020 2020 2020 ce9b 203d  e)..        .. =
+00017bb0: 206e 702e 6469 6167 28ce 9b29 0d0a 2020   np.diag(..)..  
+00017bc0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00017bd0: 2055 2c20 ce9b 2c20 5620 3d20 426c 6f63   U, .., V = Bloc
+00017be0: 6b45 6967 284f 626a 2e64 6174 612c 6375  kEig(Obj.data,cu
+00017bf0: 746f 6666 2c64 6562 7567 5f6d 6f64 6529  toff,debug_mode)
+00017c00: 0d0a 0d0a 2020 2020 7374 6570 203d 2073  ....    step = s
+00017c10: 686f 775f 7072 6f67 7265 7373 2873 7465  how_progress(ste
+00017c20: 702c 7072 6f63 6573 735f 6c65 6e67 7468  p,process_length
+00017c30: 2c70 726f 6365 7373 5f6e 616d 652b 2220  ,process_name+" 
+00017c40: 222b 223c 222b 6375 7272 656e 745f 6d65  "+"<"+current_me
+00017c50: 6d6f 7279 5f64 6973 706c 6179 2829 2b22  mory_display()+"
+00017c60: 3e22 2c63 6f6c 6f72 3d70 726f 6365 7373  >",color=process
+00017c70: 5f63 6f6c 6f72 2c74 696d 653d 7469 6d65  _color,time=time
+00017c80: 2e74 696d 6528 292d 7330 3029 2023 340d  .time()-s00) #4.
+00017c90: 0a20 2020 2023 3a3a 3a3a 3a3a 3a3a 3a3a  .    #::::::::::
+00017ca0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017cb0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017cc0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017cd0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017ce0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017cf0: 3a3a 3a3a 3a3a 0d0a 2020 2020 233a 3a3a  ::::::..    #:::
+00017d00: 3a3a 2020 2020 2020 5354 4550 2033 202d  ::      STEP 3 -
+00017d10: 2052 4543 4f4e 5354 5255 4354 2055 2c20   RECONSTRUCT U, 
+00017d20: ce9b 2c20 616e 6420 5620 4153 2047 5241  .., and V AS GRA
+00017d30: 5353 4d41 4e4e 2054 454e 534f 5253 2020  SSMANN TENSORS  
+00017d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d50: 2020 2020 2020 2020 203a 3a3a 3a3a 0d0a           :::::..
+00017d60: 2020 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a      #:::::::::::
+00017d70: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017d80: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017d90: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017da0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017db0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00017dc0: 3a3a 3a3a 3a0d 0a0d 0a20 2020 2073 6b69  :::::....    ski
+00017dd0: 705f 706f 7765 725f 6f66 5f74 776f 5f63  p_power_of_two_c
+00017de0: 6865 636b 203d 2054 7275 650d 0a0d 0a20  heck = True.... 
+00017df0: 2020 2023 7468 6520 6669 7273 7420 7761     #the first wa
+00017e00: 7920 6973 2074 6f20 666f 726d 2074 6865  y is to form the
+00017e10: 2074 656e 736f 7220 6669 7273 742c 2074   tensor first, t
+00017e20: 6865 6e20 7370 6c69 740d 0a20 2020 20ce  hen split..    .
+00017e30: 9b73 7461 746c 6566 7420 3d20 2d31 0d0a  .statleft = -1..
+00017e40: 2020 2020 ce9b 7374 6174 7269 6768 7420      ..statright 
+00017e50: 3d20 2b31 0d0a 2020 2020 0d0a 2020 2020  = +1..    ..    
+00017e60: 6966 204f 626a 2e73 7461 7469 7374 6963  if Obj.statistic
+00017e70: 5b30 5d3d 3d30 3a0d 0a20 2020 2020 2020  [0]==0:..       
+00017e80: 2055 203d 2064 656e 7365 2855 2c65 6e63   U = dense(U,enc
+00017e90: 6f64 6572 3d22 7061 7269 7479 2d70 7265  oder="parity-pre
+00017ea0: 7365 7276 696e 6722 2c66 6f72 6d61 743d  serving",format=
+00017eb0: 226d 6174 7269 7822 2c73 7461 7469 7374  "matrix",statist
+00017ec0: 6963 3d28 302c 3029 290d 0a20 2020 2020  ic=(0,0))..     
+00017ed0: 2020 20ce 9b20 3d20 6465 6e73 6528 ce9b     .. = dense(..
+00017ee0: 2c65 6e63 6f64 6572 3d22 7061 7269 7479  ,encoder="parity
+00017ef0: 2d70 7265 7365 7276 696e 6722 2c66 6f72  -preserving",for
+00017f00: 6d61 743d 226d 6174 7269 7822 2c73 7461  mat="matrix",sta
+00017f10: 7469 7374 6963 3d28 302c 3029 290d 0a20  tistic=(0,0)).. 
+00017f20: 2020 2020 2020 2056 203d 2064 656e 7365         V = dense
+00017f30: 2856 2c65 6e63 6f64 6572 3d22 7061 7269  (V,encoder="pari
+00017f40: 7479 2d70 7265 7365 7276 696e 6722 2c66  ty-preserving",f
+00017f50: 6f72 6d61 743d 226d 6174 7269 7822 2c73  ormat="matrix",s
+00017f60: 7461 7469 7374 6963 3d28 302c 4f62 6a2e  tatistic=(0,Obj.
+00017f70: 7374 6174 6973 7469 635b 315d 2929 0d0a  statistic[1]))..
+00017f80: 2020 2020 2020 2020 ce9b 7374 6174 6c65          ..statle
+00017f90: 6674 203d 2030 0d0a 2020 2020 2020 2020  ft = 0..        
+00017fa0: ce9b 7374 6174 7269 6768 7420 3d20 300d  ..statright = 0.
+00017fb0: 0a20 2020 2065 6c69 6620 4f62 6a2e 7374  .    elif Obj.st
+00017fc0: 6174 6973 7469 635b 315d 3d3d 303a 0d0a  atistic[1]==0:..
+00017fd0: 2020 2020 2020 2020 5520 3d20 6465 6e73          U = dens
+00017fe0: 6528 552c 656e 636f 6465 723d 2270 6172  e(U,encoder="par
+00017ff0: 6974 792d 7072 6573 6572 7669 6e67 222c  ity-preserving",
+00018000: 666f 726d 6174 3d22 6d61 7472 6978 222c  format="matrix",
+00018010: 7374 6174 6973 7469 633d 284f 626a 2e73  statistic=(Obj.s
+00018020: 7461 7469 7374 6963 5b30 5d2c 3029 290d  tatistic[0],0)).
+00018030: 0a20 2020 2020 2020 20ce 9b20 3d20 6465  .        .. = de
+00018040: 6e73 6528 ce9b 2c65 6e63 6f64 6572 3d22  nse(..,encoder="
+00018050: 7061 7269 7479 2d70 7265 7365 7276 696e  parity-preservin
+00018060: 6722 2c66 6f72 6d61 743d 226d 6174 7269  g",format="matri
+00018070: 7822 2c73 7461 7469 7374 6963 3d28 302c  x",statistic=(0,
+00018080: 3029 290d 0a20 2020 2020 2020 2056 203d  0))..        V =
+00018090: 2064 656e 7365 2856 2c65 6e63 6f64 6572   dense(V,encoder
+000180a0: 3d22 7061 7269 7479 2d70 7265 7365 7276  ="parity-preserv
+000180b0: 696e 6722 2c66 6f72 6d61 743d 226d 6174  ing",format="mat
+000180c0: 7269 7822 2c73 7461 7469 7374 6963 3d28  rix",statistic=(
+000180d0: 302c 3029 290d 0a20 2020 2020 2020 20ce  0,0))..        .
+000180e0: 9b73 7461 746c 6566 7420 3d20 300d 0a20  .statleft = 0.. 
+000180f0: 2020 2020 2020 20ce 9b73 7461 7472 6967         ..statrig
+00018100: 6874 203d 2030 0d0a 2020 2020 656c 7365  ht = 0..    else
+00018110: 3a0d 0a20 2020 2020 2020 2055 203d 2064  :..        U = d
+00018120: 656e 7365 2855 2c65 6e63 6f64 6572 3d22  ense(U,encoder="
+00018130: 7061 7269 7479 2d70 7265 7365 7276 696e  parity-preservin
+00018140: 6722 2c66 6f72 6d61 743d 226d 6174 7269  g",format="matri
+00018150: 7822 2c73 7461 7469 7374 6963 3d28 4f62  x",statistic=(Ob
+00018160: 6a2e 7374 6174 6973 7469 635b 305d 2c31  j.statistic[0],1
+00018170: 2929 0d0a 2020 2020 2020 2020 ce9b 203d  ))..        .. =
+00018180: 2064 656e 7365 28ce 9b2c 656e 636f 6465   dense(..,encode
+00018190: 723d 2270 6172 6974 792d 7072 6573 6572  r="parity-preser
+000181a0: 7669 6e67 222c 666f 726d 6174 3d22 6d61  ving",format="ma
+000181b0: 7472 6978 222c 7374 6174 6973 7469 633d  trix",statistic=
+000181c0: 282d 312c 3129 290d 0a20 2020 2020 2020  (-1,1))..       
+000181d0: 2056 203d 2064 656e 7365 2856 2c65 6e63   V = dense(V,enc
+000181e0: 6f64 6572 3d22 7061 7269 7479 2d70 7265  oder="parity-pre
+000181f0: 7365 7276 696e 6722 2c66 6f72 6d61 743d  serving",format=
+00018200: 226d 6174 7269 7822 2c73 7461 7469 7374  "matrix",statist
+00018210: 6963 3d28 2d31 2c4f 626a 2e73 7461 7469  ic=(-1,Obj.stati
+00018220: 7374 6963 5b31 5d29 290d 0a20 2020 2064  stic[1]))..    d
+00018230: ce9b 203d 20ce 9b2e 7368 6170 655b 305d  .. = ...shape[0]
+00018240: 0d0a 0d0a 2020 2020 7374 6570 203d 2073  ....    step = s
+00018250: 686f 775f 7072 6f67 7265 7373 2873 7465  how_progress(ste
+00018260: 702c 7072 6f63 6573 735f 6c65 6e67 7468  p,process_length
+00018270: 2c70 726f 6365 7373 5f6e 616d 652b 2220  ,process_name+" 
+00018280: 222b 223c 222b 6375 7272 656e 745f 6d65  "+"<"+current_me
+00018290: 6d6f 7279 5f64 6973 706c 6179 2829 2b22  mory_display()+"
+000182a0: 3e22 2c63 6f6c 6f72 3d70 726f 6365 7373  >",color=process
+000182b0: 5f63 6f6c 6f72 2c74 696d 653d 7469 6d65  _color,time=time
+000182c0: 2e74 696d 6528 292d 7330 3029 2023 350d  .time()-s00) #5.
+000182d0: 0a20 2020 2073 6b69 705f 706f 7765 725f  .    skip_power_
+000182e0: 6f66 5f74 776f 5f63 6865 636b 203d 2046  of_two_check = F
+000182f0: 616c 7365 0d0a 2020 2020 233a 3a3a 3a3a  alse..    #:::::
+00018300: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00018310: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00018320: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00018330: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00018340: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00018350: 3a3a 3a3a 3a3a 3a3a 3a3a 3a0d 0a20 2020  :::::::::::..   
+00018360: 2023 3a3a 3a3a 3a20 2020 2020 2053 5445   #:::::      STE
+00018370: 5020 3420 2d20 5370 6c69 7420 7468 6520  P 4 - Split the 
+00018380: 6c65 6773 2020 2020 2020 2020 2020 2020  legs            
+00018390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183b0: 2020 2020 2020 2020 2020 2020 203a 3a3a               :::
+000183c0: 3a3a 0d0a 2020 2020 233a 3a3a 3a3a 3a3a  ::..    #:::::::
+000183d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000183e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000183f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00018400: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00018410: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00018420: 3a3a 3a3a 3a3a 3a3a 3a0d 0a0d 0a20 2020  :::::::::....   
+00018430: 2023 2063 6f75 6e74 2074 6865 206e 756d   # count the num
+00018440: 6265 7220 6f66 2069 6e64 6963 6573 2069  ber of indices i
+00018450: 6e20 7468 6520 7477 6f20 6772 6f75 7073  n the two groups
+00018460: 0d0a 2020 2020 5569 6e64 203d 2022 220d  ..    Uind = "".
+00018470: 0a20 2020 2056 696e 6420 3d20 2222 0d0a  .    Vind = ""..
+00018480: 2020 2020 5573 7461 7473 203d 205b 5d0d      Ustats = [].
+00018490: 0a20 2020 2056 7374 6174 7320 3d20 5b5d  .    Vstats = []
+000184a0: 0d0a 2020 2020 5573 6861 7065 203d 205b  ..    Ushape = [
+000184b0: 5d0d 0a20 2020 2056 7368 6170 6520 3d20  ]..    Vshape = 
+000184c0: 5b5d 0d0a 2020 2020 7061 7274 6974 696f  []..    partitio
+000184d0: 6e5f 666f 756e 6420 3d20 4661 6c73 650d  n_found = False.
+000184e0: 0a20 2020 2066 6f72 2069 2c63 6861 7220  .    for i,char 
+000184f0: 696e 2065 6e75 6d65 7261 7465 2873 7472  in enumerate(str
+00018500: 696e 6729 3a0d 0a20 2020 2020 2020 2069  ing):..        i
+00018510: 6620 6368 6172 2069 6e20 7365 7061 7261  f char in separa
+00018520: 746f 725f 6c69 7374 203a 0d0a 2020 2020  tor_list :..    
+00018530: 2020 2020 2020 2020 7061 7274 6974 696f          partitio
+00018540: 6e5f 666f 756e 6420 3d20 5472 7565 0d0a  n_found = True..
+00018550: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00018560: 696e 7565 0d0a 2020 2020 2020 2020 6966  inue..        if
+00018570: 2870 6172 7469 7469 6f6e 5f66 6f75 6e64  (partition_found
+00018580: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00018590: 5669 6e64 2b3d 6368 6172 0d0a 2020 2020  Vind+=char..    
+000185a0: 2020 2020 2020 2020 5673 7461 7473 2b3d          Vstats+=
+000185b0: 5b58 4f62 6a5f 7374 6174 735b 692d 315d  [XObj_stats[i-1]
+000185c0: 5d0d 0a20 2020 2020 2020 2020 2020 2056  ]..            V
+000185d0: 7368 6170 652b 3d5b 584f 626a 5f73 6861  shape+=[XObj_sha
+000185e0: 7065 5b69 2d31 5d5d 0d0a 2020 2020 2020  pe[i-1]]..      
+000185f0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+00018600: 2020 2020 2055 696e 642b 3d63 6861 720d       Uind+=char.
+00018610: 0a20 2020 2020 2020 2020 2020 2055 7374  .            Ust
+00018620: 6174 732b 3d5b 584f 626a 5f73 7461 7473  ats+=[XObj_stats
+00018630: 5b69 5d5d 0d0a 2020 2020 2020 2020 2020  [i]]..          
+00018640: 2020 5573 6861 7065 2b3d 5b58 4f62 6a5f    Ushape+=[XObj_
+00018650: 7368 6170 655b 695d 5d0d 0a0d 0a20 2020  shape[i]]....   
+00018660: 206e 6577 5f69 6e64 3120 3d20 2222 0d0a   new_ind1 = ""..
+00018670: 2020 2020 666f 7220 6368 6172 2069 6e20      for char in 
+00018680: 6368 6172 5f6c 6973 743a 0d0a 2020 2020  char_list:..    
+00018690: 2020 2020 6966 2063 6861 7220 6e6f 7420      if char not 
+000186a0: 696e 2055 696e 642b 5669 6e64 3a0d 0a20  in Uind+Vind:.. 
+000186b0: 2020 2020 2020 2020 2020 206e 6577 5f69             new_i
+000186c0: 6e64 3120 3d20 6368 6172 0d0a 2020 2020  nd1 = char..    
+000186d0: 2020 2020 2020 2020 6272 6561 6b0d 0a0d          break...
+000186e0: 0a20 2020 2055 696e 6420 2020 3d20 2228  .    Uind   = "(
+000186f0: 222b 5569 6e64 2b22 2922 202b 206e 6577  "+Uind+")" + new
+00018700: 5f69 6e64 310d 0a20 2020 2056 696e 6420  _ind1..    Vind 
+00018710: 2020 3d20 6e65 775f 696e 6431 202b 2022    = new_ind1 + "
+00018720: 2822 2b56 696e 642b 2229 220d 0a20 2020  ("+Vind+")"..   
+00018730: 2055 7374 6174 7320 3d20 7475 706c 6528   Ustats = tuple(
+00018740: 5573 7461 7473 202b 205b 2dce 9b73 7461  Ustats + [-..sta
+00018750: 746c 6566 745d 290d 0a20 2020 2056 7374  tleft])..    Vst
+00018760: 6174 7320 3d20 7475 706c 6528 5b2d ce9b  ats = tuple([-..
+00018770: 7374 6174 7269 6768 745d 202b 2056 7374  statright] + Vst
+00018780: 6174 7329 0d0a 2020 2020 5573 6861 7065  ats)..    Ushape
+00018790: 203d 2074 7570 6c65 2855 7368 6170 6520   = tuple(Ushape 
+000187a0: 2b20 5b64 ce9b 5d29 0d0a 2020 2020 5673  + [d..])..    Vs
+000187b0: 6861 7065 203d 2074 7570 6c65 285b 64ce  hape = tuple([d.
+000187c0: 9b5d 202b 2056 7368 6170 6529 0d0a 2020  .] + Vshape)..  
+000187d0: 2020 0d0a 2020 2020 7374 6570 203d 2073    ..    step = s
+000187e0: 686f 775f 7072 6f67 7265 7373 2873 7465  how_progress(ste
+000187f0: 702c 7072 6f63 6573 735f 6c65 6e67 7468  p,process_length
+00018800: 2c70 726f 6365 7373 5f6e 616d 652b 2220  ,process_name+" 
+00018810: 222b 223c 222b 6375 7272 656e 745f 6d65  "+"<"+current_me
+00018820: 6d6f 7279 5f64 6973 706c 6179 2829 2b22  mory_display()+"
+00018830: 3e22 2c63 6f6c 6f72 3d70 726f 6365 7373  >",color=process
+00018840: 5f63 6f6c 6f72 2c74 696d 653d 7469 6d65  _color,time=time
+00018850: 2e74 696d 6528 292d 7330 3029 2023 360d  .time()-s00) #6.
+00018860: 0a20 2020 2055 203d 2055 2e73 706c 6974  .    U = U.split
+00018870: 5f6c 6567 7328 5569 6e64 2c55 7374 6174  _legs(Uind,Ustat
+00018880: 732c 5573 6861 7065 2c73 6176 655f 6d65  s,Ushape,save_me
+00018890: 6d6f 7279 3d54 7275 6529 0d0a 2020 2020  mory=True)..    
+000188a0: ce9b 203d 20ce 9b2e 7377 6974 6368 5f65  .. = ...switch_e
+000188b0: 6e63 6f64 6572 2873 6176 655f 6d65 6d6f  ncoder(save_memo
+000188c0: 7279 3d54 7275 6529 0d0a 2020 2020 5620  ry=True)..    V 
+000188d0: 3d20 562e 7370 6c69 745f 6c65 6773 2856  = V.split_legs(V
+000188e0: 696e 642c 5673 7461 7473 2c56 7368 6170  ind,Vstats,Vshap
+000188f0: 652c 7361 7665 5f6d 656d 6f72 793d 5472  e,save_memory=Tr
+00018900: 7565 290d 0a20 2020 200d 0a20 2020 2069  ue)..    ..    i
+00018910: 6628 7468 6973 5f66 6f72 6d61 7420 3d3d  f(this_format ==
+00018920: 2027 7374 616e 6461 7264 2729 3a0d 0a20   'standard'):.. 
+00018930: 2020 2020 2020 2055 203d 2055 2e73 7769         U = U.swi
+00018940: 7463 685f 666f 726d 6174 2873 6176 655f  tch_format(save_
+00018950: 6d65 6d6f 7279 3d54 7275 6529 0d0a 2020  memory=True)..  
+00018960: 2020 2020 2020 ce9b 203d 20ce 9b2e 7377        .. = ...sw
+00018970: 6974 6368 5f66 6f72 6d61 7428 7361 7665  itch_format(save
+00018980: 5f6d 656d 6f72 793d 5472 7565 290d 0a20  _memory=True).. 
+00018990: 2020 2020 2020 2056 203d 2056 2e73 7769         V = V.swi
+000189a0: 7463 685f 666f 726d 6174 2873 6176 655f  tch_format(save_
+000189b0: 6d65 6d6f 7279 3d54 7275 6529 0d0a 0d0a  memory=True)....
+000189c0: 2020 2020 6966 2874 6869 735f 656e 636f      if(this_enco
+000189d0: 6465 7220 3d3d 2027 7061 7269 7479 2d70  der == 'parity-p
+000189e0: 7265 7365 7276 696e 6727 293a 0d0a 2020  reserving'):..  
+000189f0: 2020 2020 2020 5520 3d20 552e 7377 6974        U = U.swit
+00018a00: 6368 5f65 6e63 6f64 6572 2873 6176 655f  ch_encoder(save_
+00018a10: 6d65 6d6f 7279 3d54 7275 6529 0d0a 2020  memory=True)..  
+00018a20: 2020 2020 2020 ce9b 203d 20ce 9b2e 7377        .. = ...sw
+00018a30: 6974 6368 5f65 6e63 6f64 6572 2873 6176  itch_encoder(sav
+00018a40: 655f 6d65 6d6f 7279 3d54 7275 6529 0d0a  e_memory=True)..
+00018a50: 2020 2020 2020 2020 5620 3d20 562e 7377          V = V.sw
+00018a60: 6974 6368 5f65 6e63 6f64 6572 2873 6176  itch_encoder(sav
+00018a70: 655f 6d65 6d6f 7279 3d54 7275 6529 0d0a  e_memory=True)..
+00018a80: 0d0a 2020 2020 6966 2874 6869 735f 7479  ..    if(this_ty
+00018a90: 7065 3d3d 7370 6172 7365 293a 0d0a 2020  pe==sparse):..  
+00018aa0: 2020 2020 2020 5520 3d20 7370 6172 7365        U = sparse
+00018ab0: 2855 290d 0a20 2020 2020 2020 20ce 9b20  (U)..        .. 
+00018ac0: 3d20 7370 6172 7365 28ce 9b29 0d0a 2020  = sparse(..)..  
+00018ad0: 2020 2020 2020 5620 3d20 7370 6172 7365        V = sparse
+00018ae0: 2856 290d 0a0d 0a20 2020 2063 6c65 6172  (V)....    clear
+00018af0: 5f70 726f 6772 6573 7328 290d 0a20 2020  _progress()..   
+00018b00: 2074 6162 5f75 7028 290d 0a20 2020 200d   tab_up()..    .
+00018b10: 0a20 2020 2072 6574 7572 6e20 552c 20ce  .    return U, .
+00018b20: 9b2c 2056 0d0a 0d0a 2323 2323 2323 2323  ., V....########
+00018b30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018b40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018b50: 2323 2323 2323 2323 2323 2323 0d0a 2323  ############..##
+00018b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b70: 2020 2043 6f6e 6a75 6761 7469 6f6e 2020     Conjugation  
+00018b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b90: 2323 0d0a 2323 2323 2323 2323 2323 2323  ##..############
+00018ba0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018bb0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018bc0: 2323 2323 2323 2323 0d0a 0d0a 6465 6620  ########....def 
+00018bd0: 6863 6f6e 6a75 6761 7465 2849 6e70 4f62  hconjugate(InpOb
+00018be0: 6a2c 7374 7269 6e67 2c73 6176 655f 6d65  j,string,save_me
+00018bf0: 6d6f 7279 3d46 616c 7365 293a 0d0a 0d0a  mory=False):....
+00018c00: 2020 2020 7072 6f63 6573 735f 6e61 6d65      process_name
+00018c10: 203d 2022 6863 6f6e 6a75 6761 7465 220d   = "hconjugate".
+00018c20: 0a20 2020 2070 726f 6365 7373 5f6c 656e  .    process_len
+00018c30: 6774 6820 3d20 360d 0a20 2020 2070 726f  gth = 6..    pro
+00018c40: 6365 7373 5f63 6f6c 6f72 3d22 7965 6c6c  cess_color="yell
+00018c50: 6f77 220d 0a20 2020 2073 7465 7020 3d20  ow"..    step = 
+00018c60: 310d 0a20 2020 2073 3030 203d 2074 696d  1..    s00 = tim
+00018c70: 652e 7469 6d65 2829 0d0a 2020 2020 7072  e.time()..    pr
+00018c80: 6f67 7265 7373 5f73 7061 6365 2829 2023  ogress_space() #
+00018c90: 203c 3c20 446f 6e27 7420 7265 6d6f 7665   << Don't remove
+00018ca0: 2074 6869 732e 2054 6869 7320 6973 2066   this. This is f
+00018cb0: 6f72 2074 6865 2073 686f 775f 7072 6f67  or the show_prog
+00018cc0: 7265 7373 210d 0a0d 0a20 2020 2073 7472  ress!....    str
+00018cd0: 696e 6720 3d20 6465 6e75 6d65 7261 7465  ing = denumerate
+00018ce0: 2873 7472 696e 6729 0d0a 2020 2020 0d0a  (string)..    ..
+00018cf0: 2020 2020 6966 2073 7472 696e 672e 636f      if string.co
+00018d00: 756e 7428 2228 2229 3d3d 7374 7269 6e67  unt("(")==string
+00018d10: 2e63 6f75 6e74 2822 2922 2920 616e 6420  .count(")") and 
+00018d20: 7374 7269 6e67 2e63 6f75 6e74 2822 2822  string.count("("
+00018d30: 293e 303a 0d0a 2020 2020 2020 2020 7374  )>0:..        st
+00018d40: 7269 6e67 203d 2073 7472 696e 672e 7265  ring = string.re
+00018d50: 706c 6163 6528 2220 222c 2222 290d 0a20  place(" ","").. 
+00018d60: 2020 2020 2020 2073 7472 696e 6720 3d20         string = 
+00018d70: 7374 7269 6e67 2e72 6570 6c61 6365 2822  string.replace("
+00018d80: 2928 222c 2220 2229 0d0a 2020 2020 2020  )("," ")..      
+00018d90: 2020 6966 2073 7472 696e 672e 636f 756e    if string.coun
+00018da0: 7428 2228 2229 3e31 206f 7220 7374 7269  t("(")>1 or stri
+00018db0: 6e67 2e63 6f75 6e74 2822 2922 293c 313a  ng.count(")")<1:
+00018dc0: 0d0a 2020 2020 2020 2020 2020 2020 6572  ..            er
+00018dd0: 726f 7228 2245 7272 6f72 5b68 636f 6e6a  ror("Error[hconj
+00018de0: 7567 6174 655d 3a20 5061 7265 6e74 6865  ugate]: Parenthe
+00018df0: 7365 7320 646f 6e27 7420 6d61 7463 6822  ses don't match"
+00018e00: 290d 0a20 2020 2020 2020 2073 7472 696e  )..        strin
+00018e10: 6720 3d20 7374 7269 6e67 2e72 6570 6c61  g = string.repla
+00018e20: 6365 2822 2922 2c22 2229 0d0a 2020 2020  ce(")","")..    
+00018e30: 2020 2020 7374 7269 6e67 203d 2073 7472      string = str
+00018e40: 696e 672e 7265 706c 6163 6528 2228 222c  ing.replace("(",
+00018e50: 2222 290d 0a0d 0a0d 0a20 2020 2023 2074  "")......    # t
+00018e60: 6865 2073 7472 696e 6720 6973 206f 6620  he string is of 
+00018e70: 7468 6520 666f 726d 2061 6161 617c 6262  the form aaaa|bb
+00018e80: 620d 0a0d 0a20 2020 204f 626a 203d 2049  b....    Obj = I
+00018e90: 6e70 4f62 6a2e 636f 7079 2829 0d0a 2020  npObj.copy()..  
+00018ea0: 2020 7468 6973 5f74 7970 6520 3d20 7479    this_type = ty
+00018eb0: 7065 284f 626a 290d 0a20 2020 2074 6869  pe(Obj)..    thi
+00018ec0: 735f 666f 726d 6174 203d 204f 626a 2e66  s_format = Obj.f
+00018ed0: 6f72 6d61 740d 0a20 2020 2074 6869 735f  ormat..    this_
+00018ee0: 656e 636f 6465 7220 3d20 4f62 6a2e 656e  encoder = Obj.en
+00018ef0: 636f 6465 720d 0a20 2020 2058 4f62 6a5f  coder..    XObj_
+00018f00: 7374 6174 7320 3d20 4f62 6a2e 7374 6174  stats = Obj.stat
+00018f10: 6973 7469 630d 0a20 2020 2058 4f62 6a5f  istic..    XObj_
+00018f20: 7368 6170 6520 3d20 4f62 6a2e 7368 6170  shape = Obj.shap
+00018f30: 650d 0a0d 0a20 2020 2069 6620 7361 7665  e....    if save
+00018f40: 5f6d 656d 6f72 7920 3a0d 0a20 2020 2020  _memory :..     
+00018f50: 2020 2064 656c 2049 6e70 4f62 6a2e 6461     del InpObj.da
+00018f60: 7461 0d0a 2020 2020 2020 2020 6465 6c20  ta..        del 
+00018f70: 496e 704f 626a 0d0a 2020 2020 2020 2020  InpObj..        
+00018f80: 6763 2e63 6f6c 6c65 6374 2829 0d0a 0d0a  gc.collect()....
+00018f90: 2020 2020 2369 6620 7468 6973 5f74 7970      #if this_typ
+00018fa0: 653d 3d73 7061 7273 6520 3a0d 0a20 2020  e==sparse :..   
+00018fb0: 2023 2020 2020 4f62 6a20 3d20 6465 6e73   #    Obj = dens
+00018fc0: 6528 4f62 6a29 0d0a 2020 2020 6966 2074  e(Obj)..    if t
+00018fd0: 6869 735f 7479 7065 206e 6f74 2069 6e20  his_type not in 
+00018fe0: 5b64 656e 7365 2c73 7061 7273 655d 203a  [dense,sparse] :
+00018ff0: 0d0a 2020 2020 2020 2020 6572 726f 7228  ..        error(
+00019000: 2245 7272 6f72 5b68 636f 6e6a 7567 6174  "Error[hconjugat
+00019010: 655d 3a20 4f62 6a65 6374 2074 7970 6520  e]: Object type 
+00019020: 6d75 7374 206f 6e6c 7920 6265 2064 656e  must only be den
+00019030: 7365 206f 7220 7370 6172 7365 2122 290d  se or sparse!").
+00019040: 0a20 2020 2020 2020 200d 0a20 2020 2023  .        ..    #
+00019050: 2063 6865 636b 2069 6620 4f62 6a2e 7374   check if Obj.st
+00019060: 6174 6973 7469 6320 6f72 2066 696e 616c  atistic or final
+00019070: 5f73 7461 7469 7374 6963 2069 7320 7765  _statistic is we
+00019080: 6972 6420 6f72 206e 6f74 0d0a 2020 2020  ird or not..    
+00019090: 666f 7220 7374 6174 2069 6e20 4f62 6a2e  for stat in Obj.
+000190a0: 7374 6174 6973 7469 633a 0d0a 2020 2020  statistic:..    
+000190b0: 2020 2020 6966 2873 7461 7420 6e6f 7420      if(stat not 
+000190c0: 696e 2061 6c6c 6f77 6564 5f73 7461 7429  in allowed_stat)
+000190d0: 3a0d 0a20 2020 2020 2020 2020 2020 2065  :..            e
+000190e0: 7272 6f72 2822 4572 726f 725b 6863 6f6e  rror("Error[hcon
+000190f0: 6a75 6761 7465 5d3a 2054 6865 2069 6e70  jugate]: The inp
+00019100: 7574 206f 626a 6563 7420 636f 6e74 6169  ut object contai
+00019110: 6e73 2069 6c6c 6567 616c 2073 7461 7469  ns illegal stati
+00019120: 7374 6963 2e20 2830 2c20 312c 202d 312c  stic. (0, 1, -1,
+00019130: 206f 7220 222b 6879 6272 6964 5f73 796d   or "+hybrid_sym
+00019140: 626f 6c2b 2220 6f6e 6c79 2922 290d 0a20  bol+" only)").. 
+00019150: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00019160: 2070 6172 7469 7469 6f6e 5f63 6f75 6e74   partition_count
+00019170: 203d 2030 0d0a 2020 2020 666f 7220 7061   = 0..    for pa
+00019180: 7274 6974 696f 6e20 696e 2073 6570 6172  rtition in separ
+00019190: 6174 6f72 5f6c 6973 743a 0d0a 2020 2020  ator_list:..    
+000191a0: 2020 2020 7061 7274 6974 696f 6e5f 636f      partition_co
+000191b0: 756e 7420 2b3d 2073 7472 696e 672e 636f  unt += string.co
+000191c0: 756e 7428 7061 7274 6974 696f 6e29 0d0a  unt(partition)..
+000191d0: 2020 2020 6966 2870 6172 7469 7469 6f6e      if(partition
+000191e0: 5f63 6f75 6e74 213d 3129 3a0d 0a20 2020  _count!=1):..   
+000191f0: 2020 2020 2070 6172 7469 7469 6f6e 5f73       partition_s
+00019200: 7472 696e 6720 3d20 2222 0d0a 2020 2020  tring = ""..    
+00019210: 2020 2020 666f 7220 692c 2070 6172 7469      for i, parti
+00019220: 7469 6f6e 2069 6e20 656e 756d 6572 6174  tion in enumerat
+00019230: 6528 7365 7061 7261 746f 725f 6c69 7374  e(separator_list
+00019240: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00019250: 6966 2869 3d3d 3029 3a0d 0a20 2020 2020  if(i==0):..     
+00019260: 2020 2020 2020 2020 2020 2070 6172 7469             parti
+00019270: 7469 6f6e 5f73 7472 696e 6720 2b3d 2022  tion_string += "
+00019280: 2820 220d 0a20 2020 2020 2020 2020 2020  ( "..           
+00019290: 2065 6c69 6628 693d 3d6c 656e 2873 6570   elif(i==len(sep
+000192a0: 6172 6174 6f72 5f6c 6973 7429 2d31 293a  arator_list)-1):
+000192b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000192c0: 2020 7061 7274 6974 696f 6e5f 7374 7269    partition_stri
+000192d0: 6e67 202b 3d20 222c 206f 7220 220d 0a20  ng += ", or ".. 
+000192e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000192f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019300: 2020 7061 7274 6974 696f 6e5f 7374 7269    partition_stri
+00019310: 6e67 202b 3d20 222c 2022 0d0a 0d0a 2020  ng += ", "....  
+00019320: 2020 2020 2020 2020 2020 7061 7274 6974            partit
+00019330: 696f 6e5f 7374 7269 6e67 202b 3d20 2227  ion_string += "'
+00019340: 222b 7061 7274 6974 696f 6e2b 2227 220d  "+partition+"'".
+00019350: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
+00019360: 6628 693d 3d6c 656e 2873 6570 6172 6174  f(i==len(separat
+00019370: 6f72 5f6c 6973 7429 2d31 293a 0d0a 2020  or_list)-1):..  
+00019380: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00019390: 7274 6974 696f 6e5f 7374 7269 6e67 202b  rtition_string +
+000193a0: 3d20 2220 2922 0d0a 0d0a 2020 2020 2020  = " )"....      
+000193b0: 2020 6572 726f 7228 2245 7272 6f72 5b68    error("Error[h
+000193c0: 636f 6e6a 7567 6174 655d 3a20 5468 6520  conjugate]: The 
+000193d0: 696e 7075 7420 7374 7269 6e67 206d 7573  input string mus
+000193e0: 7420 636f 6e74 6169 6e20 6f6e 6520 616e  t contain one an
+000193f0: 6420 6f6e 6c79 206f 6e65 2070 6172 7469  d only one parti
+00019400: 7469 6f6e 2022 2b70 6172 7469 7469 6f6e  tion "+partition
+00019410: 5f73 7472 696e 672b 2220 696e 2069 742e  _string+" in it.
+00019420: 2229 0d0a 2020 2020 0d0a 2020 2020 7374  ")..    ..    st
+00019430: 6570 203d 2073 686f 775f 7072 6f67 7265  ep = show_progre
+00019440: 7373 2873 7465 702c 7072 6f63 6573 735f  ss(step,process_
+00019450: 6c65 6e67 7468 2c70 726f 6365 7373 5f6e  length,process_n
+00019460: 616d 652b 2220 222b 223c 222b 6375 7272  ame+" "+"<"+curr
+00019470: 656e 745f 6d65 6d6f 7279 5f64 6973 706c  ent_memory_displ
+00019480: 6179 2829 2b22 3e22 2c63 6f6c 6f72 3d70  ay()+">",color=p
+00019490: 726f 6365 7373 5f63 6f6c 6f72 2c74 696d  rocess_color,tim
+000194a0: 653d 7469 6d65 2e74 696d 6528 292d 7330  e=time.time()-s0
+000194b0: 3029 0d0a 2020 2020 233a 3a3a 3a3a 3a3a  0)..    #:::::::
+000194c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000194d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000194e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000194f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00019500: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00019510: 3a3a 3a3a 3a3a 3a3a 3a0d 0a20 2020 2023  :::::::::..    #
+00019520: 3a3a 3a3a 3a20 2020 2020 2053 5445 5020  :::::      STEP 
+00019530: 3120 2d20 4a4f 494e 204c 4547 5320 4241  1 - JOIN LEGS BA
+00019540: 4553 4420 4f4e 2054 4845 2047 524f 5550  ESD ON THE GROUP
+00019550: 494e 4753 2020 2020 2020 2020 2020 2020  INGS            
+00019560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019570: 2020 2020 2020 2020 2020 203a 3a3a 3a3a             :::::
+00019580: 0d0a 2020 2020 233a 3a3a 3a3a 3a3a 3a3a  ..    #:::::::::
+00019590: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000195a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000195b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000195c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000195d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+000195e0: 3a3a 3a3a 3a3a 3a0d 0a0d 0a20 2020 2023  :::::::....    #
+000195f0: 2063 6f75 6e74 2074 6865 206e 756d 6265   count the numbe
+00019600: 7220 6f66 2069 6e64 6963 6573 2069 6e20  r of indices in 
+00019610: 7468 6520 7477 6f20 6772 6f75 7073 0d0a  the two groups..
+00019620: 2020 2020 6e5f 6c65 6674 203d 2030 0d0a      n_left = 0..
+00019630: 2020 2020 6e5f 7269 6768 7420 3d20 300d      n_right = 0.
+00019640: 0a20 2020 2070 6172 7469 7469 6f6e 5f66  .    partition_f
+00019650: 6f75 6e64 203d 2046 616c 7365 0d0a 2020  ound = False..  
+00019660: 2020 666f 7220 6368 6172 2069 6e20 7374    for char in st
+00019670: 7269 6e67 3a0d 0a20 2020 2020 2020 2069  ring:..        i
+00019680: 6620 6368 6172 2069 6e20 7365 7061 7261  f char in separa
+00019690: 746f 725f 6c69 7374 203a 0d0a 2020 2020  tor_list :..    
+000196a0: 2020 2020 2020 2020 7061 7274 6974 696f          partitio
+000196b0: 6e5f 666f 756e 6420 3d20 5472 7565 0d0a  n_found = True..
+000196c0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+000196d0: 696e 7565 0d0a 2020 2020 2020 2020 6966  inue..        if
+000196e0: 2870 6172 7469 7469 6f6e 5f66 6f75 6e64  (partition_found
+000196f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00019700: 6e5f 7269 6768 742b 3d31 0d0a 2020 2020  n_right+=1..    
+00019710: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00019720: 2020 2020 2020 206e 5f6c 6566 742b 3d31         n_left+=1
+00019730: 0d0a 0d0a 2020 2020 6a6f 696e 5f6c 6567  ....    join_leg
+00019740: 735f 7374 7269 6e67 5f69 6e70 7574 203d  s_string_input =
+00019750: 2073 7472 696e 670d 0a20 2020 2066 6f72   string..    for
+00019760: 2070 6172 7469 7469 6f6e 2069 6e20 7365   partition in se
+00019770: 7061 7261 746f 725f 6c69 7374 3a0d 0a20  parator_list:.. 
+00019780: 2020 2020 2020 206a 6f69 6e5f 6c65 6773         join_legs
+00019790: 5f73 7472 696e 675f 696e 7075 7420 3d20  _string_input = 
+000197a0: 6a6f 696e 5f6c 6567 735f 7374 7269 6e67  join_legs_string
+000197b0: 5f69 6e70 7574 2e72 6570 6c61 6365 2870  _input.replace(p
+000197c0: 6172 7469 7469 6f6e 2c22 2928 2229 0d0a  artition,")(")..
+000197d0: 2020 2020 6a6f 696e 5f6c 6567 735f 7374      join_legs_st
+000197e0: 7269 6e67 5f69 6e70 7574 203d 2022 2822  ring_input = "("
+000197f0: 2b6a 6f69 6e5f 6c65 6773 5f73 7472 696e  +join_legs_strin
+00019800: 675f 696e 7075 742b 2229 220d 0a0d 0a20  g_input+")".... 
+00019810: 2020 2073 6861 7065 5f6c 6566 7420 203d     shape_left  =
+00019820: 204f 626a 2e73 6861 7065 5b3a 6e5f 6c65   Obj.shape[:n_le
+00019830: 6674 5d0d 0a20 2020 2073 7461 7473 5f6c  ft]..    stats_l
+00019840: 6566 7420 203d 204f 626a 2e73 7461 7469  eft  = Obj.stati
+00019850: 7374 6963 5b3a 6e5f 6c65 6674 5d0d 0a20  stic[:n_left].. 
+00019860: 2020 2073 6861 7065 5f72 6967 6874 203d     shape_right =
+00019870: 204f 626a 2e73 6861 7065 5b6e 5f6c 6566   Obj.shape[n_lef
+00019880: 743a 5d0d 0a20 2020 2073 7461 7473 5f72  t:]..    stats_r
+00019890: 6967 6874 203d 204f 626a 2e73 7461 7469  ight = Obj.stati
+000198a0: 7374 6963 5b6e 5f6c 6566 743a 5d0d 0a20  stic[n_left:].. 
+000198b0: 2020 2064 6566 2070 726f 6428 7665 6374     def prod(vect
+000198c0: 6f72 293a 0d0a 2020 2020 2020 2020 7265  or):..        re
+000198d0: 7420 3d20 310d 0a20 2020 2020 2020 2066  t = 1..        f
+000198e0: 6f72 2065 6c65 6d20 696e 2076 6563 746f  or elem in vecto
+000198f0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+00019900: 7265 7420 2a3d 2065 6c65 6d0d 0a20 2020  ret *= elem..   
+00019910: 2020 2020 2072 6574 7572 6e20 7265 740d       return ret.
+00019920: 0a20 2020 2064 6566 2067 6574 5f73 7461  .    def get_sta
+00019930: 7428 7665 6374 6f72 2c70 7265 6665 723d  t(vector,prefer=
+00019940: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
+00019950: 626f 736f 6e5f 636f 756e 7420 3d20 300d  boson_count = 0.
+00019960: 0a20 2020 2020 2020 2066 6572 6d69 5f63  .        fermi_c
+00019970: 6f75 6e74 203d 2030 0d0a 2020 2020 2020  ount = 0..      
+00019980: 2020 666f 7220 656c 656d 2069 6e20 7665    for elem in ve
+00019990: 6374 6f72 3a0d 0a20 2020 2020 2020 2020  ctor:..         
+000199a0: 2020 2069 6620 656c 656d 2069 6e20 626f     if elem in bo
+000199b0: 7365 5f74 7970 6520 3a0d 0a20 2020 2020  se_type :..     
+000199c0: 2020 2020 2020 2020 2020 2062 6f73 6f6e             boson
+000199d0: 5f63 6f75 6e74 202b 3d20 310d 0a20 2020  _count += 1..   
+000199e0: 2020 2020 2020 2020 2069 6620 656c 656d           if elem
+000199f0: 2069 6e20 6665 726d 695f 7479 7065 203a   in fermi_type :
+00019a00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019a10: 2020 6665 726d 695f 636f 756e 7420 2b3d    fermi_count +=
+00019a20: 2031 0d0a 0d0a 2020 2020 2020 2020 6966   1....        if
+00019a30: 2862 6f73 6f6e 5f63 6f75 6e74 3d3d 3020  (boson_count==0 
+00019a40: 616e 6420 6665 726d 695f 636f 756e 743e  and fermi_count>
+00019a50: 3029 3a0d 0a20 2020 2020 2020 2020 2020  0):..           
+00019a60: 2069 6620 7072 6566 6572 2021 3d20 4e6f   if prefer != No
+00019a70: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00019a80: 2020 2020 2072 6574 7572 6e20 7072 6566       return pref
+00019a90: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
+00019aa0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00019ab0: 2020 2020 2020 2072 6574 7572 6e20 310d         return 1.
+00019ac0: 0a20 2020 2020 2020 2065 6c69 6628 626f  .        elif(bo
+00019ad0: 736f 6e5f 636f 756e 743e 3020 616e 6420  son_count>0 and 
+00019ae0: 6665 726d 695f 636f 756e 743d 3d30 293a  fermi_count==0):
+00019af0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00019b00: 2070 7265 6665 7220 213d 204e 6f6e 653a   prefer != None:
+00019b10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019b20: 2020 7265 7475 726e 2070 7265 6665 720d    return prefer.
+00019b30: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00019b40: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00019b50: 2020 2020 7265 7475 726e 2030 0d0a 2020      return 0..  
+00019b60: 2020 2020 2020 656c 6966 2862 6f73 6f6e        elif(boson
+00019b70: 5f63 6f75 6e74 3e30 2061 6e64 2066 6572  _count>0 and fer
+00019b80: 6d69 5f63 6f75 6e74 3e30 293a 0d0a 2020  mi_count>0):..  
+00019b90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00019ba0: 2068 7962 7269 645f 7379 6d62 6f6c 0d0a   hybrid_symbol..
+00019bb0: 2020 2020 7374 6570 203d 2073 686f 775f      step = show_
+00019bc0: 7072 6f67 7265 7373 2873 7465 702c 7072  progress(step,pr
+00019bd0: 6f63 6573 735f 6c65 6e67 7468 2c70 726f  ocess_length,pro
+00019be0: 6365 7373 5f6e 616d 652b 2220 222b 223c  cess_name+" "+"<
+00019bf0: 222b 6375 7272 656e 745f 6d65 6d6f 7279  "+current_memory
+00019c00: 5f64 6973 706c 6179 2829 2b22 3e22 2c63  _display()+">",c
+00019c10: 6f6c 6f72 3d70 726f 6365 7373 5f63 6f6c  olor=process_col
+00019c20: 6f72 2c74 696d 653d 7469 6d65 2e74 696d  or,time=time.tim
+00019c30: 6528 292d 7330 3029 0d0a 2020 2020 4f62  e()-s00)..    Ob
+00019c40: 6a20 3d20 4f62 6a2e 6a6f 696e 5f6c 6567  j = Obj.join_leg
+00019c50: 7328 6a6f 696e 5f6c 6567 735f 7374 7269  s(join_legs_stri
+00019c60: 6e67 5f69 6e70 7574 2c22 6d61 7472 6978  ng_input,"matrix
+00019c70: 222c 7361 7665 5f6d 656d 6f72 793d 5472  ",save_memory=Tr
+00019c80: 7565 290d 0a20 2020 200d 0a20 2020 2073  ue)..    ..    s
+00019c90: 7465 7020 3d20 7368 6f77 5f70 726f 6772  tep = show_progr
+00019ca0: 6573 7328 7374 6570 2c70 726f 6365 7373  ess(step,process
+00019cb0: 5f6c 656e 6774 682c 7072 6f63 6573 735f  _length,process_
+00019cc0: 6e61 6d65 2b22 2022 2b22 3c22 2b63 7572  name+" "+"<"+cur
+00019cd0: 7265 6e74 5f6d 656d 6f72 795f 6469 7370  rent_memory_disp
+00019ce0: 6c61 7928 292b 223e 222c 636f 6c6f 723d  lay()+">",color=
+00019cf0: 7072 6f63 6573 735f 636f 6c6f 722c 7469  process_color,ti
+00019d00: 6d65 3d74 696d 652e 7469 6d65 2829 2d73  me=time.time()-s
+00019d10: 3030 290d 0a20 2020 2023 3a3a 3a3a 3a3a  00)..    #::::::
+00019d20: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00019d30: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00019d40: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00019d50: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00019d60: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00019d70: 3a3a 3a3a 3a3a 3a3a 3a3a 0d0a 2020 2020  ::::::::::..    
+00019d80: 233a 3a3a 3a3a 2020 2020 2020 5354 4550  #:::::      STEP
+00019d90: 2032 202d 2050 6572 666f 726d 2048 6572   2 - Perform Her
+00019da0: 6d69 7469 616e 2043 6f6e 6a75 6761 7469  mitian Conjugati
+00019db0: 6f6e 2020 2020 2020 2020 2020 2020 2020  on              
+00019dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019dd0: 2020 2020 2020 2020 2020 2020 3a3a 3a3a              ::::
+00019de0: 3a0d 0a20 2020 2023 3a3a 3a3a 3a3a 3a3a  :..    #::::::::
+00019df0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00019e00: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00019e10: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00019e20: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00019e30: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+00019e40: 3a3a 3a3a 3a3a 3a3a 0d0a 0d0a 2020 2020  ::::::::....    
+00019e50: 4f62 6a2e 6461 7461 203d 206e 702e 636f  Obj.data = np.co
+00019e60: 6e6a 7567 6174 6528 6f65 2e63 6f6e 7472  njugate(oe.contr
+00019e70: 6163 7428 2769 6a2d 3e6a 6927 2c4f 626a  act('ij->ji',Obj
+00019e80: 2e64 6174 6129 290d 0a20 2020 200d 0a20  .data))..    .. 
+00019e90: 2020 206e 6577 5f73 7461 7420 3d20 5b31     new_stat = [1
+00019ea0: 2c31 5d0d 0a20 2020 200d 0a20 2020 2069  ,1]..    ..    i
+00019eb0: 6620 4f62 6a2e 7374 6174 6973 7469 635b  f Obj.statistic[
+00019ec0: 305d 2069 6e20 6665 726d 695f 7479 7065  0] in fermi_type
+00019ed0: 203a 0d0a 2020 2020 2020 2020 6e65 775f   :..        new_
+00019ee0: 7374 6174 5b31 5d20 3d20 2d4f 626a 2e73  stat[1] = -Obj.s
+00019ef0: 7461 7469 7374 6963 5b30 5d0d 0a20 2020  tatistic[0]..   
+00019f00: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00019f10: 6e65 775f 7374 6174 5b31 5d20 3d20 4f62  new_stat[1] = Ob
+00019f20: 6a2e 7374 6174 6973 7469 635b 305d 0d0a  j.statistic[0]..
+00019f30: 2020 2020 2020 2020 0d0a 2020 2020 6966          ..    if
+00019f40: 204f 626a 2e73 7461 7469 7374 6963 5b31   Obj.statistic[1
+00019f50: 5d20 696e 2066 6572 6d69 5f74 7970 6520  ] in fermi_type 
+00019f60: 3a0d 0a20 2020 2020 2020 206e 6577 5f73  :..        new_s
+00019f70: 7461 745b 305d 203d 202d 4f62 6a2e 7374  tat[0] = -Obj.st
+00019f80: 6174 6973 7469 635b 315d 0d0a 2020 2020  atistic[1]..    
+00019f90: 656c 7365 3a0d 0a20 2020 2020 2020 206e  else:..        n
+00019fa0: 6577 5f73 7461 745b 305d 203d 204f 626a  ew_stat[0] = Obj
+00019fb0: 2e73 7461 7469 7374 6963 5b31 5d0d 0a20  .statistic[1].. 
+00019fc0: 2020 200d 0a20 2020 206e 6577 5f73 7461     ..    new_sta
+00019fd0: 7420 3d20 6d61 6b65 5f74 7570 6c65 286e  t = make_tuple(n
+00019fe0: 6577 5f73 7461 7429 0d0a 2020 2020 0d0a  ew_stat)..    ..
+00019ff0: 2020 2020 4f62 6a2e 7374 6174 6973 7469      Obj.statisti
+0001a000: 6320 3d20 6e65 775f 7374 6174 0d0a 2020  c = new_stat..  
+0001a010: 2020 0d0a 2020 2020 7374 6570 203d 2073    ..    step = s
+0001a020: 686f 775f 7072 6f67 7265 7373 2873 7465  how_progress(ste
+0001a030: 702c 7072 6f63 6573 735f 6c65 6e67 7468  p,process_length
+0001a040: 2c70 726f 6365 7373 5f6e 616d 652b 2220  ,process_name+" 
+0001a050: 222b 223c 222b 6375 7272 656e 745f 6d65  "+"<"+current_me
+0001a060: 6d6f 7279 5f64 6973 706c 6179 2829 2b22  mory_display()+"
+0001a070: 3e22 2c63 6f6c 6f72 3d70 726f 6365 7373  >",color=process
+0001a080: 5f63 6f6c 6f72 2c74 696d 653d 7469 6d65  _color,time=time
+0001a090: 2e74 696d 6528 292d 7330 3029 0d0a 2020  .time()-s00)..  
+0001a0a0: 2020 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a    #:::::::::::::
+0001a0b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0001a0c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0001a0d0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0001a0e0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0001a0f0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0001a100: 3a3a 3a0d 0a20 2020 2023 3a3a 3a3a 3a20  :::..    #::::: 
+0001a110: 2020 2020 2053 5445 5020 3320 2d20 5370       STEP 3 - Sp
+0001a120: 6c69 7420 6c65 6773 2020 2020 2020 2020  lit legs        
+0001a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a160: 2020 2020 203a 3a3a 3a3a 0d0a 2020 2020       :::::..    
+0001a170: 233a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  #:::::::::::::::
+0001a180: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0001a190: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0001a1a0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0001a1b0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0001a1c0: 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a 3a3a  ::::::::::::::::
+0001a1d0: 3a0d 0a20 2020 200d 0a20 2020 200d 0a20  :..    ..    .. 
+0001a1e0: 2020 2023 2063 6f75 6e74 2074 6865 206e     # count the n
+0001a1f0: 756d 6265 7220 6f66 2069 6e64 6963 6573  umber of indices
+0001a200: 2069 6e20 7468 6520 7477 6f20 6772 6f75   in the two grou
+0001a210: 7073 0d0a 2020 2020 5569 6e64 203d 2022  ps..    Uind = "
+0001a220: 220d 0a20 2020 2056 696e 6420 3d20 2222  "..    Vind = ""
+0001a230: 0d0a 2020 2020 5573 7461 7473 203d 205b  ..    Ustats = [
+0001a240: 5d0d 0a20 2020 2056 7374 6174 7320 3d20  ]..    Vstats = 
+0001a250: 5b5d 0d0a 2020 2020 5573 6861 7065 203d  []..    Ushape =
+0001a260: 205b 5d0d 0a20 2020 2056 7368 6170 6520   []..    Vshape 
+0001a270: 3d20 5b5d 0d0a 2020 2020 7061 7274 6974  = []..    partit
+0001a280: 696f 6e5f 666f 756e 6420 3d20 4661 6c73  ion_found = Fals
+0001a290: 650d 0a20 2020 2066 6f72 2069 2c63 6861  e..    for i,cha
+0001a2a0: 7220 696e 2065 6e75 6d65 7261 7465 2873  r in enumerate(s
+0001a2b0: 7472 696e 6729 3a0d 0a20 2020 2020 2020  tring):..       
+0001a2c0: 2069 6620 6368 6172 2069 6e20 7365 7061   if char in sepa
+0001a2d0: 7261 746f 725f 6c69 7374 203a 0d0a 2020  rator_list :..  
+0001a2e0: 2020 2020 2020 2020 2020 7061 7274 6974            partit
+0001a2f0: 696f 6e5f 666f 756e 6420 3d20 5472 7565  ion_found = True
+0001a300: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+0001a310: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
+0001a320: 6966 2870 6172 7469 7469 6f6e 5f66 6f75  if(partition_fou
+0001a330: 6e64 293a 0d0a 2020 2020 2020 2020 2020  nd):..          
+0001a340: 2020 5669 6e64 2b3d 6368 6172 0d0a 2020    Vind+=char..  
+0001a350: 2020 2020 2020 2020 2020 5673 7461 7473            Vstats
+0001a360: 2b3d 5b58 4f62 6a5f 7374 6174 735b 692d  +=[XObj_stats[i-
+0001a370: 315d 5d0d 0a20 2020 2020 2020 2020 2020  1]]..           
+0001a380: 2056 7368 6170 652b 3d5b 584f 626a 5f73   Vshape+=[XObj_s
+0001a390: 6861 7065 5b69 2d31 5d5d 0d0a 2020 2020  hape[i-1]]..    
+0001a3a0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0001a3b0: 2020 2020 2020 2055 696e 642b 3d63 6861         Uind+=cha
+0001a3c0: 720d 0a20 2020 2020 2020 2020 2020 2055  r..            U
+0001a3d0: 7374 6174 732b 3d5b 584f 626a 5f73 7461  stats+=[XObj_sta
+0001a3e0: 7473 5b69 5d5d 0d0a 2020 2020 2020 2020  ts[i]]..        
+0001a3f0: 2020 2020 5573 6861 7065 2b3d 5b58 4f62      Ushape+=[XOb
+0001a400: 6a5f 7368 6170 655b 695d 5d0d 0a20 2020  j_shape[i]]..   
+0001a410: 200d 0a20 2020 206e 6577 5f69 6e64 203d   ..    new_ind =
+0001a420: 2022 2822 2b56 696e 642b 2229 2822 2b55   "("+Vind+")("+U
+0001a430: 696e 642b 2229 220d 0a20 2020 206e 6577  ind+")"..    new
+0001a440: 5f73 7461 7473 203d 2056 7374 6174 7320  _stats = Vstats 
+0001a450: 2b20 5573 7461 7473 0d0a 2020 2020 6e65  + Ustats..    ne
+0001a460: 775f 7368 6170 6520 3d20 6d61 6b65 5f74  w_shape = make_t
+0001a470: 7570 6c65 2856 7368 6170 6520 2b20 5573  uple(Vshape + Us
+0001a480: 6861 7065 290d 0a20 2020 2066 6f72 2069  hape)..    for i
+0001a490: 2069 6e20 7261 6e67 6528 6c65 6e28 6e65   in range(len(ne
+0001a4a0: 775f 7374 6174 7329 293a 0d0a 2020 2020  w_stats)):..    
+0001a4b0: 2020 2020 6966 206e 6577 5f73 7461 7473      if new_stats
+0001a4c0: 5b69 5d20 696e 2066 6572 6d69 5f74 7970  [i] in fermi_typ
+0001a4d0: 6520 3a0d 0a20 2020 2020 2020 2020 2020  e :..           
+0001a4e0: 206e 6577 5f73 7461 7473 5b69 5d2a 3d2d   new_stats[i]*=-
+0001a4f0: 310d 0a20 2020 206e 6577 5f73 7461 7473  1..    new_stats
+0001a500: 203d 206d 616b 655f 7475 706c 6528 6e65   = make_tuple(ne
+0001a510: 775f 7374 6174 7329 0d0a 2020 2020 7374  w_stats)..    st
+0001a520: 6570 203d 2073 686f 775f 7072 6f67 7265  ep = show_progre
+0001a530: 7373 2873 7465 702c 7072 6f63 6573 735f  ss(step,process_
+0001a540: 6c65 6e67 7468 2c70 726f 6365 7373 5f6e  length,process_n
+0001a550: 616d 652b 2220 222b 223c 222b 6375 7272  ame+" "+"<"+curr
+0001a560: 656e 745f 6d65 6d6f 7279 5f64 6973 706c  ent_memory_displ
+0001a570: 6179 2829 2b22 3e22 2c63 6f6c 6f72 3d70  ay()+">",color=p
+0001a580: 726f 6365 7373 5f63 6f6c 6f72 2c74 696d  rocess_color,tim
+0001a590: 653d 7469 6d65 2e74 696d 6528 292d 7330  e=time.time()-s0
+0001a5a0: 3029 0d0a 2020 2020 4f62 6a20 3d20 4f62  0)..    Obj = Ob
+0001a5b0: 6a2e 7370 6c69 745f 6c65 6773 286e 6577  j.split_legs(new
+0001a5c0: 5f69 6e64 2c6e 6577 5f73 7461 7473 2c6e  _ind,new_stats,n
+0001a5d0: 6577 5f73 6861 7065 2c73 6176 655f 6d65  ew_shape,save_me
+0001a5e0: 6d6f 7279 3d54 7275 6529 0d0a 2020 2020  mory=True)..    
+0001a5f0: 0d0a 2020 2020 2369 6620 7468 6973 5f74  ..    #if this_t
+0001a600: 7970 653d 3d73 7061 7273 6520 3a0d 0a20  ype==sparse :.. 
+0001a610: 2020 2023 2020 2020 4f62 6a20 3d20 7370     #    Obj = sp
+0001a620: 6172 7365 284f 626a 290d 0a20 2020 2069  arse(Obj)..    i
+0001a630: 6620 7468 6973 5f66 6f72 6d61 7421 3d4f  f this_format!=O
+0001a640: 626a 2e66 6f72 6d61 7420 3a0d 0a20 2020  bj.format :..   
+0001a650: 2020 2020 204f 626a 203d 204f 626a 2e73       Obj = Obj.s
+0001a660: 7769 7463 685f 666f 726d 6174 2873 6176  witch_format(sav
+0001a670: 655f 6d65 6d6f 7279 3d54 7275 6529 0d0a  e_memory=True)..
+0001a680: 2020 2020 6966 2074 6869 735f 656e 636f      if this_enco
+0001a690: 6465 7221 3d4f 626a 2e65 6e63 6f64 6572  der!=Obj.encoder
+0001a6a0: 203a 0d0a 2020 2020 2020 2020 4f62 6a20   :..        Obj 
+0001a6b0: 3d20 4f62 6a2e 7377 6974 6368 5f65 6e63  = Obj.switch_enc
+0001a6c0: 6f64 6572 2873 6176 655f 6d65 6d6f 7279  oder(save_memory
+0001a6d0: 3d54 7275 6529 0d0a 0d0a 2020 2020 636c  =True)....    cl
+0001a6e0: 6561 725f 7072 6f67 7265 7373 2829 0d0a  ear_progress()..
+0001a6f0: 2020 2020 7461 625f 7570 2829 0d0a 0d0a      tab_up()....
+0001a700: 2020 2020 7265 7475 726e 204f 626a 0d0a      return Obj..
+0001a710: 0d0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+0001a720: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a730: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a740: 2323 2323 2323 0d0a 2323 2020 2020 2020  ######..##      
+0001a750: 2020 2020 2020 2020 2020 2020 2020 5574                Ut
+0001a760: 696c 6974 6965 7320 2020 2020 2020 2020  ilities         
+0001a770: 2020 2020 2020 2020 2020 2323 0d0a 2323            ##..##
+0001a780: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a790: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a7a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001a7b0: 2323 0d0a 0d0a 6465 6620 7261 6e64 6f6d  ##....def random
+0001a7c0: 2873 6861 7065 2c73 7461 7469 7374 6963  (shape,statistic
+0001a7d0: 2c74 656e 736f 725f 666f 726d 6174 3d64  ,tensor_format=d
+0001a7e0: 656e 7365 2c64 7479 7065 3d66 6c6f 6174  ense,dtype=float
+0001a7f0: 2c73 6b69 705f 7472 696d 6d69 6e67 3d46  ,skip_trimming=F
+0001a800: 616c 7365 293a 0d0a 2020 2020 5820 3d20  alse):..    X = 
+0001a810: 6e70 2e72 616e 646f 6d2e 7261 6e64 282a  np.random.rand(*
+0001a820: 7368 6170 6529 0d0a 2020 2020 6966 2064  shape)..    if d
+0001a830: 7479 7065 203d 3d20 636f 6d70 6c65 7820  type == complex 
+0001a840: 3a0d 0a20 2020 2020 2020 2058 203d 2063  :..        X = c
+0001a850: 6f6d 706c 6578 2831 2c30 292a 5820 2b20  omplex(1,0)*X + 
+0001a860: 636f 6d70 6c65 7828 302c 3129 2a6e 702e  complex(0,1)*np.
+0001a870: 7261 6e64 6f6d 2e72 616e 6428 2a73 6861  random.rand(*sha
+0001a880: 7065 290d 0a20 2020 2041 203d 2064 656e  pe)..    A = den
+0001a890: 7365 2858 2c20 7374 6174 6973 7469 6320  se(X, statistic 
+0001a8a0: 3d20 7374 6174 6973 7469 6329 0d0a 2020  = statistic)..  
+0001a8b0: 2020 6966 206e 6f74 2073 6b69 705f 7472    if not skip_tr
+0001a8c0: 696d 6d69 6e67 3a0d 0a20 2020 2020 2020  imming:..       
+0001a8d0: 2041 203d 2074 7269 6d5f 6772 6173 736d   A = trim_grassm
+0001a8e0: 616e 6e5f 6f64 6428 4129 0d0a 2020 2020  ann_odd(A)..    
+0001a8f0: 6966 2074 656e 736f 725f 666f 726d 6174  if tensor_format
+0001a900: 3d3d 7370 6172 7365 3a0d 0a20 2020 2020  ==sparse:..     
+0001a910: 2020 2041 203d 2073 7061 7273 6528 4129     A = sparse(A)
+0001a920: 0d0a 2020 2020 2020 2020 4120 3d20 412e  ..        A = A.
+0001a930: 7265 6d6f 7665 5f7a 6572 6f73 2829 0d0a  remove_zeros()..
+0001a940: 2020 2020 7265 7475 726e 2041 0d0a 0d0a      return A....
+0001a950: 6465 6620 706f 7765 7228 542c 7029 3a0d  def power(T,p):.
+0001a960: 0a20 2020 2074 6869 735f 7479 7065 203d  .    this_type =
+0001a970: 2074 7970 6528 5429 0d0a 2020 2020 7468   type(T)..    th
+0001a980: 6973 5f66 6f72 6d61 7420 3d20 542e 666f  is_format = T.fo
+0001a990: 726d 6174 0d0a 2020 2020 7468 6973 5f65  rmat..    this_e
+0001a9a0: 6e63 6f64 6572 203d 2054 2e65 6e63 6f64  ncoder = T.encod
+0001a9b0: 6572 0d0a 2020 2020 5420 3d20 6465 6e73  er..    T = dens
+0001a9c0: 6528 5429 2e66 6f72 6365 5f66 6f72 6d61  e(T).force_forma
+0001a9d0: 7428 226d 6174 7269 7822 292e 666f 7263  t("matrix").forc
+0001a9e0: 655f 656e 636f 6465 7228 2263 616e 6f6e  e_encoder("canon
+0001a9f0: 6963 616c 2229 0d0a 2020 2020 542e 6461  ical")..    T.da
+0001aa00: 7461 203d 206e 702e 706f 7765 7228 542e  ta = np.power(T.
+0001aa10: 6461 7461 2c70 290d 0a20 2020 2054 203d  data,p)..    T =
+0001aa20: 2054 2e66 6f72 6365 5f66 6f72 6d61 7428   T.force_format(
+0001aa30: 7468 6973 5f66 6f72 6d61 7429 2e66 6f72  this_format).for
+0001aa40: 6365 5f65 6e63 6f64 6572 2874 6869 735f  ce_encoder(this_
+0001aa50: 656e 636f 6465 7229 0d0a 2020 2020 6966  encoder)..    if
+0001aa60: 2074 6869 735f 7479 7065 3d3d 7370 6172   this_type==spar
+0001aa70: 7365 203a 0d0a 2020 2020 2020 2020 5420  se :..        T 
+0001aa80: 3d20 7370 6172 7365 2854 290d 0a20 2020  = sparse(T)..   
+0001aa90: 2072 6574 7572 6e20 540d 0a0d 0a64 6566   return T....def
+0001aaa0: 2073 7172 7428 5429 3a0d 0a20 2020 2072   sqrt(T):..    r
+0001aab0: 6574 7572 6e20 706f 7765 7228 542c 302e  eturn power(T,0.
+0001aac0: 3529 0d0a                                5)..
```

### Comparing `grassmanntn-1.0/grassmanntn/param.py` & `grassmanntn-1.1/grassmanntn/param.py`

 * *Files identical despite different names*

### Comparing `grassmanntn-1.0/grassmanntn.egg-info/PKG-INFO` & `grassmanntn-1.1/grassmanntn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: grassmanntn
-Version: 1.0
+Version: 1.1
 Summary: a Python library for Grassmann tensor network computation
 Home-page: https://github.com/ayosprakob/grassmanntn
-Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_10.tar.gz
+Download-URL: https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_11.tar.gz
 Author: Atis Yosprakob
 Author-email: yosprakob2@gmail.com
 License: Apache
 Keywords: physics,lattice,gauge theory,tensor network,grassmann
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `grassmanntn-1.0/setup.py` & `grassmanntn-1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'grassmanntn',         # How you named your package folder (MyLib)
   packages = ['grassmanntn'],   # Chose the same as "name"
-  version = '1.0',      # Start with a small number and increase it with every change you make
+  version = '1.1',      # Start with a small number and increase it with every change you make
   license='Apache',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'a Python library for Grassmann tensor network computation',   # Give a short description about your library
   author = 'Atis Yosprakob',                   # Type in your name
   author_email = 'yosprakob2@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/ayosprakob/grassmanntn',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_10.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/ayosprakob/grassmanntn/archive/refs/tags/v_11.tar.gz',    # I explain this later on
   keywords = ['physics', 'lattice', 'gauge theory', 'tensor network', 'grassmann'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'numpy',
           'sparse',
           'opt_einsum',
       ],
   classifiers=[
```

