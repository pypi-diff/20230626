# Comparing `tmp/pyasic-0.9.3.tar.gz` & `tmp/pyasic-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyasic-0.9.3.tar", max compression
+gzip compressed data, was "pyasic-0.9.4.tar", max compression
```

## Comparing `pyasic-0.9.3.tar` & `pyasic-0.9.4.tar`

### file list

```diff
@@ -1,174 +1,174 @@
--rw-r--r--   0        0        0     7905 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/API/__init__.py
--rw-r--r--   0        0        0    15503 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/API/bmminer.py
--rw-r--r--   0        0        0     6917 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/API/bosminer.py
--rw-r--r--   0        0        0    25107 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/API/btminer.py
--rw-r--r--   0        0        0    15314 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/API/cgminer.py
--rw-r--r--   0        0        0     2814 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/API/unknown.py
--rw-r--r--   0        0        0        0 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/__init__.py
--rw-r--r--   0        0        0    13068 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/config/__init__.py
--rw-r--r--   0        0        0     4136 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/data/__init__.py
--rw-r--r--   0        0        0      848 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/logger/__init__.py
--rw-r--r--   0        0        0     2917 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/miners/__init__.py
--rw-r--r--   0        0        0      145 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/miners/_backends/__init__.py
--rw-r--r--   0        0        0     9280 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/miners/_backends/bmminer.py
--rw-r--r--   0        0        0    15003 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/miners/_backends/bosminer.py
--rw-r--r--   0        0        0     1585 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/miners/_backends/bosminer_old.py
--rw-r--r--   0        0        0     8479 2022-07-11 14:30:25.864376 pyasic-0.9.3/pyasic/miners/_backends/btminer.py
--rw-r--r--   0        0        0     6949 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_backends/cgminer.py
--rw-r--r--   0        0        0     1776 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_backends/hiveon.py
--rw-r--r--   0        0        0       77 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/__init__.py
--rw-r--r--   0        0        0      227 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X17/S17.py
--rw-r--r--   0        0        0      232 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X17/S17_Plus.py
--rw-r--r--   0        0        0      234 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X17/S17_Pro.py
--rw-r--r--   0        0        0      230 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X17/S17e.py
--rw-r--r--   0        0        0      227 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X17/T17.py
--rw-r--r--   0        0        0      232 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X17/T17_Plus.py
--rw-r--r--   0        0        0      229 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X17/T17e.py
--rw-r--r--   0        0        0      177 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X17/__init__.py
--rw-r--r--   0        0        0      227 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X19/S19.py
--rw-r--r--   0        0        0      235 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X19/S19_Pro.py
--rw-r--r--   0        0        0      229 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X19/S19a.py
--rw-r--r--   0        0        0      230 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X19/S19j.py
--rw-r--r--   0        0        0      237 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X19/S19j_Pro.py
--rw-r--r--   0        0        0      227 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X19/T19.py
--rw-r--r--   0        0        0      149 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X19/__init__.py
--rw-r--r--   0        0        0      225 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X9/S9.py
--rw-r--r--   0        0        0      227 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X9/S9i.py
--rw-r--r--   0        0        0      225 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X9/T9.py
--rw-r--r--   0        0        0       59 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/X9/__init__.py
--rw-r--r--   0        0        0       56 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/antminer/__init__.py
--rw-r--r--   0        0        0      242 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/avalonminer/A10X/A1026.py
--rw-r--r--   0        0        0      242 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/avalonminer/A10X/A1047.py
--rw-r--r--   0        0        0      243 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/avalonminer/A10X/A1066.py
--rw-r--r--   0        0        0       90 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/avalonminer/A10X/__init__.py
--rw-r--r--   0        0        0      295 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/avalonminer/A7X/A721.py
--rw-r--r--   0        0        0      295 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/avalonminer/A7X/A741.py
--rw-r--r--   0        0        0      295 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/avalonminer/A7X/A761.py
--rw-r--r--   0        0        0       84 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/avalonminer/A7X/__init__.py
--rw-r--r--   0        0        0      296 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/avalonminer/A8X/A821.py
--rw-r--r--   0        0        0      296 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/avalonminer/A8X/A841.py
--rw-r--r--   0        0        0      296 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/avalonminer/A8X/A851.py
--rw-r--r--   0        0        0       84 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/avalonminer/A8X/__init__.py
--rw-r--r--   0        0        0      296 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/avalonminer/A9X/A921.py
--rw-r--r--   0        0        0       28 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/avalonminer/A9X/__init__.py
--rw-r--r--   0        0        0       77 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/avalonminer/__init__.py
--rw-r--r--   0        0        0      229 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/whatsminer/M2X/M20S.py
--rw-r--r--   0        0        0      234 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/whatsminer/M2X/M20S_Plus.py
--rw-r--r--   0        0        0      228 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/whatsminer/M2X/M21.py
--rw-r--r--   0        0        0      630 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/whatsminer/M2X/M21S.py
--rw-r--r--   0        0        0      235 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/whatsminer/M2X/M21S_Plus.py
--rw-r--r--   0        0        0      150 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/whatsminer/M2X/__init__.py
--rw-r--r--   0        0        0     1039 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/whatsminer/M3X/M30S.py
--rw-r--r--   0        0        0      858 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/whatsminer/M3X/M30S_Plus.py
--rw-r--r--   0        0        0      664 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/whatsminer/M3X/M30S_Plus_Plus.py
--rw-r--r--   0        0        0      276 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/whatsminer/M3X/M31S.py
--rw-r--r--   0        0        0      441 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/whatsminer/M3X/M31S_Plus.py
--rw-r--r--   0        0        0      229 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/whatsminer/M3X/M32S.py
--rw-r--r--   0        0        0      307 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/whatsminer/M3X/__init__.py
--rw-r--r--   0        0        0       38 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/_types/whatsminer/__init__.py
--rw-r--r--   0        0        0       92 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/__init__.py
--rw-r--r--   0        0        0      228 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X17/S17.py
--rw-r--r--   0        0        0      240 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X17/S17_Plus.py
--rw-r--r--   0        0        0      237 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X17/S17_Pro.py
--rw-r--r--   0        0        0      231 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X17/S17e.py
--rw-r--r--   0        0        0      228 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X17/T17.py
--rw-r--r--   0        0        0      240 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X17/T17_Plus.py
--rw-r--r--   0        0        0      231 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X17/T17e.py
--rw-r--r--   0        0        0     3073 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X17/X17.py
--rw-r--r--   0        0        0      226 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X17/__init__.py
--rw-r--r--   0        0        0      228 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X19/S19.py
--rw-r--r--   0        0        0      237 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X19/S19_Pro.py
--rw-r--r--   0        0        0      231 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X19/S19a.py
--rw-r--r--   0        0        0      231 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X19/S19j.py
--rw-r--r--   0        0        0      240 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X19/S19j_Pro.py
--rw-r--r--   0        0        0      228 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X19/T19.py
--rw-r--r--   0        0        0     3678 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X19/X19.py
--rw-r--r--   0        0        0      191 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X19/__init__.py
--rw-r--r--   0        0        0      273 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X9/S9.py
--rw-r--r--   0        0        0      276 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X9/S9i.py
--rw-r--r--   0        0        0      273 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X9/T9.py
--rw-r--r--   0        0        0       80 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/X9/__init__.py
--rw-r--r--   0        0        0       56 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bmminer/__init__.py
--rw-r--r--   0        0        0      279 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X17/S17.py
--rw-r--r--   0        0        0      291 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X17/S17_Plus.py
--rw-r--r--   0        0        0      288 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X17/S17_Pro.py
--rw-r--r--   0        0        0      282 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X17/S17e.py
--rw-r--r--   0        0        0      279 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X17/T17.py
--rw-r--r--   0        0        0      291 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X17/T17_Plus.py
--rw-r--r--   0        0        0      282 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X17/T17e.py
--rw-r--r--   0        0        0      233 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X17/__init__.py
--rw-r--r--   0        0        0      279 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X19/S19.py
--rw-r--r--   0        0        0      288 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X19/S19_Pro.py
--rw-r--r--   0        0        0      282 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X19/S19j.py
--rw-r--r--   0        0        0      291 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X19/S19j_Pro.py
--rw-r--r--   0        0        0      279 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X19/T19.py
--rw-r--r--   0        0        0      165 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X19/__init__.py
--rw-r--r--   0        0        0      276 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X9/S9.py
--rw-r--r--   0        0        0       27 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/X9/__init__.py
--rw-r--r--   0        0        0       56 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/bosminer/__init__.py
--rw-r--r--   0        0        0      276 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X17/S17.py
--rw-r--r--   0        0        0      288 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X17/S17_Plus.py
--rw-r--r--   0        0        0      285 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X17/S17_Pro.py
--rw-r--r--   0        0        0      279 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X17/S17e.py
--rw-r--r--   0        0        0      276 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X17/T17.py
--rw-r--r--   0        0        0      288 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X17/T17_Plus.py
--rw-r--r--   0        0        0      279 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X17/T17e.py
--rw-r--r--   0        0        0      226 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X17/__init__.py
--rw-r--r--   0        0        0      337 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X19/S19.py
--rw-r--r--   0        0        0      346 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X19/S19_Pro.py
--rw-r--r--   0        0        0      340 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X19/S19j.py
--rw-r--r--   0        0        0      349 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X19/S19j_Pro.py
--rw-r--r--   0        0        0      337 2022-07-11 14:30:25.868376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X19/T19.py
--rw-r--r--   0        0        0      160 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X19/__init__.py
--rw-r--r--   0        0        0      273 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X9/S9.py
--rw-r--r--   0        0        0      329 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X9/T9.py
--rw-r--r--   0        0        0       26 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/X9/__init__.py
--rw-r--r--   0        0        0       56 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/antminer/cgminer/__init__.py
--rw-r--r--   0        0        0      270 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/antminer/hiveon/X9/T9.py
--rw-r--r--   0        0        0       25 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/antminer/hiveon/X9/__init__.py
--rw-r--r--   0        0        0       18 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/antminer/hiveon/__init__.py
--rw-r--r--   0        0        0       23 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/__init__.py
--rw-r--r--   0        0        0     8853 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A10X/A1026.py
--rw-r--r--   0        0        0     8853 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A10X/A1047.py
--rw-r--r--   0        0        0     8853 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A10X/A1066.py
--rw-r--r--   0        0        0      111 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A10X/__init__.py
--rw-r--r--   0        0        0     8850 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A7X/A721.py
--rw-r--r--   0        0        0     8850 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A7X/A741.py
--rw-r--r--   0        0        0     8850 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A7X/A761.py
--rw-r--r--   0        0        0      105 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A7X/__init__.py
--rw-r--r--   0        0        0     8850 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A8X/A821.py
--rw-r--r--   0        0        0     8826 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A8X/A841.py
--rw-r--r--   0        0        0     8850 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A8X/A851.py
--rw-r--r--   0        0        0      105 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A8X/__init__.py
--rw-r--r--   0        0        0     8850 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A9X/A921.py
--rw-r--r--   0        0        0       35 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A9X/__init__.py
--rw-r--r--   0        0        0       77 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/__init__.py
--rw-r--r--   0        0        0    20151 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/miner_factory.py
--rw-r--r--   0        0        0     1740 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/miner_listener.py
--rw-r--r--   0        0        0      456 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/unknown.py
--rw-r--r--   0        0        0       23 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/whatsminer/__init__.py
--rw-r--r--   0        0        0      279 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M2X/M20S.py
--rw-r--r--   0        0        0      291 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M2X/M20S_Plus.py
--rw-r--r--   0        0        0      276 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M2X/M21.py
--rw-r--r--   0        0        0      563 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M2X/M21S.py
--rw-r--r--   0        0        0      291 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M2X/M21S_Plus.py
--rw-r--r--   0        0        0      199 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M2X/__init__.py
--rw-r--r--   0        0        0      881 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M3X/M30S.py
--rw-r--r--   0        0        0      783 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M3X/M30S_Plus.py
--rw-r--r--   0        0        0      658 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M3X/M30S_Plus_Plus.py
--rw-r--r--   0        0        0      279 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M3X/M31S.py
--rw-r--r--   0        0        0      448 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M3X/M31S_Plus.py
--rw-r--r--   0        0        0      279 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M3X/M32S.py
--rw-r--r--   0        0        0      482 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M3X/__init__.py
--rw-r--r--   0        0        0       38 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/miners/whatsminer/btminer/__init__.py
--rw-r--r--   0        0        0        0 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/misc/__init__.py
--rw-r--r--   0        0        0     2488 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/misc/bos.py
--rw-r--r--   0        0        0     6999 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/network/__init__.py
--rw-r--r--   0        0        0     1723 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/network/net_range.py
--rw-r--r--   0        0        0     1360 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/settings/__init__.py
--rw-r--r--   0        0        0      498 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/settings/settings.toml
--rw-r--r--   0        0        0       64 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/tests/__init__.py
--rw-r--r--   0        0        0     1812 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyasic/tests/network_tests/__init__.py
--rw-r--r--   0        0        0      487 2022-07-11 14:30:25.872376 pyasic-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     2445 2022-07-11 14:30:46.943849 pyasic-0.9.3/setup.py
--rw-r--r--   0        0        0      605 2022-07-11 14:30:46.944221 pyasic-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     7905 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/API/__init__.py
+-rw-r--r--   0        0        0    15503 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/API/bmminer.py
+-rw-r--r--   0        0        0     6917 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/API/bosminer.py
+-rw-r--r--   0        0        0    25107 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/API/btminer.py
+-rw-r--r--   0        0        0    15314 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/API/cgminer.py
+-rw-r--r--   0        0        0     2814 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/API/unknown.py
+-rw-r--r--   0        0        0        0 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/__init__.py
+-rw-r--r--   0        0        0    13068 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/config/__init__.py
+-rw-r--r--   0        0        0     4136 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/data/__init__.py
+-rw-r--r--   0        0        0      848 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/logger/__init__.py
+-rw-r--r--   0        0        0     2917 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/__init__.py
+-rw-r--r--   0        0        0      145 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_backends/__init__.py
+-rw-r--r--   0        0        0     9280 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_backends/bmminer.py
+-rw-r--r--   0        0        0    15003 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_backends/bosminer.py
+-rw-r--r--   0        0        0     1585 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_backends/bosminer_old.py
+-rw-r--r--   0        0        0     8753 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_backends/btminer.py
+-rw-r--r--   0        0        0     6949 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_backends/cgminer.py
+-rw-r--r--   0        0        0     1776 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_backends/hiveon.py
+-rw-r--r--   0        0        0       77 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/__init__.py
+-rw-r--r--   0        0        0      227 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X17/S17.py
+-rw-r--r--   0        0        0      232 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X17/S17_Plus.py
+-rw-r--r--   0        0        0      234 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X17/S17_Pro.py
+-rw-r--r--   0        0        0      230 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X17/S17e.py
+-rw-r--r--   0        0        0      227 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X17/T17.py
+-rw-r--r--   0        0        0      232 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X17/T17_Plus.py
+-rw-r--r--   0        0        0      229 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X17/T17e.py
+-rw-r--r--   0        0        0      177 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X17/__init__.py
+-rw-r--r--   0        0        0      227 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X19/S19.py
+-rw-r--r--   0        0        0      235 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X19/S19_Pro.py
+-rw-r--r--   0        0        0      229 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X19/S19a.py
+-rw-r--r--   0        0        0      230 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X19/S19j.py
+-rw-r--r--   0        0        0      237 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X19/S19j_Pro.py
+-rw-r--r--   0        0        0      227 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X19/T19.py
+-rw-r--r--   0        0        0      149 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X19/__init__.py
+-rw-r--r--   0        0        0      225 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X9/S9.py
+-rw-r--r--   0        0        0      227 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X9/S9i.py
+-rw-r--r--   0        0        0      225 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X9/T9.py
+-rw-r--r--   0        0        0       59 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/X9/__init__.py
+-rw-r--r--   0        0        0       56 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/antminer/__init__.py
+-rw-r--r--   0        0        0      242 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/avalonminer/A10X/A1026.py
+-rw-r--r--   0        0        0      242 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/avalonminer/A10X/A1047.py
+-rw-r--r--   0        0        0      243 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/avalonminer/A10X/A1066.py
+-rw-r--r--   0        0        0       90 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/avalonminer/A10X/__init__.py
+-rw-r--r--   0        0        0      295 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/avalonminer/A7X/A721.py
+-rw-r--r--   0        0        0      295 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/avalonminer/A7X/A741.py
+-rw-r--r--   0        0        0      295 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/avalonminer/A7X/A761.py
+-rw-r--r--   0        0        0       84 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/avalonminer/A7X/__init__.py
+-rw-r--r--   0        0        0      296 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/avalonminer/A8X/A821.py
+-rw-r--r--   0        0        0      296 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/avalonminer/A8X/A841.py
+-rw-r--r--   0        0        0      296 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/avalonminer/A8X/A851.py
+-rw-r--r--   0        0        0       84 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/avalonminer/A8X/__init__.py
+-rw-r--r--   0        0        0      296 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/avalonminer/A9X/A921.py
+-rw-r--r--   0        0        0       28 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/avalonminer/A9X/__init__.py
+-rw-r--r--   0        0        0       77 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/avalonminer/__init__.py
+-rw-r--r--   0        0        0      229 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/whatsminer/M2X/M20S.py
+-rw-r--r--   0        0        0      234 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/whatsminer/M2X/M20S_Plus.py
+-rw-r--r--   0        0        0      228 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/whatsminer/M2X/M21.py
+-rw-r--r--   0        0        0      630 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/whatsminer/M2X/M21S.py
+-rw-r--r--   0        0        0      235 2022-07-11 16:46:24.648857 pyasic-0.9.4/pyasic/miners/_types/whatsminer/M2X/M21S_Plus.py
+-rw-r--r--   0        0        0      150 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/_types/whatsminer/M2X/__init__.py
+-rw-r--r--   0        0        0     1039 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/_types/whatsminer/M3X/M30S.py
+-rw-r--r--   0        0        0      858 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/_types/whatsminer/M3X/M30S_Plus.py
+-rw-r--r--   0        0        0      664 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/_types/whatsminer/M3X/M30S_Plus_Plus.py
+-rw-r--r--   0        0        0      276 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/_types/whatsminer/M3X/M31S.py
+-rw-r--r--   0        0        0      441 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/_types/whatsminer/M3X/M31S_Plus.py
+-rw-r--r--   0        0        0      229 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/_types/whatsminer/M3X/M32S.py
+-rw-r--r--   0        0        0      307 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/_types/whatsminer/M3X/__init__.py
+-rw-r--r--   0        0        0       38 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/_types/whatsminer/__init__.py
+-rw-r--r--   0        0        0       92 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/__init__.py
+-rw-r--r--   0        0        0      228 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X17/S17.py
+-rw-r--r--   0        0        0      240 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X17/S17_Plus.py
+-rw-r--r--   0        0        0      237 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X17/S17_Pro.py
+-rw-r--r--   0        0        0      231 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X17/S17e.py
+-rw-r--r--   0        0        0      228 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X17/T17.py
+-rw-r--r--   0        0        0      240 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X17/T17_Plus.py
+-rw-r--r--   0        0        0      231 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X17/T17e.py
+-rw-r--r--   0        0        0     3073 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X17/X17.py
+-rw-r--r--   0        0        0      226 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X17/__init__.py
+-rw-r--r--   0        0        0      228 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X19/S19.py
+-rw-r--r--   0        0        0      237 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X19/S19_Pro.py
+-rw-r--r--   0        0        0      231 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X19/S19a.py
+-rw-r--r--   0        0        0      231 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X19/S19j.py
+-rw-r--r--   0        0        0      240 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X19/S19j_Pro.py
+-rw-r--r--   0        0        0      228 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X19/T19.py
+-rw-r--r--   0        0        0     3678 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X19/X19.py
+-rw-r--r--   0        0        0      191 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X19/__init__.py
+-rw-r--r--   0        0        0      273 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X9/S9.py
+-rw-r--r--   0        0        0      276 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X9/S9i.py
+-rw-r--r--   0        0        0      273 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X9/T9.py
+-rw-r--r--   0        0        0       80 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/X9/__init__.py
+-rw-r--r--   0        0        0       56 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bmminer/__init__.py
+-rw-r--r--   0        0        0      279 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X17/S17.py
+-rw-r--r--   0        0        0      291 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X17/S17_Plus.py
+-rw-r--r--   0        0        0      288 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X17/S17_Pro.py
+-rw-r--r--   0        0        0      282 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X17/S17e.py
+-rw-r--r--   0        0        0      279 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X17/T17.py
+-rw-r--r--   0        0        0      291 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X17/T17_Plus.py
+-rw-r--r--   0        0        0      282 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X17/T17e.py
+-rw-r--r--   0        0        0      233 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X17/__init__.py
+-rw-r--r--   0        0        0      279 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X19/S19.py
+-rw-r--r--   0        0        0      288 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X19/S19_Pro.py
+-rw-r--r--   0        0        0      282 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X19/S19j.py
+-rw-r--r--   0        0        0      291 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X19/S19j_Pro.py
+-rw-r--r--   0        0        0      279 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X19/T19.py
+-rw-r--r--   0        0        0      165 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X19/__init__.py
+-rw-r--r--   0        0        0      276 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X9/S9.py
+-rw-r--r--   0        0        0       27 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/X9/__init__.py
+-rw-r--r--   0        0        0       56 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/bosminer/__init__.py
+-rw-r--r--   0        0        0      276 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X17/S17.py
+-rw-r--r--   0        0        0      288 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X17/S17_Plus.py
+-rw-r--r--   0        0        0      285 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X17/S17_Pro.py
+-rw-r--r--   0        0        0      279 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X17/S17e.py
+-rw-r--r--   0        0        0      276 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X17/T17.py
+-rw-r--r--   0        0        0      288 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X17/T17_Plus.py
+-rw-r--r--   0        0        0      279 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X17/T17e.py
+-rw-r--r--   0        0        0      226 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X17/__init__.py
+-rw-r--r--   0        0        0      337 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X19/S19.py
+-rw-r--r--   0        0        0      346 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X19/S19_Pro.py
+-rw-r--r--   0        0        0      340 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X19/S19j.py
+-rw-r--r--   0        0        0      349 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X19/S19j_Pro.py
+-rw-r--r--   0        0        0      337 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X19/T19.py
+-rw-r--r--   0        0        0      160 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X19/__init__.py
+-rw-r--r--   0        0        0      273 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X9/S9.py
+-rw-r--r--   0        0        0      329 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X9/T9.py
+-rw-r--r--   0        0        0       26 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/X9/__init__.py
+-rw-r--r--   0        0        0       56 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/cgminer/__init__.py
+-rw-r--r--   0        0        0      270 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/hiveon/X9/T9.py
+-rw-r--r--   0        0        0       25 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/hiveon/X9/__init__.py
+-rw-r--r--   0        0        0       18 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/antminer/hiveon/__init__.py
+-rw-r--r--   0        0        0       23 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/__init__.py
+-rw-r--r--   0        0        0     8853 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A10X/A1026.py
+-rw-r--r--   0        0        0     8853 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A10X/A1047.py
+-rw-r--r--   0        0        0     8853 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A10X/A1066.py
+-rw-r--r--   0        0        0      111 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A10X/__init__.py
+-rw-r--r--   0        0        0     8850 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A7X/A721.py
+-rw-r--r--   0        0        0     8850 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A7X/A741.py
+-rw-r--r--   0        0        0     8850 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A7X/A761.py
+-rw-r--r--   0        0        0      105 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A7X/__init__.py
+-rw-r--r--   0        0        0     8850 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A8X/A821.py
+-rw-r--r--   0        0        0     8826 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A8X/A841.py
+-rw-r--r--   0        0        0     8850 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A8X/A851.py
+-rw-r--r--   0        0        0      105 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A8X/__init__.py
+-rw-r--r--   0        0        0     8850 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A9X/A921.py
+-rw-r--r--   0        0        0       35 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A9X/__init__.py
+-rw-r--r--   0        0        0       77 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/__init__.py
+-rw-r--r--   0        0        0    20151 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/miner_factory.py
+-rw-r--r--   0        0        0     1740 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/miner_listener.py
+-rw-r--r--   0        0        0      456 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/unknown.py
+-rw-r--r--   0        0        0       23 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/whatsminer/__init__.py
+-rw-r--r--   0        0        0      279 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M2X/M20S.py
+-rw-r--r--   0        0        0      291 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M2X/M20S_Plus.py
+-rw-r--r--   0        0        0      276 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M2X/M21.py
+-rw-r--r--   0        0        0      563 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M2X/M21S.py
+-rw-r--r--   0        0        0      291 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M2X/M21S_Plus.py
+-rw-r--r--   0        0        0      199 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M2X/__init__.py
+-rw-r--r--   0        0        0      881 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M3X/M30S.py
+-rw-r--r--   0        0        0      783 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M3X/M30S_Plus.py
+-rw-r--r--   0        0        0      658 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M3X/M30S_Plus_Plus.py
+-rw-r--r--   0        0        0      279 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M3X/M31S.py
+-rw-r--r--   0        0        0      448 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M3X/M31S_Plus.py
+-rw-r--r--   0        0        0      279 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M3X/M32S.py
+-rw-r--r--   0        0        0      482 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M3X/__init__.py
+-rw-r--r--   0        0        0       38 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/miners/whatsminer/btminer/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/misc/__init__.py
+-rw-r--r--   0        0        0     2488 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/misc/bos.py
+-rw-r--r--   0        0        0     6999 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/network/__init__.py
+-rw-r--r--   0        0        0     1723 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/network/net_range.py
+-rw-r--r--   0        0        0     1360 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/settings/__init__.py
+-rw-r--r--   0        0        0      498 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/settings/settings.toml
+-rw-r--r--   0        0        0       64 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/tests/__init__.py
+-rw-r--r--   0        0        0     1812 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyasic/tests/network_tests/__init__.py
+-rw-r--r--   0        0        0      487 2022-07-11 16:46:24.652857 pyasic-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     2445 2022-07-11 16:46:40.223819 pyasic-0.9.4/setup.py
+-rw-r--r--   0        0        0      605 2022-07-11 16:46:40.224244 pyasic-0.9.4/PKG-INFO
```

### Comparing `pyasic-0.9.3/pyasic/API/__init__.py` & `pyasic-0.9.4/pyasic/API/__init__.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/API/bmminer.py` & `pyasic-0.9.4/pyasic/API/bmminer.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/API/bosminer.py` & `pyasic-0.9.4/pyasic/API/bosminer.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/API/btminer.py` & `pyasic-0.9.4/pyasic/API/btminer.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/API/cgminer.py` & `pyasic-0.9.4/pyasic/API/cgminer.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/API/unknown.py` & `pyasic-0.9.4/pyasic/API/unknown.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/config/__init__.py` & `pyasic-0.9.4/pyasic/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/data/__init__.py` & `pyasic-0.9.4/pyasic/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/logger/__init__.py` & `pyasic-0.9.4/pyasic/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/__init__.py` & `pyasic-0.9.4/pyasic/miners/__init__.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/_backends/bmminer.py` & `pyasic-0.9.4/pyasic/miners/_backends/bmminer.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/_backends/bosminer.py` & `pyasic-0.9.4/pyasic/miners/_backends/bosminer.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/_backends/bosminer_old.py` & `pyasic-0.9.4/pyasic/miners/_backends/bosminer_old.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/_backends/btminer.py` & `pyasic-0.9.4/pyasic/miners/_backends/btminer.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,31 +140,39 @@
         devs = miner_data.get("devs")[0]
         pools = miner_data.get("pools")[0]
 
         if summary:
             summary_data = summary.get("SUMMARY")
             if summary_data:
                 if len(summary_data) > 0:
