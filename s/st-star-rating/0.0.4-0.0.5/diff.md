# Comparing `tmp/st_star_rating-0.0.4-py3-none-any.whl.zip` & `tmp/st_star_rating-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1163797 bytes, number of entries: 25
--rw-rw-rw-  2.0 fat     3037 b- defN 23-Jun-26 21:30 streamlit_star_rating/__init__.py
+Zip file size: 1163798 bytes, number of entries: 25
+-rw-rw-rw-  2.0 fat     3036 b- defN 23-Jun-26 21:52 streamlit_star_rating/__init__.py
 -rw-rw-rw-  2.0 fat      859 b- defN 23-Jun-26 21:48 streamlit_star_rating/frontend/build/asset-manifest.json
 -rw-rw-rw-  2.0 fat   206960 b- defN 23-May-01 13:24 streamlit_star_rating/frontend/build/bootstrap.min.css
 -rw-rw-rw-  2.0 fat     2073 b- defN 23-Jun-26 21:48 streamlit_star_rating/frontend/build/index.html
 -rw-rw-rw-  2.0 fat      585 b- defN 23-May-01 13:23 streamlit_star_rating/frontend/build/precache-manifest.a982ecc6e1bfb804d4fb37038240d2af.js
 -rw-rw-rw-  2.0 fat      564 b- defN 23-Jun-26 21:48 streamlit_star_rating/frontend/build/precache-manifest.f25caae44a80dcc0ba1ebb5511dccb6c.js
 -rw-rw-rw-  2.0 fat     1183 b- defN 23-Jun-26 21:48 streamlit_star_rating/frontend/build/service-worker.js
 -rw-rw-rw-  2.0 fat   671412 b- defN 23-May-01 13:23 streamlit_star_rating/frontend/build/static/js/2.76da4152.chunk.js
@@ -16,12 +16,12 @@
 -rw-rw-rw-  2.0 fat     3628 b- defN 23-May-01 13:23 streamlit_star_rating/frontend/build/static/js/main.6fe35020.chunk.js.map
 -rw-rw-rw-  2.0 fat     1516 b- defN 23-Jun-26 21:48 streamlit_star_rating/frontend/build/static/js/main.9ac02dd7.chunk.js
 -rw-rw-rw-  2.0 fat     4478 b- defN 23-Jun-26 21:48 streamlit_star_rating/frontend/build/static/js/main.9ac02dd7.chunk.js.map
 -rw-rw-rw-  2.0 fat     1585 b- defN 23-May-01 13:23 streamlit_star_rating/frontend/build/static/js/runtime-main.044ed49b.js
 -rw-rw-rw-  2.0 fat     8303 b- defN 23-May-01 13:23 streamlit_star_rating/frontend/build/static/js/runtime-main.044ed49b.js.map
 -rw-rw-rw-  2.0 fat     1570 b- defN 23-Jun-26 21:48 streamlit_star_rating/frontend/build/static/js/runtime-main.0e210323.js
 -rw-rw-rw-  2.0 fat     8289 b- defN 23-Jun-26 21:48 streamlit_star_rating/frontend/build/static/js/runtime-main.0e210323.js.map
--rw-rw-rw-  2.0 fat     2350 b- defN 23-Jun-26 21:50 st_star_rating-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-26 21:50 st_star_rating-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       22 b- defN 23-Jun-26 21:50 st_star_rating-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2960 b- defN 23-Jun-26 21:50 st_star_rating-0.0.4.dist-info/RECORD
-25 files, 5350117 bytes uncompressed, 1158707 bytes compressed:  78.3%
+-rw-rw-rw-  2.0 fat     2350 b- defN 23-Jun-26 21:53 st_star_rating-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-26 21:53 st_star_rating-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       22 b- defN 23-Jun-26 21:53 st_star_rating-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2960 b- defN 23-Jun-26 21:53 st_star_rating-0.0.5.dist-info/RECORD
+25 files, 5350116 bytes uncompressed, 1158708 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -57,20 +57,20 @@
 
 Filename: streamlit_star_rating/frontend/build/static/js/runtime-main.0e210323.js
 Comment: 
 
 Filename: streamlit_star_rating/frontend/build/static/js/runtime-main.0e210323.js.map
 Comment: 
 
-Filename: st_star_rating-0.0.4.dist-info/METADATA
+Filename: st_star_rating-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: st_star_rating-0.0.4.dist-info/WHEEL
+Filename: st_star_rating-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: st_star_rating-0.0.4.dist-info/top_level.txt
+Filename: st_star_rating-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: st_star_rating-0.0.4.dist-info/RECORD
+Filename: st_star_rating-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_star_rating/__init__.py

```diff
@@ -1,12 +1,12 @@
 import streamlit.components.v1 as components
 import os
 import warnings 
 
-_RELEASE = False
+_RELEASE = True
 
 
 if not _RELEASE:
     _component_func = components.declare_component(
         # We give the component a simple, descriptive name ("my_component"
         # does not fit this bill, so please choose something better for your
         # own component :)
```

