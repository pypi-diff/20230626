# Comparing `tmp/Dowell Mail-1.0.1.tar.gz` & `tmp/Dowell Mail-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dowell Mail-1.0.1.tar", last modified: Mon Jun 26 11:26:06 2023, max compression
+gzip compressed data, was "Dowell Mail-1.0.2.tar", last modified: Mon Jun 26 11:30:25 2023, max compression
```

## Comparing `Dowell Mail-1.0.1.tar` & `Dowell Mail-1.0.2.tar`

### file list

```diff
@@ -1,602 +1,602 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:06.430592 Dowell Mail-1.0.1/
--rw-rw-rw-   0        0        0       48 2023-06-26 10:57:39.000000 Dowell Mail-1.0.1/.env
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.287585 Dowell Mail-1.0.1/Dowell_Mail.egg-info/
--rw-rw-rw-   0        0        0     2270 2023-06-26 11:26:03.000000 Dowell Mail-1.0.1/Dowell_Mail.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    19570 2023-06-26 11:26:03.000000 Dowell Mail-1.0.1/Dowell_Mail.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 11:26:03.000000 Dowell Mail-1.0.1/Dowell_Mail.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-26 11:26:03.000000 Dowell Mail-1.0.1/Dowell_Mail.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-26 11:26:03.000000 Dowell Mail-1.0.1/Dowell_Mail.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-15 09:01:20.000000 Dowell Mail-1.0.1/LICENCE
--rw-rw-rw-   0        0        0    11558 2023-06-15 09:38:08.000000 Dowell Mail-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      134 2023-06-21 07:35:05.000000 Dowell Mail-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2270 2023-06-26 11:26:06.430592 Dowell Mail-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1564 2023-06-26 10:08:12.000000 Dowell Mail-1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.341563 Dowell Mail-1.0.1/docs/
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.373202 Dowell Mail-1.0.1/docs/.git/
--rw-rw-rw-   0        0        0        5 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/COMMIT_EDITMSG
--rw-rw-rw-   0        0        0        0 2023-06-25 15:56:50.000000 Dowell Mail-1.0.1/docs/.git/FETCH_HEAD
--rw-rw-rw-   0        0        0       21 2023-06-22 10:20:29.000000 Dowell Mail-1.0.1/docs/.git/HEAD
--rw-rw-rw-   0        0        0      294 2023-06-22 10:20:54.000000 Dowell Mail-1.0.1/docs/.git/config
--rw-rw-rw-   0        0        0       73 2023-06-22 10:18:28.000000 Dowell Mail-1.0.1/docs/.git/description
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.444198 Dowell Mail-1.0.1/docs/.git/hooks/
--rw-rw-rw-   0        0        0      478 2023-06-22 10:18:28.000000 Dowell Mail-1.0.1/docs/.git/hooks/applypatch-msg.sample
--rw-rw-rw-   0        0        0      896 2023-06-22 10:18:28.000000 Dowell Mail-1.0.1/docs/.git/hooks/commit-msg.sample
--rw-rw-rw-   0        0        0     4726 2023-06-22 10:18:28.000000 Dowell Mail-1.0.1/docs/.git/hooks/fsmonitor-watchman.sample
--rw-rw-rw-   0        0        0      189 2023-06-22 10:18:28.000000 Dowell Mail-1.0.1/docs/.git/hooks/post-update.sample
--rw-rw-rw-   0        0        0      424 2023-06-22 10:18:28.000000 Dowell Mail-1.0.1/docs/.git/hooks/pre-applypatch.sample
--rw-rw-rw-   0        0        0     1643 2023-06-22 10:18:28.000000 Dowell Mail-1.0.1/docs/.git/hooks/pre-commit.sample
--rw-rw-rw-   0        0        0      416 2023-06-22 10:18:28.000000 Dowell Mail-1.0.1/docs/.git/hooks/pre-merge-commit.sample
--rw-rw-rw-   0        0        0     1374 2023-06-22 10:18:28.000000 Dowell Mail-1.0.1/docs/.git/hooks/pre-push.sample
--rw-rw-rw-   0        0        0     4898 2023-06-22 10:18:28.000000 Dowell Mail-1.0.1/docs/.git/hooks/pre-rebase.sample
--rw-rw-rw-   0        0        0      544 2023-06-22 10:18:28.000000 Dowell Mail-1.0.1/docs/.git/hooks/pre-receive.sample
--rw-rw-rw-   0        0        0     1492 2023-06-22 10:18:28.000000 Dowell Mail-1.0.1/docs/.git/hooks/prepare-commit-msg.sample
--rw-rw-rw-   0        0        0     2783 2023-06-22 10:18:28.000000 Dowell Mail-1.0.1/docs/.git/hooks/push-to-checkout.sample
--rw-rw-rw-   0        0        0     3650 2023-06-22 10:18:28.000000 Dowell Mail-1.0.1/docs/.git/hooks/update.sample
--rw-rw-rw-   0        0        0    18730 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/index
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.448202 Dowell Mail-1.0.1/docs/.git/info/
--rw-rw-rw-   0        0        0      240 2023-06-22 10:18:28.000000 Dowell Mail-1.0.1/docs/.git/info/exclude
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.454234 Dowell Mail-1.0.1/docs/.git/logs/
--rw-rw-rw-   0        0        0      528 2023-06-22 10:20:29.000000 Dowell Mail-1.0.1/docs/.git/logs/HEAD
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:03.923524 Dowell Mail-1.0.1/docs/.git/logs/refs/
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.458230 Dowell Mail-1.0.1/docs/.git/logs/refs/heads/
--rw-rw-rw-   0        0        0      342 2023-06-22 10:20:29.000000 Dowell Mail-1.0.1/docs/.git/logs/refs/heads/main
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:03.925519 Dowell Mail-1.0.1/docs/.git/logs/refs/remotes/
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.461235 Dowell Mail-1.0.1/docs/.git/logs/refs/remotes/origin/
--rw-rw-rw-   0        0        0      301 2023-06-22 11:01:05.000000 Dowell Mail-1.0.1/docs/.git/logs/refs/remotes/origin/main
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.193182 Dowell Mail-1.0.1/docs/.git/objects/
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.467816 Dowell Mail-1.0.1/docs/.git/objects/02/
--r--r--r--   0        0        0      163 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/02/8394883bc0686c6ec4bbdccea9a0a7d0c90032
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.476814 Dowell Mail-1.0.1/docs/.git/objects/07/
--r--r--r--   0        0        0      282 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/07/7ae5076f0cd15403d754ec6299b4537e669d50
--r--r--r--   0        0        0     3278 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/07/8d0cab706bad2c6548af839fe50f89ff29011d
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.480831 Dowell Mail-1.0.1/docs/.git/objects/0a/
--r--r--r--   0        0        0     6683 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/0a/cc10571f6e2635820e7dee824d79b24eb64082
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.492825 Dowell Mail-1.0.1/docs/.git/objects/0b/
--r--r--r--   0        0        0      135 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/0b/188f70f06269071481ceb5277c57ceed6de79b
--r--r--r--   0        0        0     3482 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/0b/efce938f1e8e31e8b131fba92285e7cbde0492
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.497813 Dowell Mail-1.0.1/docs/.git/objects/0d/
--r--r--r--   0        0        0     3150 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/0d/cf1133cd7b82c81d790bd3b165e4bef0497364
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.506816 Dowell Mail-1.0.1/docs/.git/objects/11/
--r--r--r--   0        0        0     4843 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/11/bba08eb15c8676a59416cae5c3224032806b36
--r--r--r--   0        0        0     1408 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/11/c9a999490dace18f6121e568c0190ecb04ca33
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.516816 Dowell Mail-1.0.1/docs/.git/objects/14/
--r--r--r--   0        0        0      888 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/14/b9b602f01362269bf04515443533242bd13f11
--r--r--r--   0        0        0      228 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/14/ff25cbaa43706124f10599f0dd07b08c0be525
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.519821 Dowell Mail-1.0.1/docs/.git/objects/15/
--r--r--r--   0        0        0     2292 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/15/29892c823dfa8800da280360a0876cb8627834
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.523876 Dowell Mail-1.0.1/docs/.git/objects/17/
--r--r--r--   0        0        0   168989 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/17/9792ab7540071599ca06538c571372d3788fb6
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.531814 Dowell Mail-1.0.1/docs/.git/objects/18/
--r--r--r--   0        0        0      690 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/18/522369860ece5164ab3f845d63ea18fc77b080
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.535840 Dowell Mail-1.0.1/docs/.git/objects/1b/
--r--r--r--   0        0        0      321 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/1b/f8c0e8bc6384f8c4fbf8d00171a407e9102ed2
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.545823 Dowell Mail-1.0.1/docs/.git/objects/1d/
--r--r--r--   0        0        0     2593 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/1d/768259cdbc1200244462dcd508e120087972fb
--r--r--r--   0        0        0      478 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/1d/9fffa74fbf58a10a208a481f16e53334db805f
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.550841 Dowell Mail-1.0.1/docs/.git/objects/1e/
--r--r--r--   0        0        0      490 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/1e/041805e32525ba3483b99c85ce110855d782c7
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.553840 Dowell Mail-1.0.1/docs/.git/objects/23/
--r--r--r--   0        0        0    14122 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/23/3c46dbc9802fafa8b32ec4edc4a04e9c237c99
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.558849 Dowell Mail-1.0.1/docs/.git/objects/25/
--r--r--r--   0        0        0     1622 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/25/0f5665fa64b70c822190199b3b804b10f8b9d8
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.570394 Dowell Mail-1.0.1/docs/.git/objects/27/
--r--r--r--   0        0        0     2113 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/27/3f4ad0beb8fba582b1e2390c2b7e9d406020a1
--r--r--r--   0        0        0    22495 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/27/6506ff833411e7a32ec5a0d0b6b4138c910b97
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.576393 Dowell Mail-1.0.1/docs/.git/objects/29/
--r--r--r--   0        0        0      482 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/29/8de27ef0fbefbcda3c2d319a132b9654736d0f
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.582392 Dowell Mail-1.0.1/docs/.git/objects/2a/
--r--r--r--   0        0        0       58 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/2a/924f1d6a8bc930c5296bdb2d5c2d3e39b04a1c
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.585388 Dowell Mail-1.0.1/docs/.git/objects/2b/
--r--r--r--   0        0        0      630 2023-06-22 11:01:05.000000 Dowell Mail-1.0.1/docs/.git/objects/2b/d90b52fd5e09963e064b660f9efb4752333a94
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.590390 Dowell Mail-1.0.1/docs/.git/objects/2e/
--r--r--r--   0        0        0     1848 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/2e/4b30d921c3343a19744726882b85cdf3621f5c
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.631397 Dowell Mail-1.0.1/docs/.git/objects/2f/
--r--r--r--   0        0        0      135 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/2f/1ed6f82ef1d10c599420be3cd798ecce38578e
--r--r--r--   0        0        0     2854 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/2f/9bf5aebdb39583df031edacfc61c32f399c4b8
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.637393 Dowell Mail-1.0.1/docs/.git/objects/31/
--r--r--r--   0        0        0      913 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/31/f32feb95e4c90d013340e6a8b94d5a6a2392b5
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.642398 Dowell Mail-1.0.1/docs/.git/objects/32/
--r--r--r--   0        0        0      181 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/32/6cf15faea93280cfebbb125e4598d6a694e8c7
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.661404 Dowell Mail-1.0.1/docs/.git/objects/34/
--r--r--r--   0        0        0       88 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/34/0b279b985c1f6a993dd3876c8997ce60aa51c8
--r--r--r--   0        0        0      186 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/34/8ec444d138f860514e20617e7637ad6e6eebfa
--r--r--r--   0        0        0     1692 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/34/910dfe5faba7f2cd385dca52906898127628be
--r--r--r--   0        0        0       55 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/34/ddc3897cbf4c8094ebd05a1b8118fc90dcf27e
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.664986 Dowell Mail-1.0.1/docs/.git/objects/35/
--r--r--r--   0        0        0   104197 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/35/acda2fa1196aad98c2adf4378a7611dd713aa3
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.670004 Dowell Mail-1.0.1/docs/.git/objects/36/
--r--r--r--   0        0        0     3225 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/36/eaf6a0450c5a150834345972b6eff6dc20b63c
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.675021 Dowell Mail-1.0.1/docs/.git/objects/3a/
--r--r--r--   0        0        0    16687 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/3a/73a76619e39b9d73f4e9610e60f54d6f999750
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.685004 Dowell Mail-1.0.1/docs/.git/objects/3d/
--r--r--r--   0        0        0      527 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/3d/13b1975139abbb5a4bcc84e6bfff7cd57a4d51
--r--r--r--   0        0        0     1842 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/3d/156b9c191cd246879a67c56e46baa4cfb2e17d
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.700004 Dowell Mail-1.0.1/docs/.git/objects/40/
--r--r--r--   0        0        0    97946 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/40/0014a4b06eee3d0c0d54402a47ab2601b2862b
--r--r--r--   0        0        0     1313 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/40/66129bf24ca86c1eb0cb8cf55f8730b92ca4d8
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.710006 Dowell Mail-1.0.1/docs/.git/objects/45/
--r--r--r--   0        0        0      639 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/45/842b115c602827007d69ecbcaf308511340cdb
--r--r--r--   0        0        0     9208 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/45/bffe09237d6f691365be13b11c8c205a4f35f5
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.716008 Dowell Mail-1.0.1/docs/.git/objects/48/
--r--r--r--   0        0        0      621 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/48/8c29664e6a0160871b70a81c597df7a0a5b276
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.723003 Dowell Mail-1.0.1/docs/.git/objects/4a/
--r--r--r--   0        0        0    16617 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/4a/bdd66d1abde1e9465c471010d0c1056af9c682
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.731007 Dowell Mail-1.0.1/docs/.git/objects/4b/
--r--r--r--   0        0        0       15 2023-06-22 10:19:51.000000 Dowell Mail-1.0.1/docs/.git/objects/4b/825dc642cb6eb9a060e54bf8d69288fbee4904
--r--r--r--   0        0        0      238 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/4b/9549be9b37c5e68c14034988c0557bab76d4de
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.736002 Dowell Mail-1.0.1/docs/.git/objects/4c/
--r--r--r--   0        0        0     2390 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/4c/4e6fd4fcc67b9fa4cd695b9023ac9e66d91904
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.742007 Dowell Mail-1.0.1/docs/.git/objects/4d/
--r--r--r--   0        0        0    77179 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/4d/13fc60404b91e398a37200c4a77b645cfd9586
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.749025 Dowell Mail-1.0.1/docs/.git/objects/4f/
--r--r--r--   0        0        0     3078 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/4f/60d46a956924a94f68b4725075fe3d1191edf7
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.752020 Dowell Mail-1.0.1/docs/.git/objects/50/
--r--r--r--   0        0        0     3334 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/50/dddaa04b87af93b515dd6b33d32d0040254307
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.757024 Dowell Mail-1.0.1/docs/.git/objects/51/
--r--r--r--   0        0        0     3234 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/51/7d0b29cb1193b1211c8853b58c65cddd1fa4d2
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.772607 Dowell Mail-1.0.1/docs/.git/objects/52/
--r--r--r--   0        0        0     3182 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/52/15595b510b67b720091544ea1a4eccb4722381
--r--r--r--   0        0        0     2230 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/52/632004a2414fe4aee1cf9f85696d0ae66eaa3e
--r--r--r--   0        0        0     5473 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/52/ec8be7e6cc2123f25079e19a6dfadd89d8b69d
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.778609 Dowell Mail-1.0.1/docs/.git/objects/54/
--r--r--r--   0        0        0     1097 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/54/430761163f1a6478239ae68eb9a2b8b0d3506e
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.790610 Dowell Mail-1.0.1/docs/.git/objects/55/
--r--r--r--   0        0        0     5077 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/55/901234df171e819e5ab726ebe9eb3acc25dada
--r--r--r--   0        0        0     1272 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/55/fd4172c46835b24bc52edecb319a02e5652963
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.794610 Dowell Mail-1.0.1/docs/.git/objects/56/
--r--r--r--   0        0        0     3029 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/56/a4b0dc19f7c9e8b8423e544ed5e80fbb92abd7
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.813621 Dowell Mail-1.0.1/docs/.git/objects/57/
--r--r--r--   0        0        0     3889 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/57/36305299fc9615b7b91c6778cb365be4e9ccfc
--r--r--r--   0        0        0     1567 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/57/eaee2f2272d9755e1dc69179e8e219050c6905
--r--r--r--   0        0        0       36 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/57/ef03f24a4351df334da53af3b9161bdeac6b1b
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.817612 Dowell Mail-1.0.1/docs/.git/objects/58/
--r--r--r--   0        0        0      639 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/58/40c3bbf9dd7b0b27c6a977d843940b09ae8c54
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.824613 Dowell Mail-1.0.1/docs/.git/objects/59/
--r--r--r--   0        0        0     3535 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/59/161a19db9a40ae6b96ede4cf7213570db3de9a
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.829617 Dowell Mail-1.0.1/docs/.git/objects/5a/
--r--r--r--   0        0        0     1156 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/5a/354d3c77dd2d04ceb0cd61592c0a1a848ba355
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.837634 Dowell Mail-1.0.1/docs/.git/objects/5d/
--r--r--r--   0        0        0     3768 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/5d/ea4a6e8da2f6ce6e06acec0e2662be88b5374f
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.843625 Dowell Mail-1.0.1/docs/.git/objects/5e/
--r--r--r--   0        0        0     4254 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/5e/adc1c5b64a06531d4125561cc513c8fb4ab37d
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.849607 Dowell Mail-1.0.1/docs/.git/objects/5f/
--r--r--r--   0        0        0      308 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/5f/a22e886b899683ce5de581fa0b7fcdc1cdc963
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.865225 Dowell Mail-1.0.1/docs/.git/objects/63/
--r--r--r--   0        0        0      506 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/63/130b01203f39a74b75f1ed082d2fca18a38e40
--r--r--r--   0        0        0       88 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/63/7351746cccdf6b5c72dd2b99f2a1d5b99e7252
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.870256 Dowell Mail-1.0.1/docs/.git/objects/64/
--r--r--r--   0        0        0     3145 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/64/808af3c3ac606f310b83f68ee9cfee8dbc8b03
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.888262 Dowell Mail-1.0.1/docs/.git/objects/68/
--r--r--r--   0        0        0       58 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/68/08d6b4bc94c19e336620efbd95c0ebaa9889c9
--r--r--r--   0        0        0       93 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/68/8881b021f72eb69eaef8c7cb7c7bc5a9a138ce
--r--r--r--   0        0        0      350 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/68/ebffa887dfb5a0ee10257bd15e1d73f54ff3c1
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.895273 Dowell Mail-1.0.1/docs/.git/objects/69/
--r--r--r--   0        0        0     1162 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/69/f620250d95bc3982dd8a6bd46689759a54c2a3
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.900253 Dowell Mail-1.0.1/docs/.git/objects/6c/
--r--r--r--   0        0        0    14545 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/6c/31f329c658b01ae8b2c10194e09ed1a72f4f31
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.914255 Dowell Mail-1.0.1/docs/.git/objects/6d/
--r--r--r--   0        0        0     1376 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/6d/72961051eba439a573224713613f34beebe7d5
--r--r--r--   0        0        0     1689 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/6d/af5f9d807ec44fb0cfba836a21c17dd888f8da
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.920254 Dowell Mail-1.0.1/docs/.git/objects/6e/
--r--r--r--   0        0        0      426 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/6e/36b195b2d3083c18c06bafa280ce86729aa546
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.932254 Dowell Mail-1.0.1/docs/.git/objects/70/
--r--r--r--   0        0        0    66198 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/70/15564ad166a3e9d88c82f17829f0cc01ebe29a
--r--r--r--   0        0        0      199 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/70/536a6683577925167e84e0b0f6a06228754d0a
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.943253 Dowell Mail-1.0.1/docs/.git/objects/71/
--r--r--r--   0        0        0       99 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/71/07cec93a979b9a5f64843235a16651d563ce2d
--r--r--r--   0        0        0      376 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/71/2b8e7d89c0ac96a45eea729077ebc287f3a89d
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.956276 Dowell Mail-1.0.1/docs/.git/objects/75/
--r--r--r--   0        0        0     1267 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/75/45ea35e0a5df26e09aa3b4834e736ab191aac6
--r--r--r--   0        0        0     4210 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/75/77acb1ad176e3f58c15ddf9bf1f73525dfe7ed
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.960277 Dowell Mail-1.0.1/docs/.git/objects/76/
--r--r--r--   0        0        0      541 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/76/d17f57ad903c3ea2f1b564cafb95bf9af84ee3
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.971809 Dowell Mail-1.0.1/docs/.git/objects/77/
--r--r--r--   0        0        0      904 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/77/9d5dd47a5022001209f9c9f935a9c2dde5eebd
--r--r--r--   0        0        0     3947 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/77/ad846085e4e2576ca5157789b70c9e24dc24d0
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.975801 Dowell Mail-1.0.1/docs/.git/objects/79/
--r--r--r--   0        0        0      931 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/79/e30a1f1999c22b29515767c063825cc39c58dd
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.981801 Dowell Mail-1.0.1/docs/.git/objects/7b/
--r--r--r--   0        0        0      388 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/7b/97197e91ce7488eb13f3749849f953bd5cb9aa
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.987818 Dowell Mail-1.0.1/docs/.git/objects/7c/
--r--r--r--   0        0        0    31919 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/7c/724d2e4f2d39cb2e418936f0fdf0198bd118a0
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.999799 Dowell Mail-1.0.1/docs/.git/objects/7d/
--r--r--r--   0        0        0      746 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/7d/1e8c2f1bbc45869b92d703be845f6eb20ebd0a
--r--r--r--   0        0        0    64098 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/7d/86eb1694970141b88b52f5b26e6b019f16b590
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.006811 Dowell Mail-1.0.1/docs/.git/objects/7e/
--r--r--r--   0        0        0       52 2023-06-22 11:01:05.000000 Dowell Mail-1.0.1/docs/.git/objects/7e/953140f053cc0bf5f0b2da0b762b99dc8811e2
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.011802 Dowell Mail-1.0.1/docs/.git/objects/80/
--r--r--r--   0        0        0     4111 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/80/f9d49c9bd4d7d58996254dee424b25d3164ef6
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.017799 Dowell Mail-1.0.1/docs/.git/objects/83/
--r--r--r--   0        0        0      185 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/83/4412e5f09537af46dc5026c4510b651c641831
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.023799 Dowell Mail-1.0.1/docs/.git/objects/85/
--r--r--r--   0        0        0     5711 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/85/e59c4ac73dcfde98d34e848b5c99b7714d33ae
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.029799 Dowell Mail-1.0.1/docs/.git/objects/86/
--r--r--r--   0        0        0      125 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/86/b7198fc951b7bfdf0a41e29877d9829b39f9b8
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.033796 Dowell Mail-1.0.1/docs/.git/objects/89/
--r--r--r--   0        0        0     1257 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/89/9804d75f317500aab85d5dd773814026a7e48c
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.039820 Dowell Mail-1.0.1/docs/.git/objects/8a/
--r--r--r--   0        0        0      415 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/8a/145c9117e791bbd0c472ee442cb74a90888656
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.043800 Dowell Mail-1.0.1/docs/.git/objects/8d/
--r--r--r--   0        0        0     1516 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/8d/7dd0ee7185687b4404c3e0480b20e1ed0fd4eb
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.050815 Dowell Mail-1.0.1/docs/.git/objects/8e/
--r--r--r--   0        0        0     1971 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/8e/793555684ac8caa28b91a17d26502b51629732
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.060816 Dowell Mail-1.0.1/docs/.git/objects/8f/
--r--r--r--   0        0        0     4175 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/8f/99b2771e10cbb806d18c35ce3bfce1eda46dcd
--r--r--r--   0        0        0     1578 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/8f/c9926ef0fa53320bc485118f7a870a19eda8db
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.068404 Dowell Mail-1.0.1/docs/.git/objects/91/
--r--r--r--   0        0        0     3023 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/91/3bc8210a6a2156fc818eef2d545e8b0871a518
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.074435 Dowell Mail-1.0.1/docs/.git/objects/93/
--r--r--r--   0        0        0      447 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/93/b2c8c086a53e63f7e906241a07198b2ff073bb
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.081427 Dowell Mail-1.0.1/docs/.git/objects/94/
--r--r--r--   0        0        0      298 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/94/bda2139156340fc42bb1cb678e49ac9ac8d3c6
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.088408 Dowell Mail-1.0.1/docs/.git/objects/95/
--r--r--r--   0        0        0      438 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/95/4237b9b9f2b248bb1397a15c055c0af1cad03e
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.093400 Dowell Mail-1.0.1/docs/.git/objects/97/
--r--r--r--   0        0        0     6728 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/97/d56a74d8207ec36a96a5e24f4a4b42dd51f6b2
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.102421 Dowell Mail-1.0.1/docs/.git/objects/9a/
--r--r--r--   0        0        0     1388 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/9a/a62fc22baa68906867164da4d6819dfaf72907
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.109402 Dowell Mail-1.0.1/docs/.git/objects/9d/
--r--r--r--   0        0        0     3490 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/9d/e6c09cb4238addb63e4a63a54bdf83b6c8d6ff
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.118398 Dowell Mail-1.0.1/docs/.git/objects/9e/
--r--r--r--   0        0        0      436 2023-06-22 11:01:05.000000 Dowell Mail-1.0.1/docs/.git/objects/9e/13fc18a432ac279e1c31eb305c56bbb30602e4
--r--r--r--   0        0        0    21654 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/9e/4453259d6929c2bf7b7b9a5d18c76a753c4d44
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.123399 Dowell Mail-1.0.1/docs/.git/objects/9f/
--r--r--r--   0        0        0    44332 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/9f/a211252080046a23b2449dbdced6abc2b0bb34
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.127410 Dowell Mail-1.0.1/docs/.git/objects/a1/
--r--r--r--   0        0        0     4038 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/a1/3b146a9a996aea5bc19af6bc48ac34579485a9
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.132405 Dowell Mail-1.0.1/docs/.git/objects/a2/
--r--r--r--   0        0        0     2329 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/a2/a1a0e393e42392b8046793cf3361227432fe73
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.140414 Dowell Mail-1.0.1/docs/.git/objects/a3/
--r--r--r--   0        0        0     4374 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/a3/1ae4ce3a2c809b63787b319c6ebc51df4dee6d
--r--r--r--   0        0        0      166 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/a3/a633d83087f3d0384ca9c8c241f109f0f65414
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.143400 Dowell Mail-1.0.1/docs/.git/objects/a6/
--r--r--r--   0        0        0     2022 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/a6/5d194b7adbb6fac28c1654cca5d0c165015377
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.149405 Dowell Mail-1.0.1/docs/.git/objects/a7/
--r--r--r--   0        0        0      279 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/a7/f754b66f245c8342c8dfc42de1b439f620054f
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.151429 Dowell Mail-1.0.1/docs/.git/objects/a8/
--r--r--r--   0        0        0      306 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/a8/58a410e4faa62ce324d814e4b816fff83a6fb3
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.157422 Dowell Mail-1.0.1/docs/.git/objects/a9/
--r--r--r--   0        0        0      882 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/a9/ca1c82cd661cfa1583e86fa881644d029d061f
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.160426 Dowell Mail-1.0.1/docs/.git/objects/aa/
--r--r--r--   0        0        0     1931 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/aa/e669d7ea6b1dc6edcb5c651f5d095f7a2dc6e6
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.164419 Dowell Mail-1.0.1/docs/.git/objects/ac/
--r--r--r--   0        0        0     3408 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/ac/99248044a350007567ce177ba3e2ae286bef63
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.167795 Dowell Mail-1.0.1/docs/.git/objects/ad/
--r--r--r--   0        0        0      960 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/ad/07dd68bddf8730f4584ed84fac8050473a6d95
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.175794 Dowell Mail-1.0.1/docs/.git/objects/af/
--r--r--r--   0        0        0      124 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/af/094027a710f1671668ae6590d3bf21a9f08657
--r--r--r--   0        0        0      912 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/af/5a804d593607e51ca637bebcbc9633f261691d
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.180825 Dowell Mail-1.0.1/docs/.git/objects/b0/
--r--r--r--   0        0        0    11332 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/b0/d3707062fef1eb41d2e5ac63e09d48465e6bab
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.184798 Dowell Mail-1.0.1/docs/.git/objects/b1/
--r--r--r--   0        0        0     3482 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/b1/9627e1b35eb0240db39497c70b509624c0da09
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.196794 Dowell Mail-1.0.1/docs/.git/objects/b2/
--r--r--r--   0        0        0     2992 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/b2/0fbbb83a55f6286917183d07d549846b0b8ed9
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.213799 Dowell Mail-1.0.1/docs/.git/objects/b4/
--r--r--r--   0        0        0     7881 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/b4/76b53e33b5789396e2b48d44c8abc07a037db3
--r--r--r--   0        0        0     3755 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/b4/ff1f9d02d01ec10e3808971706542a6d0ec748
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.233792 Dowell Mail-1.0.1/docs/.git/objects/b5/
--r--r--r--   0        0        0      428 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/b5/733ba707cd68b0929cea4d8e48c07b96ffe609
--r--r--r--   0        0        0      855 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/b5/9cb4eb5ff374906c380579330c0fe36fa3cc88
--r--r--r--   0        0        0     1493 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/b5/e9c8543653a3c7194b8f4879ef43646bc79c2e
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.243577 Dowell Mail-1.0.1/docs/.git/objects/b6/
--r--r--r--   0        0        0    57629 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/b6/48a3eea2d16b6ce783906d6b7d5f251b9eb56c
--r--r--r--   0        0        0    31169 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/b6/6df4ab09628c1dcce7f663a314e51332c64310
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.249660 Dowell Mail-1.0.1/docs/.git/objects/b8/
--r--r--r--   0        0        0      570 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/b8/8f108df9a4d81e94bb8d0a3ecded420c9999f7
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.260685 Dowell Mail-1.0.1/docs/.git/objects/b9/
--r--r--r--   0        0        0     2330 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/b9/b75fc0ea791147b7195473e733caee6e4fc31e
--r--r--r--   0        0        0     4285 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/b9/f5723bd8733e425085e505dd100de2cf54c6cb
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.264680 Dowell Mail-1.0.1/docs/.git/objects/ba/
--r--r--r--   0        0        0     2402 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/ba/a21647ca52c56d628adce41e076b5a837ae90d
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.273716 Dowell Mail-1.0.1/docs/.git/objects/bb/
--r--r--r--   0        0        0      330 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/bb/1c0e9cea56d06c0ec25fad185924f814778ae4
--r--r--r--   0        0        0      210 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/bb/a17fa6bc6aa2e1a0f08088b7bd685077463e8e
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.278702 Dowell Mail-1.0.1/docs/.git/objects/bc/
--r--r--r--   0        0        0     2058 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/bc/fc55fb0b780383ae096b2b5a9b47eef30bcf81
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.283700 Dowell Mail-1.0.1/docs/.git/objects/c0/
--r--r--r--   0        0        0       52 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/c0/55ebaf37a904fafc2815f4f8d0e810db0b0984
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.286700 Dowell Mail-1.0.1/docs/.git/objects/c1/
--r--r--r--   0        0        0      405 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/c1/d165229552b8adb7f91199d8ab16524c28da7d
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.290697 Dowell Mail-1.0.1/docs/.git/objects/c4/
--r--r--r--   0        0        0    36048 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/c4/c6022f2982e8dae64cebd6b9a2b59f2547faad
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.293700 Dowell Mail-1.0.1/docs/.git/objects/c5/
--r--r--r--   0        0        0       87 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/c5/5299abe93533ce599c650aa2853e1bc422f7a4
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.301698 Dowell Mail-1.0.1/docs/.git/objects/c8/
--r--r--r--   0        0        0      163 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/c8/d8fb540030e23b240ba39543609315056d8e6f
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.315714 Dowell Mail-1.0.1/docs/.git/objects/cc/
--r--r--r--   0        0        0     3311 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/cc/1b794a9b9667f1a6600afc3b3fdce4ac649719
--r--r--r--   0        0        0     1244 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/cc/a624a2ceebd47f7c807110d1e4669d88d7a11f
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.319703 Dowell Mail-1.0.1/docs/.git/objects/ce/
--r--r--r--   0        0        0      639 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/ce/62404b61db8d0ba61bb34c7f4ae5d1fcc31ca1
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.323716 Dowell Mail-1.0.1/docs/.git/objects/cf/
--r--r--r--   0        0        0      681 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/cf/58c14fbc67be0626eb95a0a8fc68baa8c2ac03
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.333710 Dowell Mail-1.0.1/docs/.git/objects/d0/
--r--r--r--   0        0        0     1774 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/d0/6a71d7518041301a303697d2a3c372648eb7bf
--r--r--r--   0        0        0     6146 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/d0/b4b7a096a9df7ca9e16e969b980e37c742149d
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.340723 Dowell Mail-1.0.1/docs/.git/objects/d2/
--r--r--r--   0        0        0       86 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/d2/eb00277d21b14f5f831bccf0fb51c5cfa1e0a4
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.345704 Dowell Mail-1.0.1/docs/.git/objects/d4/
--r--r--r--   0        0        0      367 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/d4/bb2cbb9eddb1bb1b4f366623044af8e4830919
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.349700 Dowell Mail-1.0.1/docs/.git/objects/d5/
--r--r--r--   0        0        0      186 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/d5/d0aaa972d0bf29ca687bc2cd328f575b6d4cc0
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.353747 Dowell Mail-1.0.1/docs/.git/objects/d8/
--r--r--r--   0        0        0     4371 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/d8/54b4aa71024fc8efb2f1e9fced00c21f57a2f3
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.363737 Dowell Mail-1.0.1/docs/.git/objects/d9/
--r--r--r--   0        0        0       97 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/d9/6755fdaf8bb2214971e0db9c1fd3077d7c419d
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.368248 Dowell Mail-1.0.1/docs/.git/objects/e0/
--r--r--r--   0        0        0      439 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/e0/9b6c0b00d3c7d31d0edb4e6384c756920b82c5
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.372246 Dowell Mail-1.0.1/docs/.git/objects/e1/
--r--r--r--   0        0        0      178 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/e1/f6000458504acf1ac56d147e53512e058e9f73
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.376252 Dowell Mail-1.0.1/docs/.git/objects/e3/
--r--r--r--   0        0        0       54 2023-06-22 11:01:05.000000 Dowell Mail-1.0.1/docs/.git/objects/e3/fad2dd6545c4627e88caefc23fcaed67c46251
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.383282 Dowell Mail-1.0.1/docs/.git/objects/e4/
--r--r--r--   0        0        0     3386 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/e4/e95b864519c0acc98412378441c422cecba687
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.388250 Dowell Mail-1.0.1/docs/.git/objects/e5/
--r--r--r--   0        0        0      116 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/e5/27a3089e20f9f4226e6c0df4a4d9dadb96a115
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.401248 Dowell Mail-1.0.1/docs/.git/objects/e7/
--r--r--r--   0        0        0      561 2023-06-22 11:01:05.000000 Dowell Mail-1.0.1/docs/.git/objects/e7/996d8e3406e79a393e78cf8e9c553c4702f85b
--r--r--r--   0        0        0     1460 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/e7/a7c1901ed4c6a32722f03d6d9a8c0ff5d55652
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.408292 Dowell Mail-1.0.1/docs/.git/objects/e8/
--r--r--r--   0        0        0     3942 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/e8/fb5a7df64cf44eee42ab10ad6386bb57fa9e3d
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.416275 Dowell Mail-1.0.1/docs/.git/objects/e9/
--r--r--r--   0        0        0      750 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/e9/63414845f850fffe51fa14893f6b67aed97731
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.421253 Dowell Mail-1.0.1/docs/.git/objects/ea/
--r--r--r--   0        0        0      118 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/ea/ab363250d42b878741d17cda8d1355f5768dd5
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.427245 Dowell Mail-1.0.1/docs/.git/objects/ec/
--r--r--r--   0        0        0      632 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/ec/314fea70f892ffd1dbd4a53add8891df3ca982
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.432246 Dowell Mail-1.0.1/docs/.git/objects/ed/
--r--r--r--   0        0        0      294 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/ed/99102e8b03e4af6f450d884de4d98646b1c159
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.437291 Dowell Mail-1.0.1/docs/.git/objects/ee/
--r--r--r--   0        0        0      529 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/ee/8ef373a0d0a4aa2609d7382d7b6bb605824fe6
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.443251 Dowell Mail-1.0.1/docs/.git/objects/f1/
--r--r--r--   0        0        0      794 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/f1/f525a8375f9fc814afff69f587e2123226f9ae
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.450247 Dowell Mail-1.0.1/docs/.git/objects/f3/
--r--r--r--   0        0        0     2856 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/f3/9f778b208dd9614d56b285b880f3697c15e709
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.457301 Dowell Mail-1.0.1/docs/.git/objects/f5/
--r--r--r--   0        0        0     3000 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/f5/0fc9fa6d5a0f1a479676d9c0ab72c44125d08c
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.462282 Dowell Mail-1.0.1/docs/.git/objects/f7/
--r--r--r--   0        0        0     1524 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/f7/18bb2f85762580330d3145e01b1aa4e01c51fd
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.474839 Dowell Mail-1.0.1/docs/.git/objects/f9/
--r--r--r--   0        0        0       54 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/f9/053d8d4eabfa90b1b6cc2cf6da9616fbc96de4
--r--r--r--   0        0        0      115 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/f9/06e654208eb66982d75b3a45c20db781a36303
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.484832 Dowell Mail-1.0.1/docs/.git/objects/fb/
--r--r--r--   0        0        0     1216 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/fb/846534ac59ccbedb425076d96870627575f620
--r--r--r--   0        0        0     2787 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/fb/a1ee45d9f9437f627343a4b66c0dfc59ebec0a
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.509838 Dowell Mail-1.0.1/docs/.git/objects/fd/
--r--r--r--   0        0        0     1944 2023-06-22 10:20:06.000000 Dowell Mail-1.0.1/docs/.git/objects/fd/0aae6386addf84721ec0d5fec2e997013ec6bf
--r--r--r--   0        0        0      212 2023-06-22 10:20:15.000000 Dowell Mail-1.0.1/docs/.git/objects/fd/53ed54ed8b90a7bbbe811a43518acf22c70ee4
--r--r--r--   0        0        0     1336 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/fd/f3913755aa169c74990ca316dc8bd48a4bad55
--r--r--r--   0        0        0      283 2023-06-22 10:20:05.000000 Dowell Mail-1.0.1/docs/.git/objects/fd/fc61dddbf6a74869da2ecf31879346149d532b
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.198174 Dowell Mail-1.0.1/docs/.git/refs/
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.515835 Dowell Mail-1.0.1/docs/.git/refs/heads/
--rw-rw-rw-   0        0        0       41 2023-06-22 10:20:29.000000 Dowell Mail-1.0.1/docs/.git/refs/heads/main
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.199179 Dowell Mail-1.0.1/docs/.git/refs/remotes/
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.518830 Dowell Mail-1.0.1/docs/.git/refs/remotes/origin/
--rw-rw-rw-   0        0        0       41 2023-06-22 11:01:05.000000 Dowell Mail-1.0.1/docs/.git/refs/remotes/origin/main
--rw-rw-rw-   0        0        0      634 2023-06-22 06:23:19.000000 Dowell Mail-1.0.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.230183 Dowell Mail-1.0.1/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.568384 Dowell Mail-1.0.1/docs/_build/doctrees/
--rw-rw-rw-   0        0        0    15009 2023-06-22 06:33:40.000000 Dowell Mail-1.0.1/docs/_build/doctrees/emailapp.doctree
--rw-rw-rw-   0        0        0   148054 2023-06-22 10:29:44.000000 Dowell Mail-1.0.1/docs/_build/doctrees/environment.pickle
--rw-rw-rw-   0        0        0     8345 2023-06-22 08:14:59.000000 Dowell Mail-1.0.1/docs/_build/doctrees/index.doctree
--rw-rw-rw-   0        0        0    24405 2023-06-22 06:33:40.000000 Dowell Mail-1.0.1/docs/_build/doctrees/maillib.doctree
--rw-rw-rw-   0        0        0     3057 2023-06-22 06:33:40.000000 Dowell Mail-1.0.1/docs/_build/doctrees/maillib.migrations.doctree
--rw-rw-rw-   0        0        0    26023 2023-06-22 06:33:41.000000 Dowell Mail-1.0.1/docs/_build/doctrees/maillib.tests.doctree
--rw-rw-rw-   0        0        0     2752 2023-06-22 10:29:44.000000 Dowell Mail-1.0.1/docs/_build/doctrees/modules.doctree
--rw-rw-rw-   0        0        0     7115 2023-06-22 08:10:14.000000 Dowell Mail-1.0.1/docs/_build/doctrees/static.doctree
--rw-rw-rw-   0        0        0     5517 2023-06-22 08:10:14.000000 Dowell Mail-1.0.1/docs/_build/doctrees/templates.doctree
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.652403 Dowell Mail-1.0.1/docs/_build/epub/
--rw-rw-rw-   0        0        0      234 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/.buildinfo
--rw-rw-rw-   0        0        0    23768 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/Dowell-Mail.epub
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.656404 Dowell Mail-1.0.1/docs/_build/epub/META-INF/
--rw-rw-rw-   0        0        0      246 2023-06-20 09:37:24.000000 Dowell Mail-1.0.1/docs/_build/epub/META-INF/container.xml
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.664406 Dowell Mail-1.0.1/docs/_build/epub/_partials/
--rw-rw-rw-   0        0        0      548 2023-06-13 06:52:16.000000 Dowell Mail-1.0.1/docs/_build/epub/_partials/base.html
--rw-rw-rw-   0        0        0      164 2023-06-13 09:58:30.000000 Dowell Mail-1.0.1/docs/_build/epub/_partials/messages.html
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.709933 Dowell Mail-1.0.1/docs/_build/epub/_static/
--rw-rw-rw-   0        0        0    15715 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/_static/basic.css
--rw-rw-rw-   0        0        0     4472 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/epub/_static/doctools.js
--rw-rw-rw-   0        0        0      433 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/_static/documentation_options.js
--rw-rw-rw-   0        0        0    12897 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/_static/epub.css
--rw-rw-rw-   0        0        0      286 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/epub/_static/file.png
--rw-rw-rw-   0        0        0      339 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/epub/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/epub/_static/plus.png
--rw-rw-rw-   0        0        0      539 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/_static/pygments.css
--rw-rw-rw-   0        0        0    18215 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/epub/_static/searchtools.js
--rw-rw-rw-   0        0        0     4712 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/epub/_static/sphinx_highlight.js
--rw-rw-rw-   0        0        0     3153 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/content.opf
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.714932 Dowell Mail-1.0.1/docs/_build/epub/css/
--rw-rw-rw-   0        0        0     2055 2023-06-13 09:55:15.000000 Dowell Mail-1.0.1/docs/_build/epub/css/styles.css
--rw-rw-rw-   0        0        0     4011 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/emailapp.xhtml
--rw-rw-rw-   0        0        0     7696 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/genindex.xhtml
--rw-rw-rw-   0        0        0     3070 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/index.xhtml
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.718963 Dowell Mail-1.0.1/docs/_build/epub/maillib/
--rw-rw-rw-   0        0        0     1232 2023-06-14 09:48:36.000000 Dowell Mail-1.0.1/docs/_build/epub/maillib/home.html
--rw-rw-rw-   0        0        0      980 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/maillib.migrations.xhtml
--rw-rw-rw-   0        0        0     6336 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/maillib.tests.xhtml
--rw-rw-rw-   0        0        0     9108 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/maillib.xhtml
--rw-rw-rw-   0        0        0       20 2023-06-20 09:37:24.000000 Dowell Mail-1.0.1/docs/_build/epub/mimetype
--rw-rw-rw-   0        0        0     4996 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/modules.xhtml
--rw-rw-rw-   0        0        0      630 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/nav.xhtml
--rw-rw-rw-   0        0        0     4568 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/py-modindex.xhtml
--rw-rw-rw-   0        0        0    19125 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/static.xhtml
--rw-rw-rw-   0        0        0     4173 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/templates.xhtml
--rw-rw-rw-   0        0        0      948 2023-06-22 09:51:37.000000 Dowell Mail-1.0.1/docs/_build/epub/toc.ncx
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.777478 Dowell Mail-1.0.1/docs/_build/html/
--rw-rw-rw-   0        0        0      234 2023-06-22 09:47:55.000000 Dowell Mail-1.0.1/docs/_build/html/.buildinfo
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.782484 Dowell Mail-1.0.1/docs/_build/html/_modules/
--rw-rw-rw-   0        0        0     9448 2023-06-22 09:47:54.000000 Dowell Mail-1.0.1/docs/_build/html/_modules/index.html
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.791477 Dowell Mail-1.0.1/docs/_build/html/_modules/maillib/
--rw-rw-rw-   0        0        0     3285 2023-06-22 06:33:43.000000 Dowell Mail-1.0.1/docs/_build/html/_modules/maillib/apps.html
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.800495 Dowell Mail-1.0.1/docs/_build/html/_modules/maillib/tests/
--rw-rw-rw-   0        0        0     4901 2023-06-22 06:33:43.000000 Dowell Mail-1.0.1/docs/_build/html/_modules/maillib/tests/test_urls.html
--rw-rw-rw-   0        0        0    15316 2023-06-22 06:33:43.000000 Dowell Mail-1.0.1/docs/_build/html/_modules/maillib/tests/test_views.html
--rw-rw-rw-   0        0        0    12282 2023-06-22 06:33:43.000000 Dowell Mail-1.0.1/docs/_build/html/_modules/maillib/views.html
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.807492 Dowell Mail-1.0.1/docs/_build/html/_partials/
--rw-rw-rw-   0        0        0      548 2023-06-13 06:52:16.000000 Dowell Mail-1.0.1/docs/_build/html/_partials/base.html
--rw-rw-rw-   0        0        0      164 2023-06-13 09:58:30.000000 Dowell Mail-1.0.1/docs/_build/html/_partials/messages.html
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.840627 Dowell Mail-1.0.1/docs/_build/html/_sources/
--rw-rw-rw-   0        0        0      739 2023-06-22 06:25:18.000000 Dowell Mail-1.0.1/docs/_build/html/_sources/emailapp.rst.txt
--rw-rw-rw-   0        0        0     1770 2023-06-22 08:05:11.000000 Dowell Mail-1.0.1/docs/_build/html/_sources/index.rst.txt
--rw-rw-rw-   0        0        0      187 2023-06-22 06:25:19.000000 Dowell Mail-1.0.1/docs/_build/html/_sources/maillib.migrations.rst.txt
--rw-rw-rw-   0        0        0      961 2023-06-22 06:25:19.000000 Dowell Mail-1.0.1/docs/_build/html/_sources/maillib.rst.txt
--rw-rw-rw-   0        0        0      537 2023-06-22 06:25:19.000000 Dowell Mail-1.0.1/docs/_build/html/_sources/maillib.tests.rst.txt
--rw-rw-rw-   0        0        0      116 2023-06-22 06:33:29.000000 Dowell Mail-1.0.1/docs/_build/html/_sources/modules.rst.txt
--rw-rw-rw-   0        0        0     2613 2023-06-22 08:08:05.000000 Dowell Mail-1.0.1/docs/_build/html/_sources/static.rst.txt
--rw-rw-rw-   0        0        0     1588 2023-06-22 08:10:07.000000 Dowell Mail-1.0.1/docs/_build/html/_sources/templates.rst.txt
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.919196 Dowell Mail-1.0.1/docs/_build/html/_static/
--rw-rw-rw-   0        0        0    11932 2023-06-22 06:33:43.000000 Dowell Mail-1.0.1/docs/_build/html/_static/alabaster.css
--rw-rw-rw-   0        0        0    15715 2023-06-22 09:47:55.000000 Dowell Mail-1.0.1/docs/_build/html/_static/basic.css
--rw-rw-rw-   0        0        0       42 2023-06-20 09:37:24.000000 Dowell Mail-1.0.1/docs/_build/html/_static/custom.css
--rw-rw-rw-   0        0        0     4472 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/html/_static/doctools.js
--rw-rw-rw-   0        0        0      431 2023-06-22 09:47:55.000000 Dowell Mail-1.0.1/docs/_build/html/_static/documentation_options.js
--rw-rw-rw-   0        0        0      286 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/html/_static/file.png
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.926185 Dowell Mail-1.0.1/docs/_build/html/_static/fonts/
--rw-rw-rw-   0        0        0    30724 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/fonts/font-awesome.css
--rw-rw-rw-   0        0        0      903 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/fonts/material-icons.css
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.959217 Dowell Mail-1.0.1/docs/_build/html/_static/fonts/specimen/
--rw-rw-rw-   0        0        0   165548 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/fonts/specimen/FontAwesome.ttf
--rw-rw-rw-   0        0        0    98024 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/fonts/specimen/FontAwesome.woff
--rw-rw-rw-   0        0        0    77160 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/fonts/specimen/FontAwesome.woff2
--rw-rw-rw-   0        0        0   128180 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/fonts/specimen/MaterialIcons-Regular.ttf
--rw-rw-rw-   0        0        0    57620 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/fonts/specimen/MaterialIcons-Regular.woff
--rw-rw-rw-   0        0        0    44300 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/fonts/specimen/MaterialIcons-Regular.woff2
--rw-rw-rw-   0        0        0    13292 2023-06-22 08:10:15.000000 Dowell Mail-1.0.1/docs/_build/html/_static/groundwork.css
--rw-rw-rw-   0        0        0    14145 2023-06-22 07:09:36.000000 Dowell Mail-1.0.1/docs/_build/html/_static/gw_logo.png
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.964207 Dowell Mail-1.0.1/docs/_build/html/_static/images/
--rw-rw-rw-   0        0        0      521 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/images/favicon.png
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:05.990736 Dowell Mail-1.0.1/docs/_build/html/_static/images/icons/
--rw-rw-rw-   0        0        0     1230 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/images/icons/bitbucket.1b09e088.svg
--rw-rw-rw-   0        0        0     1230 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/images/icons/bitbucket.svg
--rw-rw-rw-   0        0        0      993 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/images/icons/github.f0b8504a.svg
--rw-rw-rw-   0        0        0      993 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/images/icons/github.svg
--rw-rw-rw-   0        0        0     1138 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/images/icons/gitlab.6dd19c00.svg
--rw-rw-rw-   0        0        0     1138 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/images/icons/gitlab.svg
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:06.006742 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/
--rw-rw-rw-   0        0        0   135210 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/application.js
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:06.129293 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/
--rw-rw-rw-   0        0        0     4259 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.da.js
--rw-rw-rw-   0        0        0     5736 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.de.js
--rw-rw-rw-   0        0        0     5817 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.du.js
--rw-rw-rw-   0        0        0    11072 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.es.js
--rw-rw-rw-   0        0        0     8870 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.fi.js
--rw-rw-rw-   0        0        0    10242 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.fr.js
--rw-rw-rw-   0        0        0     9025 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.hu.js
--rw-rw-rw-   0        0        0    10739 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.it.js
--rw-rw-rw-   0        0        0     2282 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.ja.js
--rw-rw-rw-   0        0        0       36 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.jp.js
--rw-rw-rw-   0        0        0      774 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.multi.js
--rw-rw-rw-   0        0        0     5635 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.nl.js
--rw-rw-rw-   0        0        0     4340 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.no.js
--rw-rw-rw-   0        0        0     9728 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.pt.js
--rw-rw-rw-   0        0        0    10498 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.ro.js
--rw-rw-rw-   0        0        0     9808 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.ru.js
--rw-rw-rw-   0        0        0     3633 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.stemmer.support.js
--rw-rw-rw-   0        0        0     4129 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.sv.js
--rw-rw-rw-   0        0        0     1029 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.th.js
--rw-rw-rw-   0        0        0    13761 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.tr.js
--rw-rw-rw-   0        0        0    18288 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/tinyseg.js
--rw-rw-rw-   0        0        0   555307 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/wordcut.js
--rw-rw-rw-   0        0        0     7285 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/modernizr.js
--rw-rw-rw-   0        0        0     1107 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/version_dropdown.js
--rw-rw-rw-   0        0        0    89503 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/jquery.js
--rw-rw-rw-   0        0        0   137972 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/jquery.min.map
--rw-rw-rw-   0        0        0     4957 2023-06-22 09:47:55.000000 Dowell Mail-1.0.1/docs/_build/html/_static/language_data.js
--rw-rw-rw-   0        0        0      706 2023-06-22 09:47:55.000000 Dowell Mail-1.0.1/docs/_build/html/_static/material.css
--rw-rw-rw-   0        0        0       90 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/html/_static/plus.png
--rw-rw-rw-   0        0        0     4891 2023-06-22 09:47:55.000000 Dowell Mail-1.0.1/docs/_build/html/_static/pygments.css
--rw-rw-rw-   0        0        0    18215 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/html/_static/searchtools.js
--rw-rw-rw-   0        0        0     1259 2023-06-22 07:09:36.000000 Dowell Mail-1.0.1/docs/_build/html/_static/small_groundwork.css
--rw-rw-rw-   0        0        0     4712 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/html/_static/sphinx_highlight.js
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:06.147313 Dowell Mail-1.0.1/docs/_build/html/_static/stylesheets/
--rw-rw-rw-   0        0        0     9808 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/stylesheets/application-fixes.css
--rw-rw-rw-   0        0        0    43675 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/stylesheets/application-palette.css
--rw-rw-rw-   0        0        0    88621 2023-06-22 08:14:22.000000 Dowell Mail-1.0.1/docs/_build/html/_static/stylesheets/application.css
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:06.153342 Dowell Mail-1.0.1/docs/_build/html/css/
--rw-rw-rw-   0        0        0     2055 2023-06-13 09:55:15.000000 Dowell Mail-1.0.1/docs/_build/html/css/styles.css
--rw-rw-rw-   0        0        0    14649 2023-06-22 08:14:59.000000 Dowell Mail-1.0.1/docs/_build/html/emailapp.html
--rw-rw-rw-   0        0        0    15947 2023-06-22 09:47:54.000000 Dowell Mail-1.0.1/docs/_build/html/genindex.html
--rw-rw-rw-   0        0        0    13129 2023-06-22 09:47:54.000000 Dowell Mail-1.0.1/docs/_build/html/index.html
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:06.157330 Dowell Mail-1.0.1/docs/_build/html/maillib/
--rw-rw-rw-   0        0        0     1232 2023-06-14 09:48:36.000000 Dowell Mail-1.0.1/docs/_build/html/maillib/home.html
--rw-rw-rw-   0        0        0    21545 2023-06-22 08:14:59.000000 Dowell Mail-1.0.1/docs/_build/html/maillib.html
--rw-rw-rw-   0        0        0    10119 2023-06-22 08:14:59.000000 Dowell Mail-1.0.1/docs/_build/html/maillib.migrations.html
--rw-rw-rw-   0        0        0    20731 2023-06-22 08:15:00.000000 Dowell Mail-1.0.1/docs/_build/html/maillib.tests.html
--rw-rw-rw-   0        0        0    13496 2023-06-22 09:47:54.000000 Dowell Mail-1.0.1/docs/_build/html/modules.html
--rw-rw-rw-   0        0        0      619 2023-06-22 09:47:55.000000 Dowell Mail-1.0.1/docs/_build/html/objects.inv
--rw-rw-rw-   0        0        0    12875 2023-06-22 09:47:54.000000 Dowell Mail-1.0.1/docs/_build/html/py-modindex.html
--rw-rw-rw-   0        0        0     9434 2023-06-22 09:47:54.000000 Dowell Mail-1.0.1/docs/_build/html/search.html
--rw-rw-rw-   0        0        0     9506 2023-06-22 09:47:55.000000 Dowell Mail-1.0.1/docs/_build/html/searchindex.js
--rw-rw-rw-   0        0        0    29089 2023-06-22 08:15:00.000000 Dowell Mail-1.0.1/docs/_build/html/static.html
--rw-rw-rw-   0        0        0    13060 2023-06-22 08:15:00.000000 Dowell Mail-1.0.1/docs/_build/html/templates.html
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:06.339508 Dowell Mail-1.0.1/docs/_build/latex/
--rw-rw-rw-   0        0        0     4366 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/LICRcyr2utf8.xdy
--rw-rw-rw-   0        0        0    10188 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/LICRlatin2utf8.xdy
--rw-rw-rw-   0        0        0    18890 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/LatinRules.xdy
--rw-rw-rw-   0        0        0     2416 2023-06-22 10:29:44.000000 Dowell Mail-1.0.1/docs/_build/latex/Makefile
--rw-rw-rw-   0        0        0    16376 2023-06-22 08:19:00.000000 Dowell Mail-1.0.1/docs/_build/latex/dowell-mail.tex
--rw-rw-rw-   0        0        0      705 2023-06-22 10:29:44.000000 Dowell Mail-1.0.1/docs/_build/latex/latexmkjarc
--rw-rw-rw-   0        0        0      413 2023-06-22 10:29:44.000000 Dowell Mail-1.0.1/docs/_build/latex/latexmkrc
--rwxrwxrwx   0        0        0      503 2023-06-22 10:29:44.000000 Dowell Mail-1.0.1/docs/_build/latex/make.bat
--rw-rw-rw-   0        0        0      392 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/python.ist
--rw-rw-rw-   0        0        0    44560 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinx.sty
--rw-rw-rw-   0        0        0     9474 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinx.xdy
--rw-rw-rw-   0        0        0     7619 2023-06-22 10:29:44.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxhighlight.sty
--rw-rw-rw-   0        0        0     3256 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxhowto.cls
--rw-rw-rw-   0        0        0    10989 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexadmonitions.sty
--rw-rw-rw-   0        0        0      901 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexcontainers.sty
--rw-rw-rw-   0        0        0     4840 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexgraphics.sty
--rw-rw-rw-   0        0        0     2066 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexindbibtoc.sty
--rw-rw-rw-   0        0        0     5139 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexlists.sty
--rw-rw-rw-   0        0        0    46048 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexliterals.sty
--rw-rw-rw-   0        0        0     4532 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexnumfig.sty
--rw-rw-rw-   0        0        0     9067 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexobjects.sty
--rw-rw-rw-   0        0        0     5066 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexshadowbox.sty
--rw-rw-rw-   0        0        0     3445 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexstyleheadings.sty
--rw-rw-rw-   0        0        0     3064 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexstylepage.sty
--rw-rw-rw-   0        0        0     8232 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexstyletext.sty
--rw-rw-rw-   0        0        0    57830 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxlatextables.sty
--rw-rw-rw-   0        0        0     4241 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxmanual.cls
--rw-rw-rw-   0        0        0      765 2023-06-22 10:29:44.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxmessages.sty
--rw-rw-rw-   0        0        0     2061 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxoptionsgeometry.sty
--rw-rw-rw-   0        0        0     1094 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxoptionshyperref.sty
--rw-rw-rw-   0        0        0    36615 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxpackageboxes.sty
--rw-rw-rw-   0        0        0     2590 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxpackagecyrillic.sty
--rw-rw-rw-   0        0        0    15254 2023-06-20 09:37:25.000000 Dowell Mail-1.0.1/docs/_build/latex/sphinxpackagefootnote.sty
--rw-rw-rw-   0        0        0     1464 2023-06-22 09:50:58.000000 Dowell Mail-1.0.1/docs/conf.py
--rw-rw-rw-   0        0        0      739 2023-06-22 06:25:18.000000 Dowell Mail-1.0.1/docs/emailapp.rst
--rw-rw-rw-   0        0        0     1770 2023-06-22 08:11:35.000000 Dowell Mail-1.0.1/docs/index.rst
--rw-rw-rw-   0        0        0      187 2023-06-22 06:25:19.000000 Dowell Mail-1.0.1/docs/maillib.migrations.rst
--rw-rw-rw-   0        0        0      961 2023-06-22 06:25:19.000000 Dowell Mail-1.0.1/docs/maillib.rst
--rw-rw-rw-   0        0        0      537 2023-06-22 06:25:19.000000 Dowell Mail-1.0.1/docs/maillib.tests.rst
--rwxrwxrwx   0        0        0      800 2023-06-22 06:23:19.000000 Dowell Mail-1.0.1/docs/make.bat
--rw-rw-rw-   0        0        0      116 2023-06-22 06:33:29.000000 Dowell Mail-1.0.1/docs/modules.rst
--rw-rw-rw-   0        0        0     2613 2023-06-22 08:09:28.000000 Dowell Mail-1.0.1/docs/static.rst
--rw-rw-rw-   0        0        0     1588 2023-06-22 08:10:07.000000 Dowell Mail-1.0.1/docs/templates.rst
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:06.391600 Dowell Mail-1.0.1/maillib/
--rw-rw-rw-   0        0        0        0 2023-06-12 14:04:27.000000 Dowell Mail-1.0.1/maillib/__init__.py
--rw-rw-rw-   0        0        0       66 2023-06-12 14:04:27.000000 Dowell Mail-1.0.1/maillib/admin.py
--rw-rw-rw-   0        0        0      152 2023-06-12 14:04:28.000000 Dowell Mail-1.0.1/maillib/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:06.396595 Dowell Mail-1.0.1/maillib/migrations/
--rw-rw-rw-   0        0        0        0 2023-06-12 14:04:27.000000 Dowell Mail-1.0.1/maillib/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2023-06-12 14:04:27.000000 Dowell Mail-1.0.1/maillib/models.py
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:06.409598 Dowell Mail-1.0.1/maillib/tests/
--rw-rw-rw-   0        0        0        0 2023-06-14 13:01:00.000000 Dowell Mail-1.0.1/maillib/tests/__init__.py
--rw-rw-rw-   0        0        0      570 2023-06-20 07:59:06.000000 Dowell Mail-1.0.1/maillib/tests/test_urls.py
--rw-rw-rw-   0        0        0     3531 2023-06-21 06:39:18.000000 Dowell Mail-1.0.1/maillib/tests/test_views.py
--rw-rw-rw-   0        0        0      735 2023-06-21 06:37:21.000000 Dowell Mail-1.0.1/maillib/urls.py
--rw-rw-rw-   0        0        0     3323 2023-06-21 07:15:46.000000 Dowell Mail-1.0.1/maillib/views.py
--rw-rw-rw-   0        0        0      879 2023-06-26 11:26:06.435593 Dowell Mail-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      288 2023-06-26 09:34:46.000000 Dowell Mail-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.236178 Dowell Mail-1.0.1/static/
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:06.415591 Dowell Mail-1.0.1/static/css/
--rw-rw-rw-   0        0        0     2055 2023-06-13 09:55:15.000000 Dowell Mail-1.0.1/static/css/styles.css
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:04.239175 Dowell Mail-1.0.1/templates/
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:06.423595 Dowell Mail-1.0.1/templates/_partials/
--rw-rw-rw-   0        0        0      548 2023-06-13 06:52:16.000000 Dowell Mail-1.0.1/templates/_partials/base.html
--rw-rw-rw-   0        0        0      164 2023-06-13 09:58:30.000000 Dowell Mail-1.0.1/templates/_partials/messages.html
-drwxrwxrwx   0        0        0        0 2023-06-26 11:26:06.426589 Dowell Mail-1.0.1/templates/maillib/
--rw-rw-rw-   0        0        0     1232 2023-06-14 09:48:36.000000 Dowell Mail-1.0.1/templates/maillib/home.html
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:25.257910 Dowell Mail-1.0.2/
+-rw-rw-rw-   0        0        0       48 2023-06-26 10:57:39.000000 Dowell Mail-1.0.2/.env
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.456519 Dowell Mail-1.0.2/Dowell_Mail.egg-info/
+-rw-rw-rw-   0        0        0     2268 2023-06-26 11:30:21.000000 Dowell Mail-1.0.2/Dowell_Mail.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    19570 2023-06-26 11:30:21.000000 Dowell Mail-1.0.2/Dowell_Mail.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 11:30:21.000000 Dowell Mail-1.0.2/Dowell_Mail.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-26 11:30:21.000000 Dowell Mail-1.0.2/Dowell_Mail.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-26 11:30:21.000000 Dowell Mail-1.0.2/Dowell_Mail.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-15 09:01:20.000000 Dowell Mail-1.0.2/LICENCE
+-rw-rw-rw-   0        0        0    11558 2023-06-15 09:38:08.000000 Dowell Mail-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      134 2023-06-21 07:35:05.000000 Dowell Mail-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2268 2023-06-26 11:30:25.258927 Dowell Mail-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1564 2023-06-26 10:08:12.000000 Dowell Mail-1.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.580110 Dowell Mail-1.0.2/docs/
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.610118 Dowell Mail-1.0.2/docs/.git/
+-rw-rw-rw-   0        0        0        5 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/COMMIT_EDITMSG
+-rw-rw-rw-   0        0        0        0 2023-06-25 15:56:50.000000 Dowell Mail-1.0.2/docs/.git/FETCH_HEAD
+-rw-rw-rw-   0        0        0       21 2023-06-22 10:20:29.000000 Dowell Mail-1.0.2/docs/.git/HEAD
+-rw-rw-rw-   0        0        0      294 2023-06-22 10:20:54.000000 Dowell Mail-1.0.2/docs/.git/config
+-rw-rw-rw-   0        0        0       73 2023-06-22 10:18:28.000000 Dowell Mail-1.0.2/docs/.git/description
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.665703 Dowell Mail-1.0.2/docs/.git/hooks/
+-rw-rw-rw-   0        0        0      478 2023-06-22 10:18:28.000000 Dowell Mail-1.0.2/docs/.git/hooks/applypatch-msg.sample
+-rw-rw-rw-   0        0        0      896 2023-06-22 10:18:28.000000 Dowell Mail-1.0.2/docs/.git/hooks/commit-msg.sample
+-rw-rw-rw-   0        0        0     4726 2023-06-22 10:18:28.000000 Dowell Mail-1.0.2/docs/.git/hooks/fsmonitor-watchman.sample
+-rw-rw-rw-   0        0        0      189 2023-06-22 10:18:28.000000 Dowell Mail-1.0.2/docs/.git/hooks/post-update.sample
+-rw-rw-rw-   0        0        0      424 2023-06-22 10:18:28.000000 Dowell Mail-1.0.2/docs/.git/hooks/pre-applypatch.sample
+-rw-rw-rw-   0        0        0     1643 2023-06-22 10:18:28.000000 Dowell Mail-1.0.2/docs/.git/hooks/pre-commit.sample
+-rw-rw-rw-   0        0        0      416 2023-06-22 10:18:28.000000 Dowell Mail-1.0.2/docs/.git/hooks/pre-merge-commit.sample
+-rw-rw-rw-   0        0        0     1374 2023-06-22 10:18:28.000000 Dowell Mail-1.0.2/docs/.git/hooks/pre-push.sample
+-rw-rw-rw-   0        0        0     4898 2023-06-22 10:18:28.000000 Dowell Mail-1.0.2/docs/.git/hooks/pre-rebase.sample
+-rw-rw-rw-   0        0        0      544 2023-06-22 10:18:28.000000 Dowell Mail-1.0.2/docs/.git/hooks/pre-receive.sample
+-rw-rw-rw-   0        0        0     1492 2023-06-22 10:18:28.000000 Dowell Mail-1.0.2/docs/.git/hooks/prepare-commit-msg.sample
+-rw-rw-rw-   0        0        0     2783 2023-06-22 10:18:28.000000 Dowell Mail-1.0.2/docs/.git/hooks/push-to-checkout.sample
+-rw-rw-rw-   0        0        0     3650 2023-06-22 10:18:28.000000 Dowell Mail-1.0.2/docs/.git/hooks/update.sample
+-rw-rw-rw-   0        0        0    18730 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/index
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.669696 Dowell Mail-1.0.2/docs/.git/info/
+-rw-rw-rw-   0        0        0      240 2023-06-22 10:18:28.000000 Dowell Mail-1.0.2/docs/.git/info/exclude
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.672700 Dowell Mail-1.0.2/docs/.git/logs/
+-rw-rw-rw-   0        0        0      528 2023-06-22 10:20:29.000000 Dowell Mail-1.0.2/docs/.git/logs/HEAD
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.044204 Dowell Mail-1.0.2/docs/.git/logs/refs/
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.677699 Dowell Mail-1.0.2/docs/.git/logs/refs/heads/
+-rw-rw-rw-   0        0        0      342 2023-06-22 10:20:29.000000 Dowell Mail-1.0.2/docs/.git/logs/refs/heads/main
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.045206 Dowell Mail-1.0.2/docs/.git/logs/refs/remotes/
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.682697 Dowell Mail-1.0.2/docs/.git/logs/refs/remotes/origin/
+-rw-rw-rw-   0        0        0      301 2023-06-22 11:01:05.000000 Dowell Mail-1.0.2/docs/.git/logs/refs/remotes/origin/main
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.332308 Dowell Mail-1.0.2/docs/.git/objects/
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.688705 Dowell Mail-1.0.2/docs/.git/objects/02/
+-r--r--r--   0        0        0      163 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/02/8394883bc0686c6ec4bbdccea9a0a7d0c90032
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.699733 Dowell Mail-1.0.2/docs/.git/objects/07/
+-r--r--r--   0        0        0      282 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/07/7ae5076f0cd15403d754ec6299b4537e669d50
+-r--r--r--   0        0        0     3278 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/07/8d0cab706bad2c6548af839fe50f89ff29011d
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.706748 Dowell Mail-1.0.2/docs/.git/objects/0a/
+-r--r--r--   0        0        0     6683 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/0a/cc10571f6e2635820e7dee824d79b24eb64082
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.715698 Dowell Mail-1.0.2/docs/.git/objects/0b/
+-r--r--r--   0        0        0      135 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/0b/188f70f06269071481ceb5277c57ceed6de79b
+-r--r--r--   0        0        0     3482 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/0b/efce938f1e8e31e8b131fba92285e7cbde0492
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.722706 Dowell Mail-1.0.2/docs/.git/objects/0d/
+-r--r--r--   0        0        0     3150 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/0d/cf1133cd7b82c81d790bd3b165e4bef0497364
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.751723 Dowell Mail-1.0.2/docs/.git/objects/11/
+-r--r--r--   0        0        0     4843 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/11/bba08eb15c8676a59416cae5c3224032806b36
+-r--r--r--   0        0        0     1408 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/11/c9a999490dace18f6121e568c0190ecb04ca33
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.843283 Dowell Mail-1.0.2/docs/.git/objects/14/
+-r--r--r--   0        0        0      888 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/14/b9b602f01362269bf04515443533242bd13f11
+-r--r--r--   0        0        0      228 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/14/ff25cbaa43706124f10599f0dd07b08c0be525
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.850319 Dowell Mail-1.0.2/docs/.git/objects/15/
+-r--r--r--   0        0        0     2292 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/15/29892c823dfa8800da280360a0876cb8627834
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.856889 Dowell Mail-1.0.2/docs/.git/objects/17/
+-r--r--r--   0        0        0   168989 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/17/9792ab7540071599ca06538c571372d3788fb6
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.863886 Dowell Mail-1.0.2/docs/.git/objects/18/
+-r--r--r--   0        0        0      690 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/18/522369860ece5164ab3f845d63ea18fc77b080
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.866889 Dowell Mail-1.0.2/docs/.git/objects/1b/
+-r--r--r--   0        0        0      321 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/1b/f8c0e8bc6384f8c4fbf8d00171a407e9102ed2
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.916887 Dowell Mail-1.0.2/docs/.git/objects/1d/
+-r--r--r--   0        0        0     2593 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/1d/768259cdbc1200244462dcd508e120087972fb
+-r--r--r--   0        0        0      478 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/1d/9fffa74fbf58a10a208a481f16e53334db805f
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.920889 Dowell Mail-1.0.2/docs/.git/objects/1e/
+-r--r--r--   0        0        0      490 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/1e/041805e32525ba3483b99c85ce110855d782c7
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.968474 Dowell Mail-1.0.2/docs/.git/objects/23/
+-r--r--r--   0        0        0    14122 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/23/3c46dbc9802fafa8b32ec4edc4a04e9c237c99
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.974529 Dowell Mail-1.0.2/docs/.git/objects/25/
+-r--r--r--   0        0        0     1622 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/25/0f5665fa64b70c822190199b3b804b10f8b9d8
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.985476 Dowell Mail-1.0.2/docs/.git/objects/27/
+-r--r--r--   0        0        0     2113 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/27/3f4ad0beb8fba582b1e2390c2b7e9d406020a1
+-r--r--r--   0        0        0    22495 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/27/6506ff833411e7a32ec5a0d0b6b4138c910b97
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.989505 Dowell Mail-1.0.2/docs/.git/objects/29/
+-r--r--r--   0        0        0      482 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/29/8de27ef0fbefbcda3c2d319a132b9654736d0f
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.994472 Dowell Mail-1.0.2/docs/.git/objects/2a/
+-r--r--r--   0        0        0       58 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/2a/924f1d6a8bc930c5296bdb2d5c2d3e39b04a1c
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.003481 Dowell Mail-1.0.2/docs/.git/objects/2b/
+-r--r--r--   0        0        0      630 2023-06-22 11:01:05.000000 Dowell Mail-1.0.2/docs/.git/objects/2b/d90b52fd5e09963e064b660f9efb4752333a94
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.011476 Dowell Mail-1.0.2/docs/.git/objects/2e/
+-r--r--r--   0        0        0     1848 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/2e/4b30d921c3343a19744726882b85cdf3621f5c
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.034476 Dowell Mail-1.0.2/docs/.git/objects/2f/
+-r--r--r--   0        0        0      135 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/2f/1ed6f82ef1d10c599420be3cd798ecce38578e
+-r--r--r--   0        0        0     2854 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/2f/9bf5aebdb39583df031edacfc61c32f399c4b8
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.041501 Dowell Mail-1.0.2/docs/.git/objects/31/
+-r--r--r--   0        0        0      913 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/31/f32feb95e4c90d013340e6a8b94d5a6a2392b5
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.049526 Dowell Mail-1.0.2/docs/.git/objects/32/
+-r--r--r--   0        0        0      181 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/32/6cf15faea93280cfebbb125e4598d6a694e8c7
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.094072 Dowell Mail-1.0.2/docs/.git/objects/34/
+-r--r--r--   0        0        0       88 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/34/0b279b985c1f6a993dd3876c8997ce60aa51c8
+-r--r--r--   0        0        0      186 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/34/8ec444d138f860514e20617e7637ad6e6eebfa
+-r--r--r--   0        0        0     1692 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/34/910dfe5faba7f2cd385dca52906898127628be
+-r--r--r--   0        0        0       55 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/34/ddc3897cbf4c8094ebd05a1b8118fc90dcf27e
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.113093 Dowell Mail-1.0.2/docs/.git/objects/35/
+-r--r--r--   0        0        0   104197 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/35/acda2fa1196aad98c2adf4378a7611dd713aa3
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.120074 Dowell Mail-1.0.2/docs/.git/objects/36/
+-r--r--r--   0        0        0     3225 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/36/eaf6a0450c5a150834345972b6eff6dc20b63c
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.126075 Dowell Mail-1.0.2/docs/.git/objects/3a/
+-r--r--r--   0        0        0    16687 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/3a/73a76619e39b9d73f4e9610e60f54d6f999750
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.135074 Dowell Mail-1.0.2/docs/.git/objects/3d/
+-r--r--r--   0        0        0      527 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/3d/13b1975139abbb5a4bcc84e6bfff7cd57a4d51
+-r--r--r--   0        0        0     1842 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/3d/156b9c191cd246879a67c56e46baa4cfb2e17d
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.145090 Dowell Mail-1.0.2/docs/.git/objects/40/
+-r--r--r--   0        0        0    97946 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/40/0014a4b06eee3d0c0d54402a47ab2601b2862b
+-r--r--r--   0        0        0     1313 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/40/66129bf24ca86c1eb0cb8cf55f8730b92ca4d8
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.156668 Dowell Mail-1.0.2/docs/.git/objects/45/
+-r--r--r--   0        0        0      639 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/45/842b115c602827007d69ecbcaf308511340cdb
+-r--r--r--   0        0        0     9208 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/45/bffe09237d6f691365be13b11c8c205a4f35f5
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.159665 Dowell Mail-1.0.2/docs/.git/objects/48/
+-r--r--r--   0        0        0      621 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/48/8c29664e6a0160871b70a81c597df7a0a5b276
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.167686 Dowell Mail-1.0.2/docs/.git/objects/4a/
+-r--r--r--   0        0        0    16617 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/4a/bdd66d1abde1e9465c471010d0c1056af9c682
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.180689 Dowell Mail-1.0.2/docs/.git/objects/4b/
+-r--r--r--   0        0        0       15 2023-06-22 10:19:51.000000 Dowell Mail-1.0.2/docs/.git/objects/4b/825dc642cb6eb9a060e54bf8d69288fbee4904
+-r--r--r--   0        0        0      238 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/4b/9549be9b37c5e68c14034988c0557bab76d4de
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.186671 Dowell Mail-1.0.2/docs/.git/objects/4c/
+-r--r--r--   0        0        0     2390 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/4c/4e6fd4fcc67b9fa4cd695b9023ac9e66d91904
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.195667 Dowell Mail-1.0.2/docs/.git/objects/4d/
+-r--r--r--   0        0        0    77179 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/4d/13fc60404b91e398a37200c4a77b645cfd9586
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.202666 Dowell Mail-1.0.2/docs/.git/objects/4f/
+-r--r--r--   0        0        0     3078 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/4f/60d46a956924a94f68b4725075fe3d1191edf7
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.208667 Dowell Mail-1.0.2/docs/.git/objects/50/
+-r--r--r--   0        0        0     3334 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/50/dddaa04b87af93b515dd6b33d32d0040254307
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.214672 Dowell Mail-1.0.2/docs/.git/objects/51/
+-r--r--r--   0        0        0     3234 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/51/7d0b29cb1193b1211c8853b58c65cddd1fa4d2
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.232666 Dowell Mail-1.0.2/docs/.git/objects/52/
+-r--r--r--   0        0        0     3182 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/52/15595b510b67b720091544ea1a4eccb4722381
+-r--r--r--   0        0        0     2230 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/52/632004a2414fe4aee1cf9f85696d0ae66eaa3e
+-r--r--r--   0        0        0     5473 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/52/ec8be7e6cc2123f25079e19a6dfadd89d8b69d
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.237668 Dowell Mail-1.0.2/docs/.git/objects/54/
+-r--r--r--   0        0        0     1097 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/54/430761163f1a6478239ae68eb9a2b8b0d3506e
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.248686 Dowell Mail-1.0.2/docs/.git/objects/55/
+-r--r--r--   0        0        0     5077 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/55/901234df171e819e5ab726ebe9eb3acc25dada
+-r--r--r--   0        0        0     1272 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/55/fd4172c46835b24bc52edecb319a02e5652963
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.254680 Dowell Mail-1.0.2/docs/.git/objects/56/
+-r--r--r--   0        0        0     3029 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/56/a4b0dc19f7c9e8b8423e544ed5e80fbb92abd7
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.267275 Dowell Mail-1.0.2/docs/.git/objects/57/
+-r--r--r--   0        0        0     3889 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/57/36305299fc9615b7b91c6778cb365be4e9ccfc
+-r--r--r--   0        0        0     1567 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/57/eaee2f2272d9755e1dc69179e8e219050c6905
+-r--r--r--   0        0        0       36 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/57/ef03f24a4351df334da53af3b9161bdeac6b1b
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.273294 Dowell Mail-1.0.2/docs/.git/objects/58/
+-r--r--r--   0        0        0      639 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/58/40c3bbf9dd7b0b27c6a977d843940b09ae8c54
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.279276 Dowell Mail-1.0.2/docs/.git/objects/59/
+-r--r--r--   0        0        0     3535 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/59/161a19db9a40ae6b96ede4cf7213570db3de9a
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.284275 Dowell Mail-1.0.2/docs/.git/objects/5a/
+-r--r--r--   0        0        0     1156 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/5a/354d3c77dd2d04ceb0cd61592c0a1a848ba355
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.288281 Dowell Mail-1.0.2/docs/.git/objects/5d/
+-r--r--r--   0        0        0     3768 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/5d/ea4a6e8da2f6ce6e06acec0e2662be88b5374f
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.293276 Dowell Mail-1.0.2/docs/.git/objects/5e/
+-r--r--r--   0        0        0     4254 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/5e/adc1c5b64a06531d4125561cc513c8fb4ab37d
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.298296 Dowell Mail-1.0.2/docs/.git/objects/5f/
+-r--r--r--   0        0        0      308 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/5f/a22e886b899683ce5de581fa0b7fcdc1cdc963
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.306280 Dowell Mail-1.0.2/docs/.git/objects/63/
+-r--r--r--   0        0        0      506 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/63/130b01203f39a74b75f1ed082d2fca18a38e40
+-r--r--r--   0        0        0       88 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/63/7351746cccdf6b5c72dd2b99f2a1d5b99e7252
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.310277 Dowell Mail-1.0.2/docs/.git/objects/64/
+-r--r--r--   0        0        0     3145 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/64/808af3c3ac606f310b83f68ee9cfee8dbc8b03
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.323296 Dowell Mail-1.0.2/docs/.git/objects/68/
+-r--r--r--   0        0        0       58 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/68/08d6b4bc94c19e336620efbd95c0ebaa9889c9
+-r--r--r--   0        0        0       93 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/68/8881b021f72eb69eaef8c7cb7c7bc5a9a138ce
+-r--r--r--   0        0        0      350 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/68/ebffa887dfb5a0ee10257bd15e1d73f54ff3c1
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.326274 Dowell Mail-1.0.2/docs/.git/objects/69/
+-r--r--r--   0        0        0     1162 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/69/f620250d95bc3982dd8a6bd46689759a54c2a3
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.331277 Dowell Mail-1.0.2/docs/.git/objects/6c/
+-r--r--r--   0        0        0    14545 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/6c/31f329c658b01ae8b2c10194e09ed1a72f4f31
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.341316 Dowell Mail-1.0.2/docs/.git/objects/6d/
+-r--r--r--   0        0        0     1376 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/6d/72961051eba439a573224713613f34beebe7d5
+-r--r--r--   0        0        0     1689 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/6d/af5f9d807ec44fb0cfba836a21c17dd888f8da
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.346332 Dowell Mail-1.0.2/docs/.git/objects/6e/
+-r--r--r--   0        0        0      426 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/6e/36b195b2d3083c18c06bafa280ce86729aa546
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.358866 Dowell Mail-1.0.2/docs/.git/objects/70/
+-r--r--r--   0        0        0    66198 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/70/15564ad166a3e9d88c82f17829f0cc01ebe29a
+-r--r--r--   0        0        0      199 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/70/536a6683577925167e84e0b0f6a06228754d0a
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.366853 Dowell Mail-1.0.2/docs/.git/objects/71/
+-r--r--r--   0        0        0       99 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/71/07cec93a979b9a5f64843235a16651d563ce2d
+-r--r--r--   0        0        0      376 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/71/2b8e7d89c0ac96a45eea729077ebc287f3a89d
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.378858 Dowell Mail-1.0.2/docs/.git/objects/75/
+-r--r--r--   0        0        0     1267 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/75/45ea35e0a5df26e09aa3b4834e736ab191aac6
+-r--r--r--   0        0        0     4210 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/75/77acb1ad176e3f58c15ddf9bf1f73525dfe7ed
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.384861 Dowell Mail-1.0.2/docs/.git/objects/76/
+-r--r--r--   0        0        0      541 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/76/d17f57ad903c3ea2f1b564cafb95bf9af84ee3
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.395880 Dowell Mail-1.0.2/docs/.git/objects/77/
+-r--r--r--   0        0        0      904 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/77/9d5dd47a5022001209f9c9f935a9c2dde5eebd
+-r--r--r--   0        0        0     3947 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/77/ad846085e4e2576ca5157789b70c9e24dc24d0
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.401881 Dowell Mail-1.0.2/docs/.git/objects/79/
+-r--r--r--   0        0        0      931 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/79/e30a1f1999c22b29515767c063825cc39c58dd
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.408917 Dowell Mail-1.0.2/docs/.git/objects/7b/
+-r--r--r--   0        0        0      388 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/7b/97197e91ce7488eb13f3749849f953bd5cb9aa
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.414852 Dowell Mail-1.0.2/docs/.git/objects/7c/
+-r--r--r--   0        0        0    31919 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/7c/724d2e4f2d39cb2e418936f0fdf0198bd118a0
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.425897 Dowell Mail-1.0.2/docs/.git/objects/7d/
+-r--r--r--   0        0        0      746 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/7d/1e8c2f1bbc45869b92d703be845f6eb20ebd0a
+-r--r--r--   0        0        0    64098 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/7d/86eb1694970141b88b52f5b26e6b019f16b590
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.432853 Dowell Mail-1.0.2/docs/.git/objects/7e/
+-r--r--r--   0        0        0       52 2023-06-22 11:01:05.000000 Dowell Mail-1.0.2/docs/.git/objects/7e/953140f053cc0bf5f0b2da0b762b99dc8811e2
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.437880 Dowell Mail-1.0.2/docs/.git/objects/80/
+-r--r--r--   0        0        0     4111 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/80/f9d49c9bd4d7d58996254dee424b25d3164ef6
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.446966 Dowell Mail-1.0.2/docs/.git/objects/83/
+-r--r--r--   0        0        0      185 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/83/4412e5f09537af46dc5026c4510b651c641831
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.543602 Dowell Mail-1.0.2/docs/.git/objects/85/
+-r--r--r--   0        0        0     5711 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/85/e59c4ac73dcfde98d34e848b5c99b7714d33ae
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.547621 Dowell Mail-1.0.2/docs/.git/objects/86/
+-r--r--r--   0        0        0      125 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/86/b7198fc951b7bfdf0a41e29877d9829b39f9b8
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.551613 Dowell Mail-1.0.2/docs/.git/objects/89/
+-r--r--r--   0        0        0     1257 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/89/9804d75f317500aab85d5dd773814026a7e48c
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.557144 Dowell Mail-1.0.2/docs/.git/objects/8a/
+-r--r--r--   0        0        0      415 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/8a/145c9117e791bbd0c472ee442cb74a90888656
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.560152 Dowell Mail-1.0.2/docs/.git/objects/8d/
+-r--r--r--   0        0        0     1516 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/8d/7dd0ee7185687b4404c3e0480b20e1ed0fd4eb
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.564149 Dowell Mail-1.0.2/docs/.git/objects/8e/
+-r--r--r--   0        0        0     1971 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/8e/793555684ac8caa28b91a17d26502b51629732
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.572149 Dowell Mail-1.0.2/docs/.git/objects/8f/
+-r--r--r--   0        0        0     4175 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/8f/99b2771e10cbb806d18c35ce3bfce1eda46dcd
+-r--r--r--   0        0        0     1578 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/8f/c9926ef0fa53320bc485118f7a870a19eda8db
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.575144 Dowell Mail-1.0.2/docs/.git/objects/91/
+-r--r--r--   0        0        0     3023 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/91/3bc8210a6a2156fc818eef2d545e8b0871a518
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.580149 Dowell Mail-1.0.2/docs/.git/objects/93/
+-r--r--r--   0        0        0      447 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/93/b2c8c086a53e63f7e906241a07198b2ff073bb
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.584147 Dowell Mail-1.0.2/docs/.git/objects/94/
+-r--r--r--   0        0        0      298 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/94/bda2139156340fc42bb1cb678e49ac9ac8d3c6
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.590149 Dowell Mail-1.0.2/docs/.git/objects/95/
+-r--r--r--   0        0        0      438 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/95/4237b9b9f2b248bb1397a15c055c0af1cad03e
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.594150 Dowell Mail-1.0.2/docs/.git/objects/97/
+-r--r--r--   0        0        0     6728 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/97/d56a74d8207ec36a96a5e24f4a4b42dd51f6b2
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.601151 Dowell Mail-1.0.2/docs/.git/objects/9a/
+-r--r--r--   0        0        0     1388 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/9a/a62fc22baa68906867164da4d6819dfaf72907
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.608162 Dowell Mail-1.0.2/docs/.git/objects/9d/
+-r--r--r--   0        0        0     3490 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/9d/e6c09cb4238addb63e4a63a54bdf83b6c8d6ff
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.621176 Dowell Mail-1.0.2/docs/.git/objects/9e/
+-r--r--r--   0        0        0      436 2023-06-22 11:01:05.000000 Dowell Mail-1.0.2/docs/.git/objects/9e/13fc18a432ac279e1c31eb305c56bbb30602e4
+-r--r--r--   0        0        0    21654 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/9e/4453259d6929c2bf7b7b9a5d18c76a753c4d44
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.627147 Dowell Mail-1.0.2/docs/.git/objects/9f/
+-r--r--r--   0        0        0    44332 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/9f/a211252080046a23b2449dbdced6abc2b0bb34
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.635178 Dowell Mail-1.0.2/docs/.git/objects/a1/
+-r--r--r--   0        0        0     4038 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/a1/3b146a9a996aea5bc19af6bc48ac34579485a9
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.643182 Dowell Mail-1.0.2/docs/.git/objects/a2/
+-r--r--r--   0        0        0     2329 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/a2/a1a0e393e42392b8046793cf3361227432fe73
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.656721 Dowell Mail-1.0.2/docs/.git/objects/a3/
+-r--r--r--   0        0        0     4374 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/a3/1ae4ce3a2c809b63787b319c6ebc51df4dee6d
+-r--r--r--   0        0        0      166 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/a3/a633d83087f3d0384ca9c8c241f109f0f65414
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.662767 Dowell Mail-1.0.2/docs/.git/objects/a6/
+-r--r--r--   0        0        0     2022 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/a6/5d194b7adbb6fac28c1654cca5d0c165015377
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.668747 Dowell Mail-1.0.2/docs/.git/objects/a7/
+-r--r--r--   0        0        0      279 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/a7/f754b66f245c8342c8dfc42de1b439f620054f
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.675752 Dowell Mail-1.0.2/docs/.git/objects/a8/
+-r--r--r--   0        0        0      306 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/a8/58a410e4faa62ce324d814e4b816fff83a6fb3
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.686764 Dowell Mail-1.0.2/docs/.git/objects/a9/
+-r--r--r--   0        0        0      882 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/a9/ca1c82cd661cfa1583e86fa881644d029d061f
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.695762 Dowell Mail-1.0.2/docs/.git/objects/aa/
+-r--r--r--   0        0        0     1931 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/aa/e669d7ea6b1dc6edcb5c651f5d095f7a2dc6e6
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.702779 Dowell Mail-1.0.2/docs/.git/objects/ac/
+-r--r--r--   0        0        0     3408 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/ac/99248044a350007567ce177ba3e2ae286bef63
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.709741 Dowell Mail-1.0.2/docs/.git/objects/ad/
+-r--r--r--   0        0        0      960 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/ad/07dd68bddf8730f4584ed84fac8050473a6d95
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.720765 Dowell Mail-1.0.2/docs/.git/objects/af/
+-r--r--r--   0        0        0      124 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/af/094027a710f1671668ae6590d3bf21a9f08657
+-r--r--r--   0        0        0      912 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/af/5a804d593607e51ca637bebcbc9633f261691d
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.727774 Dowell Mail-1.0.2/docs/.git/objects/b0/
+-r--r--r--   0        0        0    11332 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/b0/d3707062fef1eb41d2e5ac63e09d48465e6bab
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.733752 Dowell Mail-1.0.2/docs/.git/objects/b1/
+-r--r--r--   0        0        0     3482 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/b1/9627e1b35eb0240db39497c70b509624c0da09
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.738748 Dowell Mail-1.0.2/docs/.git/objects/b2/
+-r--r--r--   0        0        0     2992 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/b2/0fbbb83a55f6286917183d07d549846b0b8ed9
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.749828 Dowell Mail-1.0.2/docs/.git/objects/b4/
+-r--r--r--   0        0        0     7881 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/b4/76b53e33b5789396e2b48d44c8abc07a037db3
+-r--r--r--   0        0        0     3755 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/b4/ff1f9d02d01ec10e3808971706542a6d0ec748
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.765420 Dowell Mail-1.0.2/docs/.git/objects/b5/
+-r--r--r--   0        0        0      428 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/b5/733ba707cd68b0929cea4d8e48c07b96ffe609
+-r--r--r--   0        0        0      855 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/b5/9cb4eb5ff374906c380579330c0fe36fa3cc88
+-r--r--r--   0        0        0     1493 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/b5/e9c8543653a3c7194b8f4879ef43646bc79c2e
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.776387 Dowell Mail-1.0.2/docs/.git/objects/b6/
+-r--r--r--   0        0        0    57629 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/b6/48a3eea2d16b6ce783906d6b7d5f251b9eb56c
+-r--r--r--   0        0        0    31169 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/b6/6df4ab09628c1dcce7f663a314e51332c64310
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.782395 Dowell Mail-1.0.2/docs/.git/objects/b8/
+-r--r--r--   0        0        0      570 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/b8/8f108df9a4d81e94bb8d0a3ecded420c9999f7
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.791392 Dowell Mail-1.0.2/docs/.git/objects/b9/
+-r--r--r--   0        0        0     2330 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/b9/b75fc0ea791147b7195473e733caee6e4fc31e
+-r--r--r--   0        0        0     4285 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/b9/f5723bd8733e425085e505dd100de2cf54c6cb
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.795399 Dowell Mail-1.0.2/docs/.git/objects/ba/
+-r--r--r--   0        0        0     2402 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/ba/a21647ca52c56d628adce41e076b5a837ae90d
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.806394 Dowell Mail-1.0.2/docs/.git/objects/bb/
+-r--r--r--   0        0        0      330 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/bb/1c0e9cea56d06c0ec25fad185924f814778ae4
+-r--r--r--   0        0        0      210 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/bb/a17fa6bc6aa2e1a0f08088b7bd685077463e8e
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.810387 Dowell Mail-1.0.2/docs/.git/objects/bc/
+-r--r--r--   0        0        0     2058 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/bc/fc55fb0b780383ae096b2b5a9b47eef30bcf81
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.816397 Dowell Mail-1.0.2/docs/.git/objects/c0/
+-r--r--r--   0        0        0       52 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/c0/55ebaf37a904fafc2815f4f8d0e810db0b0984
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.820401 Dowell Mail-1.0.2/docs/.git/objects/c1/
+-r--r--r--   0        0        0      405 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/c1/d165229552b8adb7f91199d8ab16524c28da7d
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.825405 Dowell Mail-1.0.2/docs/.git/objects/c4/
+-r--r--r--   0        0        0    36048 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/c4/c6022f2982e8dae64cebd6b9a2b59f2547faad
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.830394 Dowell Mail-1.0.2/docs/.git/objects/c5/
+-r--r--r--   0        0        0       87 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/c5/5299abe93533ce599c650aa2853e1bc422f7a4
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.834393 Dowell Mail-1.0.2/docs/.git/objects/c8/
+-r--r--r--   0        0        0      163 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/c8/d8fb540030e23b240ba39543609315056d8e6f
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.844411 Dowell Mail-1.0.2/docs/.git/objects/cc/
+-r--r--r--   0        0        0     3311 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/cc/1b794a9b9667f1a6600afc3b3fdce4ac649719
+-r--r--r--   0        0        0     1244 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/cc/a624a2ceebd47f7c807110d1e4669d88d7a11f
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.850455 Dowell Mail-1.0.2/docs/.git/objects/ce/
+-r--r--r--   0        0        0      639 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/ce/62404b61db8d0ba61bb34c7f4ae5d1fcc31ca1
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.854417 Dowell Mail-1.0.2/docs/.git/objects/cf/
+-r--r--r--   0        0        0      681 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/cf/58c14fbc67be0626eb95a0a8fc68baa8c2ac03
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.865086 Dowell Mail-1.0.2/docs/.git/objects/d0/
+-r--r--r--   0        0        0     1774 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/d0/6a71d7518041301a303697d2a3c372648eb7bf
+-r--r--r--   0        0        0     6146 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/d0/b4b7a096a9df7ca9e16e969b980e37c742149d
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.869040 Dowell Mail-1.0.2/docs/.git/objects/d2/
+-r--r--r--   0        0        0       86 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/d2/eb00277d21b14f5f831bccf0fb51c5cfa1e0a4
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.874112 Dowell Mail-1.0.2/docs/.git/objects/d4/
+-r--r--r--   0        0        0      367 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/d4/bb2cbb9eddb1bb1b4f366623044af8e4830919
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.878043 Dowell Mail-1.0.2/docs/.git/objects/d5/
+-r--r--r--   0        0        0      186 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/d5/d0aaa972d0bf29ca687bc2cd328f575b6d4cc0
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.884234 Dowell Mail-1.0.2/docs/.git/objects/d8/
+-r--r--r--   0        0        0     4371 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/d8/54b4aa71024fc8efb2f1e9fced00c21f57a2f3
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.889207 Dowell Mail-1.0.2/docs/.git/objects/d9/
+-r--r--r--   0        0        0       97 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/d9/6755fdaf8bb2214971e0db9c1fd3077d7c419d
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.894771 Dowell Mail-1.0.2/docs/.git/objects/e0/
+-r--r--r--   0        0        0      439 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/e0/9b6c0b00d3c7d31d0edb4e6384c756920b82c5
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.900764 Dowell Mail-1.0.2/docs/.git/objects/e1/
+-r--r--r--   0        0        0      178 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/e1/f6000458504acf1ac56d147e53512e058e9f73
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.904772 Dowell Mail-1.0.2/docs/.git/objects/e3/
+-r--r--r--   0        0        0       54 2023-06-22 11:01:05.000000 Dowell Mail-1.0.2/docs/.git/objects/e3/fad2dd6545c4627e88caefc23fcaed67c46251
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.909761 Dowell Mail-1.0.2/docs/.git/objects/e4/
+-r--r--r--   0        0        0     3386 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/e4/e95b864519c0acc98412378441c422cecba687
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.914768 Dowell Mail-1.0.2/docs/.git/objects/e5/
+-r--r--r--   0        0        0      116 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/e5/27a3089e20f9f4226e6c0df4a4d9dadb96a115
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.924781 Dowell Mail-1.0.2/docs/.git/objects/e7/
+-r--r--r--   0        0        0      561 2023-06-22 11:01:05.000000 Dowell Mail-1.0.2/docs/.git/objects/e7/996d8e3406e79a393e78cf8e9c553c4702f85b
+-r--r--r--   0        0        0     1460 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/e7/a7c1901ed4c6a32722f03d6d9a8c0ff5d55652
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.927761 Dowell Mail-1.0.2/docs/.git/objects/e8/
+-r--r--r--   0        0        0     3942 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/e8/fb5a7df64cf44eee42ab10ad6386bb57fa9e3d
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.933781 Dowell Mail-1.0.2/docs/.git/objects/e9/
+-r--r--r--   0        0        0      750 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/e9/63414845f850fffe51fa14893f6b67aed97731
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.938772 Dowell Mail-1.0.2/docs/.git/objects/ea/
+-r--r--r--   0        0        0      118 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/ea/ab363250d42b878741d17cda8d1355f5768dd5
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.943783 Dowell Mail-1.0.2/docs/.git/objects/ec/
+-r--r--r--   0        0        0      632 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/ec/314fea70f892ffd1dbd4a53add8891df3ca982
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.948799 Dowell Mail-1.0.2/docs/.git/objects/ed/
+-r--r--r--   0        0        0      294 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/ed/99102e8b03e4af6f450d884de4d98646b1c159
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.952781 Dowell Mail-1.0.2/docs/.git/objects/ee/
+-r--r--r--   0        0        0      529 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/ee/8ef373a0d0a4aa2609d7382d7b6bb605824fe6
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.957340 Dowell Mail-1.0.2/docs/.git/objects/f1/
+-r--r--r--   0        0        0      794 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/f1/f525a8375f9fc814afff69f587e2123226f9ae
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.962353 Dowell Mail-1.0.2/docs/.git/objects/f3/
+-r--r--r--   0        0        0     2856 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/f3/9f778b208dd9614d56b285b880f3697c15e709
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.967341 Dowell Mail-1.0.2/docs/.git/objects/f5/
+-r--r--r--   0        0        0     3000 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/f5/0fc9fa6d5a0f1a479676d9c0ab72c44125d08c
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.971393 Dowell Mail-1.0.2/docs/.git/objects/f7/
+-r--r--r--   0        0        0     1524 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/f7/18bb2f85762580330d3145e01b1aa4e01c51fd
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.982342 Dowell Mail-1.0.2/docs/.git/objects/f9/
+-r--r--r--   0        0        0       54 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/f9/053d8d4eabfa90b1b6cc2cf6da9616fbc96de4
+-r--r--r--   0        0        0      115 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/f9/06e654208eb66982d75b3a45c20db781a36303
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:23.990362 Dowell Mail-1.0.2/docs/.git/objects/fb/
+-r--r--r--   0        0        0     1216 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/fb/846534ac59ccbedb425076d96870627575f620
+-r--r--r--   0        0        0     2787 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/fb/a1ee45d9f9437f627343a4b66c0dfc59ebec0a
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.011340 Dowell Mail-1.0.2/docs/.git/objects/fd/
+-r--r--r--   0        0        0     1944 2023-06-22 10:20:06.000000 Dowell Mail-1.0.2/docs/.git/objects/fd/0aae6386addf84721ec0d5fec2e997013ec6bf
+-r--r--r--   0        0        0      212 2023-06-22 10:20:15.000000 Dowell Mail-1.0.2/docs/.git/objects/fd/53ed54ed8b90a7bbbe811a43518acf22c70ee4
+-r--r--r--   0        0        0     1336 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/fd/f3913755aa169c74990ca316dc8bd48a4bad55
+-r--r--r--   0        0        0      283 2023-06-22 10:20:05.000000 Dowell Mail-1.0.2/docs/.git/objects/fd/fc61dddbf6a74869da2ecf31879346149d532b
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.336310 Dowell Mail-1.0.2/docs/.git/refs/
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.017340 Dowell Mail-1.0.2/docs/.git/refs/heads/
+-rw-rw-rw-   0        0        0       41 2023-06-22 10:20:29.000000 Dowell Mail-1.0.2/docs/.git/refs/heads/main
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.337307 Dowell Mail-1.0.2/docs/.git/refs/remotes/
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.020348 Dowell Mail-1.0.2/docs/.git/refs/remotes/origin/
+-rw-rw-rw-   0        0        0       41 2023-06-22 11:01:05.000000 Dowell Mail-1.0.2/docs/.git/refs/remotes/origin/main
+-rw-rw-rw-   0        0        0      634 2023-06-22 06:23:19.000000 Dowell Mail-1.0.2/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.386868 Dowell Mail-1.0.2/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.064907 Dowell Mail-1.0.2/docs/_build/doctrees/
+-rw-rw-rw-   0        0        0    15009 2023-06-22 06:33:40.000000 Dowell Mail-1.0.2/docs/_build/doctrees/emailapp.doctree
+-rw-rw-rw-   0        0        0   148054 2023-06-22 10:29:44.000000 Dowell Mail-1.0.2/docs/_build/doctrees/environment.pickle
+-rw-rw-rw-   0        0        0     8345 2023-06-22 08:14:59.000000 Dowell Mail-1.0.2/docs/_build/doctrees/index.doctree
+-rw-rw-rw-   0        0        0    24405 2023-06-22 06:33:40.000000 Dowell Mail-1.0.2/docs/_build/doctrees/maillib.doctree
+-rw-rw-rw-   0        0        0     3057 2023-06-22 06:33:40.000000 Dowell Mail-1.0.2/docs/_build/doctrees/maillib.migrations.doctree
+-rw-rw-rw-   0        0        0    26023 2023-06-22 06:33:41.000000 Dowell Mail-1.0.2/docs/_build/doctrees/maillib.tests.doctree
+-rw-rw-rw-   0        0        0     2752 2023-06-22 10:29:44.000000 Dowell Mail-1.0.2/docs/_build/doctrees/modules.doctree
+-rw-rw-rw-   0        0        0     7115 2023-06-22 08:10:14.000000 Dowell Mail-1.0.2/docs/_build/doctrees/static.doctree
+-rw-rw-rw-   0        0        0     5517 2023-06-22 08:10:14.000000 Dowell Mail-1.0.2/docs/_build/doctrees/templates.doctree
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.141917 Dowell Mail-1.0.2/docs/_build/epub/
+-rw-rw-rw-   0        0        0      234 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/.buildinfo
+-rw-rw-rw-   0        0        0    23768 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/Dowell-Mail.epub
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.145920 Dowell Mail-1.0.2/docs/_build/epub/META-INF/
+-rw-rw-rw-   0        0        0      246 2023-06-20 09:37:24.000000 Dowell Mail-1.0.2/docs/_build/epub/META-INF/container.xml
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.153927 Dowell Mail-1.0.2/docs/_build/epub/_partials/
+-rw-rw-rw-   0        0        0      548 2023-06-13 06:52:16.000000 Dowell Mail-1.0.2/docs/_build/epub/_partials/base.html
+-rw-rw-rw-   0        0        0      164 2023-06-13 09:58:30.000000 Dowell Mail-1.0.2/docs/_build/epub/_partials/messages.html
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.207511 Dowell Mail-1.0.2/docs/_build/epub/_static/
+-rw-rw-rw-   0        0        0    15715 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/_static/basic.css
+-rw-rw-rw-   0        0        0     4472 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/epub/_static/doctools.js
+-rw-rw-rw-   0        0        0      433 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/_static/documentation_options.js
+-rw-rw-rw-   0        0        0    12897 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/_static/epub.css
+-rw-rw-rw-   0        0        0      286 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/epub/_static/file.png
+-rw-rw-rw-   0        0        0      339 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/epub/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/epub/_static/plus.png
+-rw-rw-rw-   0        0        0      539 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/_static/pygments.css
+-rw-rw-rw-   0        0        0    18215 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/epub/_static/searchtools.js
+-rw-rw-rw-   0        0        0     4712 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/epub/_static/sphinx_highlight.js
+-rw-rw-rw-   0        0        0     3153 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/content.opf
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.214518 Dowell Mail-1.0.2/docs/_build/epub/css/
+-rw-rw-rw-   0        0        0     2055 2023-06-13 09:55:15.000000 Dowell Mail-1.0.2/docs/_build/epub/css/styles.css
+-rw-rw-rw-   0        0        0     4011 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/emailapp.xhtml
+-rw-rw-rw-   0        0        0     7696 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/genindex.xhtml
+-rw-rw-rw-   0        0        0     3070 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/index.xhtml
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.218513 Dowell Mail-1.0.2/docs/_build/epub/maillib/
+-rw-rw-rw-   0        0        0     1232 2023-06-14 09:48:36.000000 Dowell Mail-1.0.2/docs/_build/epub/maillib/home.html
+-rw-rw-rw-   0        0        0      980 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/maillib.migrations.xhtml
+-rw-rw-rw-   0        0        0     6336 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/maillib.tests.xhtml
+-rw-rw-rw-   0        0        0     9108 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/maillib.xhtml
+-rw-rw-rw-   0        0        0       20 2023-06-20 09:37:24.000000 Dowell Mail-1.0.2/docs/_build/epub/mimetype
+-rw-rw-rw-   0        0        0     4996 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/modules.xhtml
+-rw-rw-rw-   0        0        0      630 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/nav.xhtml
+-rw-rw-rw-   0        0        0     4568 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/py-modindex.xhtml
+-rw-rw-rw-   0        0        0    19125 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/static.xhtml
+-rw-rw-rw-   0        0        0     4173 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/templates.xhtml
+-rw-rw-rw-   0        0        0      948 2023-06-22 09:51:37.000000 Dowell Mail-1.0.2/docs/_build/epub/toc.ncx
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.317099 Dowell Mail-1.0.2/docs/_build/html/
+-rw-rw-rw-   0        0        0      234 2023-06-22 09:47:55.000000 Dowell Mail-1.0.2/docs/_build/html/.buildinfo
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.321104 Dowell Mail-1.0.2/docs/_build/html/_modules/
+-rw-rw-rw-   0        0        0     9448 2023-06-22 09:47:54.000000 Dowell Mail-1.0.2/docs/_build/html/_modules/index.html
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.333104 Dowell Mail-1.0.2/docs/_build/html/_modules/maillib/
+-rw-rw-rw-   0        0        0     3285 2023-06-22 06:33:43.000000 Dowell Mail-1.0.2/docs/_build/html/_modules/maillib/apps.html
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.347113 Dowell Mail-1.0.2/docs/_build/html/_modules/maillib/tests/
+-rw-rw-rw-   0        0        0     4901 2023-06-22 06:33:43.000000 Dowell Mail-1.0.2/docs/_build/html/_modules/maillib/tests/test_urls.html
+-rw-rw-rw-   0        0        0    15316 2023-06-22 06:33:43.000000 Dowell Mail-1.0.2/docs/_build/html/_modules/maillib/tests/test_views.html
+-rw-rw-rw-   0        0        0    12282 2023-06-22 06:33:43.000000 Dowell Mail-1.0.2/docs/_build/html/_modules/maillib/views.html
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.366665 Dowell Mail-1.0.2/docs/_build/html/_partials/
+-rw-rw-rw-   0        0        0      548 2023-06-13 06:52:16.000000 Dowell Mail-1.0.2/docs/_build/html/_partials/base.html
+-rw-rw-rw-   0        0        0      164 2023-06-13 09:58:30.000000 Dowell Mail-1.0.2/docs/_build/html/_partials/messages.html
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.420691 Dowell Mail-1.0.2/docs/_build/html/_sources/
+-rw-rw-rw-   0        0        0      739 2023-06-22 06:25:18.000000 Dowell Mail-1.0.2/docs/_build/html/_sources/emailapp.rst.txt
+-rw-rw-rw-   0        0        0     1770 2023-06-22 08:05:11.000000 Dowell Mail-1.0.2/docs/_build/html/_sources/index.rst.txt
+-rw-rw-rw-   0        0        0      187 2023-06-22 06:25:19.000000 Dowell Mail-1.0.2/docs/_build/html/_sources/maillib.migrations.rst.txt
+-rw-rw-rw-   0        0        0      961 2023-06-22 06:25:19.000000 Dowell Mail-1.0.2/docs/_build/html/_sources/maillib.rst.txt
+-rw-rw-rw-   0        0        0      537 2023-06-22 06:25:19.000000 Dowell Mail-1.0.2/docs/_build/html/_sources/maillib.tests.rst.txt
+-rw-rw-rw-   0        0        0      116 2023-06-22 06:33:29.000000 Dowell Mail-1.0.2/docs/_build/html/_sources/modules.rst.txt
+-rw-rw-rw-   0        0        0     2613 2023-06-22 08:08:05.000000 Dowell Mail-1.0.2/docs/_build/html/_sources/static.rst.txt
+-rw-rw-rw-   0        0        0     1588 2023-06-22 08:10:07.000000 Dowell Mail-1.0.2/docs/_build/html/_sources/templates.rst.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.598832 Dowell Mail-1.0.2/docs/_build/html/_static/
+-rw-rw-rw-   0        0        0    11932 2023-06-22 06:33:43.000000 Dowell Mail-1.0.2/docs/_build/html/_static/alabaster.css
+-rw-rw-rw-   0        0        0    15715 2023-06-22 09:47:55.000000 Dowell Mail-1.0.2/docs/_build/html/_static/basic.css
+-rw-rw-rw-   0        0        0       42 2023-06-20 09:37:24.000000 Dowell Mail-1.0.2/docs/_build/html/_static/custom.css
+-rw-rw-rw-   0        0        0     4472 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/html/_static/doctools.js
+-rw-rw-rw-   0        0        0      431 2023-06-22 09:47:55.000000 Dowell Mail-1.0.2/docs/_build/html/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      286 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/html/_static/file.png
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.614839 Dowell Mail-1.0.2/docs/_build/html/_static/fonts/
+-rw-rw-rw-   0        0        0    30724 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/fonts/font-awesome.css
+-rw-rw-rw-   0        0        0      903 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/fonts/material-icons.css
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.703459 Dowell Mail-1.0.2/docs/_build/html/_static/fonts/specimen/
+-rw-rw-rw-   0        0        0   165548 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/fonts/specimen/FontAwesome.ttf
+-rw-rw-rw-   0        0        0    98024 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/fonts/specimen/FontAwesome.woff
+-rw-rw-rw-   0        0        0    77160 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/fonts/specimen/FontAwesome.woff2
+-rw-rw-rw-   0        0        0   128180 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/fonts/specimen/MaterialIcons-Regular.ttf
+-rw-rw-rw-   0        0        0    57620 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/fonts/specimen/MaterialIcons-Regular.woff
+-rw-rw-rw-   0        0        0    44300 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/fonts/specimen/MaterialIcons-Regular.woff2
+-rw-rw-rw-   0        0        0    13292 2023-06-22 08:10:15.000000 Dowell Mail-1.0.2/docs/_build/html/_static/groundwork.css
+-rw-rw-rw-   0        0        0    14145 2023-06-22 07:09:36.000000 Dowell Mail-1.0.2/docs/_build/html/_static/gw_logo.png
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.709445 Dowell Mail-1.0.2/docs/_build/html/_static/images/
+-rw-rw-rw-   0        0        0      521 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/images/favicon.png
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.742462 Dowell Mail-1.0.2/docs/_build/html/_static/images/icons/
+-rw-rw-rw-   0        0        0     1230 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/images/icons/bitbucket.1b09e088.svg
+-rw-rw-rw-   0        0        0     1230 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/images/icons/bitbucket.svg
+-rw-rw-rw-   0        0        0      993 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/images/icons/github.f0b8504a.svg
+-rw-rw-rw-   0        0        0      993 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/images/icons/github.svg
+-rw-rw-rw-   0        0        0     1138 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/images/icons/gitlab.6dd19c00.svg
+-rw-rw-rw-   0        0        0     1138 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/images/icons/gitlab.svg
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.760040 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/
+-rw-rw-rw-   0        0        0   135210 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/application.js
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.906587 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/
+-rw-rw-rw-   0        0        0     4259 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.da.js
+-rw-rw-rw-   0        0        0     5736 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.de.js
+-rw-rw-rw-   0        0        0     5817 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.du.js
+-rw-rw-rw-   0        0        0    11072 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.es.js
+-rw-rw-rw-   0        0        0     8870 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.fi.js
+-rw-rw-rw-   0        0        0    10242 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.fr.js
+-rw-rw-rw-   0        0        0     9025 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.hu.js
+-rw-rw-rw-   0        0        0    10739 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.it.js
+-rw-rw-rw-   0        0        0     2282 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.ja.js
+-rw-rw-rw-   0        0        0       36 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.jp.js
+-rw-rw-rw-   0        0        0      774 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.multi.js
+-rw-rw-rw-   0        0        0     5635 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.nl.js
+-rw-rw-rw-   0        0        0     4340 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.no.js
+-rw-rw-rw-   0        0        0     9728 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.pt.js
+-rw-rw-rw-   0        0        0    10498 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.ro.js
+-rw-rw-rw-   0        0        0     9808 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.ru.js
+-rw-rw-rw-   0        0        0     3633 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.stemmer.support.js
+-rw-rw-rw-   0        0        0     4129 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.sv.js
+-rw-rw-rw-   0        0        0     1029 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.th.js
+-rw-rw-rw-   0        0        0    13761 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.tr.js
+-rw-rw-rw-   0        0        0    18288 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/tinyseg.js
+-rw-rw-rw-   0        0        0   555307 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/wordcut.js
+-rw-rw-rw-   0        0        0     7285 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/modernizr.js
+-rw-rw-rw-   0        0        0     1107 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/version_dropdown.js
+-rw-rw-rw-   0        0        0    89503 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/jquery.js
+-rw-rw-rw-   0        0        0   137972 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/jquery.min.map
+-rw-rw-rw-   0        0        0     4957 2023-06-22 09:47:55.000000 Dowell Mail-1.0.2/docs/_build/html/_static/language_data.js
+-rw-rw-rw-   0        0        0      706 2023-06-22 09:47:55.000000 Dowell Mail-1.0.2/docs/_build/html/_static/material.css
+-rw-rw-rw-   0        0        0       90 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/html/_static/plus.png
+-rw-rw-rw-   0        0        0     4891 2023-06-22 09:47:55.000000 Dowell Mail-1.0.2/docs/_build/html/_static/pygments.css
+-rw-rw-rw-   0        0        0    18215 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/html/_static/searchtools.js
+-rw-rw-rw-   0        0        0     1259 2023-06-22 07:09:36.000000 Dowell Mail-1.0.2/docs/_build/html/_static/small_groundwork.css
+-rw-rw-rw-   0        0        0     4712 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/html/_static/sphinx_highlight.js
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.928584 Dowell Mail-1.0.2/docs/_build/html/_static/stylesheets/
+-rw-rw-rw-   0        0        0     9808 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/stylesheets/application-fixes.css
+-rw-rw-rw-   0        0        0    43675 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/stylesheets/application-palette.css
+-rw-rw-rw-   0        0        0    88621 2023-06-22 08:14:22.000000 Dowell Mail-1.0.2/docs/_build/html/_static/stylesheets/application.css
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.933638 Dowell Mail-1.0.2/docs/_build/html/css/
+-rw-rw-rw-   0        0        0     2055 2023-06-13 09:55:15.000000 Dowell Mail-1.0.2/docs/_build/html/css/styles.css
+-rw-rw-rw-   0        0        0    14649 2023-06-22 08:14:59.000000 Dowell Mail-1.0.2/docs/_build/html/emailapp.html
+-rw-rw-rw-   0        0        0    15947 2023-06-22 09:47:54.000000 Dowell Mail-1.0.2/docs/_build/html/genindex.html
+-rw-rw-rw-   0        0        0    13129 2023-06-22 09:47:54.000000 Dowell Mail-1.0.2/docs/_build/html/index.html
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:24.941604 Dowell Mail-1.0.2/docs/_build/html/maillib/
+-rw-rw-rw-   0        0        0     1232 2023-06-14 09:48:36.000000 Dowell Mail-1.0.2/docs/_build/html/maillib/home.html
+-rw-rw-rw-   0        0        0    21545 2023-06-22 08:14:59.000000 Dowell Mail-1.0.2/docs/_build/html/maillib.html
+-rw-rw-rw-   0        0        0    10119 2023-06-22 08:14:59.000000 Dowell Mail-1.0.2/docs/_build/html/maillib.migrations.html
+-rw-rw-rw-   0        0        0    20731 2023-06-22 08:15:00.000000 Dowell Mail-1.0.2/docs/_build/html/maillib.tests.html
+-rw-rw-rw-   0        0        0    13496 2023-06-22 09:47:54.000000 Dowell Mail-1.0.2/docs/_build/html/modules.html
+-rw-rw-rw-   0        0        0      619 2023-06-22 09:47:55.000000 Dowell Mail-1.0.2/docs/_build/html/objects.inv
+-rw-rw-rw-   0        0        0    12875 2023-06-22 09:47:54.000000 Dowell Mail-1.0.2/docs/_build/html/py-modindex.html
+-rw-rw-rw-   0        0        0     9434 2023-06-22 09:47:54.000000 Dowell Mail-1.0.2/docs/_build/html/search.html
+-rw-rw-rw-   0        0        0     9506 2023-06-22 09:47:55.000000 Dowell Mail-1.0.2/docs/_build/html/searchindex.js
+-rw-rw-rw-   0        0        0    29089 2023-06-22 08:15:00.000000 Dowell Mail-1.0.2/docs/_build/html/static.html
+-rw-rw-rw-   0        0        0    13060 2023-06-22 08:15:00.000000 Dowell Mail-1.0.2/docs/_build/html/templates.html
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:25.153815 Dowell Mail-1.0.2/docs/_build/latex/
+-rw-rw-rw-   0        0        0     4366 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/LICRcyr2utf8.xdy
+-rw-rw-rw-   0        0        0    10188 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/LICRlatin2utf8.xdy
+-rw-rw-rw-   0        0        0    18890 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/LatinRules.xdy
+-rw-rw-rw-   0        0        0     2416 2023-06-22 10:29:44.000000 Dowell Mail-1.0.2/docs/_build/latex/Makefile
+-rw-rw-rw-   0        0        0    16376 2023-06-22 08:19:00.000000 Dowell Mail-1.0.2/docs/_build/latex/dowell-mail.tex
+-rw-rw-rw-   0        0        0      705 2023-06-22 10:29:44.000000 Dowell Mail-1.0.2/docs/_build/latex/latexmkjarc
+-rw-rw-rw-   0        0        0      413 2023-06-22 10:29:44.000000 Dowell Mail-1.0.2/docs/_build/latex/latexmkrc
+-rwxrwxrwx   0        0        0      503 2023-06-22 10:29:44.000000 Dowell Mail-1.0.2/docs/_build/latex/make.bat
+-rw-rw-rw-   0        0        0      392 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/python.ist
+-rw-rw-rw-   0        0        0    44560 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinx.sty
+-rw-rw-rw-   0        0        0     9474 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinx.xdy
+-rw-rw-rw-   0        0        0     7619 2023-06-22 10:29:44.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxhighlight.sty
+-rw-rw-rw-   0        0        0     3256 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxhowto.cls
+-rw-rw-rw-   0        0        0    10989 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexadmonitions.sty
+-rw-rw-rw-   0        0        0      901 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexcontainers.sty
+-rw-rw-rw-   0        0        0     4840 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexgraphics.sty
+-rw-rw-rw-   0        0        0     2066 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexindbibtoc.sty
+-rw-rw-rw-   0        0        0     5139 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexlists.sty
+-rw-rw-rw-   0        0        0    46048 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexliterals.sty
+-rw-rw-rw-   0        0        0     4532 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexnumfig.sty
+-rw-rw-rw-   0        0        0     9067 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexobjects.sty
+-rw-rw-rw-   0        0        0     5066 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexshadowbox.sty
+-rw-rw-rw-   0        0        0     3445 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexstyleheadings.sty
+-rw-rw-rw-   0        0        0     3064 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexstylepage.sty
+-rw-rw-rw-   0        0        0     8232 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexstyletext.sty
+-rw-rw-rw-   0        0        0    57830 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxlatextables.sty
+-rw-rw-rw-   0        0        0     4241 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxmanual.cls
+-rw-rw-rw-   0        0        0      765 2023-06-22 10:29:44.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxmessages.sty
+-rw-rw-rw-   0        0        0     2061 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxoptionsgeometry.sty
+-rw-rw-rw-   0        0        0     1094 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxoptionshyperref.sty
+-rw-rw-rw-   0        0        0    36615 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxpackageboxes.sty
+-rw-rw-rw-   0        0        0     2590 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxpackagecyrillic.sty
+-rw-rw-rw-   0        0        0    15254 2023-06-20 09:37:25.000000 Dowell Mail-1.0.2/docs/_build/latex/sphinxpackagefootnote.sty
+-rw-rw-rw-   0        0        0     1464 2023-06-22 09:50:58.000000 Dowell Mail-1.0.2/docs/conf.py
+-rw-rw-rw-   0        0        0      739 2023-06-22 06:25:18.000000 Dowell Mail-1.0.2/docs/emailapp.rst
+-rw-rw-rw-   0        0        0     1770 2023-06-22 08:11:35.000000 Dowell Mail-1.0.2/docs/index.rst
+-rw-rw-rw-   0        0        0      187 2023-06-22 06:25:19.000000 Dowell Mail-1.0.2/docs/maillib.migrations.rst
+-rw-rw-rw-   0        0        0      961 2023-06-22 06:25:19.000000 Dowell Mail-1.0.2/docs/maillib.rst
+-rw-rw-rw-   0        0        0      537 2023-06-22 06:25:19.000000 Dowell Mail-1.0.2/docs/maillib.tests.rst
+-rwxrwxrwx   0        0        0      800 2023-06-22 06:23:19.000000 Dowell Mail-1.0.2/docs/make.bat
+-rw-rw-rw-   0        0        0      116 2023-06-22 06:33:29.000000 Dowell Mail-1.0.2/docs/modules.rst
+-rw-rw-rw-   0        0        0     2613 2023-06-22 08:09:28.000000 Dowell Mail-1.0.2/docs/static.rst
+-rw-rw-rw-   0        0        0     1588 2023-06-22 08:10:07.000000 Dowell Mail-1.0.2/docs/templates.rst
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:25.202339 Dowell Mail-1.0.2/maillib/
+-rw-rw-rw-   0        0        0        0 2023-06-12 14:04:27.000000 Dowell Mail-1.0.2/maillib/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-06-12 14:04:27.000000 Dowell Mail-1.0.2/maillib/admin.py
+-rw-rw-rw-   0        0        0      152 2023-06-12 14:04:28.000000 Dowell Mail-1.0.2/maillib/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:25.209344 Dowell Mail-1.0.2/maillib/migrations/
+-rw-rw-rw-   0        0        0        0 2023-06-12 14:04:27.000000 Dowell Mail-1.0.2/maillib/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-06-12 14:04:27.000000 Dowell Mail-1.0.2/maillib/models.py
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:25.228344 Dowell Mail-1.0.2/maillib/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-14 13:01:00.000000 Dowell Mail-1.0.2/maillib/tests/__init__.py
+-rw-rw-rw-   0        0        0      570 2023-06-20 07:59:06.000000 Dowell Mail-1.0.2/maillib/tests/test_urls.py
+-rw-rw-rw-   0        0        0     3531 2023-06-21 06:39:18.000000 Dowell Mail-1.0.2/maillib/tests/test_views.py
+-rw-rw-rw-   0        0        0      735 2023-06-21 06:37:21.000000 Dowell Mail-1.0.2/maillib/urls.py
+-rw-rw-rw-   0        0        0     3323 2023-06-21 07:15:46.000000 Dowell Mail-1.0.2/maillib/views.py
+-rw-rw-rw-   0        0        0      879 2023-06-26 11:30:25.272937 Dowell Mail-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      288 2023-06-26 09:34:46.000000 Dowell Mail-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.393871 Dowell Mail-1.0.2/static/
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:25.233345 Dowell Mail-1.0.2/static/css/
+-rw-rw-rw-   0        0        0     2055 2023-06-13 09:55:15.000000 Dowell Mail-1.0.2/static/css/styles.css
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:22.400877 Dowell Mail-1.0.2/templates/
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:25.247371 Dowell Mail-1.0.2/templates/_partials/
+-rw-rw-rw-   0        0        0      548 2023-06-13 06:52:16.000000 Dowell Mail-1.0.2/templates/_partials/base.html
+-rw-rw-rw-   0        0        0      164 2023-06-13 09:58:30.000000 Dowell Mail-1.0.2/templates/_partials/messages.html
+drwxrwxrwx   0        0        0        0 2023-06-26 11:30:25.253371 Dowell Mail-1.0.2/templates/maillib/
+-rw-rw-rw-   0        0        0     1232 2023-06-14 09:48:36.000000 Dowell Mail-1.0.2/templates/maillib/home.html
```

### Comparing `Dowell Mail-1.0.1/Dowell_Mail.egg-info/PKG-INFO` & `Dowell Mail-1.0.2/Dowell_Mail.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dowell-Mail
-Version: 1.0.1
+Version: 1.0.2
 Summary: Dowell Mail Package
 Author: Marvin
 Author-email: marvin.wekesa@gmail.com
 Keywords: Dowell Django Mail
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -51,8 +51,8 @@
 
 ## Features
 
 Dowell Mail offers a reliable and user-friendly API for sending and validating emails. Our API services provide a seamless experience for sending emails from your own email ID and validating email addresses for accuracy. Whether you need to send important notifications or verify email addresses, Dowell Mail API has got you covered.
 
 To understand the API calls and their functionality, I recommend reading the documentation. The documentation provides comprehensive information on making API requests and utilizing the available endpoints. It explains the required parameters, request methods, and response formats for each API call.
 
