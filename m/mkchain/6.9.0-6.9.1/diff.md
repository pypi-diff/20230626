# Comparing `tmp/mkchain-6.9.0-py3-none-any.whl.zip` & `tmp/mkchain-6.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9043 bytes, number of entries: 9
--rw-r--r--  2.0 unx      497 b- defN 22-Sep-16 20:31 tqchain/_version.py
--rw-r--r--  2.0 unx     1913 b- defN 22-Sep-16 20:31 tqchain/keys.py
--rw-r--r--  2.0 unx    12207 b- defN 22-Sep-16 20:31 tqchain/mkchain.py
--rw-r--r--  2.0 unx     1837 b- defN 22-Sep-16 20:31 tqchain/parameters.yaml
--rw-r--r--  2.0 unx     5003 b- defN 22-Sep-16 20:31 mkchain-6.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Sep-16 20:31 mkchain-6.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 22-Sep-16 20:31 mkchain-6.9.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 22-Sep-16 20:31 mkchain-6.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      695 b- defN 22-Sep-16 20:31 mkchain-6.9.0.dist-info/RECORD
-9 files, 22302 bytes uncompressed, 7851 bytes compressed:  64.8%
+Zip file size: 9166 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      497 b- defN 22-Oct-05 19:32 tqchain/_version.py
+-rw-r--r--  2.0 unx     1913 b- defN 22-Oct-05 19:32 tqchain/keys.py
+-rw-r--r--  2.0 unx    12207 b- defN 22-Oct-05 19:32 tqchain/mkchain.py
+-rw-r--r--  2.0 unx     2236 b- defN 22-Oct-05 19:32 tqchain/parameters.yaml
+-rw-r--r--  2.0 unx     5003 b- defN 22-Oct-05 19:32 mkchain-6.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Oct-05 19:32 mkchain-6.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 22-Oct-05 19:32 mkchain-6.9.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 22-Oct-05 19:32 mkchain-6.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      695 b- defN 22-Oct-05 19:32 mkchain-6.9.1.dist-info/RECORD
+9 files, 22701 bytes uncompressed, 7974 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: tqchain/mkchain.py
 Comment: 
 
 Filename: tqchain/parameters.yaml
 Comment: 
 
-Filename: mkchain-6.9.0.dist-info/METADATA
+Filename: mkchain-6.9.1.dist-info/METADATA
 Comment: 
 
-Filename: mkchain-6.9.0.dist-info/WHEEL
+Filename: mkchain-6.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: mkchain-6.9.0.dist-info/entry_points.txt
+Filename: mkchain-6.9.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: mkchain-6.9.0.dist-info/top_level.txt
+Filename: mkchain-6.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: mkchain-6.9.0.dist-info/RECORD
+Filename: mkchain-6.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tqchain/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2022-09-16T22:29:43+0200",
+ "date": "2022-10-05T12:30:29-0700",
  "dirty": false,
  "error": null,
- "full-revisionid": "cc8e0d5162bcccdac78be6206eb6459f5982f6b9",
- "version": "6.9.0"
+ "full-revisionid": "171d0ab26662f8b184bfaa04a5fa5524e6d91aa5",
+ "version": "6.9.1"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## tqchain/mkchain.py

```diff
@@ -185,15 +185,15 @@
             # Needs a quotedstring otherwise helm interprets "Y" as true and it does not work
             "env": {
                 "all": {"TEZOS_CLIENT_UNSAFE_DISABLE_DISCLAIMER": QuotedString("Y")}
             }
         },
         "protocols": [
             {
-                "command": "013-PtJakart",
+                "command": "014-PtKathma",
                 "vote": {"liquidity_baking_toggle_vote": "pass"},
             }
         ],
     }
 
     # preserve pre-existing values, if any (in case of scale-up)
     old_create_values = {}
@@ -291,15 +291,15 @@
 
     with open(
         f"{os.path.dirname(os.path.realpath(__file__))}/parameters.yaml", "r"
     ) as yaml_file:
         parametersYaml = yaml.safe_load(yaml_file)
         activation = {
             "activation": {
-                "protocol_hash": "PtJakart2xVj7pYXJBXrqHgd82rdkLey5ZeeGwDgPp9rhQUbSqY",
+                "protocol_hash": "PtKathmankSpLLDALzWw7CGD2j2MtyveTwboEYokqUCP4a1LxMg",
                 "protocol_parameters": parametersYaml,
             },
         }
 
     bootstrap_peers = args.bootstrap_peers if args.bootstrap_peers else []
 
     creation_constants = {
```

## tqchain/parameters.yaml

```diff
@@ -2,15 +2,15 @@
 blocks_per_cycle: 8
 blocks_per_commitment: 4
 blocks_per_stake_snapshot: 4
 cycles_per_voting_period: 1
 hard_gas_limit_per_operation: '1040000'
 hard_gas_limit_per_block: '5200000'
 proof_of_work_threshold: '-1'
-tokens_per_roll: '8000000000'
+tokens_per_roll: '6000000000'
 seed_nonce_revelation_tip: '125000'
 baking_reward_fixed_portion: '10000000'
 baking_reward_bonus_per_slot: '4286'
 endorsing_reward_per_slot: '2857'
 hard_storage_limit_per_operation: '60000'
 origination_size: 257
 cost_per_byte: '250'
@@ -33,26 +33,39 @@
 double_baking_punishment: "640000000"
 ratio_of_frozen_deposits_slashed_per_double_endorsement:
   numerator: 1
   denominator: 2
 cache_script_size: 100000000
 cache_stake_distribution_cycles: 8
 cache_sampler_state_cycles: 8
+nonce_revelation_threshold: 4
+vdf_difficulty: '100000'
 tx_rollup_enable: true
 tx_rollup_origination_size: 4000
 tx_rollup_hard_size_limit_per_inbox: 500000
 tx_rollup_hard_size_limit_per_message: 5000
-tx_rollup_max_withdrawals_per_batch: 15
 tx_rollup_commitment_bond: "10000000000"
 tx_rollup_finality_period: 10
 tx_rollup_max_inboxes_count: 15
 tx_rollup_withdraw_period: 10
 tx_rollup_max_messages_per_inbox: 1010
 tx_rollup_max_commitments_count: 30
 tx_rollup_cost_per_byte_ema_factor: 120
+tx_rollup_max_withdrawals_per_batch: 15
 tx_rollup_max_ticket_payload_size: 2048
 tx_rollup_rejection_max_proof_size: 30000
-tx_rollup_sunset_level: 17280
-sc_rollup_enable: false
+tx_rollup_sunset_level: 10000000
+dal_parametric:
+  feature_enable: true
+  number_of_slots: 256
+  number_of_shards: 2048
+  endorsement_lag: 2
+  availability_threshold: 50
+sc_rollup_enable: true
 sc_rollup_origination_size: 6314
 sc_rollup_challenge_window_in_blocks: 40
 sc_rollup_max_available_messages: 1000000
+sc_rollup_stake_amount: "32000000"
+sc_rollup_commitment_period_in_blocks: 20
+sc_rollup_max_lookahead_in_blocks: 30000
+sc_rollup_max_active_outbox_levels: 20160
+sc_rollup_max_outbox_messages_per_level: 100
```

## Comparing `mkchain-6.9.0.dist-info/METADATA` & `mkchain-6.9.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkchain
-Version: 6.9.0
+Version: 6.9.1
 Summary: A utility to generate k8s configs for a Tezos blockchain
 Home-page: https://github.com/oxheadalpha/tezos-k8s
 Author: TQ Tezos
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

