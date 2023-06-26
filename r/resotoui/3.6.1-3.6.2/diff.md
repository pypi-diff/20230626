# Comparing `tmp/resotoui-3.6.1.tar.gz` & `tmp/resotoui-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoui-3.6.1.tar", last modified: Fri Jun 23 15:37:25 2023, max compression
+gzip compressed data, was "resotoui-3.6.2.tar", last modified: Mon Jun 26 19:22:01 2023, max compression
```

## Comparing `resotoui-3.6.1.tar` & `resotoui-3.6.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:37:25.040501 resotoui-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 15:36:16.000000 resotoui-3.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-23 15:37:25.040501 resotoui-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-23 15:36:16.000000 resotoui-3.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:37:25.012501 resotoui-3.6.1/resotoui/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-23 15:36:16.000000 resotoui-3.6.1/resotoui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:37:25.020501 resotoui-3.6.1/resotoui/ui/
--rw-r--r--   0 runner    (1001) docker     (123)    30624 2023-06-23 15:37:06.000000 resotoui-3.6.1/resotoui/ui/index.apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-06-23 15:37:06.000000 resotoui-3.6.1/resotoui/ui/index.audio.worklet.js
--rw-r--r--   0 runner    (1001) docker     (123)    29953 2023-06-23 15:37:06.000000 resotoui-3.6.1/resotoui/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-06-23 15:37:06.000000 resotoui-3.6.1/resotoui/ui/index.icon.png
--rw-r--r--   0 runner    (1001) docker     (123)   350804 2023-06-23 15:37:06.000000 resotoui-3.6.1/resotoui/ui/index.js
--rw-r--r--   0 runner    (1001) docker     (123)  6941664 2023-06-23 15:37:06.000000 resotoui-3.6.1/resotoui/ui/index.pck
--rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-06-23 15:37:06.000000 resotoui-3.6.1/resotoui/ui/index.png
--rw-r--r--   0 runner    (1001) docker     (123) 17862218 2023-06-23 15:37:06.000000 resotoui-3.6.1/resotoui/ui/index.wasm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:37:25.012501 resotoui-3.6.1/resotoui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-23 15:37:25.000000 resotoui-3.6.1/resotoui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-23 15:37:25.000000 resotoui-3.6.1/resotoui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:37:25.000000 resotoui-3.6.1/resotoui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:37:24.000000 resotoui-3.6.1/resotoui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 15:37:25.000000 resotoui-3.6.1/resotoui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:37:25.040501 resotoui-3.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-23 15:36:16.000000 resotoui-3.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:01.514580 resotoui-3.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 19:20:36.000000 resotoui-3.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-26 19:22:01.514580 resotoui-3.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-26 19:20:36.000000 resotoui-3.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:01.482578 resotoui-3.6.2/resotoui/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-26 19:20:36.000000 resotoui-3.6.2/resotoui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:01.494579 resotoui-3.6.2/resotoui/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    30624 2023-06-26 19:21:40.000000 resotoui-3.6.2/resotoui/ui/index.apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-06-26 19:21:40.000000 resotoui-3.6.2/resotoui/ui/index.audio.worklet.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-06-26 19:21:40.000000 resotoui-3.6.2/resotoui/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-06-26 19:21:40.000000 resotoui-3.6.2/resotoui/ui/index.icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   350804 2023-06-26 19:21:40.000000 resotoui-3.6.2/resotoui/ui/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)  6941664 2023-06-26 19:21:40.000000 resotoui-3.6.2/resotoui/ui/index.pck
+-rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-06-26 19:21:40.000000 resotoui-3.6.2/resotoui/ui/index.png
+-rw-r--r--   0 runner    (1001) docker     (123) 17862218 2023-06-26 19:21:40.000000 resotoui-3.6.2/resotoui/ui/index.wasm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:01.482578 resotoui-3.6.2/resotoui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-26 19:22:01.000000 resotoui-3.6.2/resotoui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-26 19:22:01.000000 resotoui-3.6.2/resotoui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:22:01.000000 resotoui-3.6.2/resotoui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:22:01.000000 resotoui-3.6.2/resotoui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 19:22:01.000000 resotoui-3.6.2/resotoui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:22:01.514580 resotoui-3.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-26 19:20:36.000000 resotoui-3.6.2/setup.py
```

### Comparing `resotoui-3.6.1/PKG-INFO` & `resotoui-3.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoui
-Version: 3.6.1
+Version: 3.6.2
 Summary: The Resoto UI.
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `resotoui-3.6.1/README.md` & `resotoui-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `resotoui-3.6.1/resotoui/ui/index.apple-touch-icon.png` & `resotoui-3.6.2/resotoui/ui/index.apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `resotoui-3.6.1/resotoui/ui/index.audio.worklet.js` & `resotoui-3.6.2/resotoui/ui/index.audio.worklet.js`

 * *Files identical despite different names*

