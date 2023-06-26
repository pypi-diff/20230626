# Comparing `tmp/araste-3.1-py3-none-any.whl.zip` & `tmp/araste-3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,20 @@
-Zip file size: 35138 bytes, number of entries: 15
--rw-rw-r--  2.0 unx    10346 b- defN 23-Jun-16 16:17 araste/__init__.py
--rw-rw-r--  2.0 unx     6731 b- defN 23-Jun-06 15:24 araste/filters.py
+Zip file size: 41751 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx    10515 b- defN 23-Jun-26 17:32 araste/__init__.py
+-rw-rw-r--  2.0 unx     9774 b- defN 23-Jun-25 12:23 araste/char_maps.py
+-rw-rw-r--  2.0 unx     8732 b- defN 23-Jun-25 12:06 araste/filters.py
+-rw-rw-r--  2.0 unx     2687 b- defN 23-Jun-25 12:11 araste/tmp.py
 -rw-rw-r--  2.0 unx    21914 b- defN 22-Nov-05 11:36 araste/fonts/aipara.aff
--rw-rw-r--  2.0 unx     4767 b- defN 22-Nov-05 11:36 araste/fonts/aipara_mini.aff
--rw-rw-r--  2.0 unx     7851 b- defN 23-Jun-16 11:57 araste/fonts/naqshe.aff
--rw-rw-r--  2.0 unx    22358 b- defN 23-Jun-16 13:23 araste/fonts/nima.aff
+-rw-rw-r--  2.0 unx     4504 b- defN 23-Jun-25 12:48 araste/fonts/aipara_mini.aff
+-rw-rw-r--  2.0 unx    22447 b- defN 23-Jun-24 16:56 araste/fonts/danial.aff
+-rw-rw-r--  2.0 unx     7862 b- defN 23-Jun-25 11:38 araste/fonts/naqshe.aff
+-rw-rw-r--  2.0 unx    22358 b- defN 23-Jun-25 12:08 araste/fonts/nima.aff
 -rw-rw-r--  2.0 unx    22232 b- defN 23-Jun-16 16:15 araste/fonts/nima2.aff
 -rw-rw-r--  2.0 unx    20050 b- defN 22-Nov-05 11:36 araste/fonts/zivar.aff
--rwxrwxr-x  2.0 unx     2778 b- defN 23-Jun-16 16:18 araste-3.1.data/scripts/araste
--rwxrwxr-x  2.0 unx     3797 b- defN 23-Jun-16 16:18 araste-3.1.data/scripts/araste-get
--rw-rw-r--  2.0 unx    34523 b- defN 23-Jun-16 16:18 araste-3.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2215 b- defN 23-Jun-16 16:18 araste-3.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-16 16:18 araste-3.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jun-16 16:18 araste-3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1184 b- defN 23-Jun-16 16:18 araste-3.1.dist-info/RECORD
-15 files, 160845 bytes uncompressed, 33212 bytes compressed:  79.4%
+-rwxrwxr-x  2.0 unx     2778 b- defN 23-Jun-26 17:32 araste-3.2.data/scripts/araste
+-rwxrwxr-x  2.0 unx     3797 b- defN 23-Jun-26 17:32 araste-3.2.data/scripts/araste-get
+-rw-rw-r--  2.0 unx    34523 b- defN 23-Jun-26 17:32 araste-3.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3657 b- defN 23-Jun-26 17:32 araste-3.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 17:32 araste-3.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-26 17:32 araste-3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1411 b- defN 23-Jun-26 17:32 araste-3.2.dist-info/RECORD
+18 files, 199340 bytes uncompressed, 39487 bytes compressed:  80.2%
```

## zipnote {}

```diff
@@ -1,46 +1,55 @@
 Filename: araste/__init__.py
 Comment: 
 
+Filename: araste/char_maps.py
+Comment: 
+
 Filename: araste/filters.py
 Comment: 
 
+Filename: araste/tmp.py
+Comment: 
+
 Filename: araste/fonts/aipara.aff
 Comment: 
 
 Filename: araste/fonts/aipara_mini.aff
 Comment: 
 
