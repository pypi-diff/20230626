# Comparing `tmp/dinero-0.2.0.tar.gz` & `tmp/dinero-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinero-0.2.0.tar", max compression
+gzip compressed data, was "dinero-0.2.1.tar", max compression
```

## Comparing `dinero-0.2.0.tar` & `dinero-0.2.1.tar`

### file list

```diff
@@ -1,137 +1,139 @@
--rw-r--r--   0        0        0     1068 2023-05-08 23:53:16.955810 dinero-0.2.0/LICENSE
--rw-r--r--   0        0        0     5114 2023-05-14 23:48:13.953964 dinero-0.2.0/README.md
--rw-r--r--   0        0        0       74 2023-05-10 02:57:39.253099 dinero-0.2.0/dinero/__init__.py
--rw-r--r--   0        0        0    17552 2023-05-09 22:33:57.525601 dinero-0.2.0/dinero/_dinero.py
--rw-r--r--   0        0        0      384 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/_utils.py
--rw-r--r--   0        0        0     2494 2023-05-10 00:19:53.843673 dinero-0.2.0/dinero/_validators.py
--rw-r--r--   0        0        0     4008 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/__init__.py
--rw-r--r--   0        0        0      166 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_aed.py
--rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_afn.py
--rw-r--r--   0        0        0      127 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_amd.py
--rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_aoa.py
--rw-r--r--   0        0        0      128 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_ars.py
--rw-r--r--   0        0        0      131 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_aud.py
--rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_awg.py
--rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_azn.py
--rw-r--r--   0        0        0      129 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bbd.py
--rw-r--r--   0        0        0      150 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bdt.py
--rw-r--r--   0        0        0      149 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bgn.py
--rw-r--r--   0        0        0      128 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bhd.py
--rw-r--r--   0        0        0      129 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bif.py
--rw-r--r--   0        0        0      130 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bmd.py
--rw-r--r--   0        0        0      127 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bnd.py
--rw-r--r--   0        0        0      128 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bov.py
--rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_brl.py
--rw-r--r--   0        0        0      146 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bwp.py
--rw-r--r--   0        0        0      130 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_byn.py
--rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bzd.py
--rw-r--r--   0        0        0      129 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_cdf.py
--rw-r--r--   0        0        0      122 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_che.py
--rw-r--r--   0        0        0      146 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_chf.py
--rw-r--r--   0        0        0      123 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_chw.py
--rw-r--r--   0        0        0      125 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_clp.py
--rw-r--r--   0        0        0      145 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_cny.py
--rw-r--r--   0        0        0      128 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_cop.py
--rw-r--r--   0        0        0      134 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_cou.py
--rw-r--r--   0        0        0      144 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_crc.py
--rw-r--r--   0        0        0      136 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_cuc.py
--rw-r--r--   0        0        0      133 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_cve.py
--rw-r--r--   0        0        0      147 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_czk.py
--rw-r--r--   0        0        0      130 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_djf.py
--rw-r--r--   0        0        0      147 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_dkk.py
--rw-r--r--   0        0        0      149 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_dop.py
--rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_dzd.py
--rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_egp.py
--rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_etb.py
--rw-r--r--   0        0        0      139 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_eur.py
--rw-r--r--   0        0        0      125 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_fjd.py
--rw-r--r--   0        0        0      136 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_fkp.py
--rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_gbp.py
--rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_gtq.py
--rw-r--r--   0        0        0      127 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_hrk.py
--rw-r--r--   0        0        0      128 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_htg.py
--rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_idr.py
--rw-r--r--   0        0        0      132 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_ils.py
--rw-r--r--   0        0        0      147 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_inr.py
--rw-r--r--   0        0        0      125 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_iqd.py
--rw-r--r--   0        0        0      126 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_irr.py
--rw-r--r--   0        0        0      130 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_isk.py
--rw-r--r--   0        0        0      129 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_jmd.py
--rw-r--r--   0        0        0      145 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_jpy.py
--rw-r--r--   0        0        0      150 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_kes.py
--rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_kgs.py
--rw-r--r--   0        0        0      149 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_khr.py
--rw-r--r--   0        0        0      126 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_kmf.py
--rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_krw.py
--rw-r--r--   0        0        0      127 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_kwd.py
--rw-r--r--   0        0        0      131 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_kzt.py
--rw-r--r--   0        0        0      121 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_lak.py
--rw-r--r--   0        0        0      150 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_lkr.py
--rw-r--r--   0        0        0      129 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_lrd.py
--rw-r--r--   0        0        0      126 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_lsl.py
--rw-r--r--   0        0        0      149 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mad.py
--rw-r--r--   0        0        0      126 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mdl.py
--rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mga.py
--rw-r--r--   0        0        0      145 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mmk.py
--rw-r--r--   0        0        0      153 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mnt.py
--rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mop.py
--rw-r--r--   0        0        0      149 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mur.py
--rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mvr.py
--rw-r--r--   0        0        0      141 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_mxv.py
--rw-r--r--   0        0        0      152 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_mzn.py
--rw-r--r--   0        0        0      153 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_nio.py
--rw-r--r--   0        0        0      148 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_npr.py
--rw-r--r--   0        0        0      132 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_nzd.py
--rw-r--r--   0        0        0      124 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_omr.py
--rw-r--r--   0        0        0      131 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_pab.py
--rw-r--r--   0        0        0      147 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_pen.py
--rw-r--r--   0        0        0      155 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_pgk.py
--rw-r--r--   0        0        0      150 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_php.py
--rw-r--r--   0        0        0      127 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_pln.py
--rw-r--r--   0        0        0      153 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_pyg.py
--rw-r--r--   0        0        0      126 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_ron.py
--rw-r--r--   0        0        0      127 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_rsd.py
--rw-r--r--   0        0        0      148 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_rub.py
--rw-r--r--   0        0        0      125 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_sar.py
--rw-r--r--   0        0        0      136 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_sbd.py
--rw-r--r--   0        0        0      150 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_scr.py
--rw-r--r--   0        0        0      128 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_sdg.py
--rw-r--r--   0        0        0      127 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_sek.py
--rw-r--r--   0        0        0      130 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_sgd.py
--rw-r--r--   0        0        0      134 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_sll.py
--rw-r--r--   0        0        0      129 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_sos.py
--rw-r--r--   0        0        0      134 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_ssp.py
--rw-r--r--   0        0        0      144 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_stn.py
--rw-r--r--   0        0        0      131 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_svc.py
--rw-r--r--   0        0        0      147 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_syp.py
--rw-r--r--   0        0        0      129 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_szl.py
--rw-r--r--   0        0        0      123 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_thb.py
--rw-r--r--   0        0        0      132 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_tjs.py
--rw-r--r--   0        0        0      132 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_tmt.py
--rw-r--r--   0        0        0      128 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_tnd.py
--rw-r--r--   0        0        0      140 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_ttd.py
--rw-r--r--   0        0        0      131 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_twd.py
--rw-r--r--   0        0        0      132 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_tzs.py
--rw-r--r--   0        0        0      151 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_ugx.py
--rw-r--r--   0        0        0      133 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_usd.py
--rw-r--r--   0        0        0      145 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_usn.py
--rw-r--r--   0        0        0      148 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_uyi.py
--rw-r--r--   0        0        0      132 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_vnd.py
--rw-r--r--   0        0        0      126 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_vuv.py
--rw-r--r--   0        0        0      148 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_wst.py
--rw-r--r--   0        0        0      156 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_xcd.py
--rw-r--r--   0        0        0      157 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_xof.py
--rw-r--r--   0        0        0      123 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_xpf.py
--rw-r--r--   0        0        0      125 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_yer.py
--rw-r--r--   0        0        0      151 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_zar.py
--rw-r--r--   0        0        0      149 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_zmw.py
--rw-r--r--   0        0        0      131 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_zwl.py
--rw-r--r--   0        0        0      387 2023-05-09 23:46:15.080607 dinero-0.2.0/dinero/exceptions.py
--rw-r--r--   0        0        0      362 2023-05-10 01:59:35.240655 dinero-0.2.0/dinero/tools/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-10 02:53:58.158738 dinero-0.2.0/dinero/tools/calculate_compound_interest.py
--rw-r--r--   0        0        0     1339 2023-05-14 22:42:56.383362 dinero-0.2.0/dinero/tools/calculate_percentage.py
--rw-r--r--   0        0        0     1858 2023-05-14 22:46:39.176259 dinero-0.2.0/dinero/tools/calculate_simple_interest.py
--rw-r--r--   0        0        0     1356 2023-05-14 22:29:33.710063 dinero-0.2.0/dinero/tools/calculate_vat.py
--rw-r--r--   0        0        0      331 2023-05-09 22:06:45.830428 dinero-0.2.0/dinero/types.py
--rw-r--r--   0        0        0      850 2023-05-10 02:57:31.043073 dinero-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5814 1970-01-01 00:00:00.000000 dinero-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-08 23:53:16.955810 dinero-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5115 2023-05-15 00:02:21.791426 dinero-0.2.1/README.md
+-rw-r--r--   0        0        0       74 2023-06-26 18:14:37.697608 dinero-0.2.1/dinero/__init__.py
+-rw-r--r--   0        0        0     2433 2023-06-26 18:13:42.684762 dinero-0.2.1/dinero/_base.py
+-rw-r--r--   0        0        0    12845 2023-06-26 17:24:05.536926 dinero-0.2.1/dinero/_dinero.py
+-rw-r--r--   0        0        0     2975 2023-06-26 17:47:08.382374 dinero-0.2.1/dinero/_operations.py
+-rw-r--r--   0        0        0      384 2023-06-26 03:39:36.512426 dinero-0.2.1/dinero/_utils.py
+-rw-r--r--   0        0        0     2494 2023-06-26 18:11:03.725254 dinero-0.2.1/dinero/_validators.py
+-rw-r--r--   0        0        0     4008 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/__init__.py
+-rw-r--r--   0        0        0      166 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_aed.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_afn.py
+-rw-r--r--   0        0        0      127 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_amd.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_aoa.py
+-rw-r--r--   0        0        0      128 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_ars.py
+-rw-r--r--   0        0        0      131 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_aud.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_awg.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_azn.py
+-rw-r--r--   0        0        0      129 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_bbd.py
+-rw-r--r--   0        0        0      150 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_bdt.py
+-rw-r--r--   0        0        0      149 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_bgn.py
+-rw-r--r--   0        0        0      128 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_bhd.py
+-rw-r--r--   0        0        0      129 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_bif.py
+-rw-r--r--   0        0        0      130 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_bmd.py
+-rw-r--r--   0        0        0      127 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_bnd.py
+-rw-r--r--   0        0        0      128 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_bov.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_brl.py
+-rw-r--r--   0        0        0      146 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_bwp.py
+-rw-r--r--   0        0        0      130 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_byn.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_bzd.py
+-rw-r--r--   0        0        0      129 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_cdf.py
+-rw-r--r--   0        0        0      122 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_che.py
+-rw-r--r--   0        0        0      146 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_chf.py
+-rw-r--r--   0        0        0      123 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_chw.py
+-rw-r--r--   0        0        0      125 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_clp.py
+-rw-r--r--   0        0        0      145 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_cny.py
+-rw-r--r--   0        0        0      128 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_cop.py
+-rw-r--r--   0        0        0      134 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_cou.py
+-rw-r--r--   0        0        0      144 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_crc.py
+-rw-r--r--   0        0        0      136 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_cuc.py
+-rw-r--r--   0        0        0      133 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_cve.py
+-rw-r--r--   0        0        0      147 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_czk.py
+-rw-r--r--   0        0        0      130 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_djf.py
+-rw-r--r--   0        0        0      147 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_dkk.py
+-rw-r--r--   0        0        0      149 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_dop.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_dzd.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_egp.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_etb.py
+-rw-r--r--   0        0        0      139 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_eur.py
+-rw-r--r--   0        0        0      125 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_fjd.py
+-rw-r--r--   0        0        0      136 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_fkp.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_gbp.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_gtq.py
+-rw-r--r--   0        0        0      127 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_hrk.py
+-rw-r--r--   0        0        0      128 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_htg.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_idr.py
+-rw-r--r--   0        0        0      132 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_ils.py
+-rw-r--r--   0        0        0      147 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_inr.py
+-rw-r--r--   0        0        0      125 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_iqd.py
+-rw-r--r--   0        0        0      126 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_irr.py
+-rw-r--r--   0        0        0      130 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_isk.py
+-rw-r--r--   0        0        0      129 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_jmd.py
+-rw-r--r--   0        0        0      145 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_jpy.py
+-rw-r--r--   0        0        0      150 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_kes.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_kgs.py
+-rw-r--r--   0        0        0      149 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_khr.py
+-rw-r--r--   0        0        0      126 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_kmf.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_krw.py
+-rw-r--r--   0        0        0      127 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_kwd.py
+-rw-r--r--   0        0        0      131 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_kzt.py
+-rw-r--r--   0        0        0      121 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_lak.py
+-rw-r--r--   0        0        0      150 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_lkr.py
+-rw-r--r--   0        0        0      129 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_lrd.py
+-rw-r--r--   0        0        0      126 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_lsl.py
+-rw-r--r--   0        0        0      149 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_mad.py
+-rw-r--r--   0        0        0      126 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_mdl.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_mga.py
+-rw-r--r--   0        0        0      145 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_mmk.py
+-rw-r--r--   0        0        0      153 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_mnt.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_mop.py
+-rw-r--r--   0        0        0      149 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_mur.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.1/dinero/currencies/_mvr.py
+-rw-r--r--   0        0        0      141 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_mxv.py
+-rw-r--r--   0        0        0      152 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_mzn.py
+-rw-r--r--   0        0        0      153 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_nio.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_npr.py
+-rw-r--r--   0        0        0      132 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_nzd.py
+-rw-r--r--   0        0        0      124 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_omr.py
+-rw-r--r--   0        0        0      131 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_pab.py
+-rw-r--r--   0        0        0      147 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_pen.py
+-rw-r--r--   0        0        0      155 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_pgk.py
+-rw-r--r--   0        0        0      150 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_php.py
+-rw-r--r--   0        0        0      127 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_pln.py
+-rw-r--r--   0        0        0      153 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_pyg.py
+-rw-r--r--   0        0        0      126 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_ron.py
+-rw-r--r--   0        0        0      127 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_rsd.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_rub.py
+-rw-r--r--   0        0        0      125 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_sar.py
+-rw-r--r--   0        0        0      136 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_sbd.py
+-rw-r--r--   0        0        0      150 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_scr.py
+-rw-r--r--   0        0        0      128 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_sdg.py
+-rw-r--r--   0        0        0      127 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_sek.py
+-rw-r--r--   0        0        0      130 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_sgd.py
+-rw-r--r--   0        0        0      134 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_sll.py
+-rw-r--r--   0        0        0      129 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_sos.py
+-rw-r--r--   0        0        0      134 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_ssp.py
+-rw-r--r--   0        0        0      144 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_stn.py
+-rw-r--r--   0        0        0      131 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_svc.py
+-rw-r--r--   0        0        0      147 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_syp.py
+-rw-r--r--   0        0        0      129 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_szl.py
+-rw-r--r--   0        0        0      123 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_thb.py
+-rw-r--r--   0        0        0      132 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_tjs.py
+-rw-r--r--   0        0        0      132 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_tmt.py
+-rw-r--r--   0        0        0      128 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_tnd.py
+-rw-r--r--   0        0        0      140 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_ttd.py
+-rw-r--r--   0        0        0      131 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_twd.py
+-rw-r--r--   0        0        0      132 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_tzs.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_ugx.py
+-rw-r--r--   0        0        0      133 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_usd.py
+-rw-r--r--   0        0        0      145 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_usn.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_uyi.py
+-rw-r--r--   0        0        0      132 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_vnd.py
+-rw-r--r--   0        0        0      126 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_vuv.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_wst.py
+-rw-r--r--   0        0        0      156 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_xcd.py
+-rw-r--r--   0        0        0      157 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_xof.py
+-rw-r--r--   0        0        0      123 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_xpf.py
+-rw-r--r--   0        0        0      125 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_yer.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_zar.py
+-rw-r--r--   0        0        0      149 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_zmw.py
+-rw-r--r--   0        0        0      131 2023-05-08 23:53:16.965810 dinero-0.2.1/dinero/currencies/_zwl.py
+-rw-r--r--   0        0        0      387 2023-05-09 23:46:15.080607 dinero-0.2.1/dinero/exceptions.py
+-rw-r--r--   0        0        0      362 2023-05-10 01:59:35.240655 dinero-0.2.1/dinero/tools/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-10 02:53:58.158738 dinero-0.2.1/dinero/tools/calculate_compound_interest.py
+-rw-r--r--   0        0        0     1339 2023-05-14 22:42:56.383362 dinero-0.2.1/dinero/tools/calculate_percentage.py
+-rw-r--r--   0        0        0     1858 2023-05-14 22:46:39.176259 dinero-0.2.1/dinero/tools/calculate_simple_interest.py
+-rw-r--r--   0        0        0     1356 2023-05-14 22:29:33.710063 dinero-0.2.1/dinero/tools/calculate_vat.py
+-rw-r--r--   0        0        0      340 2023-06-26 17:51:20.464454 dinero-0.2.1/dinero/types.py
+-rw-r--r--   0        0        0      850 2023-06-26 18:14:49.837612 dinero-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5815 1970-01-01 00:00:00.000000 dinero-0.2.1/PKG-INFO
```

### Comparing `dinero-0.2.0/LICENSE` & `dinero-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dinero-0.2.0/README.md` & `dinero-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     duration=10,
     compound_frequency=12,
 )
 total_interest.format(symbol=True, currency=True)
 '$1,294.02 USD'
 ```
 
-See al the available tools in the [tools](https://wilfredinni.github.io/dinero/tools/) section.
+See all the available tools in the [tools](https://wilfredinni.github.io/dinero/tools/) section.
 
 ### Custom currencies
 
 You can easily create custom currencies:
 
 ```python
 from dinero import Dinero