### Comparing `resotoui-3.6.1/resotoui/ui/index.html` & `resotoui-3.6.2/resotoui/ui/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -133,25 +133,29 @@
 		}
 	</style>
 	<script src="https://cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/crypto-js.min.js"></script>
 	<script>
 		var jwt;
 		var expirationTime = 0;
 		var key;
-		var iv;
 		var t = "";
-		var ejwt;
 		window.onload = async function() {
+
+			let iv = localStorage.getItem("iv");
+			if (iv != null) {
+				// previous version of jwt, remove it
+				localStorage.removeItem("jwt");
+				localStorage.removeItem("iv");
+			}
+
 			key = await generateKey();
-			ejwt = localStorage.getItem("jwt");
-			var eiv = localStorage.getItem("iv");
-			if (ejwt != null && eiv != null){
-				jwt = crypto.sublte === undefined ? ejwt : new Uint8Array( JSON.parse(ejwt));
-				iv = crypto.sublte === undefined ? eiv : new Uint8Array(JSON.parse(eiv));
-				t = await decryptData(key, eiv, ejwt);
+			jwt = localStorage.getItem("jwt");
+
+			if (jwt != null){
+				t = await decryptData(key, jwt);
 				var parts = t.split(".");
 				if (parts.length > 1){
 					var payload = JSON.parse(atob(parts[1]));
 					if ("exp" in payload && payload["exp"] * 1000.0 > Date.now()){
 						expirationTime = payload["exp"] * 1000.0;
 						setTimeout(renewJWT, expirationTime - Date.now() - 300000);
 						return;
@@ -170,18 +174,16 @@
 						let params = (new URL(this.responseURL)).searchParams;
 						const urlParams = new URLSearchParams(params);
 						const redirect = urlParams.get('redirect');
 						if (redirect == "/authorization/user?"){
 							window.location = "/login?" + encodeJSONToURL({"redirect": window.location});
 						} else {
 							var r = await encryptData(key, xhr.getResponseHeader("Authorization").split(" ")[1]);
-							iv = r.iv;
 							jwt = r.data;
-							localStorage.setItem("jwt", crypto.sublte === undefined ? jwt : JSON.stringify(Array.from(jwt)));
-							localStorage.setItem("iv", crypto.sublte === undefined ? iv : JSON.stringify(Array.from(iv)));
+							localStorage.setItem("jwt", jwt);
 							await refreshExpirationTime();
 							let url = new URL(window.location.href);
 							url.search = "";
 							window.history.replaceState({}, document.title, url.toString());
 						}
 					} else {
 						window.location.replace(window.location.origin + "/login?" + encodeJSONToURL({"redirect": window.location}));
@@ -197,15 +199,15 @@
 			xhr.open("GET", url, true);
 			xhr.send();
 		};
 
 		async function refreshExpirationTime(){
 			if (jwt === "") return;
 
-			t = await decryptData(key, iv, jwt);
+			t = await decryptData(key, jwt);
 			var parts = t.split(".")
 			if (parts.length > 1){
 				var payload = JSON.parse(atob(parts[1]));
 				expirationTime = payload["exp"] * 1000.0;
 				var timeToExpire = Math.max(expirationTime - Date.now() - 300000, 10000);
 				setTimeout(renewJWT, timeToExpire);
 			}
@@ -214,17 +216,15 @@
 		function renewJWT(){
 			var xhr = new XMLHttpRequest();
 			xhr.onreadystatechange = async function() {
 				if (this.readyState == 4){
 					if (this.status == 200) {
 						var r = await encryptData(key, xhr.getResponseHeader("Authorization").split(" ")[1]);
 						jwt = r.data;
-						iv = r.iv;
-						localStorage.setItem("jwt", crypto.sublte === undefined ? jwt : JSON.stringify(Array.from(jwt)));
-						localStorage.setItem("iv", crypto.sublte === undefined ? iv : JSON.stringify(Array.from(iv)));
+						localStorage.setItem("jwt", jwt);
 						refreshExpirationTime();
 					}
 				}
 			};
 			xhr.open("GET", window.location.origin + "/authorization/renew", true);
 			xhr.setRequestHeader("Authorization",  "Bearer " + t);
 			xhr.send();
@@ -233,48 +233,25 @@
 		function encodeJSONToURL(json) {
 			return Object.entries(json)
 				.map(([key, value]) => `${encodeURIComponent(key)}=${encodeURIComponent(value)}`)
 				.join("&");
 		}
 
 		async function generateKey() {
-			if (crypto.subtle == undefined){
-				return 'resoto-secret';
-			}
-			const _0x3116df=_0x20a0;function _0x4670(){const _0x1f8d88=['302636qyhbRd','30505GOFyWJ','4613HrqjEk','AES-GCM','subtle','243990CtJenz','258IovlEo','encrypt','1938128IxAuhU','decrypt','6IHzAjB','240SUOGZG','1259176kGMNeg','importKey','518220YMgFvP'];_0x4670=function(){return _0x1f8d88;};return _0x4670();}function _0x20a0(_0x5e9956,_0x45c6fd){const _0x4670c1=_0x4670();return _0x20a0=function(_0x20a0f5,_0x86fbf9){_0x20a0f5=_0x20a0f5-0x150;let _0x5bce5d=_0x4670c1[_0x20a0f5];return _0x5bce5d;},_0x20a0(_0x5e9956,_0x45c6fd);}(function(_0x3131ee,_0x7aca7f){const _0x23c719=_0x20a0,_0xf3e675=_0x3131ee();while(!![]){try{const _0x1a15e1=parseInt(_0x23c719(0x15d))/0x1+-parseInt(_0x23c719(0x15c))/0x2*(-parseInt(_0x23c719(0x157))/0x3)+parseInt(_0x23c719(0x155))/0x4+-parseInt(_0x23c719(0x15b))/0x5+-parseInt(_0x23c719(0x153))/0x6*(-parseInt(_0x23c719(0x15e))/0x7)+parseInt(_0x23c719(0x159))/0x8+parseInt(_0x23c719(0x152))/0x9*(-parseInt(_0x23c719(0x158))/0xa);if(_0x1a15e1===_0x7aca7f)break;else _0xf3e675['push'](_0xf3e675['shift']());}catch(_0x217369){_0xf3e675['push'](_0xf3e675['shift']());}}}(_0x4670,0x3cd23));const bytes=new Uint8Array([0x1,0x2,0x3,0x4,0x5,0x6,0x7,0x8,0x9,0xa,0xb,0xc,0xd,0xe,0xf,0x10]),key=await crypto[_0x3116df(0x151)][_0x3116df(0x15a)]('raw',bytes,{'name':_0x3116df(0x150)},![],[_0x3116df(0x154),_0x3116df(0x156)]);return key;
+			return 'resoto-secret';
 		}
 
 		async function encryptData(key, data) {
-			const encoder = new TextEncoder();
-			if (crypto.subtle === undefined){
-				const iv = CryptoJS.lib.WordArray.random(12);
 				const encryptedData = CryptoJS.AES.encrypt(data, key).toString();
-				return { iv: iv, data: encryptedData };
-			}
-			const iv = crypto.getRandomValues(new Uint8Array(12));
-			const encodedData = encoder.encode(data);
-			const encryptedData = await crypto.subtle.encrypt(
-				{ name: 'AES-GCM', iv },
-				key, encodedData
-			);
-
-			return { iv: iv, data: new Uint8Array(encryptedData) };
+				return { data: encryptedData };
 		}	
 
-		async function decryptData(key, iv, encryptedData) {
-			const decoder = new TextDecoder();
-			if (crypto.subtle === undefined) {
+		async function decryptData(key, encryptedData) {
 				const decryptedData = CryptoJS.AES.decrypt(encryptedData, key);
 				return decryptedData.toString(CryptoJS.enc.Utf8);
-			}
-			const decryptedData = await crypto.subtle.decrypt(
-				{ name: 'AES-GCM', iv },
-				key, encryptedData
-			);
-			return decoder.decode(decryptedData);
 		}
 
 	</script>
 	<script>
 		var reader = new FileReader();
 		var input = document.createElement('INPUT');
 		function getOS() {
```

### Comparing `resotoui-3.6.1/resotoui/ui/index.icon.png` & `resotoui-3.6.2/resotoui/ui/index.icon.png`

 * *Files identical despite different names*

### Comparing `resotoui-3.6.1/resotoui/ui/index.js` & `resotoui-3.6.2/resotoui/ui/index.js`

 * *Files identical despite different names*

### Comparing `resotoui-3.6.1/resotoui/ui/index.pck` & `resotoui-3.6.2/resotoui/ui/index.pck`

 * *Files 0% similar despite different names*

```diff
@@ -6329,15 +6329,15 @@
 00018b80: 746f 6c6f 6164 732f 676c 6f62 616c 2e67  toloads/global.g
 00018b90: 642e 7265 6d61 7000 d06b 6900 0000 0000  d.remap..ki.....
 00018ba0: 3300 0000 0000 0000 e785 3d92 7708 6721  3.........=.w.g!
 00018bb0: 4e79 86f9 49ed 9b23 2400 0000 7265 733a  Ny..I..#$...res:
 00018bc0: 2f2f 7363 7269 7074 732f 6175 746f 6c6f  //scripts/autolo
 00018bd0: 6164 732f 676c 6f62 616c 2e67 6463 0000  ads/global.gdc..
 00018be0: 901d 6700 0000 0000 cc0d 0000 0000 0000  ..g.............
-00018bf0: 32cc b3a4 b943 f97e 6d13 87d5 c3d0 7af2  2....C.~m.....z.
+00018bf0: 9991 07a7 c016 7cbb 9436 7e60 5a7d 07e7  ......|..6~`Z}..
 00018c00: 2c00 0000 7265 733a 2f2f 7363 7269 7074  ,...res://script
 00018c10: 732f 6175 746f 6c6f 6164 732f 6874 6d6c  s/autoloads/html
 00018c20: 5f66 696c 6573 2e67 642e 7265 6d61 7000  _files.gd.remap.
 00018c30: 106c 6900 0000 0000 3700 0000 0000 0000  .li.....7.......
 00018c40: e360 efb1 7a49 3540 9a66 a08e e66e 3601  .`..zI5@.f...n6.
 00018c50: 2800 0000 7265 733a 2f2f 7363 7269 7074  (...res://script
 00018c60: 732f 6175 746f 6c6f 6164 732f 6874 6d6c  s/autoloads/html
@@ -422464,15 +422464,15 @@
 006723f0: 0200 0000 3200 0000 0400 0000 0700 0000  ....2...........
 00672400: 7265 736f 746f 5f00 0400 0000 1400 0000  resoto_.........
 00672410: 7265 736f 746f 2e75 692e 6461 7368 626f  resoto.ui.dashbo
 00672420: 6172 642e 0400 0000 2200 0000 6874 7470  ard....."...http
 00672430: 733a 2f2f 6469 7363 6f72 642e 6767 2f73  s://discord.gg/s
 00672440: 6f6d 6565 6e67 696e 6565 7269 6e67 0000  omeengineering..
 00672450: 0100 0000 0000 0000 0300 0000 0000 803f  ...............?
-00672460: 0400 0000 0500 0000 332e 362e 3100 0000  ........3.6.1...
+00672460: 0400 0000 0500 0000 332e 362e 3200 0000  ........3.6.2...
 00672470: 0400 0000 0300 0000 6e2f 6100 0400 0000  ........n/a.....
 00672480: 0700 0000 5769 6e64 6f77 7300 0400 0000  ....Windows.....
 00672490: 0000 0000 0000 0000 0400 0000 0900 0000  ................
 006724a0: 6164 645f 746f 6173 7400 0000 0400 0000  add_toast.......
 006724b0: 0600 0000 5363 616c 6520 0000 0200 0000  ....Scale ......
 006724c0: 6400 0000 0400 0000 0100 0000 2500 0000  d...........%...
 006724d0: 0200 0000 0300 0000 0300 0100 6666 6666  ............ffff
```

### Comparing `resotoui-3.6.1/resotoui/ui/index.png` & `resotoui-3.6.2/resotoui/ui/index.png`

 * *Files identical despite different names*

### Comparing `resotoui-3.6.1/resotoui/ui/index.wasm` & `resotoui-3.6.2/resotoui/ui/index.wasm`

 * *Files identical despite different names*

### Comparing `resotoui-3.6.1/resotoui.egg-info/PKG-INFO` & `resotoui-3.6.2/resotoui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotoui
-Version: 3.6.1
+Version: 3.6.2
 Summary: The Resoto UI.
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `resotoui-3.6.1/setup.py` & `resotoui-3.6.2/setup.py`

 * *Files identical despite different names*