+Filename: araste/fonts/danial.aff
+Comment: 
+
 Filename: araste/fonts/naqshe.aff
 Comment: 
 
 Filename: araste/fonts/nima.aff
 Comment: 
 
 Filename: araste/fonts/nima2.aff
 Comment: 
 
 Filename: araste/fonts/zivar.aff
 Comment: 
 
-Filename: araste-3.1.data/scripts/araste
+Filename: araste-3.2.data/scripts/araste
 Comment: 
 
-Filename: araste-3.1.data/scripts/araste-get
+Filename: araste-3.2.data/scripts/araste-get
 Comment: 
 
-Filename: araste-3.1.dist-info/LICENSE
+Filename: araste-3.2.dist-info/LICENSE
 Comment: 
 
-Filename: araste-3.1.dist-info/METADATA
+Filename: araste-3.2.dist-info/METADATA
 Comment: 
 
-Filename: araste-3.1.dist-info/WHEEL
+Filename: araste-3.2.dist-info/WHEEL
 Comment: 
 
-Filename: araste-3.1.dist-info/top_level.txt
+Filename: araste-3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: araste-3.1.dist-info/RECORD
+Filename: araste-3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## araste/__init__.py

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python3
-__version__ = "3.1"
+__version__ = "3.2"
 
 import os
 import sys
 from araste.filters import apply_filter
 
 # copy a block into the board
 def copyboard_glyph(blockstr: str, cursor: int, board: list, korsi: int) -> tuple:
@@ -251,15 +251,21 @@
     else:
         boardw = width
 
     # get width of each character
     glyphs_width = {}
     for character in glyph_data.keys():
         # max_line_width = max([len(line) for line in font_glyphs[character].split('\n')])
-        max_line_width = len(glyph_data[character][1].split('\n')[korsi])
+
+        try:
+            max_line_width = len(glyph_data[character][1].split('\n')[korsi])
+        except IndexError:
+            print(f'there is an Error in font file. is the Korsi set correctly?', file=sys.stderr)
+            sys.exit(1)
+
         glyphs_width[character] = max_line_width
 
     # generate an empty board
     board = [[empty_char for _ in range(boardw)] for _ in range(boardh)]
 
     # rtl cursor
     cursor = boardw
```

## araste/filters.py

```diff
@@ -1,22 +1,23 @@
 # filters for araste output are here
 import re