-[Documentation](`https://dowellmail.onrender.com/`)
+[Documentation](https://dowellmail.onrender.com/)
```

### Comparing `Dowell Mail-1.0.1/Dowell_Mail.egg-info/SOURCES.txt` & `Dowell Mail-1.0.2/Dowell_Mail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/LICENCE` & `Dowell Mail-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/LICENSE` & `Dowell Mail-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/PKG-INFO` & `Dowell Mail-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dowell Mail
-Version: 1.0.1
+Version: 1.0.2
 Summary: Dowell Mail Package
 Author: Marvin
 Author-email: marvin.wekesa@gmail.com
 Keywords: Dowell Django Mail
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -51,8 +51,8 @@
 
 ## Features
 
 Dowell Mail offers a reliable and user-friendly API for sending and validating emails. Our API services provide a seamless experience for sending emails from your own email ID and validating email addresses for accuracy. Whether you need to send important notifications or verify email addresses, Dowell Mail API has got you covered.
 
 To understand the API calls and their functionality, I recommend reading the documentation. The documentation provides comprehensive information on making API requests and utilizing the available endpoints. It explains the required parameters, request methods, and response formats for each API call.
 
-[Documentation](`https://dowellmail.onrender.com/`)
+[Documentation](https://dowellmail.onrender.com/)
```

### Comparing `Dowell Mail-1.0.1/README.rst` & `Dowell Mail-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/hooks/commit-msg.sample` & `Dowell Mail-1.0.2/docs/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/hooks/fsmonitor-watchman.sample` & `Dowell Mail-1.0.2/docs/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/hooks/pre-commit.sample` & `Dowell Mail-1.0.2/docs/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/hooks/pre-push.sample` & `Dowell Mail-1.0.2/docs/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/hooks/pre-rebase.sample` & `Dowell Mail-1.0.2/docs/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/hooks/pre-receive.sample` & `Dowell Mail-1.0.2/docs/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/hooks/prepare-commit-msg.sample` & `Dowell Mail-1.0.2/docs/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/hooks/push-to-checkout.sample` & `Dowell Mail-1.0.2/docs/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/hooks/update.sample` & `Dowell Mail-1.0.2/docs/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/index` & `Dowell Mail-1.0.2/docs/.git/index`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/logs/HEAD` & `Dowell Mail-1.0.2/docs/.git/logs/HEAD`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/07/8d0cab706bad2c6548af839fe50f89ff29011d` & `Dowell Mail-1.0.2/docs/.git/objects/07/8d0cab706bad2c6548af839fe50f89ff29011d`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/0a/cc10571f6e2635820e7dee824d79b24eb64082` & `Dowell Mail-1.0.2/docs/.git/objects/0a/cc10571f6e2635820e7dee824d79b24eb64082`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/0b/efce938f1e8e31e8b131fba92285e7cbde0492` & `Dowell Mail-1.0.2/docs/.git/objects/0b/efce938f1e8e31e8b131fba92285e7cbde0492`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/0d/cf1133cd7b82c81d790bd3b165e4bef0497364` & `Dowell Mail-1.0.2/docs/.git/objects/0d/cf1133cd7b82c81d790bd3b165e4bef0497364`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/11/bba08eb15c8676a59416cae5c3224032806b36` & `Dowell Mail-1.0.2/docs/.git/objects/11/bba08eb15c8676a59416cae5c3224032806b36`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/11/c9a999490dace18f6121e568c0190ecb04ca33` & `Dowell Mail-1.0.2/docs/.git/objects/11/c9a999490dace18f6121e568c0190ecb04ca33`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/14/b9b602f01362269bf04515443533242bd13f11` & `Dowell Mail-1.0.2/docs/.git/objects/14/b9b602f01362269bf04515443533242bd13f11`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/15/29892c823dfa8800da280360a0876cb8627834` & `Dowell Mail-1.0.2/docs/.git/objects/15/29892c823dfa8800da280360a0876cb8627834`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/17/9792ab7540071599ca06538c571372d3788fb6` & `Dowell Mail-1.0.2/docs/.git/objects/17/9792ab7540071599ca06538c571372d3788fb6`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/18/522369860ece5164ab3f845d63ea18fc77b080` & `Dowell Mail-1.0.2/docs/.git/objects/18/522369860ece5164ab3f845d63ea18fc77b080`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/1d/768259cdbc1200244462dcd508e120087972fb` & `Dowell Mail-1.0.2/docs/.git/objects/1d/768259cdbc1200244462dcd508e120087972fb`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/23/3c46dbc9802fafa8b32ec4edc4a04e9c237c99` & `Dowell Mail-1.0.2/docs/.git/objects/23/3c46dbc9802fafa8b32ec4edc4a04e9c237c99`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/25/0f5665fa64b70c822190199b3b804b10f8b9d8` & `Dowell Mail-1.0.2/docs/.git/objects/25/0f5665fa64b70c822190199b3b804b10f8b9d8`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/27/3f4ad0beb8fba582b1e2390c2b7e9d406020a1` & `Dowell Mail-1.0.2/docs/.git/objects/27/3f4ad0beb8fba582b1e2390c2b7e9d406020a1`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/27/6506ff833411e7a32ec5a0d0b6b4138c910b97` & `Dowell Mail-1.0.2/docs/.git/objects/27/6506ff833411e7a32ec5a0d0b6b4138c910b97`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/2b/d90b52fd5e09963e064b660f9efb4752333a94` & `Dowell Mail-1.0.2/docs/.git/objects/2b/d90b52fd5e09963e064b660f9efb4752333a94`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/2e/4b30d921c3343a19744726882b85cdf3621f5c` & `Dowell Mail-1.0.2/docs/.git/objects/2e/4b30d921c3343a19744726882b85cdf3621f5c`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/2f/9bf5aebdb39583df031edacfc61c32f399c4b8` & `Dowell Mail-1.0.2/docs/.git/objects/2f/9bf5aebdb39583df031edacfc61c32f399c4b8`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/31/f32feb95e4c90d013340e6a8b94d5a6a2392b5` & `Dowell Mail-1.0.2/docs/.git/objects/31/f32feb95e4c90d013340e6a8b94d5a6a2392b5`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/34/910dfe5faba7f2cd385dca52906898127628be` & `Dowell Mail-1.0.2/docs/.git/objects/34/910dfe5faba7f2cd385dca52906898127628be`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/35/acda2fa1196aad98c2adf4378a7611dd713aa3` & `Dowell Mail-1.0.2/docs/.git/objects/35/acda2fa1196aad98c2adf4378a7611dd713aa3`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/36/eaf6a0450c5a150834345972b6eff6dc20b63c` & `Dowell Mail-1.0.2/docs/.git/objects/36/eaf6a0450c5a150834345972b6eff6dc20b63c`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/3a/73a76619e39b9d73f4e9610e60f54d6f999750` & `Dowell Mail-1.0.2/docs/.git/objects/3a/73a76619e39b9d73f4e9610e60f54d6f999750`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/3d/13b1975139abbb5a4bcc84e6bfff7cd57a4d51` & `Dowell Mail-1.0.2/docs/.git/objects/3d/13b1975139abbb5a4bcc84e6bfff7cd57a4d51`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/3d/156b9c191cd246879a67c56e46baa4cfb2e17d` & `Dowell Mail-1.0.2/docs/.git/objects/3d/156b9c191cd246879a67c56e46baa4cfb2e17d`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/40/0014a4b06eee3d0c0d54402a47ab2601b2862b` & `Dowell Mail-1.0.2/docs/.git/objects/40/0014a4b06eee3d0c0d54402a47ab2601b2862b`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/40/66129bf24ca86c1eb0cb8cf55f8730b92ca4d8` & `Dowell Mail-1.0.2/docs/.git/objects/40/66129bf24ca86c1eb0cb8cf55f8730b92ca4d8`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/45/842b115c602827007d69ecbcaf308511340cdb` & `Dowell Mail-1.0.2/docs/.git/objects/45/842b115c602827007d69ecbcaf308511340cdb`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/45/bffe09237d6f691365be13b11c8c205a4f35f5` & `Dowell Mail-1.0.2/docs/.git/objects/45/bffe09237d6f691365be13b11c8c205a4f35f5`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/48/8c29664e6a0160871b70a81c597df7a0a5b276` & `Dowell Mail-1.0.2/docs/.git/objects/48/8c29664e6a0160871b70a81c597df7a0a5b276`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/4a/bdd66d1abde1e9465c471010d0c1056af9c682` & `Dowell Mail-1.0.2/docs/.git/objects/4a/bdd66d1abde1e9465c471010d0c1056af9c682`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/4c/4e6fd4fcc67b9fa4cd695b9023ac9e66d91904` & `Dowell Mail-1.0.2/docs/.git/objects/4c/4e6fd4fcc67b9fa4cd695b9023ac9e66d91904`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/4d/13fc60404b91e398a37200c4a77b645cfd9586` & `Dowell Mail-1.0.2/docs/.git/objects/4d/13fc60404b91e398a37200c4a77b645cfd9586`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/4f/60d46a956924a94f68b4725075fe3d1191edf7` & `Dowell Mail-1.0.2/docs/.git/objects/4f/60d46a956924a94f68b4725075fe3d1191edf7`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/50/dddaa04b87af93b515dd6b33d32d0040254307` & `Dowell Mail-1.0.2/docs/.git/objects/50/dddaa04b87af93b515dd6b33d32d0040254307`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/51/7d0b29cb1193b1211c8853b58c65cddd1fa4d2` & `Dowell Mail-1.0.2/docs/.git/objects/51/7d0b29cb1193b1211c8853b58c65cddd1fa4d2`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/52/15595b510b67b720091544ea1a4eccb4722381` & `Dowell Mail-1.0.2/docs/.git/objects/52/15595b510b67b720091544ea1a4eccb4722381`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/52/632004a2414fe4aee1cf9f85696d0ae66eaa3e` & `Dowell Mail-1.0.2/docs/.git/objects/52/632004a2414fe4aee1cf9f85696d0ae66eaa3e`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/52/ec8be7e6cc2123f25079e19a6dfadd89d8b69d` & `Dowell Mail-1.0.2/docs/.git/objects/52/ec8be7e6cc2123f25079e19a6dfadd89d8b69d`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/54/430761163f1a6478239ae68eb9a2b8b0d3506e` & `Dowell Mail-1.0.2/docs/.git/objects/54/430761163f1a6478239ae68eb9a2b8b0d3506e`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/55/901234df171e819e5ab726ebe9eb3acc25dada` & `Dowell Mail-1.0.2/docs/.git/objects/55/901234df171e819e5ab726ebe9eb3acc25dada`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/55/fd4172c46835b24bc52edecb319a02e5652963` & `Dowell Mail-1.0.2/docs/.git/objects/55/fd4172c46835b24bc52edecb319a02e5652963`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/56/a4b0dc19f7c9e8b8423e544ed5e80fbb92abd7` & `Dowell Mail-1.0.2/docs/.git/objects/56/a4b0dc19f7c9e8b8423e544ed5e80fbb92abd7`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/57/36305299fc9615b7b91c6778cb365be4e9ccfc` & `Dowell Mail-1.0.2/docs/.git/objects/57/36305299fc9615b7b91c6778cb365be4e9ccfc`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/57/eaee2f2272d9755e1dc69179e8e219050c6905` & `Dowell Mail-1.0.2/docs/.git/objects/57/eaee2f2272d9755e1dc69179e8e219050c6905`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/58/40c3bbf9dd7b0b27c6a977d843940b09ae8c54` & `Dowell Mail-1.0.2/docs/.git/objects/58/40c3bbf9dd7b0b27c6a977d843940b09ae8c54`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/59/161a19db9a40ae6b96ede4cf7213570db3de9a` & `Dowell Mail-1.0.2/docs/.git/objects/59/161a19db9a40ae6b96ede4cf7213570db3de9a`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/5a/354d3c77dd2d04ceb0cd61592c0a1a848ba355` & `Dowell Mail-1.0.2/docs/.git/objects/5a/354d3c77dd2d04ceb0cd61592c0a1a848ba355`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/5d/ea4a6e8da2f6ce6e06acec0e2662be88b5374f` & `Dowell Mail-1.0.2/docs/.git/objects/5d/ea4a6e8da2f6ce6e06acec0e2662be88b5374f`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/5e/adc1c5b64a06531d4125561cc513c8fb4ab37d` & `Dowell Mail-1.0.2/docs/.git/objects/5e/adc1c5b64a06531d4125561cc513c8fb4ab37d`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/64/808af3c3ac606f310b83f68ee9cfee8dbc8b03` & `Dowell Mail-1.0.2/docs/.git/objects/64/808af3c3ac606f310b83f68ee9cfee8dbc8b03`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/69/f620250d95bc3982dd8a6bd46689759a54c2a3` & `Dowell Mail-1.0.2/docs/.git/objects/69/f620250d95bc3982dd8a6bd46689759a54c2a3`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/6c/31f329c658b01ae8b2c10194e09ed1a72f4f31` & `Dowell Mail-1.0.2/docs/.git/objects/6c/31f329c658b01ae8b2c10194e09ed1a72f4f31`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/6d/72961051eba439a573224713613f34beebe7d5` & `Dowell Mail-1.0.2/docs/.git/objects/6d/72961051eba439a573224713613f34beebe7d5`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/6d/af5f9d807ec44fb0cfba836a21c17dd888f8da` & `Dowell Mail-1.0.2/docs/.git/objects/6d/af5f9d807ec44fb0cfba836a21c17dd888f8da`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/70/15564ad166a3e9d88c82f17829f0cc01ebe29a` & `Dowell Mail-1.0.2/docs/.git/objects/70/15564ad166a3e9d88c82f17829f0cc01ebe29a`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/75/45ea35e0a5df26e09aa3b4834e736ab191aac6` & `Dowell Mail-1.0.2/docs/.git/objects/75/45ea35e0a5df26e09aa3b4834e736ab191aac6`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/75/77acb1ad176e3f58c15ddf9bf1f73525dfe7ed` & `Dowell Mail-1.0.2/docs/.git/objects/75/77acb1ad176e3f58c15ddf9bf1f73525dfe7ed`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/76/d17f57ad903c3ea2f1b564cafb95bf9af84ee3` & `Dowell Mail-1.0.2/docs/.git/objects/76/d17f57ad903c3ea2f1b564cafb95bf9af84ee3`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/77/9d5dd47a5022001209f9c9f935a9c2dde5eebd` & `Dowell Mail-1.0.2/docs/.git/objects/77/9d5dd47a5022001209f9c9f935a9c2dde5eebd`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/77/ad846085e4e2576ca5157789b70c9e24dc24d0` & `Dowell Mail-1.0.2/docs/.git/objects/77/ad846085e4e2576ca5157789b70c9e24dc24d0`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/79/e30a1f1999c22b29515767c063825cc39c58dd` & `Dowell Mail-1.0.2/docs/.git/objects/79/e30a1f1999c22b29515767c063825cc39c58dd`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/7c/724d2e4f2d39cb2e418936f0fdf0198bd118a0` & `Dowell Mail-1.0.2/docs/.git/objects/7c/724d2e4f2d39cb2e418936f0fdf0198bd118a0`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/7d/1e8c2f1bbc45869b92d703be845f6eb20ebd0a` & `Dowell Mail-1.0.2/docs/.git/objects/7d/1e8c2f1bbc45869b92d703be845f6eb20ebd0a`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/7d/86eb1694970141b88b52f5b26e6b019f16b590` & `Dowell Mail-1.0.2/docs/.git/objects/7d/86eb1694970141b88b52f5b26e6b019f16b590`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/80/f9d49c9bd4d7d58996254dee424b25d3164ef6` & `Dowell Mail-1.0.2/docs/.git/objects/80/f9d49c9bd4d7d58996254dee424b25d3164ef6`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/85/e59c4ac73dcfde98d34e848b5c99b7714d33ae` & `Dowell Mail-1.0.2/docs/.git/objects/85/e59c4ac73dcfde98d34e848b5c99b7714d33ae`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/89/9804d75f317500aab85d5dd773814026a7e48c` & `Dowell Mail-1.0.2/docs/.git/objects/89/9804d75f317500aab85d5dd773814026a7e48c`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/8d/7dd0ee7185687b4404c3e0480b20e1ed0fd4eb` & `Dowell Mail-1.0.2/docs/.git/objects/8d/7dd0ee7185687b4404c3e0480b20e1ed0fd4eb`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/8e/793555684ac8caa28b91a17d26502b51629732` & `Dowell Mail-1.0.2/docs/.git/objects/8e/793555684ac8caa28b91a17d26502b51629732`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/8f/99b2771e10cbb806d18c35ce3bfce1eda46dcd` & `Dowell Mail-1.0.2/docs/.git/objects/8f/99b2771e10cbb806d18c35ce3bfce1eda46dcd`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/8f/c9926ef0fa53320bc485118f7a870a19eda8db` & `Dowell Mail-1.0.2/docs/.git/objects/8f/c9926ef0fa53320bc485118f7a870a19eda8db`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/91/3bc8210a6a2156fc818eef2d545e8b0871a518` & `Dowell Mail-1.0.2/docs/.git/objects/91/3bc8210a6a2156fc818eef2d545e8b0871a518`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/97/d56a74d8207ec36a96a5e24f4a4b42dd51f6b2` & `Dowell Mail-1.0.2/docs/.git/objects/97/d56a74d8207ec36a96a5e24f4a4b42dd51f6b2`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/9a/a62fc22baa68906867164da4d6819dfaf72907` & `Dowell Mail-1.0.2/docs/.git/objects/9a/a62fc22baa68906867164da4d6819dfaf72907`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/9d/e6c09cb4238addb63e4a63a54bdf83b6c8d6ff` & `Dowell Mail-1.0.2/docs/.git/objects/9d/e6c09cb4238addb63e4a63a54bdf83b6c8d6ff`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/9e/4453259d6929c2bf7b7b9a5d18c76a753c4d44` & `Dowell Mail-1.0.2/docs/.git/objects/9e/4453259d6929c2bf7b7b9a5d18c76a753c4d44`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/9f/a211252080046a23b2449dbdced6abc2b0bb34` & `Dowell Mail-1.0.2/docs/.git/objects/9f/a211252080046a23b2449dbdced6abc2b0bb34`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/a1/3b146a9a996aea5bc19af6bc48ac34579485a9` & `Dowell Mail-1.0.2/docs/.git/objects/a1/3b146a9a996aea5bc19af6bc48ac34579485a9`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/a2/a1a0e393e42392b8046793cf3361227432fe73` & `Dowell Mail-1.0.2/docs/.git/objects/a2/a1a0e393e42392b8046793cf3361227432fe73`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/a3/1ae4ce3a2c809b63787b319c6ebc51df4dee6d` & `Dowell Mail-1.0.2/docs/.git/objects/a3/1ae4ce3a2c809b63787b319c6ebc51df4dee6d`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/a6/5d194b7adbb6fac28c1654cca5d0c165015377` & `Dowell Mail-1.0.2/docs/.git/objects/a6/5d194b7adbb6fac28c1654cca5d0c165015377`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/a9/ca1c82cd661cfa1583e86fa881644d029d061f` & `Dowell Mail-1.0.2/docs/.git/objects/a9/ca1c82cd661cfa1583e86fa881644d029d061f`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/aa/e669d7ea6b1dc6edcb5c651f5d095f7a2dc6e6` & `Dowell Mail-1.0.2/docs/.git/objects/aa/e669d7ea6b1dc6edcb5c651f5d095f7a2dc6e6`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/ac/99248044a350007567ce177ba3e2ae286bef63` & `Dowell Mail-1.0.2/docs/.git/objects/ac/99248044a350007567ce177ba3e2ae286bef63`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/ad/07dd68bddf8730f4584ed84fac8050473a6d95` & `Dowell Mail-1.0.2/docs/.git/objects/ad/07dd68bddf8730f4584ed84fac8050473a6d95`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/af/5a804d593607e51ca637bebcbc9633f261691d` & `Dowell Mail-1.0.2/docs/.git/objects/af/5a804d593607e51ca637bebcbc9633f261691d`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/b0/d3707062fef1eb41d2e5ac63e09d48465e6bab` & `Dowell Mail-1.0.2/docs/.git/objects/b0/d3707062fef1eb41d2e5ac63e09d48465e6bab`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/b1/9627e1b35eb0240db39497c70b509624c0da09` & `Dowell Mail-1.0.2/docs/.git/objects/b1/9627e1b35eb0240db39497c70b509624c0da09`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/b2/0fbbb83a55f6286917183d07d549846b0b8ed9` & `Dowell Mail-1.0.2/docs/.git/objects/b2/0fbbb83a55f6286917183d07d549846b0b8ed9`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/b4/76b53e33b5789396e2b48d44c8abc07a037db3` & `Dowell Mail-1.0.2/docs/.git/objects/b4/76b53e33b5789396e2b48d44c8abc07a037db3`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/b4/ff1f9d02d01ec10e3808971706542a6d0ec748` & `Dowell Mail-1.0.2/docs/.git/objects/b4/ff1f9d02d01ec10e3808971706542a6d0ec748`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/b5/9cb4eb5ff374906c380579330c0fe36fa3cc88` & `Dowell Mail-1.0.2/docs/.git/objects/b5/9cb4eb5ff374906c380579330c0fe36fa3cc88`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/b5/e9c8543653a3c7194b8f4879ef43646bc79c2e` & `Dowell Mail-1.0.2/docs/.git/objects/b5/e9c8543653a3c7194b8f4879ef43646bc79c2e`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/b6/48a3eea2d16b6ce783906d6b7d5f251b9eb56c` & `Dowell Mail-1.0.2/docs/.git/objects/b6/48a3eea2d16b6ce783906d6b7d5f251b9eb56c`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/b6/6df4ab09628c1dcce7f663a314e51332c64310` & `Dowell Mail-1.0.2/docs/.git/objects/b6/6df4ab09628c1dcce7f663a314e51332c64310`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/b8/8f108df9a4d81e94bb8d0a3ecded420c9999f7` & `Dowell Mail-1.0.2/docs/.git/objects/b8/8f108df9a4d81e94bb8d0a3ecded420c9999f7`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/b9/b75fc0ea791147b7195473e733caee6e4fc31e` & `Dowell Mail-1.0.2/docs/.git/objects/b9/b75fc0ea791147b7195473e733caee6e4fc31e`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/b9/f5723bd8733e425085e505dd100de2cf54c6cb` & `Dowell Mail-1.0.2/docs/.git/objects/b9/f5723bd8733e425085e505dd100de2cf54c6cb`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/ba/a21647ca52c56d628adce41e076b5a837ae90d` & `Dowell Mail-1.0.2/docs/.git/objects/ba/a21647ca52c56d628adce41e076b5a837ae90d`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/bc/fc55fb0b780383ae096b2b5a9b47eef30bcf81` & `Dowell Mail-1.0.2/docs/.git/objects/bc/fc55fb0b780383ae096b2b5a9b47eef30bcf81`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/c4/c6022f2982e8dae64cebd6b9a2b59f2547faad` & `Dowell Mail-1.0.2/docs/.git/objects/c4/c6022f2982e8dae64cebd6b9a2b59f2547faad`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/cc/1b794a9b9667f1a6600afc3b3fdce4ac649719` & `Dowell Mail-1.0.2/docs/.git/objects/cc/1b794a9b9667f1a6600afc3b3fdce4ac649719`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/cc/a624a2ceebd47f7c807110d1e4669d88d7a11f` & `Dowell Mail-1.0.2/docs/.git/objects/cc/a624a2ceebd47f7c807110d1e4669d88d7a11f`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/ce/62404b61db8d0ba61bb34c7f4ae5d1fcc31ca1` & `Dowell Mail-1.0.2/docs/.git/objects/ce/62404b61db8d0ba61bb34c7f4ae5d1fcc31ca1`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/cf/58c14fbc67be0626eb95a0a8fc68baa8c2ac03` & `Dowell Mail-1.0.2/docs/.git/objects/cf/58c14fbc67be0626eb95a0a8fc68baa8c2ac03`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/d0/6a71d7518041301a303697d2a3c372648eb7bf` & `Dowell Mail-1.0.2/docs/.git/objects/d0/6a71d7518041301a303697d2a3c372648eb7bf`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/d0/b4b7a096a9df7ca9e16e969b980e37c742149d` & `Dowell Mail-1.0.2/docs/.git/objects/d0/b4b7a096a9df7ca9e16e969b980e37c742149d`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/d8/54b4aa71024fc8efb2f1e9fced00c21f57a2f3` & `Dowell Mail-1.0.2/docs/.git/objects/d8/54b4aa71024fc8efb2f1e9fced00c21f57a2f3`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/e4/e95b864519c0acc98412378441c422cecba687` & `Dowell Mail-1.0.2/docs/.git/objects/e4/e95b864519c0acc98412378441c422cecba687`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/e7/996d8e3406e79a393e78cf8e9c553c4702f85b` & `Dowell Mail-1.0.2/docs/.git/objects/e7/996d8e3406e79a393e78cf8e9c553c4702f85b`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/e7/a7c1901ed4c6a32722f03d6d9a8c0ff5d55652` & `Dowell Mail-1.0.2/docs/.git/objects/e7/a7c1901ed4c6a32722f03d6d9a8c0ff5d55652`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/e8/fb5a7df64cf44eee42ab10ad6386bb57fa9e3d` & `Dowell Mail-1.0.2/docs/.git/objects/e8/fb5a7df64cf44eee42ab10ad6386bb57fa9e3d`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/e9/63414845f850fffe51fa14893f6b67aed97731` & `Dowell Mail-1.0.2/docs/.git/objects/e9/63414845f850fffe51fa14893f6b67aed97731`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/ec/314fea70f892ffd1dbd4a53add8891df3ca982` & `Dowell Mail-1.0.2/docs/.git/objects/ec/314fea70f892ffd1dbd4a53add8891df3ca982`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/ee/8ef373a0d0a4aa2609d7382d7b6bb605824fe6` & `Dowell Mail-1.0.2/docs/.git/objects/ee/8ef373a0d0a4aa2609d7382d7b6bb605824fe6`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/f1/f525a8375f9fc814afff69f587e2123226f9ae` & `Dowell Mail-1.0.2/docs/.git/objects/f1/f525a8375f9fc814afff69f587e2123226f9ae`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/f3/9f778b208dd9614d56b285b880f3697c15e709` & `Dowell Mail-1.0.2/docs/.git/objects/f3/9f778b208dd9614d56b285b880f3697c15e709`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/f5/0fc9fa6d5a0f1a479676d9c0ab72c44125d08c` & `Dowell Mail-1.0.2/docs/.git/objects/f5/0fc9fa6d5a0f1a479676d9c0ab72c44125d08c`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/f7/18bb2f85762580330d3145e01b1aa4e01c51fd` & `Dowell Mail-1.0.2/docs/.git/objects/f7/18bb2f85762580330d3145e01b1aa4e01c51fd`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/fb/846534ac59ccbedb425076d96870627575f620` & `Dowell Mail-1.0.2/docs/.git/objects/fb/846534ac59ccbedb425076d96870627575f620`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/fb/a1ee45d9f9437f627343a4b66c0dfc59ebec0a` & `Dowell Mail-1.0.2/docs/.git/objects/fb/a1ee45d9f9437f627343a4b66c0dfc59ebec0a`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/fd/0aae6386addf84721ec0d5fec2e997013ec6bf` & `Dowell Mail-1.0.2/docs/.git/objects/fd/0aae6386addf84721ec0d5fec2e997013ec6bf`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/.git/objects/fd/f3913755aa169c74990ca316dc8bd48a4bad55` & `Dowell Mail-1.0.2/docs/.git/objects/fd/f3913755aa169c74990ca316dc8bd48a4bad55`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/Makefile` & `Dowell Mail-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/doctrees/emailapp.doctree` & `Dowell Mail-1.0.2/docs/_build/doctrees/emailapp.doctree`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/doctrees/environment.pickle` & `Dowell Mail-1.0.2/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/doctrees/index.doctree` & `Dowell Mail-1.0.2/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/doctrees/maillib.doctree` & `Dowell Mail-1.0.2/docs/_build/doctrees/maillib.doctree`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/doctrees/maillib.migrations.doctree` & `Dowell Mail-1.0.2/docs/_build/doctrees/maillib.migrations.doctree`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/doctrees/maillib.tests.doctree` & `Dowell Mail-1.0.2/docs/_build/doctrees/maillib.tests.doctree`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/doctrees/modules.doctree` & `Dowell Mail-1.0.2/docs/_build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/doctrees/static.doctree` & `Dowell Mail-1.0.2/docs/_build/doctrees/static.doctree`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/doctrees/templates.doctree` & `Dowell Mail-1.0.2/docs/_build/doctrees/templates.doctree`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/Dowell-Mail.epub` & `Dowell Mail-1.0.2/docs/_build/epub/Dowell-Mail.epub`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/_partials/base.html` & `Dowell Mail-1.0.2/docs/_build/epub/_partials/base.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/_static/basic.css` & `Dowell Mail-1.0.2/docs/_build/epub/_static/basic.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/_static/doctools.js` & `Dowell Mail-1.0.2/docs/_build/epub/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/_static/epub.css` & `Dowell Mail-1.0.2/docs/_build/epub/_static/epub.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/_static/pygments.css` & `Dowell Mail-1.0.2/docs/_build/epub/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/_static/searchtools.js` & `Dowell Mail-1.0.2/docs/_build/epub/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/_static/sphinx_highlight.js` & `Dowell Mail-1.0.2/docs/_build/epub/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/content.opf` & `Dowell Mail-1.0.2/docs/_build/epub/content.opf`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/css/styles.css` & `Dowell Mail-1.0.2/docs/_build/epub/css/styles.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/emailapp.xhtml` & `Dowell Mail-1.0.2/docs/_build/epub/emailapp.xhtml`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/genindex.xhtml` & `Dowell Mail-1.0.2/docs/_build/epub/genindex.xhtml`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/index.xhtml` & `Dowell Mail-1.0.2/docs/_build/epub/index.xhtml`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/maillib/home.html` & `Dowell Mail-1.0.2/docs/_build/epub/maillib/home.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/maillib.migrations.xhtml` & `Dowell Mail-1.0.2/docs/_build/epub/maillib.migrations.xhtml`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/maillib.tests.xhtml` & `Dowell Mail-1.0.2/docs/_build/epub/maillib.tests.xhtml`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/maillib.xhtml` & `Dowell Mail-1.0.2/docs/_build/epub/maillib.xhtml`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/modules.xhtml` & `Dowell Mail-1.0.2/docs/_build/epub/modules.xhtml`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/nav.xhtml` & `Dowell Mail-1.0.2/docs/_build/epub/nav.xhtml`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/py-modindex.xhtml` & `Dowell Mail-1.0.2/docs/_build/epub/py-modindex.xhtml`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/static.xhtml` & `Dowell Mail-1.0.2/docs/_build/epub/static.xhtml`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/templates.xhtml` & `Dowell Mail-1.0.2/docs/_build/epub/templates.xhtml`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/epub/toc.ncx` & `Dowell Mail-1.0.2/docs/_build/epub/toc.ncx`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_modules/index.html` & `Dowell Mail-1.0.2/docs/_build/html/_modules/index.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_modules/maillib/apps.html` & `Dowell Mail-1.0.2/docs/_build/html/_modules/maillib/apps.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_modules/maillib/tests/test_urls.html` & `Dowell Mail-1.0.2/docs/_build/html/_modules/maillib/tests/test_urls.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_modules/maillib/tests/test_views.html` & `Dowell Mail-1.0.2/docs/_build/html/_modules/maillib/tests/test_views.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_modules/maillib/views.html` & `Dowell Mail-1.0.2/docs/_build/html/_modules/maillib/views.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_partials/base.html` & `Dowell Mail-1.0.2/docs/_build/html/_partials/base.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_sources/emailapp.rst.txt` & `Dowell Mail-1.0.2/docs/_build/html/_sources/emailapp.rst.txt`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_sources/index.rst.txt` & `Dowell Mail-1.0.2/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_sources/maillib.rst.txt` & `Dowell Mail-1.0.2/docs/_build/html/_sources/maillib.rst.txt`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_sources/maillib.tests.rst.txt` & `Dowell Mail-1.0.2/docs/_build/html/_sources/maillib.tests.rst.txt`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_sources/static.rst.txt` & `Dowell Mail-1.0.2/docs/_build/html/_sources/static.rst.txt`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_sources/templates.rst.txt` & `Dowell Mail-1.0.2/docs/_build/html/_sources/templates.rst.txt`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/alabaster.css` & `Dowell Mail-1.0.2/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/basic.css` & `Dowell Mail-1.0.2/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/doctools.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/fonts/font-awesome.css` & `Dowell Mail-1.0.2/docs/_build/html/_static/fonts/font-awesome.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/fonts/material-icons.css` & `Dowell Mail-1.0.2/docs/_build/html/_static/fonts/material-icons.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/fonts/specimen/FontAwesome.ttf` & `Dowell Mail-1.0.2/docs/_build/html/_static/fonts/specimen/FontAwesome.ttf`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/fonts/specimen/FontAwesome.woff` & `Dowell Mail-1.0.2/docs/_build/html/_static/fonts/specimen/FontAwesome.woff`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/fonts/specimen/FontAwesome.woff2` & `Dowell Mail-1.0.2/docs/_build/html/_static/fonts/specimen/FontAwesome.woff2`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/fonts/specimen/MaterialIcons-Regular.ttf` & `Dowell Mail-1.0.2/docs/_build/html/_static/fonts/specimen/MaterialIcons-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/fonts/specimen/MaterialIcons-Regular.woff` & `Dowell Mail-1.0.2/docs/_build/html/_static/fonts/specimen/MaterialIcons-Regular.woff`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/fonts/specimen/MaterialIcons-Regular.woff2` & `Dowell Mail-1.0.2/docs/_build/html/_static/fonts/specimen/MaterialIcons-Regular.woff2`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/groundwork.css` & `Dowell Mail-1.0.2/docs/_build/html/_static/groundwork.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/gw_logo.png` & `Dowell Mail-1.0.2/docs/_build/html/_static/gw_logo.png`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/images/favicon.png` & `Dowell Mail-1.0.2/docs/_build/html/_static/images/favicon.png`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/images/icons/bitbucket.1b09e088.svg` & `Dowell Mail-1.0.2/docs/_build/html/_static/images/icons/bitbucket.1b09e088.svg`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/images/icons/bitbucket.svg` & `Dowell Mail-1.0.2/docs/_build/html/_static/images/icons/bitbucket.svg`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/images/icons/github.f0b8504a.svg` & `Dowell Mail-1.0.2/docs/_build/html/_static/images/icons/github.f0b8504a.svg`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/images/icons/github.svg` & `Dowell Mail-1.0.2/docs/_build/html/_static/images/icons/github.svg`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/images/icons/gitlab.6dd19c00.svg` & `Dowell Mail-1.0.2/docs/_build/html/_static/images/icons/gitlab.6dd19c00.svg`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/images/icons/gitlab.svg` & `Dowell Mail-1.0.2/docs/_build/html/_static/images/icons/gitlab.svg`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/application.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/application.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.da.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.da.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.de.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.de.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.du.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.du.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.es.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.es.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.fi.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.fi.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.fr.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.fr.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.hu.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.hu.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.it.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.it.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.ja.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.ja.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.multi.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.multi.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.nl.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.nl.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.no.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.no.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.pt.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.pt.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.ro.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.ro.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.ru.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.ru.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.stemmer.support.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.stemmer.support.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.sv.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.sv.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.th.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.th.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/lunr.tr.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/lunr.tr.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/tinyseg.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/lunr/wordcut.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/modernizr.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/modernizr.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/javascripts/version_dropdown.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/javascripts/version_dropdown.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/jquery.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/jquery.min.map` & `Dowell Mail-1.0.2/docs/_build/html/_static/jquery.min.map`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/language_data.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/material.css` & `Dowell Mail-1.0.2/docs/_build/html/_static/material.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/pygments.css` & `Dowell Mail-1.0.2/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/searchtools.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/small_groundwork.css` & `Dowell Mail-1.0.2/docs/_build/html/_static/small_groundwork.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/sphinx_highlight.js` & `Dowell Mail-1.0.2/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/stylesheets/application-fixes.css` & `Dowell Mail-1.0.2/docs/_build/html/_static/stylesheets/application-fixes.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/stylesheets/application-palette.css` & `Dowell Mail-1.0.2/docs/_build/html/_static/stylesheets/application-palette.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/_static/stylesheets/application.css` & `Dowell Mail-1.0.2/docs/_build/html/_static/stylesheets/application.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/css/styles.css` & `Dowell Mail-1.0.2/docs/_build/html/css/styles.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/emailapp.html` & `Dowell Mail-1.0.2/docs/_build/html/emailapp.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/genindex.html` & `Dowell Mail-1.0.2/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/index.html` & `Dowell Mail-1.0.2/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/maillib/home.html` & `Dowell Mail-1.0.2/docs/_build/html/maillib/home.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/maillib.html` & `Dowell Mail-1.0.2/docs/_build/html/maillib.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/maillib.migrations.html` & `Dowell Mail-1.0.2/docs/_build/html/maillib.migrations.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/maillib.tests.html` & `Dowell Mail-1.0.2/docs/_build/html/maillib.tests.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/modules.html` & `Dowell Mail-1.0.2/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/objects.inv` & `Dowell Mail-1.0.2/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/py-modindex.html` & `Dowell Mail-1.0.2/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/search.html` & `Dowell Mail-1.0.2/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/searchindex.js` & `Dowell Mail-1.0.2/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/static.html` & `Dowell Mail-1.0.2/docs/_build/html/static.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/html/templates.html` & `Dowell Mail-1.0.2/docs/_build/html/templates.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/LICRcyr2utf8.xdy` & `Dowell Mail-1.0.2/docs/_build/latex/LICRcyr2utf8.xdy`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/LICRlatin2utf8.xdy` & `Dowell Mail-1.0.2/docs/_build/latex/LICRlatin2utf8.xdy`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/LatinRules.xdy` & `Dowell Mail-1.0.2/docs/_build/latex/LatinRules.xdy`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/Makefile` & `Dowell Mail-1.0.2/docs/_build/latex/Makefile`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/dowell-mail.tex` & `Dowell Mail-1.0.2/docs/_build/latex/dowell-mail.tex`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/latexmkjarc` & `Dowell Mail-1.0.2/docs/_build/latex/latexmkjarc`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinx.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinx.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinx.xdy` & `Dowell Mail-1.0.2/docs/_build/latex/sphinx.xdy`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxhighlight.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxhighlight.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxhowto.cls` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxhowto.cls`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexadmonitions.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexadmonitions.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexcontainers.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexcontainers.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexgraphics.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexgraphics.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexindbibtoc.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexindbibtoc.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexlists.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexlists.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexliterals.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexliterals.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexnumfig.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexnumfig.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexobjects.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexobjects.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexshadowbox.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexshadowbox.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexstyleheadings.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexstyleheadings.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexstylepage.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexstylepage.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxlatexstyletext.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxlatexstyletext.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxlatextables.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxlatextables.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxmanual.cls` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxmanual.cls`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxmessages.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxmessages.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxoptionsgeometry.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxoptionsgeometry.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxoptionshyperref.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxoptionshyperref.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxpackageboxes.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxpackageboxes.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxpackagecyrillic.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxpackagecyrillic.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/_build/latex/sphinxpackagefootnote.sty` & `Dowell Mail-1.0.2/docs/_build/latex/sphinxpackagefootnote.sty`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/conf.py` & `Dowell Mail-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/emailapp.rst` & `Dowell Mail-1.0.2/docs/emailapp.rst`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/index.rst` & `Dowell Mail-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/maillib.rst` & `Dowell Mail-1.0.2/docs/maillib.rst`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/maillib.tests.rst` & `Dowell Mail-1.0.2/docs/maillib.tests.rst`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/make.bat` & `Dowell Mail-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/static.rst` & `Dowell Mail-1.0.2/docs/static.rst`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/docs/templates.rst` & `Dowell Mail-1.0.2/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/maillib/tests/test_urls.py` & `Dowell Mail-1.0.2/maillib/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/maillib/tests/test_views.py` & `Dowell Mail-1.0.2/maillib/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/maillib/urls.py` & `Dowell Mail-1.0.2/maillib/urls.py`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/maillib/views.py` & `Dowell Mail-1.0.2/maillib/views.py`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/setup.cfg` & `Dowell Mail-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6f77 656c 6c2d 6d61 696c 0d0a   = dowell-mail..
-00000020: 7665 7273 696f 6e20 3d20 312e 302e 310d  version = 1.0.1.
+00000020: 7665 7273 696f 6e20 3d20 312e 302e 320d  version = 1.0.2.
 00000030: 0a61 7574 686f 7220 3d20 4d61 7276 696e  .author = Marvin
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 206d 6172 7669 6e2e 7765 6b65 7361 4067   marvin.wekesa@g
 00000060: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000070: 7074 696f 6e20 3d20 446f 7765 6c6c 204d  ption = Dowell M
 00000080: 6169 6c20 5061 636b 6167 650d 0a6c 6f6e  ail Package..lon
 00000090: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description =
```

### Comparing `Dowell Mail-1.0.1/static/css/styles.css` & `Dowell Mail-1.0.2/static/css/styles.css`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/templates/_partials/base.html` & `Dowell Mail-1.0.2/templates/_partials/base.html`

 * *Files identical despite different names*

### Comparing `Dowell Mail-1.0.1/templates/maillib/home.html` & `Dowell Mail-1.0.2/templates/maillib/home.html`

 * *Files identical despite different names*