+                    wattage_limit = None
                     if summary_data[0].get("MAC"):
                         mac = summary_data[0]["MAC"]
 
                     if summary_data[0].get("Env Temp"):
                         data.env_temp = summary_data[0]["Env Temp"]
 
+                    if summary_data[0].get("Power Limit"):
+                        wattage_limit = summary_data[0]["Power Limit"]
+
                     data.fan_1 = summary_data[0]["Fan Speed In"]
                     data.fan_2 = summary_data[0]["Fan Speed Out"]
 
                     hr = summary_data[0].get("MHS 1m")
                     if hr:
                         data.hashrate = round(hr / 1000000, 2)
 
                     wattage = summary_data[0].get("Power")
                     if wattage:
                         data.wattage = round(wattage)
-                        data.wattage_limit = round(wattage)
+
+                        if not wattage_limit:
+                            wattage_limit = round(wattage)
+
+                    data.wattage_limit = wattage_limit
 
         if devs:
             temp_data = devs.get("DEVS")
             if temp_data:
                 board_map = {0: "left_board", 1: "center_board", 2: "right_board"}
                 for board in temp_data:
                     _id = board["ASC"]
```

### Comparing `pyasic-0.9.3/pyasic/miners/_backends/cgminer.py` & `pyasic-0.9.4/pyasic/miners/_backends/cgminer.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/_backends/hiveon.py` & `pyasic-0.9.4/pyasic/miners/_backends/hiveon.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/_types/whatsminer/M2X/M21S.py` & `pyasic-0.9.4/pyasic/miners/_types/whatsminer/M2X/M21S.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/_types/whatsminer/M3X/M30S.py` & `pyasic-0.9.4/pyasic/miners/_types/whatsminer/M3X/M30S.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/_types/whatsminer/M3X/M30S_Plus.py` & `pyasic-0.9.4/pyasic/miners/_types/whatsminer/M3X/M30S_Plus.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/_types/whatsminer/M3X/M30S_Plus_Plus.py` & `pyasic-0.9.4/pyasic/miners/_types/whatsminer/M3X/M30S_Plus_Plus.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/antminer/bmminer/X17/X17.py` & `pyasic-0.9.4/pyasic/miners/antminer/bmminer/X17/X17.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/antminer/bmminer/X19/X19.py` & `pyasic-0.9.4/pyasic/miners/antminer/bmminer/X19/X19.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A10X/A1026.py` & `pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A10X/A1026.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A10X/A1047.py` & `pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A10X/A1047.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A10X/A1066.py` & `pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A10X/A1066.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A7X/A721.py` & `pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A7X/A721.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A7X/A741.py` & `pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A7X/A741.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A7X/A761.py` & `pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A7X/A761.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A8X/A821.py` & `pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A8X/A821.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A8X/A841.py` & `pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A8X/A841.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A8X/A851.py` & `pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A8X/A851.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/avalonminer/cgminer/A9X/A921.py` & `pyasic-0.9.4/pyasic/miners/avalonminer/cgminer/A9X/A921.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/miner_factory.py` & `pyasic-0.9.4/pyasic/miners/miner_factory.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/miner_listener.py` & `pyasic-0.9.4/pyasic/miners/miner_listener.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M2X/M21S.py` & `pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M2X/M21S.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M3X/M30S.py` & `pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M3X/M30S.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M3X/M30S_Plus.py` & `pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M3X/M30S_Plus.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/miners/whatsminer/btminer/M3X/M30S_Plus_Plus.py` & `pyasic-0.9.4/pyasic/miners/whatsminer/btminer/M3X/M30S_Plus_Plus.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/misc/bos.py` & `pyasic-0.9.4/pyasic/misc/bos.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/network/__init__.py` & `pyasic-0.9.4/pyasic/network/__init__.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/network/net_range.py` & `pyasic-0.9.4/pyasic/network/net_range.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/settings/__init__.py` & `pyasic-0.9.4/pyasic/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/pyasic/tests/network_tests/__init__.py` & `pyasic-0.9.4/pyasic/tests/network_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyasic-0.9.3/setup.py` & `pyasic-0.9.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
  'httpx>=0.23.0,<0.24.0',
  'passlib>=1.7.4,<2.0.0',
  'pyaml>=21.10.1,<22.0.0',
  'toml>=0.10.2,<0.11.0']
 
 setup_kwargs = {
     'name': 'pyasic',
-    'version': '0.9.3',
+    'version': '0.9.4',
     'description': 'A set of modules for interfacing with many common types of ASIC bitcoin miners, using both their API and SSH.',
     'long_description': None,
     'author': 'UpstreamData',
     'author_email': 'brett@upstreamdata.ca',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `pyasic-0.9.3/PKG-INFO` & `pyasic-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyasic
-Version: 0.9.3
+Version: 0.9.4
 Summary: A set of modules for interfacing with many common types of ASIC bitcoin miners, using both their API and SSH.
 Author: UpstreamData
 Author-email: brett@upstreamdata.ca
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