+from .char_maps import hmirror_character_alternatives, vmirror_character_alternatives, flip90_character_alternatives
 
 def apply_filter(text: str, filter_name: str) -> str:
 
     filter_map = {
         'rainbow': rainbow,
         'vrainbow': rainbow_vertical,
         'hrainbow': rainbow_horizontal,
         'box': box,
-        'vmirror': vertical_mirror,
-        'hmirror': horizontal_mirror,
+        'vmirror': character_aware_vertical_mirror,
+        'hmirror': character_aware_horizontal_mirror,
         'ritalic': italic_right,
         'litalic': italic_left,
-        'flip90': flip90,
+        'flip90': character_aware_flip90,
         'hgrow': grow_horizontal,
         'vgrow': grow_vertical,
         'red': lambda x: color('red', x),
         'orange': lambda x: color('orange', x),
         'yellow': lambda x: color('yellow', x),
         'green': lambda x: color('green', x),
         'cyan': lambda x: color('cyan', x),
@@ -140,14 +141,27 @@
 def vertical_mirror(art: str) -> str:
     art_lines = art.split('\n')
     art_lines.reverse()
     output = '\n'.join(art_lines)
 
     return output
 
+
+def character_aware_vertical_mirror(art: str) -> str:
+    art_lines = art.split('\n')
+    art_lines.reverse()
+    output = ''
+    for line in art_lines:
+        output_line = ''.join([vmirror_character_alternatives[char] if char in vmirror_character_alternatives.keys() else char for char in line])
+        output += output_line + '\n'
+    output = output[:-1]
+
+    return output
+
+
 def horizontal_mirror(art: str) -> str:
     art_lines = art.split('\n')
     ansi_escape_regex = r'((\x9B|\x1B\[)[0-?]*[ -\/]*[@-~])'
 
     output = ''
 
     for line in art_lines:    
@@ -159,14 +173,42 @@
                 reversed_string += code
             else:
                 reversed_string += code[::-1]
         output += reversed_string + '\n'
 
     return output[:-1]
 
+
+def character_aware_horizontal_mirror(art:str) -> str:
+    art_lines = art.split('\n')
+    ansi_escape_regex = r'((\x9B|\x1B\[)[0-?]*[ -\/]*[@-~])'
+
+    output = ''
+
+    for line in art_lines:    
+        chars_and_escape_codes = re.split(ansi_escape_regex, line)
+        # chars_and_escape_codes.reverse()
+        reversed_string = ''
+        for code in chars_and_escape_codes[::-1]:
+            if re.match(ansi_escape_regex, code):
+                reversed_string += code
+            else:
+                line = ''
+                for char in code[::-1]:
+                    if char in hmirror_character_alternatives.keys():
+                        reversed_string += hmirror_character_alternatives[char]
+                    else:
+                        reversed_string += char
+
+                # reversed_string += code[::-1]
+        output += reversed_string + '\n'
+
+    return output[:-1]
+
+
 def italic_right(art: str) -> str:
     art_lines = art.split('\n')
     output = ''
     numof_lines = len(art_lines)
     for i, line in enumerate(art_lines):
         output += ' ' * ((numof_lines - i)) + line + '\n'
     
@@ -196,14 +238,35 @@
     output = ''
 
     for line in char_list_flipped[::-1]:
         output += ''.join(line) + '\n'
 
     return output[:-1]
 
+
+def character_aware_flip90(art: str) -> str:
+    art_lines = art.split('\n')
+
+    # make a 2d matrix of chars
+    art_char_list = [
+        [flip90_character_alternatives[char] if char in flip90_character_alternatives.keys() else char for char in list(line)]
+        for line in art_lines]
+
+    # transpose char matrix
+    char_list_flipped = list(map(list, zip(*art_char_list)))
+
+    # start writing matrix content into output
+    output = ''
+
+    for line in char_list_flipped[::-1]:
+        output += ''.join(line) + '\n'
+
+    return output[:-1]
+
+
 def grow_horizontal(art: str) -> str:
     grow_ratio = 2
 
     art_lines = art.split('\n')
 
     output = ''
```

## araste/fonts/aipara_mini.aff

```diff
@@ -1,1101 +1,833 @@
-aff3 6 5 4 5 137 1
+aff3 4 3 4 5 138 1
 aipara_mini font
     this is a font file for araste
     designed by Erfan Kheyrollahi <ekm507@gmail.com>
 
 ا
 4 1
-
-
 ▗
 ▐
 ▝
  
 ا
 3 1
-
-
 ▗
 ▐
 ▝
  
 ا
 2 1
-
-
 ▗
 ▐
 ▝
  
 ا
 1 1
-
-
 ▗
 ▐
 ▝
  
 ب
 4 1
-
-
    
 ▗ ▗
 ▝▀▀
  ▝ 
 ب
 3 1
-
-
    
 ▗ ▗
 ▝▀▀
  ▝ 
 ب
 2 1
-
-
  
 ▗
 ▀
 ▝
 ب
 1 1
-
-
  
 ▗
 ▀
 ▝
 پ
 4 1
-
-
    
 ▗ ▗
 ▝▀▀
  ▝▍
 پ
 3 1
-
-
    
 ▗ ▗
 ▝▀▀
  ▝▍
 پ
 2 1
-
-
   
  ▖
 ▀▀
 ▝▍
 پ
 1 1
-
-
   
  ▖
 ▀▘
 ▝▍
 ت
 4 1
-
-
  ▃ 
 ▗ ▗
 ▝▀▀
    
 ت
 3 1
-
-
  ▃ 
 ▗ ▗
 ▝▀▀
    
 ت
 2 1
-
-
 ▗▖
  ▖
 ▀▀
   
 ت
 1 1
-
-
 ▗▖
  ▖
 ▀▘
   
 ث
 4 1
-
-
  ▟ 
 ▗ ▗
 ▝▀▀
    
 ث
 3 1
-
-
  ▟ 
 ▗ ▗
 ▝▀▀
    
 ث
 2 1
-
-
 ▗▍
  ▖
 ▀▀
   
 ث
 1 1
-
-
 ▗▍
  ▖
 ▀▘
   
 ج
 4 1
-
-
    
  ▝▖
 ▗▀▘
 ▝▖▘
 ج
 3 1
-
-
    
  ▝▖
 ▗▀▀
 ▝▖▘
 ج
 2 1
-
-
   
 ▝▖
 ▀▀
 ▝ 
 ج
 1 1
-
-
   
 ▝▖
 ▀▘
 ▝ 
 چ
 4 1
-
-
    
  ▝▖
 ▗▀▘
 ▝▞▍
 چ
 3 1
-
-
    
  ▝▖
 ▗▀▀
 ▝▞▍
 چ
 2 1
-
-
   
 ▝▖
 ▀▀
 ▝▍
 چ
 1 1
-
-
   
 ▝▖
 ▀▘
 ▝▍
 ح
 4 1
-
-
    
  ▝▖
 ▗▀▘
 ▝▖ 
 ح
 3 1
-
-
    
  ▝▖
 ▗▀▀
 ▝▖ 
 ح
 2 1
-
-
   
 ▝▖
 ▀▀
   
 ح
 1 1
-
-
   
 ▝▖
 ▀▘
   
 خ
 4 1
-
-
  ▝ 
  ▝▖
 ▗▀▘
 ▝▖ 
 خ
 3 1
-
-
  ▝ 
  ▝▖
 ▗▀▀
 ▝▖ 
 خ
 2 1
-
-
 ▝ 
 ▝▖
 ▀▀
   
 خ
 1 1
-
-
 ▝ 
 ▝▖
 ▀▘
   
 د
 4 1
-
-
   
 ▝▖
 ▝▘
   
 د
 3 1
-
-
   
 ▝▖
 ▝▀
   
 د
 2 1
-
-
   
 ▝▖
 ▝▀
   
 د
 1 1
-
-
   
 ▝▖
 ▝▘
   
 ذ
 4 1
-
-
 ▝ 
 ▝▖
 ▝▘
   
 ذ
 3 1
-
-
 ▝ 
 ▝▖
 ▝▀
   
 ذ
 2 1
-
-
 ▝ 
 ▝▖
 ▝▀
   
 ذ
 1 1
-
-
 ▝ 
 ▝▖
 ▝▘
   
 ر
 4 1
-
-
   
  ▖
  ▍
 ▝ 
 ر
 3 1
-
-
   
  ▖
  ▛
 ▝ 
 ر
 2 1
-
-
   
  ▖
  ▛
 ▝ 
 ر
 1 1
-
-
   
  ▖
  ▍
 ▝ 
 ز
 4 1
-
-
  ▖
  ▖
  ▍
 ▝ 
 ز
 3 1
-
-
  ▖
  ▖
  ▛
 ▝ 
 ز
 2 1
-
-
  ▖
  ▖
  ▛
 ▝ 
 ز
 1 1
-
-
  ▖
  ▖
  ▍
 ▝ 
 ٓ
 4 1
-
-
  
  
  
  
 ٓ
 3 1
-
-
  
  
  
  
 ٓ
 2 1
-
-
  
  
  
  
 ٓ
 1 1
-
-
  
  
  
  
 س
 4 1
-
-
      
   ▖▖▖
 ▐ ▛▀▘
 ▝▀▘  
 س
 3 1
-
-
      
   ▖▖▖
 ▐ ▛▀▀
 ▝▀▘  
 س
 2 1
-
-
     
  ▖▖▖
 ▀▀▀▀
     
 س
 1 1
-
-
     
  ▖▖▖
 ▀▀▀▘
     
 ش
 4 1
-
-
   ▗▍ 
   ▖▖▖
 ▐ ▛▀▘
 ▝▀▘  
 ش
 3 1
-
-
   ▗▍ 
   ▖▖▖
 ▐ ▛▀▀
 ▝▀▘  
 ش
 2 1
-
-
  ▗▍ 
  ▖▖▖
 ▀▀▀▀
     
 ش
 1 1
-
-
  ▗▍ 
  ▖▖▖
 ▀▀▀▘
     
 ص
 4 1
-
-
      
   ▖▞▍
 ▐ ▛▀▘
 ▝▀▘  
 ص
 3 1
-
-
      
   ▖▞▍
 ▐ ▛▀▀
 ▝▀▘  
 ص
 2 1
-
-
    
 ▗▗▜
 ▀▀▀
    
 ص
 1 1
-
-
    
 ▗▗▜
 ▀▀▀
    
 ض
 4 1
-
-
    ▝ 
   ▖▞▍
 ▐ ▛▀▘
 ▝▀▘  
 ض
 3 1
-
-
    ▝ 
   ▖▞▍
 ▐ ▛▀▀
 ▝▀▘  
 ض
 2 1
-
-
   ▘
 ▗▗▜
 ▀▀▀
    
 ض
 1 1
-
-
   ▘
 ▗▗▜
 ▀▀▀
    
 ط
 4 1
-
-
  ▖ 
  ▙▖
 ▝▀▘
    
 ط
 3 1
-
-
  ▖ 
  ▙▖
 ▝▀▀
    
 ط
 2 1
-
-
 ▗ 
 ▐▃
 ▀▀
   
 ط
 1 1
-
-
 ▗ 
 ▐▃
 ▀▀
   
 ظ
 4 1
-
-
  ▖▖
  ▙▖
 ▝▀▘
    
 ظ
 3 1
-
-
  ▖▖
  ▙▖
 ▝▀▀
    
 ظ
 2 1
-
-
 ▗▗
 ▐▃
 ▀▀
   
 ظ
 1 1
-
-
 ▗▗
 ▐▃
 ▀▀
   
 ع
 4 1
-
-
    
  ▐▘
 ▗▀▘
 ▝▃ 
 ع
 3 1
-
-
    
  ▜▘
 ▗▀▀
 ▝▃ 
 ع
 2 1
-
-
   
 ▝▛
 ▀▀
   
 ع
 1 1
-
-
   
 ▐▘
 ▀▘
   
 غ
 4 1
-
-
   ▘
  ▐▘
 ▗▀▘
 ▝▃ 
 غ
 3 1
-
-
  ▝ 
  ▜▘
 ▗▀▀
 ▝▃ 
 غ
 2 1
-
-
  ▘
 ▝▛
 ▀▀
   
 غ
 1 1
-
-
  ▘
 ▐▘
 ▀▘
   
 ف
 4 1
-
-
    ▖
 ▗ ▗▖
 ▝▀▀▘
     
 ف
 3 1
-
-
    ▖
 ▗ ▗▖
 ▝▀▀▀
     
 ف
 2 1
-
-
  ▖
 ▗▖
 ▀▀
   
 ف
 1 1
-
-
  ▖
 ▗▖
 ▀▘
   
 ق
 4 1
-
-
   ▃
   ▃
 ▐ ▜
 ▝▃▞
 ق
 3 1
-
-
   ▃
   ▃
 ▐ ▜
 ▝▃▞
 ق
 2 1
-
-
 ▗▖
 ▗▖
 ▀▀
   
 ق
 1 1
-
-
 ▗▖
 ▗▖
 ▀▘
   
 ک
 4 1
-
-
    ▖
 ▗ ▐▖
 ▝▀▀▘
     
 ک
 3 1
-
-
    ▖
 ▗ ▐▖
 ▝▀▀▀
     
 ک
 2 1
-
-
  ▖
 ▐▖
 ▀▀
   
 ک
 1 1
-
-
  ▖
 ▐▖
 ▀▘
   
 گ
 4 1
-
-
   ▝▖
 ▗ ▐▖
 ▝▀▀▘
     
 گ
 3 1
-
-
   ▝▖
 ▗ ▐▖
 ▝▀▀▀
     
 گ
 2 1
-
-
 ▝▖
 ▐▖
 ▀▀
   
 گ
 1 1
-
-
 ▝▖
 ▐▖
 ▀▘
   
 ل
 4 1
-
-
   ▖
   ▍
 ▗ ▍
 ▝▃▘
 ل
 3 1
-
-
   ▖
   ▍
 ▗ ▛
 ▝▃▘
 ل
 2 1
-
-
 ▗
 ▐
 ▀
  
 ل
 1 1
-
-
 ▗
 ▐
 ▀
  
 م
 4 1
-
-
   
  ▃
 ▐▀
 ▐ 
 م
 3 1
-
-
   
  ▃
 ▐▀
 ▐ 
 م
 2 1
-
-
   
   
 ▜▛
   
 م
 1 1
-
-
   
 ▗▖
 ▀▘
   
 ن
 4 1
-
-
    
  ▘▖
 ▐ ▍
 ▝▀▘
 ن
 3 1
-
-
    
  ▘▖
 ▐ ▛
 ▝▀▘
 ن
 2 1
-
-
 ▗
 ▗
 ▀
  
 ن
 1 1
-
-
 ▗
 ▗
 ▀
  
 و
 4 1
-
-
   
 ▗▖
 ▝▍
 ▝ 
 و
 3 1
-
-
   
 ▗▖
 ▝▛
 ▝ 
 و
 2 1
-
-
   
 ▗▖
 ▝▛
 ▝ 
 و
 1 1
-
-
   
 ▗▖
 ▝▍
 ▝ 
 ه
 4 1
-
-
   
 ▗▍
 ▝▘
   
 ه
 3 1
-
-
   
 ▐▍
  ▀
   
 ه
 2 1
-
-
  
  
 ▚
  
 ه
 1 1
-
-
   
 ▗▍
 ▀▘
   
 ی
 4 1
-
-
    
   ▖
 ▐▝▖
  ▀ 
 ی
 3 1
-
-
    
    
 ▗▗▀
 ▝▃▘
 ی
 2 1
-
-
   
  ▖
 ▀▀
 ▝▘
 ی
 1 1
-
-
   
  ▖
 ▀▘
 ▝▘
 ژ
 4 1
-
-
 ▗▍
  ▖
  ▍
 ▝ 
 ژ
 3 1
-
-
 ▗▍
  ▖
  ▛
 ▝ 
 ژ
 2 1
-
-
 ▗▍
  ▖
  ▛
 ▝ 
 ژ
 1 1
-
-
 ▗▍
  ▖
  ▍
 ▝ 
 آ
 4 1
-
-
 ▐▀
  ▍
  ▘
   
 آ
 3 1
-
-
 ▐▀
  ▍
  ▘
   
 آ
 2 1
-
-
 ▐▀
  ▍
  ▘
   
 آ
 1 1
-
-
 ▐▀
  ▍
  ▘
   
  
 4 0
 
 
  
- 
- 
- 
+  
+‌
+4 0
+
+
+
+
```

## araste/fonts/naqshe.aff

```diff
@@ -665,14 +665,19 @@
 ⢠⠀⣔⡂
 ⠈⠒⠒⠁
  
 0 0
 ⠀⠀
 ⠀⠀
 ⠀⠀
+‌
+0 0
+
+
+
 (
 3 1
 ⢠⠀
 ⠀⡇
 ⠰⠁
 (
 2 1
```

## Comparing `araste-3.1.data/scripts/araste` & `araste-3.2.data/scripts/araste`

 * *Files identical despite different names*

## Comparing `araste-3.1.data/scripts/araste-get` & `araste-3.2.data/scripts/araste-get`

 * *Files identical despite different names*

## Comparing `araste-3.1.dist-info/LICENSE` & `araste-3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `araste-3.1.dist-info/RECORD` & `araste-3.2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-araste/__init__.py,sha256=IQR7JHBsVV3aQWcT9lrEurogaKXhl4lL6Up0zfZgKvs,10346
-araste/filters.py,sha256=Gvi89NFKDm04D7FB1oCU4N4-N3TNs5YzcKB_wtWg6qk,6731
+araste/__init__.py,sha256=GN6Gd0BrKQwZAm2xtn1EbPDt29MEpZ_d7pIFg6yBYgg,10515
+araste/char_maps.py,sha256=yxWVXH-c2Aqtqfnc6TLoxXhEECl3h1WsuGZe38FaFl0,9774
+araste/filters.py,sha256=hYPbd3a10tYp51WpsyLGiQCFO4K7PeBXQAJ63QATt5o,8732
+araste/tmp.py,sha256=hBNMkFstflKKAijudX1kwg01VfofFo8KOPvXWDNkKIU,2687
 araste/fonts/aipara.aff,sha256=l2P0fP8LvXe31wkuhrDTbFrmBzPr304y2RkaLFVwAsQ,21914
-araste/fonts/aipara_mini.aff,sha256=lXrk1OpVJLtc45K5lqN74KXw8n5KfLi0NdQrDCU_M-c,4767
-araste/fonts/naqshe.aff,sha256=dAd4UKA_R64f7tKPnsah0g6GlRqwUoQmsdnZK5OaAp8,7851
+araste/fonts/aipara_mini.aff,sha256=KLhu6LYI82FQJ5r4oIA5oBU7tANhmBah4PaIfpw-sYM,4504
+araste/fonts/danial.aff,sha256=SQw7i8kJhbgQ2p68Bo3VykiqKuwNyCtS0Wek4GiIbHc,22447
+araste/fonts/naqshe.aff,sha256=HjgNSgNVPPWkpHXxOdgWR-IeOEyG_eBlBc99a0kFYJE,7862
 araste/fonts/nima.aff,sha256=KNiuYeyiPZzKqpodgOJVUcP5TQ-GEMms4J_aw0SQBA4,22358
 araste/fonts/nima2.aff,sha256=xPLJ3tqKBW4z0Jwt_iYdjjl93ih7NPi6HZpj_zZMcBA,22232
 araste/fonts/zivar.aff,sha256=rBTpxxJ_AAFx9KuDb6lZplq3DVM8PyzN_IsgFoTX4Ps,20050
-araste-3.1.data/scripts/araste,sha256=mbO-pzer332TrjpBLQZPEOYILzZUZ7AhmuHBspoXQsw,2778
-araste-3.1.data/scripts/araste-get,sha256=i14FcpyzNO0gIQUYxMpGAeLb2fmXxuiCIIPHmlP-NaQ,3797
-araste-3.1.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-araste-3.1.dist-info/METADATA,sha256=cNxw8j9FFFtaiCKU5nGmb03qns9HtwFjpmsvQU65xbQ,2215
-araste-3.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-araste-3.1.dist-info/top_level.txt,sha256=4kgusdipgAhPRJu18_01Rx9zsgSwu5uApfskLdcopIw,7
-araste-3.1.dist-info/RECORD,,
+araste-3.2.data/scripts/araste,sha256=mbO-pzer332TrjpBLQZPEOYILzZUZ7AhmuHBspoXQsw,2778
+araste-3.2.data/scripts/araste-get,sha256=i14FcpyzNO0gIQUYxMpGAeLb2fmXxuiCIIPHmlP-NaQ,3797
+araste-3.2.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+araste-3.2.dist-info/METADATA,sha256=-Xw83npj-GsXd2VkMofxwNHRT32pSnvfG6VD37QuvcE,3657
+araste-3.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+araste-3.2.dist-info/top_level.txt,sha256=4kgusdipgAhPRJu18_01Rx9zsgSwu5uApfskLdcopIw,7
+araste-3.2.dist-info/RECORD,,
```