## Comparing `st_star_rating-0.0.4.dist-info/METADATA` & `st_star_rating-0.0.5.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-star-rating
-Version: 0.0.4
+Version: 0.0.5
 Summary: Streamlit Component for Star Ratings
 Home-page: 
 Author: 
 Author-email: 
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit (>=0.63)
```

### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_losazas6_/tmpqk_iibk0_ZipContainer/METADATA", line 70, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_losazas6_/tmpqk_iibk0_ZipContainer/METADATA", line 70, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: st-star-rating Version: 0.0.4 Summary: Streamlit
+Metadata-Version: 2.1 Name: st-star-rating Version: 0.0.5 Summary: Streamlit
 Component for Star Ratings Home-page: Author: Author-email: Requires-Python:
 >=3.6 Description-Content-Type: text/markdown Requires-Dist: streamlit (>=0.63)
 Streamlit Star Rating Component === This streamlit component adds a star
 selector to Streamlit Apps. It implements the Baseui Rating implementation:
 https://baseweb.design/components/rating/ Installation ----------- $ pip
 install st-star-rating Usage ------------ ## Import the Component $ from
 streamlit_star_rating import st_star_rating $ stars = st_star_rating("Please
```

## Comparing `st_star_rating-0.0.4.dist-info/RECORD` & `st_star_rating-0.0.5.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-streamlit_star_rating/__init__.py,sha256=zkNTNMM9Tl8BiT3KUhLyrb_MPvnGriyH7vp_UQC3woQ,3037
+streamlit_star_rating/__init__.py,sha256=56MR1_QOjI94__9cyIwhGv-ZXnJeVUQjZ_AF1Xr37eo,3036
 streamlit_star_rating/frontend/build/asset-manifest.json,sha256=YJAvAjpJYVBdveTBnxv5JzPEXVSq5Cx0ptEbEnf81no,859
 streamlit_star_rating/frontend/build/bootstrap.min.css,sha256=X9ITP3t3djkRs4SffIkA1Q2WMy-oYl6au5HFYTVShe0,206960
 streamlit_star_rating/frontend/build/index.html,sha256=qaioWqZwhIY-AOLKgvKaXaJ06peEkLqwHOOPm1ZN5LQ,2073
 streamlit_star_rating/frontend/build/precache-manifest.a982ecc6e1bfb804d4fb37038240d2af.js,sha256=4eN7RRP61PEFZqphruJ350ItVOoGWHo57pqNIriWikg,585
 streamlit_star_rating/frontend/build/precache-manifest.f25caae44a80dcc0ba1ebb5511dccb6c.js,sha256=ESiG8usgqZEsNulXo9_ReB1Ff46bt1BfXoIerx95xHc,564
 streamlit_star_rating/frontend/build/service-worker.js,sha256=K6jEh3At34BPZHSXp3hhVSL6x4qlCKdQNsgsAIh8bEo,1183
 streamlit_star_rating/frontend/build/static/js/2.76da4152.chunk.js,sha256=ReeGMww1uecDDnmIONTvfqXKPDTaW1UOWdqjCU5LnUs,671412
@@ -15,11 +15,11 @@
 streamlit_star_rating/frontend/build/static/js/main.6fe35020.chunk.js.map,sha256=mdrPa9v-uF7yVyZ6o8mDfsakwe-xZxF4g2VEW8g6Ep0,3628
 streamlit_star_rating/frontend/build/static/js/main.9ac02dd7.chunk.js,sha256=H1FxRxeOsUPbksmjRC5Sx4JeZXkvDelkugW6BTJe5rs,1516
 streamlit_star_rating/frontend/build/static/js/main.9ac02dd7.chunk.js.map,sha256=Iq8DjUWFIQev1uDqOZaXiKyHl5eXvMRhGfrop4pxkMo,4478
 streamlit_star_rating/frontend/build/static/js/runtime-main.044ed49b.js,sha256=4SRplXOrTUUw873Lb-ZJ0mQEoTatptNpKHyYPE4-VlU,1585
 streamlit_star_rating/frontend/build/static/js/runtime-main.044ed49b.js.map,sha256=kSuBgeFfR4YfdMPy5fe37W9opUPkT3dergoUyRWLljg,8303
 streamlit_star_rating/frontend/build/static/js/runtime-main.0e210323.js,sha256=4TpqVLYNzMygtOl5NlFGjkNR9pTnTjzd5JdvyernJgM,1570
 streamlit_star_rating/frontend/build/static/js/runtime-main.0e210323.js.map,sha256=LmI-jnb1JtayIxnFClk79gOZSVh9CSUdvIYEV0h7pLw,8289
-st_star_rating-0.0.4.dist-info/METADATA,sha256=dV6ErkunLMYPnEzzEYrmYHL7cK-m5tNu7RkPx67HNSo,2350
-st_star_rating-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-st_star_rating-0.0.4.dist-info/top_level.txt,sha256=c3OZMIZJp2pST4NzQDjDkPWImhSL2v9baszqE3yc1O4,22
-st_star_rating-0.0.4.dist-info/RECORD,,
+st_star_rating-0.0.5.dist-info/METADATA,sha256=rt-sJov7zZUk735WFVvwqUQsyFKncG39QJvdXPBmCTU,2350
+st_star_rating-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+st_star_rating-0.0.5.dist-info/top_level.txt,sha256=c3OZMIZJp2pST4NzQDjDkPWImhSL2v9baszqE3yc1O4,22
+st_star_rating-0.0.5.dist-info/RECORD,,
```