```

#### html2text {}

```diff
@@ -40,14 +40,14 @@
 #comparisons). ### Tools Dinero give you access to some useful tools that allow
 you to perform common monetary calculations, like percentages, VAT, simple and
 compound interests, etc. ```python from dinero import Dinero from
 dinero.currencies import USD from dinero.tools import
 calculate_compound_interest principal = Dinero("2000", USD) total_interest =
 calculate_compound_interest( principal=principal, interest_rate=5, duration=10,
 compound_frequency=12, ) total_interest.format(symbol=True, currency=True)
-'$1,294.02 USD' ``` See al the available tools in the [tools](https://
+'$1,294.02 USD' ``` See all the available tools in the [tools](https://
 wilfredinni.github.io/dinero/tools/) section. ### Custom currencies You can
 easily create custom currencies: ```python from dinero import Dinero BTC =
 { "code": "BTC", "base": 10, "exponent": 2, "symbol": "â¿", } Dinero(1000.5,
 BTC) ``` ```python Dinero(amount=1000.5, currency={'code': 'BTC', 'base': 10,
 'exponent': 2, 'symbol': 'â¿'}) ``` More about [custom currencies](https://
 wilfredinni.github.io/dinero/currencies/#custom-currencies).
```

### Comparing `dinero-0.2.0/dinero/_dinero.py` & `dinero-0.2.1/dinero/_dinero.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,176 +11,37 @@
 - less_than_or_equal:: Checks whether an object is less than or equal the other.
 - greater_than:: Checks whether an object is greater or equal the other.
 - greater_than_or_equal:: Checks whether an object is greater or equal the other.
 - to_dict:: Returns the object's data as a Python Dictionary.
 - to_json:: Returns the object's data as a JSON string.
 """
 
+
 import json
-from decimal import Decimal, getcontext
+from decimal import Decimal
 from typing import Any
 
+from ._operations import Operations
 from ._utils import DecimalEncoder
 from ._validators import Validators
-from .exceptions import DifferentCurrencyError
 from .types import Currency, OperationType
 
 validate = Validators()
 
 
-class Base:
-    """The base Dinero class with the constructor and properties."""
-
-    def __init__(self, amount: int | float | str | Decimal, currency: Currency):
-        self.amount = amount
-        self.currency = currency
-
-        validate.dinero_amount(amount)
-
-    @property
-    def symbol(self):
-        return self.currency.get("symbol", "$")
-
-    @property
-    def code(self):
-        return self.currency.get("code")
-
-    @property
-    def exponent(self):
-        return self.currency.get("exponent")
-
-    @property
-    def precision(self):
-        return self.currency.get("base")
-
-
-class Utils(Base):
-    """Utility class with the most important methods to count money exactly."""
-
-    def _get_instance(self, amount: "OperationType | object") -> "Dinero":
-        """Return a Dinero object after checking the currency codes are equal and
-        transforming it to Dinero if needed.
-
-        Args:
-            amount (str, int, float, Decimal, Dinero): amount to be instantiated
-
-        Returns:
-            DINERO: Dinero object.
-        """
-
-        if isinstance(amount, Dinero):
-            amount_obj = amount
-        else:
-            amount_obj = Dinero(str(amount), self.currency)
-
-        if amount_obj.code != self.code:
-            raise DifferentCurrencyError("Currencies can not be different")
-
-        return amount_obj
-
-    def _normalize(self, quantize: bool = False) -> Decimal:
-        """Return a Decimal object, that can be quantize.
-
-        Args:
-            quantize (bool): Only for the final result. Defaults to False.
-
-        Returns
-            DECIMAL: Decimal object.
-        """
-
-        getcontext().prec = self.precision
-        normalized_amount = Decimal(self.amount).normalize()
-
-        if quantize:
-            places = Decimal(f"1e-{self.exponent}")
-            normalized_amount = normalized_amount.quantize(places)
-
-        return normalized_amount
-
-    @property
-    def _formatted_amount(self) -> str:
-        currency_format = f",.{self.exponent}f"
-        return f"{self._normalize(quantize=True):{currency_format}}"
-
-    @property
-    def raw_amount(self) -> Decimal:
-        return self._normalize(quantize=True)
-
-
-class Operations(Utils):
-    """All the operations supported between Dinero objects."""
-
-    def __add__(self, addend: "OperationType | Dinero") -> "Dinero":
-        validate.addition_and_subtraction_amount(addend)
-        addend_obj = self._get_instance(addend)
-        total = self._normalize() + addend_obj._normalize()
-        return Dinero(str(total), self.currency)
-
-    def __radd__(self, obj):
-        return self
-
-    def __sub__(self, subtrahend: "OperationType | Dinero") -> "Dinero":
-        validate.addition_and_subtraction_amount(subtrahend)
-        subtrahend_obj = self._get_instance(subtrahend)
-        total = self._normalize() - subtrahend_obj._normalize()
-        return Dinero(str(total), self.currency)
-
-    def __mul__(self, multiplicand: int | float | Decimal) -> "Dinero":
-        validate.multiplication_and_division_amount(multiplicand)
-        multiplicand_obj = self._get_instance(multiplicand)
-        total = self._normalize() * multiplicand_obj._normalize()
-        return Dinero(str(total), self.currency)
-
-    def __truediv__(self, divisor: int | float | Decimal) -> "Dinero":
-        validate.multiplication_and_division_amount(divisor)
-        divisor_obj = self._get_instance(divisor)
-        total = self._normalize() / divisor_obj._normalize()
-        return Dinero(str(total), self.currency)
-
-    def __eq__(self, amount: object) -> bool:
-        validate.comparison_amount(amount)
-        num_2 = self._get_instance(amount)._normalize(quantize=True)
-        num_1 = self._normalize(quantize=True)
-        return bool(num_1 == num_2)
-
-    def __lt__(self, amount: object) -> bool:
-        validate.comparison_amount(amount)
-        num_1 = self._normalize(quantize=True)
-        num_2 = self._get_instance(amount)._normalize(quantize=True)
-        return bool(num_1 < num_2)
-
-    def __le__(self, amount: object) -> bool:
-        validate.comparison_amount(amount)
-        num_1 = self._normalize(quantize=True)
-        num_2 = self._get_instance(amount)._normalize(quantize=True)
-        return bool(num_1 <= num_2)
-
-    def __gt__(self, amount: object) -> bool:
-        validate.comparison_amount(amount)
-        num_1 = self._normalize(quantize=True)
-        num_2 = self._get_instance(amount)._normalize(quantize=True)
-        return bool(num_1 > num_2)
-
-    def __ge__(self, amount: object) -> bool:
-        validate.comparison_amount(amount)
-        num_1 = self._normalize(quantize=True)
-        num_2 = self._get_instance(amount)._normalize(quantize=True)
-        return bool(num_1 >= num_2)
-
-
-class Dinero(Operations, Base):
+class Dinero(Operations):
     """A Dinero object is an immutable data structure representing a specific monetary value.
     It comes with methods for creating, parsing, manipulating, testing and formatting them.
 
     Args:
         amount (str, int, float, Decimal): The amount to work with.
         currency (dict): Expressed as an ISO 4217 currency code.
     """
 
-    def __init__(self, amount: int | float | str, currency: Currency):
+    def __init__(self, amount: int | float | str | Decimal, currency: Currency):
         super().__init__(amount, currency)
 
     def format(self, symbol: bool = False, currency: bool = False) -> str:
         """Format a Dinero object with his decimals, symbol and/or code.
 
         Examples:
             >>> Dinero('234342.3010', USD).format()
@@ -488,23 +349,23 @@
             InvalidOperationError: An operation between unsupported types was executed.
 
         Returns:
             DICT: The object's data as a Python Dictionary.
         """
 
         normalized_amount = self._normalize(quantize=True)
-        if amount_with_format:
-            amount = self._formatted_amount
-        else:
-            amount = str(normalized_amount)
-
-        _dict = self.__dict__
-        _dict["amount"] = amount
-        _dict["currency"].setdefault("symbol", "$")
-        return _dict
+        amount = (
+            self._formatted_amount if amount_with_format else str(normalized_amount)
+        )
+
+        dict_repr = self.__dict__
+        dict_repr["amount"] = amount
+        dict_repr["currency"].setdefault("symbol", "$")
+        del dict_repr["dinero"]
+        return dict_repr
 
     def to_json(self, amount_with_format: bool = False) -> str:
         """Returns the object's data as a JSON string.
 
         Examples:
             >>> Dinero('2,00', USD).to_json()
             '{"amount": "3333.20", "currency": {"code": "USD", "base": 10...'
```

### Comparing `dinero-0.2.0/dinero/_validators.py` & `dinero-0.2.1/dinero/_validators.py`

 * *Files identical despite different names*

### Comparing `dinero-0.2.0/dinero/currencies/__init__.py` & `dinero-0.2.1/dinero/currencies/__init__.py`

 * *Files identical despite different names*

### Comparing `dinero-0.2.0/dinero/tools/calculate_compound_interest.py` & `dinero-0.2.1/dinero/tools/calculate_compound_interest.py`

 * *Files identical despite different names*

### Comparing `dinero-0.2.0/dinero/tools/calculate_percentage.py` & `dinero-0.2.1/dinero/tools/calculate_percentage.py`

 * *Files identical despite different names*

### Comparing `dinero-0.2.0/dinero/tools/calculate_simple_interest.py` & `dinero-0.2.1/dinero/tools/calculate_simple_interest.py`

 * *Files identical despite different names*

### Comparing `dinero-0.2.0/dinero/tools/calculate_vat.py` & `dinero-0.2.1/dinero/tools/calculate_vat.py`

 * *Files identical despite different names*

### Comparing `dinero-0.2.0/pyproject.toml` & `dinero-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dinero"
-version = "0.2.0"
+version = "0.2.1"
 description = "Dinero is a library for working with monetary values in Python."
 license = "MIT"
 authors = ["Carlos Montecinos Geisse <carlos@pythoncheatsheet.org>"]
 readme = "README.md"
 repository = "https://github.com/wilfredinni/dinero"
 keywords = ["python3", "money", "decimals", "calculations", "currency"]
 
@@ -22,13 +22,13 @@
 pandas = "^2.0.0"
 coverage = "^7.0.0"
 pytest-cov = "^4.0.0"
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
-mkdocstrings = {extras = ["python"], version = "^0.21.0"}
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 mkdocs-material = "^9.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dinero-0.2.0/PKG-INFO` & `dinero-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dinero
-Version: 0.2.0
+Version: 0.2.1
 Summary: Dinero is a library for working with monetary values in Python.
 Home-page: https://github.com/wilfredinni/dinero
 License: MIT
 Keywords: python3,money,decimals,calculations,currency
 Author: Carlos Montecinos Geisse
 Author-email: carlos@pythoncheatsheet.org
 Requires-Python: >=3.10,<4.0
@@ -156,15 +156,15 @@
     duration=10,
     compound_frequency=12,
 )
 total_interest.format(symbol=True, currency=True)
 '$1,294.02 USD'
 ```
 
-See al the available tools in the [tools](https://wilfredinni.github.io/dinero/tools/) section.
+See all the available tools in the [tools](https://wilfredinni.github.io/dinero/tools/) section.
 
 ### Custom currencies
 
 You can easily create custom currencies:
 
 ```python
 from dinero import Dinero
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dinero Version: 0.2.0 Summary: Dinero is a library
+Metadata-Version: 2.1 Name: dinero Version: 0.2.1 Summary: Dinero is a library
 for working with monetary values in Python. Home-page: https://github.com/
 wilfredinni/dinero License: MIT Keywords:
 python3,money,decimals,calculations,currency Author: Carlos Montecinos Geisse
 Author-email: carlos@pythoncheatsheet.org Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: typing-
@@ -50,14 +50,14 @@
 #comparisons). ### Tools Dinero give you access to some useful tools that allow
 you to perform common monetary calculations, like percentages, VAT, simple and
 compound interests, etc. ```python from dinero import Dinero from
 dinero.currencies import USD from dinero.tools import
 calculate_compound_interest principal = Dinero("2000", USD) total_interest =
 calculate_compound_interest( principal=principal, interest_rate=5, duration=10,
 compound_frequency=12, ) total_interest.format(symbol=True, currency=True)
-'$1,294.02 USD' ``` See al the available tools in the [tools](https://
+'$1,294.02 USD' ``` See all the available tools in the [tools](https://
 wilfredinni.github.io/dinero/tools/) section. ### Custom currencies You can
 easily create custom currencies: ```python from dinero import Dinero BTC =
 { "code": "BTC", "base": 10, "exponent": 2, "symbol": "â¿", } Dinero(1000.5,
 BTC) ``` ```python Dinero(amount=1000.5, currency={'code': 'BTC', 'base': 10,
 'exponent': 2, 'symbol': 'â¿'}) ``` More about [custom currencies](https://
 wilfredinni.github.io/dinero/currencies/#custom-currencies).
```

