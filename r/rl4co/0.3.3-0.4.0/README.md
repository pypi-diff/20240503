# Comparing `tmp/rl4co-0.3.3.tar.gz` & `tmp/rl4co-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl4co-0.3.3.tar", last modified: Sun Mar  3 04:34:38 2024, max compression
+gzip compressed data, was "rl4co-0.4.0.tar", last modified: Fri May  3 11:06:18 2024, max compression
```

## Comparing `rl4co-0.3.3.tar` & `rl4co-0.4.0.tar`

### file list

```diff
@@ -1,165 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.265066 rl4co-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-03-03 04:34:33.000000 rl4co-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22769 2024-03-03 04:34:38.265066 rl4co-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-03-03 04:34:33.000000 rl4co-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-03-03 04:34:33.000000 rl4co-0.3.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.241066 rl4co-0.3.3/rl4co/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.241066 rl4co-0.3.3/rl4co/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/data/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/data/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.245066 rl4co-0.3.3/rl4co/envs/
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.245066 rl4co-0.3.3/rl4co/envs/common/
--rw-r--r--   0 runner    (1001) docker     (127)    11129 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/common/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.245066 rl4co-0.3.3/rl4co/envs/eda/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15197 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/eda/dpp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/eda/mdpp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.245066 rl4co-0.3.3/rl4co/envs/routing/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/routing/atsp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15133 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/routing/cvrp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/routing/cvrptw.py
--rw-r--r--   0 runner    (1001) docker     (127)    19489 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/routing/mpdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/routing/mtsp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14479 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/routing/op.py
--rw-r--r--   0 runner    (1001) docker     (127)    15971 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/routing/pctsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/routing/pdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/routing/sdvrp.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/routing/spctsp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14796 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/routing/svrp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/routing/tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.249066 rl4co-0.3.3/rl4co/envs/scheduling/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/scheduling/ffsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/envs/scheduling/smtwtp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.249066 rl4co-0.3.3/rl4co/models/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.249066 rl4co-0.3.3/rl4co/models/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/nn/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/nn/dec_strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.249066 rl4co-0.3.3/rl4co/models/nn/env_embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/nn/env_embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10070 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/nn/env_embeddings/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/nn/env_embeddings/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/nn/env_embeddings/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/nn/flash_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.249066 rl4co-0.3.3/rl4co/models/nn/graph/
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/nn/graph/attnnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/nn/graph/gcn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/nn/graph/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/nn/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/nn/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.249066 rl4co-0.3.3/rl4co/models/rl/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/rl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.249066 rl4co-0.3.3/rl4co/models/rl/common/
--rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/rl/common/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/rl/common/critic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.249066 rl4co-0.3.3/rl4co/models/rl/ppo/
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/rl/ppo/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.253066 rl4co-0.3.3/rl4co/models/rl/reinforce/
--rw-r--r--   0 runner    (1001) docker     (127)    10448 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/rl/reinforce/baselines.py
--rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/rl/reinforce/reinforce.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.253066 rl4co-0.3.3/rl4co/models/zoo/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.253066 rl4co-0.3.3/rl4co/models/zoo/active_search/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/active_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7585 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/active_search/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.253066 rl4co-0.3.3/rl4co/models/zoo/am/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/am/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/am/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/am/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.237066 rl4co-0.3.3/rl4co/models/zoo/common/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.253066 rl4co-0.3.3/rl4co/models/zoo/common/autoregressive/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/common/autoregressive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14798 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/common/autoregressive/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/common/autoregressive/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/common/autoregressive/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.253066 rl4co-0.3.3/rl4co/models/zoo/common/search/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/common/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/common/search/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.253066 rl4co-0.3.3/rl4co/models/zoo/eas/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/eas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/eas/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/eas/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/eas/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.257066 rl4co-0.3.3/rl4co/models/zoo/equity_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/equity_transformer/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/equity_transformer/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/equity_transformer/positional_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.257066 rl4co-0.3.3/rl4co/models/zoo/ham/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/ham/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18979 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/ham/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/ham/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/ham/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/ham/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.257066 rl4co-0.3.3/rl4co/models/zoo/matnet/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/matnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/matnet/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/matnet/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/matnet/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/matnet/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.257066 rl4co-0.3.3/rl4co/models/zoo/mdam/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/mdam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/mdam/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/mdam/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/mdam/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/mdam/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.257066 rl4co-0.3.3/rl4co/models/zoo/pomo/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/pomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/pomo/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/pomo/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.261067 rl4co-0.3.3/rl4co/models/zoo/ppo/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/ppo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/ppo/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/ppo/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.261067 rl4co-0.3.3/rl4co/models/zoo/ptrnet/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/ptrnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/ptrnet/critic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/ptrnet/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/ptrnet/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/ptrnet/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/ptrnet/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.261067 rl4co-0.3.3/rl4co/models/zoo/symnco/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/symnco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/symnco/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/symnco/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/models/zoo/symnco/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.261067 rl4co-0.3.3/rl4co/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13121 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/tasks/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/tasks/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.265066 rl4co-0.3.3/rl4co/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.265066 rl4co-0.3.3/rl4co/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/utils/callbacks/speed_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/utils/instantiators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/utils/lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/utils/optim_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/utils/param_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/utils/pylogger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/utils/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/utils/transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-03-03 04:34:33.000000 rl4co-0.3.3/rl4co/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.265066 rl4co-0.3.3/rl4co.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22769 2024-03-03 04:34:38.000000 rl4co-0.3.3/rl4co.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-03-03 04:34:38.000000 rl4co-0.3.3/rl4co.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 04:34:38.000000 rl4co-0.3.3/rl4co.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-03 04:34:38.000000 rl4co-0.3.3/rl4co.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-03 04:34:38.000000 rl4co-0.3.3/rl4co.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 04:34:38.265066 rl4co-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 04:34:38.265066 rl4co-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-03 04:34:33.000000 rl4co-0.3.3/tests/test_envs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-03 04:34:33.000000 rl4co-0.3.3/tests/test_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-03 04:34:33.000000 rl4co-0.3.3/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-03 04:34:33.000000 rl4co-0.3.3/tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-03 04:34:33.000000 rl4co-0.3.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.350594 rl4co-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-03 11:06:11.000000 rl4co-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-05-03 11:06:18.350594 rl4co-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-05-03 11:06:11.000000 rl4co-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-03 11:06:11.000000 rl4co-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.322593 rl4co-0.4.0/rl4co/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.322593 rl4co-0.4.0/rl4co/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/data/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/data/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.322593 rl4co-0.4.0/rl4co/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.322593 rl4co-0.4.0/rl4co/envs/common/
+-rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.326593 rl4co-0.4.0/rl4co/envs/eda/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/eda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.326593 rl4co-0.4.0/rl4co/envs/eda/dpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/eda/dpp/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/eda/dpp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/eda/dpp/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.326593 rl4co-0.4.0/rl4co/envs/eda/mdpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/eda/mdpp/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/eda/mdpp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/eda/mdpp/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.326593 rl4co-0.4.0/rl4co/envs/routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.326593 rl4co-0.4.0/rl4co/envs/routing/atsp/
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/atsp/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/atsp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/atsp/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.326593 rl4co-0.4.0/rl4co/envs/routing/cvrp/
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/cvrp/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/cvrp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/cvrp/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.326593 rl4co-0.4.0/rl4co/envs/routing/cvrptw/
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/cvrptw/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/cvrptw/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/cvrptw/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.326593 rl4co-0.4.0/rl4co/envs/routing/mdcpdp/
+-rw-r--r--   0 runner    (1001) docker     (127)    15355 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/mdcpdp/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/mdcpdp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/mdcpdp/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.326593 rl4co-0.4.0/rl4co/envs/routing/mpdp/
+-rw-r--r--   0 runner    (1001) docker     (127)    15592 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/mpdp/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/mpdp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/mpdp/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.330593 rl4co-0.4.0/rl4co/envs/routing/mtsp/
+-rw-r--r--   0 runner    (1001) docker     (127)     9114 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/mtsp/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/mtsp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/mtsp/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.330593 rl4co-0.4.0/rl4co/envs/routing/op/
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/op/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/op/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/op/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.330593 rl4co-0.4.0/rl4co/envs/routing/pctsp/
+-rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/pctsp/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/pctsp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/pctsp/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.330593 rl4co-0.4.0/rl4co/envs/routing/pdp/
+-rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/pdp/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/pdp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/pdp/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.330593 rl4co-0.4.0/rl4co/envs/routing/sdvrp/
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/sdvrp/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.330593 rl4co-0.4.0/rl4co/envs/routing/spctsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/spctsp/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.330593 rl4co-0.4.0/rl4co/envs/routing/svrp/
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/svrp/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/svrp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/svrp/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.330593 rl4co-0.4.0/rl4co/envs/routing/tsp/
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/tsp/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/tsp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/routing/tsp/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.330593 rl4co-0.4.0/rl4co/envs/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/scheduling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.330593 rl4co-0.4.0/rl4co/envs/scheduling/ffsp/
+-rw-r--r--   0 runner    (1001) docker     (127)    18822 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/scheduling/ffsp/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/scheduling/ffsp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/scheduling/ffsp/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.330593 rl4co-0.4.0/rl4co/envs/scheduling/smtwtp/
+-rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/scheduling/smtwtp/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/scheduling/smtwtp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/envs/scheduling/smtwtp/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.334593 rl4co-0.4.0/rl4co/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.334593 rl4co-0.4.0/rl4co/models/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.334593 rl4co-0.4.0/rl4co/models/common/constructive/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/common/constructive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.334593 rl4co-0.4.0/rl4co/models/common/constructive/autoregressive/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/common/constructive/autoregressive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/common/constructive/autoregressive/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/common/constructive/autoregressive/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/common/constructive/autoregressive/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10679 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/common/constructive/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.334593 rl4co-0.4.0/rl4co/models/common/constructive/nonautoregressive/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/common/constructive/nonautoregressive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/common/constructive/nonautoregressive/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/common/constructive/nonautoregressive/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/common/constructive/nonautoregressive/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.334593 rl4co-0.4.0/rl4co/models/common/improvement/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/common/improvement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.334593 rl4co-0.4.0/rl4co/models/common/transductive/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/common/transductive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/common/transductive/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.334593 rl4co-0.4.0/rl4co/models/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/nn/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.334593 rl4co-0.4.0/rl4co/models/nn/env_embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/nn/env_embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/nn/env_embeddings/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/nn/env_embeddings/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/nn/env_embeddings/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/nn/env_embeddings/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/nn/flash_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.338594 rl4co-0.4.0/rl4co/models/nn/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/nn/graph/attnnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/nn/graph/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/nn/graph/gnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/nn/graph/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/nn/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/nn/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.338594 rl4co-0.4.0/rl4co/models/rl/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/rl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.338594 rl4co-0.4.0/rl4co/models/rl/a2c/
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/rl/a2c/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.338594 rl4co-0.4.0/rl4co/models/rl/common/
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/rl/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/rl/common/critic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.338594 rl4co-0.4.0/rl4co/models/rl/ppo/
+-rw-r--r--   0 runner    (1001) docker     (127)    10347 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/rl/ppo/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.338594 rl4co-0.4.0/rl4co/models/rl/reinforce/
+-rw-r--r--   0 runner    (1001) docker     (127)    10810 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/rl/reinforce/baselines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/rl/reinforce/reinforce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.338594 rl4co-0.4.0/rl4co/models/zoo/
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.338594 rl4co-0.4.0/rl4co/models/zoo/active_search/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/active_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7580 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/active_search/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.338594 rl4co-0.4.0/rl4co/models/zoo/am/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/am/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/am/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/am/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/am/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/am/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.338594 rl4co-0.4.0/rl4co/models/zoo/amppo/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/amppo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/amppo/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.342594 rl4co-0.4.0/rl4co/models/zoo/deepaco/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/deepaco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9933 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/deepaco/antsystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/deepaco/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/deepaco/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/deepaco/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.342594 rl4co-0.4.0/rl4co/models/zoo/eas/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/eas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/eas/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/eas/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13667 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/eas/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.342594 rl4co-0.4.0/rl4co/models/zoo/equity_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/equity_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/equity_transformer/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/equity_transformer/positional_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.342594 rl4co-0.4.0/rl4co/models/zoo/ham/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/ham/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18988 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/ham/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/ham/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/ham/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/ham/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.342594 rl4co-0.4.0/rl4co/models/zoo/matnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/matnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/matnet/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/matnet/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/matnet/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/matnet/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.342594 rl4co-0.4.0/rl4co/models/zoo/mdam/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/mdam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/mdam/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/mdam/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/mdam/mha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/mdam/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/mdam/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.346594 rl4co-0.4.0/rl4co/models/zoo/nargnn/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/nargnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/nargnn/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/nargnn/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.346594 rl4co-0.4.0/rl4co/models/zoo/pomo/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/pomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/pomo/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.346594 rl4co-0.4.0/rl4co/models/zoo/ptrnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/ptrnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/ptrnet/critic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/ptrnet/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/ptrnet/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/ptrnet/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/ptrnet/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.346594 rl4co-0.4.0/rl4co/models/zoo/symnco/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/symnco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/symnco/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/symnco/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/models/zoo/symnco/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.346594 rl4co-0.4.0/rl4co/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/tasks/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/tasks/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.350594 rl4co-0.4.0/rl4co/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.350594 rl4co-0.4.0/rl4co/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/utils/callbacks/speed_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20683 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/utils/decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/utils/instantiators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/utils/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8006 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/utils/optim_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/utils/param_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/utils/pylogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/utils/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-05-03 11:06:11.000000 rl4co-0.4.0/rl4co/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.350594 rl4co-0.4.0/rl4co.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-05-03 11:06:18.000000 rl4co-0.4.0/rl4co.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-03 11:06:18.000000 rl4co-0.4.0/rl4co.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:06:18.000000 rl4co-0.4.0/rl4co.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-03 11:06:18.000000 rl4co-0.4.0/rl4co.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 11:06:18.000000 rl4co-0.4.0/rl4co.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:06:18.350594 rl4co-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:06:18.350594 rl4co-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-03 11:06:11.000000 rl4co-0.4.0/tests/test_envs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-03 11:06:11.000000 rl4co-0.4.0/tests/test_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-03 11:06:11.000000 rl4co-0.4.0/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-03 11:06:11.000000 rl4co-0.4.0/tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-03 11:06:11.000000 rl4co-0.4.0/tests/test_utils.py
```

### Comparing `rl4co-0.3.3/README.md` & `rl4co-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 <div align="center">
 
 
-<img src="https://github.com/ai4co/rl4co/assets/48984123/01a547b2-9722-4540-b0e1-9c12af094b15" style="width:40%">
-
+<div align="center">
+    <img src="https://raw.githubusercontent.com/ai4co/assets/main/svg/rl4co_animated_full.svg" alt="AI4CO Logo" style="width: 40%; height: auto;">
+</div>
 
 </br></br>
 
 
 <a href="https://pytorch.org/get-started/locally/"><img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white"></a>
 <a href="https://pytorchlightning.ai/"><img alt="Lightning" src="https://img.shields.io/badge/-Lightning-792ee5?logo=pytorchlightning&logoColor=white"></a>
 <a href="https://github.com/pytorch/rl"><img alt="base: TorchRL" src="https://img.shields.io/badge/base-TorchRL-red">
 <a href="https://hydra.cc/"><img alt="config: Hydra" src="https://img.shields.io/badge/config-Hydra-89b8cd"></a> [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Slack](https://img.shields.io/badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)
-![license](https://img.shields.io/badge/license-Apache%202.0-green.svg?) <a href="https://colab.research.google.com/github/ai4co/rl4co/blob/main/notebooks/1-quickstart.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a> [![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
+[![License: MIT](https://img.shields.io/badge/License-MIT-red.svg)](https://opensource.org/licenses/MIT) <a href="https://colab.research.google.com/github/ai4co/rl4co/blob/main/examples/1-quickstart.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a> [![PyPI](https://img.shields.io/pypi/v/rl4co?logo=pypi)](https://pypi.org/project/rl4co)
 [![Test](https://github.com/ai4co/rl4co/actions/workflows/tests.yml/badge.svg)](https://github.com/ai4co/rl4co/actions/workflows/tests.yml)
 
 [**Documentation**](https://rl4co.readthedocs.io/) |  [**Getting Started**](#getting-started) | [**Usage**](#usage) | [**Contributing**](#contributing) | [**Paper**](https://arxiv.org/abs/2306.17100) | [**Join Us**](#join-us)
 
 </div>
 
 ---
@@ -33,26 +34,27 @@
 - [TensorDict](https://github.com/pytorch-labs/tensordict): a library to easily handle heterogeneous data such as states, actions and rewards
 - [PyTorch Lightning](https://github.com/Lightning-AI/lightning): a lightweight PyTorch wrapper for high-performance AI research
 - [Hydra](https://github.com/facebookresearch/hydra): a framework for elegantly configuring complex applications
 
 ![RL4CO Overview](https://github.com/ai4co/rl4co/assets/34462374/4d9a670f-ab7c-4fc8-9135-82d17cb6d0ee)
 
 
-We provide several utilities and modularization. For autoregressive policies, we modularize reusable components such as _environment embeddings_ that can easily be swapped to [solve new problems](https://github.com/ai4co/rl4co/blob/main/notebooks/tutorials/2-creating-new-env-model.ipynb)
+We provide several utilities and modularization. For autoregressive policies, we modularize reusable components such as _environment embeddings_ that can easily be swapped to [solve new problems](https://github.com/ai4co/rl4co/blob/main/examples/3-creating-new-env-model.ipynb).
+
 ![RL4CO Policy](https://github.com/ai4co/rl4co/assets/48984123/ca88f159-d0b3-459e-8fd9-89799be9d1b0)
 
 ## Getting started
-<a href="https://colab.research.google.com/github/ai4co/rl4co/blob/main/notebooks/1-quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
+<a href="https://colab.research.google.com/github/ai4co/rl4co/blob/main/examples/1-quickstart.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>
 
 RL4CO is now available for installation on `pip`!
 ```bash
 pip install rl4co
 ```
 
-To get started, we recommend checking out our [quickstart notebook](notebooks/1-quickstart.ipynb) or the [minimalistic example](#minimalistic-example) below.
+To get started, we recommend checking out our [quickstart notebook](examples/1-quickstart.ipynb) or the [minimalistic example](#minimalistic-example) below.
 
 ### Install from source
 This command installs the bleeding edge `main` version, useful for staying up-to-date with the latest developments - for instance, if a bug has been fixed since the last official release but a new release hasn’t been rolled out yet:
 
 ```bash
 pip install -U git+https://github.com/ai4co/rl4co.git
 ```
@@ -73,25 +75,31 @@
 
 
 Train model with default configuration (AM on TSP environment):
 ```bash
 python run.py
 ```
 
+> [!TIP]
+> You may check out [this notebook](examples/advanced/1-hydra-config.ipynb) to get started with Hydra!
 
 <details>
-    <summary>Change experiment</summary>
+    <summary>Change experiment settings</summary>
 
-Train model with chosen experiment configuration from [configs/experiment/](configs/experiment/) (e.g. tsp/am, and environment with 42 cities)
+Train model with chosen experiment configuration from [configs/experiment/](configs/experiment/)
 ```bash
-python run.py experiment=routing/am env.num_loc=42
+python run.py experiment=routing/am env=tsp env.num_loc=50 model.optimizer_kwargs.lr=2e-4
 ```
+Here you may change the environment, e.g. with `env=cvrp` by command line or by modifying the corresponding experiment e.g. [configs/experiment/routing/am.yaml](configs/experiment/routing/am.yaml).
+
 </details>
 
 
+
+
 <details>
     <summary>Disable logging</summary>
 
 ```bash
 python run.py experiment=routing/am logger=none '~callbacks.learning_rate_monitor'
 ```
 Note that `~` is used to disable a callback that would need a logger.
@@ -99,15 +107,15 @@
 </details>
 
 
 <details>
     <summary>Create a sweep over hyperparameters (-m for multirun)</summary>
 
 ```bash
-python run.py -m experiment=routing/am  train.optimizer.lr=1e-3,1e-4,1e-5
+python run.py -m experiment=routing/am  model.optimizer.lr=1e-3,1e-4,1e-5
 ```
 </details>
 
 
 
 ### Minimalistic Example
 
@@ -188,12 +196,12 @@
 ## Join us
 [![Slack](https://img.shields.io/badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ)
 
 We invite you to join our AI4CO community, an open research group in Artificial Intelligence (AI) for Combinatorial Optimization (CO)!
 
 
 
-<p align="center">
-  <img width="30%" src="https://github.com/ai4co/rl4co/assets/48984123/2f1298ef-15e1-4a66-9741-78ee75938789">
-</p>
+<div align="center">
+    <img src="https://raw.githubusercontent.com/ai4co/assets/main/svg/ai4co_animated_full.svg" alt="AI4CO Logo" style="width: 30%; height: auto;">
+</div>
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-   [https://github.com/ai4co/rl4co/assets/48984123/01a547b2-9722-4540-b0e1-
- 9c12af094b15]_[_P_y_T_o_r_c_h_]_[_L_i_g_h_t_n_i_n_g_]_[_b_a_s_e_:_ _T_o_r_c_h_R_L_]_[_c_o_n_f_i_g_:_ _H_y_d_r_a_]_[_!_[_C_o_d_e_ _s_t_y_l_e_:
- _b_l_a_c_k_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_)_]_(_h_t_t_p_s_:_/_/
-   _g_i_t_h_u_b_._c_o_m_/_p_s_f_/_b_l_a_c_k_)_ _[_!_[_S_l_a_c_k_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_s_l_a_c_k_-_c_h_a_t_-
+                                 [AI4CO Logo]
+_[_P_y_T_o_r_c_h_]_[_L_i_g_h_t_n_i_n_g_]_[_b_a_s_e_:_ _T_o_r_c_h_R_L_]_[_c_o_n_f_i_g_:_ _H_y_d_r_a_]_[_!_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_(_h_t_t_p_s_:_/
+ _/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_p_s_f_/
+           _b_l_a_c_k_)_ _[_!_[_S_l_a_c_k_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_s_l_a_c_k_-_c_h_a_t_-
    _6_1_1_f_6_9_._s_v_g_?_l_o_g_o_=_s_l_a_c_k_)_]_(_h_t_t_p_s_:_/_/_j_o_i_n_._s_l_a_c_k_._c_o_m_/_t_/_r_l_4_c_o_/_s_h_a_r_e_d___i_n_v_i_t_e_/_z_t_-
-  _1_y_t_z_2_c_1_v_4_-_0_I_k_Q_8_N_Q_H_4_T_R_X_I_X_8_P_r_R_m_D_h_Q_)_ _!_[_l_i_c_e_n_s_e_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
-       _l_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_g_r_e_e_n_._s_v_g_?_)_ _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_[_!_[_P_y_P_I_]_(_h_t_t_p_s_:_/_/
-  _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_r_l_4_c_o_?_l_o_g_o_=_p_y_p_i_)_]_(_h_t_t_p_s_:_/_/_p_y_p_i_._o_r_g_/_p_r_o_j_e_c_t_/_r_l_4_c_o_)_ _[_!
- _[_T_e_s_t_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_i_4_c_o_/_r_l_4_c_o_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_t_e_s_t_s_._y_m_l_/_b_a_d_g_e_._s_v_g_)_]
-         _(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_i_4_c_o_/_r_l_4_c_o_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_t_e_s_t_s_._y_m_l_)_ 
-  _[_*_*_D_o_c_u_m_e_n_t_a_t_i_o_n_*_*_]_(_h_t_t_p_s_:_/_/_r_l_4_c_o_._r_e_a_d_t_h_e_d_o_c_s_._i_o_/_)_ _|_ _[_*_*_G_e_t_t_i_n_g_ _S_t_a_r_t_e_d_*_*_]
-_(_#_g_e_t_t_i_n_g_-_s_t_a_r_t_e_d_)_ _|_ _[_*_*_U_s_a_g_e_*_*_]_(_#_u_s_a_g_e_)_ _|_ _[_*_*_C_o_n_t_r_i_b_u_t_i_n_g_*_*_]_(_#_c_o_n_t_r_i_b_u_t_i_n_g_)_ _|_ 
-    _[_*_*_P_a_p_e_r_*_*_]_(_h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/_2_3_0_6_._1_7_1_0_0_)_ _|_ _[_*_*_J_o_i_n_ _U_s_*_*_]_(_#_j_o_i_n_-_u_s_)
+  _1_y_t_z_2_c_1_v_4_-_0_I_k_Q_8_N_Q_H_4_T_R_X_I_X_8_P_r_R_m_D_h_Q_)_ _[_!_[_L_i_c_e_n_s_e_:_ _M_I_T_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
+   _b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_r_e_d_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_o_p_e_n_s_o_u_r_c_e_._o_r_g_/_l_i_c_e_n_s_e_s_/_M_I_T_)_ _[_O_p_e_n_ _I_n
+    _C_o_l_a_b_]_[_!_[_P_y_P_I_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_r_l_4_c_o_?_l_o_g_o_=_p_y_p_i_)_]_(_h_t_t_p_s_:_/_/
+   _p_y_p_i_._o_r_g_/_p_r_o_j_e_c_t_/_r_l_4_c_o_)_ _[_!_[_T_e_s_t_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_i_4_c_o_/_r_l_4_c_o_/_a_c_t_i_o_n_s_/
+    _w_o_r_k_f_l_o_w_s_/_t_e_s_t_s_._y_m_l_/_b_a_d_g_e_._s_v_g_)_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_a_i_4_c_o_/_r_l_4_c_o_/_a_c_t_i_o_n_s_/
+  _w_o_r_k_f_l_o_w_s_/_t_e_s_t_s_._y_m_l_)_ _[_*_*_D_o_c_u_m_e_n_t_a_t_i_o_n_*_*_]_(_h_t_t_p_s_:_/_/_r_l_4_c_o_._r_e_a_d_t_h_e_d_o_c_s_._i_o_/_)_ _|_ 
+       _[_*_*_G_e_t_t_i_n_g_ _S_t_a_r_t_e_d_*_*_]_(_#_g_e_t_t_i_n_g_-_s_t_a_r_t_e_d_)_ _|_ _[_*_*_U_s_a_g_e_*_*_]_(_#_u_s_a_g_e_)_ _|_ 
+    _[_*_*_C_o_n_t_r_i_b_u_t_i_n_g_*_*_]_(_#_c_o_n_t_r_i_b_u_t_i_n_g_)_ _|_ _[_*_*_P_a_p_e_r_*_*_]_(_h_t_t_p_s_:_/_/_a_r_x_i_v_._o_r_g_/_a_b_s_/
+                     _2_3_0_6_._1_7_1_0_0_)_ _|_ _[_*_*_J_o_i_n_ _U_s_*_*_]_(_#_j_o_i_n_-_u_s_)
 --- RL4CO has been accepted as an oral presentation at the [NeurIPS 2023
 GLFrontiers Workshop](https://glfrontiers.github.io/)! ð --- An extensive
 Reinforcement Learning (RL) for Combinatorial Optimization (CO) benchmark. Our
 goal is to provide a unified framework for RL-based CO algorithms, and to
 facilitate reproducible research in this field, decoupling the science from the
 engineering. RL4CO is built upon: - [TorchRL](https://github.com/pytorch/rl):
 official PyTorch framework for RL algorithms and vectorized environments on
@@ -23,37 +24,41 @@
 Lightning](https://github.com/Lightning-AI/lightning): a lightweight PyTorch
 wrapper for high-performance AI research - [Hydra](https://github.com/
 facebookresearch/hydra): a framework for elegantly configuring complex
 applications ![RL4CO Overview](https://github.com/ai4co/rl4co/assets/34462374/
 4d9a670f-ab7c-4fc8-9135-82d17cb6d0ee) We provide several utilities and
 modularization. For autoregressive policies, we modularize reusable components
 such as _environment embeddings_ that can easily be swapped to [solve new
-problems](https://github.com/ai4co/rl4co/blob/main/notebooks/tutorials/2-
-creating-new-env-model.ipynb) ![RL4CO Policy](https://github.com/ai4co/rl4co/
-assets/48984123/ca88f159-d0b3-459e-8fd9-89799be9d1b0) ## Getting started _[_O_p_e_n
-_I_n_ _C_o_l_a_b_]RL4CO is now available for installation on `pip`! ```bash pip install
-rl4co ``` To get started, we recommend checking out our [quickstart notebook]
-(notebooks/1-quickstart.ipynb) or the [minimalistic example](#minimalistic-
-example) below. ### Install from source This command installs the bleeding edge
-`main` version, useful for staying up-to-date with the latest developments -
-for instance, if a bug has been fixed since the last official release but a new
-release hasnât been rolled out yet: ```bash pip install -U git+https://
-github.com/ai4co/rl4co.git ``` ### Local install and development If you want to
-develop RL4CO we recommend you to install it locally with `pip` in editable
-mode: ```bash git clone https://github.com/ai4co/rl4co && cd rl4co pip install
--e . ``` We recommend using a virtual environment such as `conda` to install
-`rl4co` locally. ## Usage Train model with default configuration (AM on TSP
-environment): ```bash python run.py ``` Change experiment Train model with
-chosen experiment configuration from [configs/experiment/](configs/experiment/
-) (e.g. tsp/am, and environment with 42 cities) ```bash python run.py
-experiment=routing/am env.num_loc=42 ``` Disable logging ```bash python run.py
-experiment=routing/am logger=none '~callbacks.learning_rate_monitor' ``` Note
-that `~` is used to disable a callback that would need a logger. Create a sweep
-over hyperparameters (-m for multirun) ```bash python run.py -
-m experiment=routing/am train.optimizer.lr=1e-3,1e-4,1e-5 ``` ### Minimalistic
+problems](https://github.com/ai4co/rl4co/blob/main/examples/3-creating-new-env-
+model.ipynb). ![RL4CO Policy](https://github.com/ai4co/rl4co/assets/48984123/
+ca88f159-d0b3-459e-8fd9-89799be9d1b0) ## Getting started _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]RL4CO
+is now available for installation on `pip`! ```bash pip install rl4co ``` To
+get started, we recommend checking out our [quickstart notebook](examples/1-
+quickstart.ipynb) or the [minimalistic example](#minimalistic-example) below.
+### Install from source This command installs the bleeding edge `main` version,
+useful for staying up-to-date with the latest developments - for instance, if a
+bug has been fixed since the last official release but a new release hasnât
+been rolled out yet: ```bash pip install -U git+https://github.com/ai4co/
+rl4co.git ``` ### Local install and development If you want to develop RL4CO we
+recommend you to install it locally with `pip` in editable mode: ```bash git
+clone https://github.com/ai4co/rl4co && cd rl4co pip install -e . ``` We
+recommend using a virtual environment such as `conda` to install `rl4co`
+locally. ## Usage Train model with default configuration (AM on TSP
+environment): ```bash python run.py ``` > [!TIP] > You may check out [this
+notebook](examples/advanced/1-hydra-config.ipynb) to get started with Hydra!
+Change experiment settings Train model with chosen experiment configuration
+from [configs/experiment/](configs/experiment/) ```bash python run.py
+experiment=routing/am env=tsp env.num_loc=50 model.optimizer_kwargs.lr=2e-4 ```
+Here you may change the environment, e.g. with `env=cvrp` by command line or by
+modifying the corresponding experiment e.g. [configs/experiment/routing/
+am.yaml](configs/experiment/routing/am.yaml). Disable logging ```bash python
+run.py experiment=routing/am logger=none '~callbacks.learning_rate_monitor' ```
+Note that `~` is used to disable a callback that would need a logger. Create a
+sweep over hyperparameters (-m for multirun) ```bash python run.py -
+m experiment=routing/am model.optimizer.lr=1e-3,1e-4,1e-5 ``` ### Minimalistic
 Example Here is a minimalistic example training the Attention Model with greedy
 rollout baseline on TSP in less than 30 lines of code: ```python from
 rl4co.envs import TSPEnv from rl4co.models import AttentionModel from
 rl4co.utils import RL4COTrainer # Environment, Model, and Lightning Module env
 = TSPEnv(num_loc=20) model = AttentionModel(env, baseline="rollout",
 train_data_size=100_000, test_data_size=10_000, optimizer_kwargs={'lr': 1e-4} )
 # Trainer trainer = RL4COTrainer(max_epochs=3) # Fit the model trainer.fit
@@ -80,9 +85,8 @@
 booktitle={NeurIPS 2023 Workshop: New Frontiers in Graph Learning}, year=
 {2023}, url={https://openreview.net/forum?id=YXSJxi8dOV}, note={\url{https://
 github.com/ai4co/rl4co}} } ``` ## Join us [![Slack](https://img.shields.io/
 badge/slack-chat-611f69.svg?logo=slack)](https://join.slack.com/t/rl4co/
 shared_invite/zt-1ytz2c1v4-0IkQ8NQH4TRXIX8PrRmDhQ) We invite you to join our
 AI4CO community, an open research group in Artificial Intelligence (AI) for
 Combinatorial Optimization (CO)!
-   [https://github.com/ai4co/rl4co/assets/48984123/2f1298ef-15e1-4a66-9741-
-                                 78ee75938789]
+                                 [AI4CO Logo]
```

### Comparing `rl4co-0.3.3/pyproject.toml` & `rl4co-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "License :: OSI Approved :: Apache Software License",
+    "License :: OSI Approved :: MIT License",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
```

### Comparing `rl4co-0.3.3/rl4co/data/dataset.py` & `rl4co-0.4.0/rl4co/data/dataset.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/data/generate_data.py` & `rl4co-0.4.0/rl4co/data/generate_data.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/data/transforms.py` & `rl4co-0.4.0/rl4co/data/transforms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import math
-
+from typing import Union
 import torch
 
 from tensordict.tensordict import TensorDict
 from torch import Tensor
 
 from rl4co.utils.ops import batchify
+from rl4co.utils.pylogger import get_pylogger
+
+
+log = get_pylogger(__name__)
 
 
 def dihedral_8_augmentation(xy: Tensor) -> Tensor:
     """
     Augmentation (x8) for grid-based data (x, y) as done in POMO.
     This is a Dihedral group of order 8 (rotations and reflections)
     https://en.wikipedia.org/wiki/Examples_of_groups#dihedral_group_of_order_8
@@ -79,58 +83,68 @@
     # set phi to 0 for first , i.e. no augmentation as in SymNCO
     if not first_augment:
         phi[: xy.shape[0] // num_augment] = 0.0
     x, y = xy[..., [0]], xy[..., [1]]
     return symmetric_transform(x, y, phi[:, None, None])
 
 
-def env_aug_feats(env_name: str = None):
-    """What features to augment for a given environment
-    Usually, locs already includes depot, so we don't need to augment depot
-    """
-    return ["locs"]
-
-
 def min_max_normalize(x):
     return (x - x.min()) / (x.max() - x.min())
 
 
+def get_augment_function(augment_fn: Union[str, callable]):
+    if callable(augment_fn):
+        return augment_fn
+    if augment_fn == "dihedral8":
+        return dihedral_8_augmentation_wrapper
+    if augment_fn == "symmetric":
+        return symmetric_augmentation
+    raise ValueError(f"Unknown augment_fn: {augment_fn}. Available options: 'symmetric', 'dihedral8' or a custom callable")
+
+
 class StateAugmentation(object):
     """Augment state by N times via symmetric rotation/reflection transform
 
     Args:
-        env_name: environment name
         num_augment: number of augmentations
-        use_dihedral_8: whether to use dihedral_8_augmentation.  If True, then num_augment must be 8
+        augment_fn: augmentation function to use, e.g. 'symmetric' (default) or 'dihedral8', if callable, 
+            then use the function directly. If 'dihedral8', then num_augment must be 8
+        first_aug_identity: whether to augment the first data point too
         normalize: whether to normalize the augmented data
         feats: list of features to augment
     """
 
     def __init__(
         self,
-        env_name: str = None,
         num_augment: int = 8,
-        use_dihedral_8: bool = False,
+        augment_fn: Union[str, callable] = 'symmetric', 
+        first_aug_identity: bool = True,
         normalize: bool = False,
         feats: list = None,
     ):
+        self.augmentation = get_augment_function(augment_fn)
         assert not (
-            use_dihedral_8 and num_augment != 8
-        ), "If `use_dihedral_8` is True, then num_augment must be 8"
-        if use_dihedral_8:
-            self.augmentation = dihedral_8_augmentation_wrapper
-        else:
-            self.augmentation = symmetric_augmentation
+            self.augmentation == dihedral_8_augmentation_wrapper and num_augment != 8
+        ), "When using the `dihedral8` augmentation function, then num_augment must be 8"
 
-        self.feats = env_aug_feats(env_name) if feats is None else feats
+        if feats is None:
+            log.info("Features not passed, defaulting to 'locs'")
+            self.feats = ["locs"]
+        else:
+            self.feats = feats
         self.num_augment = num_augment
         self.normalize = normalize
+        self.first_aug_identity = first_aug_identity
 
     def __call__(self, td: TensorDict) -> TensorDict:
         td_aug = batchify(td, self.num_augment)
         for feat in self.feats:
+            if not self.first_aug_identity:
+                init_aug_feat = td_aug[feat][list(td.size()), 0].clone()
             aug_feat = self.augmentation(td_aug[feat], self.num_augment)
-            td_aug[feat] = aug_feat
             if self.normalize:
-                td_aug[feat] = min_max_normalize(td_aug[feat])
+                aug_feat = min_max_normalize(aug_feat)
+            if not self.first_aug_identity:
+                aug_feat[list(td.size()), 0] = init_aug_feat
+            td_aug[feat] = aug_feat
 
         return td_aug
```

### Comparing `rl4co-0.3.3/rl4co/data/utils.py` & `rl4co-0.4.0/rl4co/data/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,25 @@
     """
     x = np.load(filename)
     x_dict = dict(x)
     batch_size = x_dict[list(x_dict.keys())[0]].shape[0]
     return TensorDict(x_dict, batch_size=batch_size)
 
 
+def save_tensordict_to_npz(tensordict, filename, compress: bool = False):
+    """Save a TensorDict to a npz file
+    We assume that the TensorDict contains a dictionary of tensors
+    """
+    x_dict = {k: v.numpy() for k, v in tensordict.items()}
+    if compress:
+        np.savez_compressed(filename, **x_dict)
+    else:
+        np.savez(filename, **x_dict)
+
+
 def check_extension(filename, extension=".npz"):
     """Check that filename has extension, otherwise add it"""
     if os.path.splitext(filename)[1] != extension:
         return filename + extension
     return filename
```

### Comparing `rl4co-0.3.3/rl4co/envs/__init__.py` & `rl4co-0.4.0/rl4co/envs/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     OPEnv,
     PCTSPEnv,
     PDPEnv,
     SDVRPEnv,
     SVRPEnv,
     SPCTSPEnv,
     TSPEnv,
+    MDCPDPEnv,
 )
 
 # Scheduling
 from rl4co.envs.scheduling import FFSPEnv, SMTWTPEnv
 
 # Register environments
 ENV_REGISTRY = {
@@ -35,14 +36,15 @@
     "pctsp": PCTSPEnv,
     "pdp": PDPEnv,
     "sdvrp": SDVRPEnv,
     "svrp": SVRPEnv,
     "spctsp": SPCTSPEnv,
     "tsp": TSPEnv,
     "smtwtp": SMTWTPEnv,
+    "mdcpdp": MDCPDPEnv,
 }
 
 
 def get_env(env_name: str, *args, **kwargs) -> RL4COEnvBase:
     """Get environment by name.
 
     Args:
```

### Comparing `rl4co-0.3.3/rl4co/envs/common/base.py` & `rl4co-0.4.0/rl4co/envs/common/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import abc
+
 from os.path import join as pjoin
 from typing import Iterable, Optional
 
 import torch
 
 from tensordict.tensordict import TensorDict
 from torchrl.envs import EnvBase
 
 from rl4co.data.dataset import TensorDictDataset
 from rl4co.data.utils import load_npz_to_tensordict
+from rl4co.utils.ops import get_num_starts, select_start_nodes
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
-class RL4COEnvBase(EnvBase):
+class RL4COEnvBase(EnvBase, metaclass=abc.ABCMeta):
     """Base class for RL4CO environments based on TorchRL EnvBase.
     The environment has the usual methods for stepping, resetting, and getting the specifications of the environment
     that shoud be implemented by the subclasses of this class.
     It also has methods for getting the reward, action mask, and checking the validity of the solution, and
     for generating and loading the datasets (supporting multiple dataloaders as well for validation and testing).
 
     Args:
@@ -122,14 +125,24 @@
             # Default: just return the TensorDict without farther checks etc is faster
             td = self._step(td)
             return {"next": td}
         else:
             # Since we simplify the syntax
             return self._torchrl_step(td)
 
+    def reset(self, td: Optional[TensorDict] = None, batch_size = None) -> TensorDict:
+        """Reset function to call at the beginning of each episode"""
+        if batch_size is None:
+            batch_size = self.batch_size if td is None else td.batch_size
+        if td is None or td.is_empty():
+            td = self.generator(batch_size=batch_size)
+        batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
+        self.to(td.device)
+        return super().reset(td, batch_size=batch_size)
+
     def _torchrl_step(self, td: TensorDict) -> TensorDict:
         """See :meth:`super().step` for more details.
         This is the usual way to do it in TorchRL, but inefficient in our case
 
         Note:
             Here we clone the TensorDict to avoid recursion error, since we allow
             for directly updating the TensorDict in the step function
@@ -143,40 +156,57 @@
         )  # NOTE: we clone to avoid recursion error
         next_tensordict = self._step_proc_data(next_tensordict)
         if next_preset is not None:
             next_tensordict.update(next_preset.exclude(*next_tensordict.keys(True, True)))
         td.set("next", next_tensordict)
         return td
 
+    @abc.abstractmethod
     def _step(self, td: TensorDict) -> TensorDict:
         """Step function to call at each step of the episode containing an action.
         Gives the next observation, reward, done
         """
         raise NotImplementedError
 
+    @abc.abstractmethod
     def _reset(self, td: Optional[TensorDict] = None, batch_size=None) -> TensorDict:
         """Reset function to call at the beginning of each episode"""
         raise NotImplementedError
 
     def _make_spec(self, td_params: TensorDict = None):
         """Make the specifications of the environment (observation, action, reward, done)"""
         raise NotImplementedError
 
     def get_reward(self, td, actions) -> TensorDict:
         """Function to compute the reward. Can be called by the agent to compute the reward of the current state
         This is faster than calling step() and getting the reward from the returned TensorDict at each time for CO tasks
         """
+        if self.check_solution:
+            self.check_solution_validity(td, actions)
+        return self._get_reward(td, actions)
+    
+    @abc.abstractmethod
+    def _get_reward(self, td, actions) -> TensorDict:
+        """Function to compute the reward. Can be called by the agent to compute the reward of the current state
+        This is faster than calling step() and getting the reward from the returned TensorDict at each time for CO tasks
+        """
         raise NotImplementedError
 
     def get_action_mask(self, td: TensorDict) -> torch.Tensor:
         """Function to compute the action mask (feasible actions) for the current state
         Action mask is 1 if the action is feasible, 0 otherwise
         """
         raise NotImplementedError
 
+    def get_num_starts(self, td):
+        return get_num_starts(td, self.name)
+
+    def select_start_nodes(self, td, num_starts):
+        return select_start_nodes(td, self, num_starts)
+
     def check_solution_validity(self, td, actions) -> TensorDict:
         """Function to check whether the solution is valid. Can be called by the agent to check the validity of the current state
         This is called with the full solution (i.e. all actions) at the end of the episode
         """
         raise NotImplementedError
 
     def dataset(self, batch_size=[], phase="train", filename=None):
@@ -185,15 +215,15 @@
         """
         if filename is not None:
             log.info(f"Overriding dataset filename from {filename}")
         f = getattr(self, f"{phase}_file") if filename is None else filename
         if f is None:
             if phase != "train":
                 log.warning(f"{phase}_file not set. Generating dataset instead")
-            td = self.generate_data(batch_size)
+            td = self.generator(batch_size)
         else:
             log.info(f"Loading {phase} dataset from {f}")
             if phase == "train":
                 log.warning(
                     "Loading training dataset from file. This may not be desired in RL since "
                     "the dataset is fixed and the agent will not be able to explore new states"
                 )
@@ -207,22 +237,18 @@
                 else:
                     td = self.load_data(f, batch_size)
             except FileNotFoundError:
                 log.error(
                     f"Provided file name {f} not found. Make sure to provide a file in the right path first or "
                     f"unset {phase}_file to generate data automatically instead"
                 )
-                td = self.generate_data(batch_size)
+                td = self.generator(batch_size)
 
         return self.dataset_cls(td)
 
-    def generate_data(self, batch_size):
-        """Dataset generation"""
-        raise NotImplementedError
-
     def transform(self):
         """Used for converting TensorDict variables (such as with torch.cat) efficiently
         https://pytorch.org/rl/reference/generated/torchrl.envs.transforms.Transform.html
         By default, we do not need to transform the environment since we use specific embeddings
         """
         return self
```

### Comparing `rl4co-0.3.3/rl4co/envs/routing/atsp.py` & `rl4co-0.4.0/rl4co/envs/routing/cvrp/env.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,223 +6,230 @@
 from torchrl.data import (
     BoundedTensorSpec,
     CompositeSpec,
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
+from rl4co.data.utils import load_npz_to_tensordict
 from rl4co.envs.common.base import RL4COEnvBase
-from rl4co.envs.common.utils import batch_to_scalar
+from rl4co.utils.ops import gather_by_index, get_tour_length
 from rl4co.utils.pylogger import get_pylogger
 
+from .generator import CVRPGenerator
+from .render import render
+
 log = get_pylogger(__name__)
 
 
-class ATSPEnv(RL4COEnvBase):
-    """
-    Asymmetric Traveling Salesman Problem environment
-    At each step, the agent chooses a city to visit. The reward is 0 unless the agent visits all the cities.
+class CVRPEnv(RL4COEnvBase):
+    """Capacitated Vehicle Routing Problem (CVRP) environment.
+    At each step, the agent chooses a customer to visit depending on the current location and the remaining capacity.
+    When the agent visits a customer, the remaining capacity is updated. If the remaining capacity is not enough to
+    visit any customer, the agent must go back to the depot. The reward is 0 unless the agent visits all the cities.
     In that case, the reward is (-)length of the path: maximizing the reward is equivalent to minimizing the path length.
-    Unlike the TSP, the distance matrix is asymmetric, i.e., the distance from A to B is not necessarily the same as the distance from B to A.
+
+    Observations:
+        - location of the depot.
+        - locations and demand of each customer.
+        - current location of the vehicle.
+        - the remaining customer of the vehicle,
+
+    Constraints:
+        - the tour starts and ends at the depot.
+        - each customer must be visited exactly once.
+        - the vehicle cannot visit customers exceed the remaining capacity.
+        - the vehicle can return to the depot to refill the capacity.
+
+    Finish Condition:
+        - the vehicle has visited all customers and returned to the depot.
+
+    Reward:
+        - (minus) the negative length of the path.
 
     Args:
-        num_loc: number of locations (cities) in the TSP
-        td_params: parameters of the environment
-        seed: seed for the environment
-        device: device to use.  Generally, no need to set as tensors are updated on the fly
+        generator: CVRPGenerator instance as the data generator
+        generator_params: parameters for the generator
     """
 
-    name = "atsp"
+    name = "cvrp"
 
     def __init__(
         self,
-        num_loc: int = 10,
-        min_dist: float = 0,
-        max_dist: float = 1,
-        tmat_class: bool = True,
-        td_params: TensorDict = None,
+        generator: CVRPGenerator = None,
+        generator_params: dict = {},
         **kwargs,
     ):
         super().__init__(**kwargs)
-        self.num_loc = num_loc
-        self.min_dist = min_dist
-        self.max_dist = max_dist
-        self.tmat_class = tmat_class
-        self._make_spec(td_params)
-
-    @staticmethod
-    def _step(td: TensorDict) -> TensorDict:
-        current_node = td["action"]
-        first_node = current_node if batch_to_scalar(td["i"]) == 0 else td["first_node"]
-
-        # Set not visited to 0 (i.e., we visited the node)
-        available = td["action_mask"].scatter(
-            -1, current_node.unsqueeze(-1).expand_as(td["action_mask"]), 0
-        )
+        if generator is None:
+            generator = CVRPGenerator(**generator_params)
+        self.generator = generator
+        self._make_spec(self.generator)
+
+    def _step(self, td: TensorDict) -> TensorDict:
+        current_node = td["action"][:, None]  # Add dimension for step
+        n_loc = td["demand"].size(-1)  # Excludes depot
+
+        # Not selected_demand is demand of first node (by clamp) so incorrect for nodes that visit depot!
+        selected_demand = gather_by_index(
+            td["demand"], torch.clamp(current_node - 1, 0, n_loc - 1), squeeze=False
+        )
+
+        # Increase capacity if depot is not visited, otherwise set to 0
+        used_capacity = (td["used_capacity"] + selected_demand) * (
+            current_node != 0
+        ).float()
+
+        # Note: here we do not subtract one as we have to scatter so the first column allows scattering depot
+        # Add one dimension since we write a single value
+        visited = td["visited"].scatter(-1, current_node[..., None], 1)
 
-        # We are done there are no unvisited locations
-        done = torch.count_nonzero(available, dim=-1) <= 0
-
-        # The reward is calculated outside via get_reward for efficiency, so we set it to 0 here
+        # SECTION: get done
+        done = visited.sum(-1) == visited.size(-1)
         reward = torch.zeros_like(done)
 
         td.update(
             {
-                "first_node": first_node,
                 "current_node": current_node,
-                "i": td["i"] + 1,
-                "action_mask": available,
+                "used_capacity": used_capacity,
+                "visited": visited,
                 "reward": reward,
                 "done": done,
-            },
+            }
         )
+        td.set("action_mask", self.get_action_mask(td))
         return td
 
-    def _reset(self, td: Optional[TensorDict] = None, batch_size=None) -> TensorDict:
-        # Initialize distance matrix
-        cost_matrix = (
-            td["cost_matrix"] if td is not None else None
-        )  # dm = distance matrix
-        if batch_size is None:
-            batch_size = (
-                self.batch_size if cost_matrix is None else cost_matrix.shape[:-2]
-            )
-        device = cost_matrix.device if cost_matrix is not None else self.device
-        self.to(device)
-        if cost_matrix is None:
-            cost_matrix = self.generate_data(batch_size=batch_size).to(device)[
-                "cost_matrix"
-            ]
-
-        # Other variables
-        current_node = torch.zeros((*batch_size, 1), dtype=torch.int64, device=device)
-        available = torch.ones(
-            (*batch_size, self.num_loc), dtype=torch.bool, device=device
-        )  # 1 means not visited, i.e. action is allowed
-        i = torch.zeros((*batch_size, 1), dtype=torch.int64, device=device)
+    def _reset(
+        self,
+        td: Optional[TensorDict] = None,
+        batch_size: Optional[list] = None,
+    ) -> TensorDict:
+        device = td.device
 
-        return TensorDict(
+        # Create reset TensorDict
+        td_reset = TensorDict(
             {
-                "cost_matrix": cost_matrix,
-                "first_node": current_node,
-                "current_node": current_node,
-                "i": i,
-                "action_mask": available,
+                "locs": torch.cat((td["depot"][:, None, :], td["locs"]), -2),
+                "demand": td["demand"],
+                "current_node": torch.zeros(
+                    *batch_size, 1, dtype=torch.long, device=device
+                ),
+                "used_capacity": torch.zeros((*batch_size, 1), device=device),
+                "vehicle_capacity": torch.full(
+                    (*batch_size, 1), self.generator.vehicle_capacity, device=device
+                ),
+                "visited": torch.zeros(
+                    (*batch_size, 1, td["locs"].shape[-2] + 1),
+                    dtype=torch.uint8,
+                    device=device,
+                ),
             },
             batch_size=batch_size,
         )
+        td_reset.set("action_mask", self.get_action_mask(td_reset))
+        return td_reset
 
-    def _make_spec(self, td_params: TensorDict = None):
+    @staticmethod
+    def get_action_mask(td: TensorDict) -> torch.Tensor:
+        # For demand steps_dim is inserted by indexing with id, for used_capacity insert node dim for broadcasting
+        exceeds_cap = (
+            td["demand"][:, None, :] + td["used_capacity"][..., None] > td["vehicle_capacity"][..., None]
+        )
+
+        # Nodes that cannot be visited are already visited or too much demand to be served now
+        mask_loc = td["visited"][..., 1:].to(exceeds_cap.dtype) | exceeds_cap
+
+        # Cannot visit the depot if just visited and still unserved nodes
+        mask_depot = (td["current_node"] == 0) & ((mask_loc == 0).int().sum(-1) > 0)
+        return ~torch.cat((mask_depot[..., None], mask_loc), -1).squeeze(-2)
+
+    def _get_reward(self, td: TensorDict, actions: TensorDict) -> TensorDict:
+        # Gather dataset in order of tour
+        batch_size = td["locs"].shape[0]
+        depot = td["locs"][..., 0:1, :]
+        locs_ordered = torch.cat(
+            [
+                depot,
+                gather_by_index(td["locs"], actions).reshape(
+                    [batch_size, actions.size(-1), 2]
+                ),
+            ],
+            dim=1,
+        )
+        return -get_tour_length(locs_ordered)
+
+    @staticmethod
+    def check_solution_validity(td: TensorDict, actions: torch.Tensor):
+        """Check that solution is valid: nodes are not visited twice except depot and capacity is not exceeded"""
+        # Check if tour is valid, i.e. contain 0 to n-1
+        batch_size, graph_size = td["demand"].size()
+        sorted_pi = actions.data.sort(1)[0]
+
+        # Sorting it should give all zeros at front and then 1...n
+        assert (
+            torch.arange(1, graph_size + 1, out=sorted_pi.data.new())
+            .view(1, -1)
+            .expand(batch_size, graph_size)
+            == sorted_pi[:, -graph_size:]
+        ).all() and (sorted_pi[:, :-graph_size] == 0).all(), "Invalid tour"
+
+        # Visiting depot resets capacity so we add demand = -capacity (we make sure it does not become negative)
+        demand_with_depot = torch.cat((-td["vehicle_capacity"], td["demand"]), 1)
+        d = demand_with_depot.gather(1, actions)
+
+        used_cap = torch.zeros_like(td["demand"][:, 0])
+        for i in range(actions.size(1)):
+            used_cap += d[
+                :, i
+            ]  # This will reset/make capacity negative if i == 0, e.g. depot visited
+            # Cannot use less than 0
+            used_cap[used_cap < 0] = 0
+            assert (
+                used_cap <= td["vehicle_capacity"] + 1e-5
+            ).all(), "Used more than capacity"
+
+    @staticmethod
+    def load_data(fpath, batch_size=[]):
+        """Dataset loading from file
+        Normalize demand by capacity to be in [0, 1]
+        """
+        td_load = load_npz_to_tensordict(fpath)
+        td_load.set("demand", td_load["demand"] / td_load["capacity"][:, None])
+        return td_load
+
+    def _make_spec(self, generator: CVRPGenerator):
         self.observation_spec = CompositeSpec(
-            cost_matrix=BoundedTensorSpec(
-                low=self.min_dist,
-                high=self.max_dist,
-                shape=(self.num_loc, self.num_loc),
+            locs=BoundedTensorSpec(
+                low=generator.min_loc,
+                high=generator.max_loc,
+                shape=(generator.num_loc + 1, 2),
                 dtype=torch.float32,
             ),
-            first_node=UnboundedDiscreteTensorSpec(
-                shape=(1),
-                dtype=torch.int64,
-            ),
             current_node=UnboundedDiscreteTensorSpec(
                 shape=(1),
                 dtype=torch.int64,
             ),
-            i=UnboundedDiscreteTensorSpec(
-                shape=(1),
-                dtype=torch.int64,
+            demand=BoundedTensorSpec(
+                low=-generator.capacity,
+                high=generator.max_demand,
+                shape=(generator.num_loc + 1, 1),
+                dtype=torch.float32,
             ),
             action_mask=UnboundedDiscreteTensorSpec(
-                shape=(self.num_loc),
+                shape=(generator.num_loc + 1, 1),
                 dtype=torch.bool,
             ),
             shape=(),
         )
         self.action_spec = BoundedTensorSpec(
             shape=(1,),
             dtype=torch.int64,
             low=0,
-            high=self.num_loc,
+            high=generator.num_loc + 1,
         )
         self.reward_spec = UnboundedContinuousTensorSpec(shape=(1,))
         self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
 
-    def get_reward(self, td, actions) -> TensorDict:
-        distance_matrix = td["cost_matrix"]
-        assert (
-            torch.arange(actions.size(1), out=actions.data.new())
-            .view(1, -1)
-            .expand_as(actions)
-            == actions.data.sort(1)[0]
-        ).all(), "Invalid tour"
-
-        # Get indexes of tour edges
-        nodes_src = actions
-        nodes_tgt = torch.roll(actions, 1, dims=1)
-        batch_idx = torch.arange(
-            distance_matrix.shape[0], device=distance_matrix.device
-        ).unsqueeze(1)
-        # return negative tour length
-        return -distance_matrix[batch_idx, nodes_src, nodes_tgt].sum(-1)
-
-    def generate_data(self, batch_size) -> TensorDict:
-        # Generate distance matrices inspired by the reference MatNet (Kwon et al., 2021)
-        # We satifsy the triangle inequality (TMAT class) in a batch
-        batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
-        dms = (
-            torch.rand((*batch_size, self.num_loc, self.num_loc), generator=self.rng)
-            * (self.max_dist - self.min_dist)
-            + self.min_dist
-        )
-        dms[..., torch.arange(self.num_loc), torch.arange(self.num_loc)] = 0
-        log.info("Using TMAT class (triangle inequality): {}".format(self.tmat_class))
-        if self.tmat_class:
-            while True:
-                old_dms = dms.clone()
-                dms, _ = (
-                    dms[..., :, None, :] + dms[..., None, :, :].transpose(-2, -1)
-                ).min(dim=-1)
-                if (dms == old_dms).all():
-                    break
-        return TensorDict({"cost_matrix": dms}, batch_size=batch_size)
-
     @staticmethod
-    def render(td, actions=None, ax=None):
-        try:
-            import networkx as nx
-        except ImportError:
-            log.warn(
-                "Networkx is not installed. Please install it with `pip install networkx`"
-            )
-            return
-
-        td = td.detach().cpu()
-        if actions is None:
-            actions = td.get("action", None)
-
-        # if batch_size greater than 0 , we need to select the first batch element
-        if td.batch_size != torch.Size([]):
-            td = td[0]
-            actions = actions[0]
-
-        src_nodes = actions
-        tgt_nodes = torch.roll(actions, 1, dims=0)
-
-        # Plot with networkx
-        G = nx.DiGraph(td["cost_matrix"].numpy())
-        pos = nx.spring_layout(G)
-        nx.draw(
-            G,
-            pos,
-            with_labels=True,
-            node_color="skyblue",
-            node_size=800,
-            edge_color="white",
-        )
-
-        # draw edges src_nodes -> tgt_nodes
-        edgelist = [
-            (src_nodes[i].item(), tgt_nodes[i].item()) for i in range(len(src_nodes))
-        ]
-        nx.draw_networkx_edges(
-            G, pos, edgelist=edgelist, width=2, alpha=1, edge_color="black"
-        )
+    def render(td: TensorDict, actions: torch.Tensor=None, ax = None):
+        return render(td, actions, ax)
```

### Comparing `rl4co-0.3.3/rl4co/envs/routing/cvrptw.py` & `rl4co-0.4.0/rl4co/envs/routing/cvrptw/env.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,177 +4,109 @@
 from tensordict.tensordict import TensorDict
 from torchrl.data import (
     BoundedTensorSpec,
     CompositeSpec,
     UnboundedContinuousTensorSpec,
 )
 
-from rl4co.envs.routing.cvrp import CVRPEnv, CAPACITIES
+from rl4co.envs.routing.cvrp.env import CVRPEnv
+from rl4co.envs.routing.cvrp.generator import CAPACITIES
 from rl4co.utils.ops import gather_by_index, get_distance
 from rl4co.data.utils import (
     load_npz_to_tensordict,
     load_solomon_instance,
     load_solomon_solution,
 )
 
+from ..cvrp.generator import CVRPGenerator
+from .generator import CVRPTWGenerator
+from .render import render
+
 
 class CVRPTWEnv(CVRPEnv):
     """Capacitated Vehicle Routing Problem with Time Windows (CVRPTW) environment.
-    Inherits from the CVRPEnv class in which capacities are considered.
+    Inherits from the CVRPEnv class in which customers are considered.
     Additionally considers time windows within which a service has to be started.
 
+    Observations:
+        - location of the depot.
+        - locations and demand of each customer.
+        - current location of the vehicle.
+        - the remaining customer of the vehicle.
+        - the current time.
+        - service durations of each location.
+        - time windows of each location.
+
+    Constraints:
+        - the tour starts and ends at the depot.
+        - each customer must be visited exactly once.
+        - the vehicle cannot visit customers exceed the remaining customer.
+        - the vehicle can return to the depot to refill the customer.
+        - the vehicle must start the service within the time window of each location.
+
+    Finish Condition:
+        - the vehicle has visited all customers and returned to the depot.
+
+    Reward:
+        - (minus) the negative length of the path.
+
     Args:
-        num_loc (int): number of locations (cities) in the VRP, without the depot. (e.g. 10 means 10 locs + 1 depot)
-        min_loc (float): minimum value for the location coordinates
-        max_loc (float): maximum value for the location coordinates. Defaults to 150.
-        min_demand (float): minimum value for the demand of each customer
-        max_demand (float): maximum value for the demand of each customer
-        max_time (int): maximum time for the environment. Defaults to 480.
-        vehicle_capacity (float): capacity of the vehicle
-        capacity (float): capacity of the vehicle
-        scale (bool): if True, the time windows and service durations are scaled to [0, 1]. Defaults to False.
-        td_params: parameters of the environment
+        generator: CVRPTWGenerator instance as the data generator
+        generator_params: parameters for the generator
     """
 
     name = "cvrptw"
 
     def __init__(
         self,
-        max_loc: float = 150,  # different default value to CVRPEnv to match max_time, will be scaled
-        max_time: int = 480,
-        scale: bool = False,
+        generator: CVRPTWGenerator = None,
+        generator_params: dict = {},
         **kwargs,
     ):
-        self.min_time = 0  # always 0
-        self.max_time = max_time
-        self.scale = scale
-        super().__init__(max_loc=max_loc, **kwargs)
-
-    def _make_spec(self, td_params: TensorDict):
-        super()._make_spec(td_params)
-
-        current_time = UnboundedContinuousTensorSpec(
-            shape=(1), dtype=torch.float32, device=self.device
-        )
-
-        current_loc = UnboundedContinuousTensorSpec(
-            shape=(2), dtype=torch.float32, device=self.device
-        )
-
-        durations = BoundedTensorSpec(
-            low=self.min_time,
-            high=self.max_time,
-            shape=(self.num_loc, 1),
-            dtype=torch.int64,
-            device=self.device,
-        )
-
-        time_windows = BoundedTensorSpec(
-            low=self.min_time,
-            high=self.max_time,
-            shape=(
-                self.num_loc,
-                2,
-            ),  # each location has a 2D time window (start, end)
-            dtype=torch.int64,
-            device=self.device,
-        )
-
-        # extend observation specs
-        self.observation_spec = CompositeSpec(
-            **self.observation_spec,
-            current_time=current_time,
-            current_loc=current_loc,
-            durations=durations,
-            time_windows=time_windows,
-            # vehicle_idx=vehicle_idx,
-        )
-
-    def generate_data(self, batch_size) -> TensorDict:
-        """
-        Generates time windows and service durations for the locations. The depot has a time window of [0, self.max_time].
-        The time windows define the time span within which a service has to be started. To reach the depot in time from the last node,
-        the end time of each node is bounded by the service duration and the distance back to the depot.
-        The start times of the time windows are bounded by how long it takes to travel there from the depot.
-        """
-        td = super().generate_data(batch_size)
-
-        batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
-
-        ## define service durations
-        # generate randomly (first assume service durations of 0, to be changed later)
-        durations = torch.zeros(
-            *batch_size, self.num_loc + 1, dtype=torch.float32, device=self.device
-        )
-
-        ## define time windows
-        # 1. get distances from depot
-        dist = get_distance(td["depot"], td["locs"].transpose(0, 1)).transpose(0, 1)
-        dist = torch.cat((torch.zeros(*batch_size, 1, device=self.device), dist), dim=1)
-        # 2. define upper bound for time windows to make sure the vehicle can get back to the depot in time
-        upper_bound = self.max_time - dist - durations
-        # 3. create random values between 0 and 1
-        ts_1 = torch.rand(*batch_size, self.num_loc + 1, device=self.device)
-        ts_2 = torch.rand(*batch_size, self.num_loc + 1, device=self.device)
-        # 4. scale values to lie between their respective min_time and max_time and convert to integer values
-        min_ts = (dist + (upper_bound - dist) * ts_1).int()
-        max_ts = (dist + (upper_bound - dist) * ts_2).int()
-        # 5. set the lower value to min, the higher to max
-        min_times = torch.min(min_ts, max_ts)
-        max_times = torch.max(min_ts, max_ts)
-        # 6. reset times for depot
-        min_times[..., :, 0] = 0.0
-        max_times[..., :, 0] = self.max_time
-
-        # 7. ensure min_times < max_times to prevent numerical errors in attention.py
-        # min_times == max_times may lead to nan values in _inner_mha()
-        mask = min_times == max_times
-        if torch.any(mask):
-            min_tmp = min_times.clone()
-            min_tmp[mask] = torch.max(
-                dist[mask].int(), min_tmp[mask] - 1
-            )  # we are handling integer values, so we can simply substract 1
-            min_times = min_tmp
-
-            mask = min_times == max_times  # update mask to new min_times
-            if torch.any(mask):
-                max_tmp = max_times.clone()
-                max_tmp[mask] = torch.min(
-                    torch.floor(upper_bound[mask]).int(),
-                    torch.max(
-                        torch.ceil(min_tmp[mask] + durations[mask]).int(),
-                        max_tmp[mask] + 1,
-                    ),
-                )
-                max_times = max_tmp
-
-        # scale to [0, 1]
-        if self.scale:
-            durations = durations / self.max_time
-            min_times = min_times / self.max_time
-            max_times = max_times / self.max_time
-            td["depot"] = td["depot"] / self.max_time
-            td["locs"] = td["locs"] / self.max_time
-
-        # 8. stack to tensor time_windows
-        time_windows = torch.stack((min_times, max_times), dim=-1)
-
-        assert torch.all(
-            min_times < max_times
-        ), "Please make sure the relation between max_loc and max_time allows for feasible solutions."
-
-        # reset duration at depot to 0
-        durations[:, 0] = 0.0
-        td.update(
-            {
-                "durations": durations,
-                "time_windows": time_windows,
-            }
-        )
-        return td
+        super().__init__(**kwargs)
+        if generator is None:
+            generator = CVRPTWGenerator(**generator_params)
+        self.generator = generator
+        self._make_spec(self.generator)
+
+    def _make_spec(self, generator: CVRPTWGenerator):
+        if isinstance(generator, CVRPGenerator):
+            super()._make_spec(generator)
+        else:
+            current_time = UnboundedContinuousTensorSpec(
+                shape=(1), dtype=torch.float32, device=self.device
+            )
+            current_loc = UnboundedContinuousTensorSpec(
+                shape=(2), dtype=torch.float32, device=self.device
+            )
+            durations = BoundedTensorSpec(
+                low=generator.min_time,
+                high=generator.max_time,
+                shape=(generator.num_loc, 1),
+                dtype=torch.int64,
+                device=self.device,
+            )
+            time_windows = BoundedTensorSpec(
+                low=generator.min_time,
+                high=generator.max_time,
+                shape=(
+                    generator.num_loc,
+                    2,
+                ),  # Each location has a 2D time window (start, end)
+                dtype=torch.int64,
+                device=self.device,
+            )
+            # Extend observation specs
+            self.observation_spec = CompositeSpec(
+                **self.observation_spec,
+                current_time=current_time,
+                current_loc=current_loc,
+                durations=durations,
+                time_windows=time_windows,
+            )
 
     @staticmethod
     def get_action_mask(td: TensorDict) -> torch.Tensor:
         """In addition to the constraints considered in the CVRPEnv, the time windows are considered.
         The vehicle can only visit a location if it can reach it in time, i.e. before its time window ends.
         """
         not_masked = CVRPEnv.get_action_mask(td)
@@ -207,53 +139,46 @@
         # current_node is updated to the selected action
         td = super()._step(td)
         return td
 
     def _reset(
         self, td: Optional[TensorDict] = None, batch_size: Optional[list] = None
     ) -> TensorDict:
-        if batch_size is None:
-            batch_size = self.batch_size if td is None else td["locs"].shape[:-2]
-        if td is None or td.is_empty():
-            td = self.generate_data(batch_size=batch_size)
-        batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
-
-        self.to(td.device)
-        # Create reset TensorDict
+        device = td.device
         td_reset = TensorDict(
             {
                 "locs": torch.cat((td["depot"][..., None, :], td["locs"]), -2),
                 "demand": td["demand"],
                 "current_node": torch.zeros(
-                    *batch_size, 1, dtype=torch.long, device=self.device
+                    *batch_size, 1, dtype=torch.long, device=device
                 ),
                 "current_time": torch.zeros(
-                    *batch_size, 1, dtype=torch.float32, device=self.device
+                    *batch_size, 1, dtype=torch.float32, device=device
                 ),
-                "used_capacity": torch.zeros((*batch_size, 1), device=self.device),
+                "used_capacity": torch.zeros((*batch_size, 1), device=device),
                 "vehicle_capacity": torch.full(
-                    (*batch_size, 1), self.vehicle_capacity, device=self.device
+                    (*batch_size, 1), self.generator.vehicle_capacity, device=device
                 ),
                 "visited": torch.zeros(
                     (*batch_size, 1, td["locs"].shape[-2] + 1),
                     dtype=torch.uint8,
-                    device=self.device,
+                    device=device,
                 ),
                 "durations": td["durations"],
                 "time_windows": td["time_windows"],
             },
             batch_size=batch_size,
         )
         td_reset.set("action_mask", self.get_action_mask(td_reset))
         return td_reset
 
-    def get_reward(self, td: TensorDict, actions: TensorDict) -> TensorDict:
+    def _get_reward(self, td: TensorDict, actions: TensorDict) -> TensorDict:
         """The reward is the negative tour length. Time windows
         are not considered for the calculation of the reward."""
-        return super().get_reward(td, actions)
+        return super()._get_reward(td, actions)
 
     @staticmethod
     def check_solution_validity(td: TensorDict, actions: torch.Tensor):
         CVRPEnv.check_solution_validity(td, actions)
         batch_size = td["locs"].shape[0]
         # distances to depot
         distances = get_distance(
@@ -296,16 +221,16 @@
             curr_time = curr_time + gather_by_index(td["durations"], next_node).reshape(
                 [batch_size, 1]
             )
             curr_node = next_node
             curr_time[curr_node == 0] = 0.0  # reset time for depot
 
     @staticmethod
-    def render(td: TensorDict, actions=None, ax=None, scale_xy: bool = False, **kwargs):
-        CVRPEnv.render(td=td, actions=actions, ax=ax, scale_xy=scale_xy, **kwargs)
+    def render(td: TensorDict, actions: torch.Tensor=None, ax = None):
+        render(td, actions, ax)
 
     @staticmethod
     def load_data(
         name: str,
         solomon=False,
         path_instances: str = None,
         type: str = None,
```

### Comparing `rl4co-0.3.3/rl4co/envs/routing/mpdp.py` & `rl4co-0.4.0/rl4co/utils/decoding.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,528 +1,540 @@
-from typing import Optional
+import abc
+
+from typing import Optional, Tuple
 
 import torch
+import torch.nn.functional as F
 
 from tensordict.tensordict import TensorDict
-from torchrl.data import (
-    BoundedTensorSpec,
-    CompositeSpec,
-    UnboundedContinuousTensorSpec,
-    UnboundedDiscreteTensorSpec,
-)
 
-from rl4co.envs.common.base import RL4COEnvBase
-from rl4co.utils.ops import gather_by_index
+from rl4co.envs import RL4COEnvBase
+from rl4co.utils.ops import batchify
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
-class MPDPEnv(RL4COEnvBase):
-    """Multi-agent Pickup and Delivery Problem environment.
-    The goal is to pick up and deliver all the packages while satisfying the precedence constraints.
-    When an agent goes back to the depot, a new agent is spawned. In the min-max version, the goal is to minimize the
-    maximum tour length among all agents.
-    The reward is 0 unless the agent visits all the cities.
-    In that case, the reward is (-)length of the path: maximizing the reward is equivalent to minimizing the path length.
+def get_decoding_strategy(decoding_strategy, **config):
+    strategy_registry = {
+        "greedy": Greedy,
+        "sampling": Sampling,
+        "multistart_greedy": Greedy,
+        "multistart_sampling": Sampling,
+        "beam_search": BeamSearch,
+        "evaluate": Evaluate,
+    }
+
+    if decoding_strategy not in strategy_registry:
+        log.warning(
+            f"Unknown decode type '{decoding_strategy}'. Available decode types: {strategy_registry.keys()}. Defaulting to Sampling."
+        )
+
+    if "multistart" in decoding_strategy:
+        config["multistart"] = True
+
+    return strategy_registry.get(decoding_strategy, Sampling)(**config)
+
+
+def get_log_likelihood(logprobs, actions, mask=None, return_sum: bool = True):
+    """Get log likelihood of selected actions.
+    Note that mask is a boolean tensor where True means the value should be kept.
+
+    Args:
+        logprobs: Log probabilities of actions from the model (batch_size, seq_len, action_dim).
+        actions: Selected actions (batch_size, seq_len).
+        mask: Action mask. 1 if feasible, 0 otherwise (so we keep if 1 as done in PyTorch).
+        return_sum: Whether to return the sum of log probabilities or not. Defaults to True.
+    """
+    logprobs = logprobs.gather(-1, actions.unsqueeze(-1)).squeeze(-1)
+
+    # Optional: mask out actions irrelevant to objective so they do not get reinforced
+    if mask is not None:
+        logprobs[~mask] = 0
+
+    assert (
+        logprobs > -1000
+    ).data.all(), "Logprobs should not be -inf, check sampling procedure!"
+
+    # Calculate log_likelihood
+    if return_sum:
+        return logprobs.sum(1)  # [batch]
+    else:
+        return logprobs  # [batch, decode_len]
+
+
+def decode_logprobs(logprobs, mask, decode_type="sampling"):
+    """Decode log probabilities to select actions with mask.
+    Note that mask is a boolean tensor where True means the value should be kept.
+    """
+    if "greedy" in decode_type:
+        selected = DecodingStrategy.greedy(logprobs, mask)
+    elif "sampling" in decode_type:
+        selected = DecodingStrategy.sampling(logprobs, mask)
+    else:
+        assert False, "Unknown decode type: {}".format(decode_type)
+    return selected
+
+
+def random_policy(td):
+    """Helper function to select a random action from available actions"""
+    action = torch.multinomial(td["action_mask"].float(), 1).squeeze(-1)
+    td.set("action", action)
+    return td
+
+
+def rollout(env, td, policy, max_steps: int = None):
+    """Helper function to rollout a policy. Currently, TorchRL does not allow to step
+    over envs when done with `env.rollout()`. We need this because for environments that complete at different steps.
+    """
+
+    max_steps = float("inf") if max_steps is None else max_steps
+    actions = []
+    steps = 0
+
+    while not td["done"].all():
+        td = policy(td)
+        actions.append(td["action"])
+        td = env.step(td)["next"]
+        steps += 1
+        if steps > max_steps:
+            log.info("Max steps reached")
+            break
+    return (
+        env.get_reward(td, torch.stack(actions, dim=1)),
+        td,
+        torch.stack(actions, dim=1),
+    )
+
+
+def modify_logits_for_top_k_filtering(logits, top_k):
+    """Set the logits for none top-k values to -inf. Done out-of-place.
+    Ref: https://github.com/togethercomputer/stripedhyena/blob/7e13f618027fea9625be1f2d2d94f9a361f6bd02/stripedhyena/sample.py#L6
+    """
+    indices_to_remove = logits < torch.topk(logits, top_k)[0][..., -1, None]
+    return logits.masked_fill(indices_to_remove, float("-inf"))
+
+
+def modify_logits_for_top_p_filtering(logits, top_p):
+    """Set the logits for none top-p values to -inf. Done out-of-place.
+    Ref: https://github.com/togethercomputer/stripedhyena/blob/7e13f618027fea9625be1f2d2d94f9a361f6bd02/stripedhyena/sample.py#L14
+    """
+    if top_p <= 0.0 or top_p >= 1.0:
+        return logits
+
+    # First sort and calculate cumulative sum of probabilities.
+    sorted_logits, sorted_indices = torch.sort(logits, descending=False)
+    cumulative_probs = sorted_logits.softmax(dim=-1).cumsum(dim=-1)
+
+    # Remove tokens with cumulative top_p above the threshold (token with 0 are kept)
+    sorted_indices_to_remove = cumulative_probs <= (1 - top_p)
+
+    # Scatter sorted tensors to original indexing
+    indices_to_remove = sorted_indices_to_remove.scatter(
+        -1, sorted_indices, sorted_indices_to_remove
+    )
+    return logits.masked_fill(indices_to_remove, float("-inf"))
+
+
+def process_logits(
+    logits: torch.Tensor,
+    mask: torch.Tensor = None,
+    temperature: float = 1.0,
+    top_p: float = 0.0,
+    top_k: int = 0,
+    tanh_clipping: float = 0,
+    mask_logits: bool = True,
+):
+    """Convert logits to log probabilities with additional features like temperature scaling, top-k and top-p sampling.
+
+    Note:
+        We convert to log probabilities instead of probabilities to avoid numerical instability.
+        This is because, roughly, softmax = exp(logits) / sum(exp(logits)) and log(softmax) = logits - log(sum(exp(logits))),
+        and avoiding the division by the sum of exponentials can help with numerical stability.
+        You may check the [official PyTorch documentation](https://pytorch.org/docs/stable/generated/torch.nn.functional.log_softmax.html).
+
+    Args:
+        logits: Logits from the model (batch_size, num_actions).
+        mask: Action mask. 1 if feasible, 0 otherwise (so we keep if 1 as done in PyTorch).
+        temperature: Temperature scaling. Higher values make the distribution more uniform (exploration),
+            lower values make it more peaky (exploitation).
+        top_p: Top-p sampling, a.k.a. Nucleus Sampling (https://arxiv.org/abs/1904.09751). Remove tokens that have a cumulative probability
+            less than the threshold 1 - top_p (lower tail of the distribution). If 0, do not perform.
+        top_k: Top-k sampling, i.e. restrict sampling to the top k logits. If 0, do not perform. Note that we only do filtering and
+            do not return all the top-k logits here.
+        tanh_clipping: Tanh clipping (https://arxiv.org/abs/1611.09940).
+        mask_logits: Whether to mask logits of infeasible actions.
+    """
+
+    # Tanh clipping from Bello et al. 2016
+    if tanh_clipping > 0:
+        logits = torch.tanh(logits) * tanh_clipping
+
+    # In RL, we want to mask the logits to prevent the agent from selecting infeasible actions
+    if mask_logits:
+        assert mask is not None, "mask must be provided if mask_logits is True"
+        logits[~mask] = float("-inf")
+
+    logits = logits / temperature  # temperature scaling
+
+    if top_k > 0:
+        top_k = min(top_k, logits.size(-1))  # safety check
+        logits = modify_logits_for_top_k_filtering(logits, top_k)
+
+    if top_p > 0:
+        assert top_p <= 1.0, "top-p should be in (0, 1]."
+        logits = modify_logits_for_top_p_filtering(logits, top_p)
+
+    # Compute log probabilities
+    return F.log_softmax(logits, dim=-1)
+
+
+class DecodingStrategy(metaclass=abc.ABCMeta):
+    """Base class for decoding strategies. Subclasses should implement the :meth:`_step` method.
+    Includes hooks for pre and post main decoding operations.
 
     Args:
-        num_loc: number of locations (cities) in the TSP
-        min_loc: minimum location coordinate. Used for data generation
-        max_loc: maximum location coordinate. Used for data generation
-        min_num_agents: minimum number of agents. Used for data generation
-        max_num_agents: maximum number of agents. Used for data generation
-        objective: objective to optimize. Either 'minmax' or 'minsum'
-        check_solution: whether to check the validity of the solution
-        td_params: parameters of the environment
+        temperature: Temperature scaling. Higher values make the distribution more uniform (exploration),
+            lower values make it more peaky (exploitation). Defaults to 1.0.
+        top_p: Top-p sampling, a.k.a. Nucleus Sampling (https://arxiv.org/abs/1904.09751). Defaults to 0.0.
+        top_k: Top-k sampling, i.e. restrict sampling to the top k logits. If 0, do not perform. Defaults to 0.
+        mask_logits: Whether to mask logits of infeasible actions. Defaults to True.
+        tanh_clipping: Tanh clipping (https://arxiv.org/abs/1611.09940). Defaults to 0.
+        multistart: Whether to use multistart decoding. Defaults to False.
+        num_starts: Number of starts for multistart decoding. Defaults to None.
     """
 
-    name = "mpdp"
+    name = "base"
 
     def __init__(
         self,
-        num_loc: int = 20,
-        min_loc: float = 0,
-        max_loc: float = 1,
-        min_num_agents: int = 2,
-        max_num_agents: int = 10,
-        objective: str = "minmax",
-        check_solution: bool = False,
-        td_params: TensorDict = None,
+        temperature: float = 1.0,
+        top_p: float = 0.0,
+        top_k: int = 0,
+        mask_logits: bool = True,
+        tanh_clipping: float = 0,
+        multistart: bool = False,
+        num_starts: Optional[int] = None,
+        select_start_nodes_fn: Optional[callable] = None,
         **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.num_loc = num_loc
-        self.min_loc = min_loc
-        self.max_loc = max_loc
-        self.min_num_agents = min_num_agents
-        self.max_num_agents = max_num_agents
-        self.objective = objective
-        self.check_solution = check_solution
-        self._make_spec(td_params)
-
-    def _step(self, td: TensorDict) -> TensorDict:
-        selected = td["action"][:, None]  # Add dimension for step
-
-        agent_num = td["lengths"].size(1)
-        n_loc = td["to_delivery"].size(-1) - agent_num - 1
-
-        new_to_delivery = (selected + n_loc // 2) % (
-            n_loc + agent_num + 1
-        )  # the pair node of selected node
-
-        is_request = (selected > agent_num) & (selected <= agent_num + n_loc // 2)
-        td["left_request"][is_request] -= 1
-        depot_distance = td["depot_distance"].scatter(-1, selected, 0)
+    ) -> None:
+        self.temperature = temperature
+        self.top_p = top_p
+        self.top_k = top_k
+        self.mask_logits = mask_logits
+        self.tanh_clipping = tanh_clipping
+        self.multistart = multistart
+        self.num_starts = num_starts
+        self.select_start_nodes_fn = select_start_nodes_fn
+        # initialize buffers
+        self.actions = []
+        self.logprobs = []
 
-        add_pd = td["add_pd_distance"][is_request.squeeze(-1), :].gather(
-            -1, selected[is_request.squeeze(-1), :] - agent_num - 1
-        )
-        td["longest_lengths"][is_request.squeeze(-1), :].scatter_add_(
-            -1, td["count_depot"][is_request.squeeze(-1), :], add_pd
-        )
-        td["add_pd_distance"][is_request.squeeze(-1), :].scatter_(
-            -1, selected[is_request.squeeze(-1), :] - agent_num - 1, 0
-        )
-        remain_sum_paired_distance = td["add_pd_distance"].sum(-1, keepdim=True)
-        remain_pickup_max_distance = depot_distance[:, : agent_num + 1 + n_loc // 2].max(
-            dim=-1, keepdim=True
-        )[0]
-        remain_delivery_max_distance = depot_distance[
-            :, agent_num + 1 + n_loc // 2 :
-        ].max(dim=-1, keepdim=True)[0]
-
-        # Calculate makespan
-        cur_coord = gather_by_index(td["locs"], selected)
-        path_lengths = (cur_coord - td["cur_coord"]).norm(p=2, dim=-1)
-
-        td["lengths"].scatter_add_(-1, td["count_depot"], path_lengths.unsqueeze(-1))
-
-        # If visit depot then plus one to count_depot\
-        td["count_depot"][
-            (selected == td["agent_idx"]) & (td["agent_idx"] < agent_num)
-        ] += 1  # torch.ones(td["count_depot"][(selected == 0) & (td["agent_idx"] < agent_num)].shape, dtype=torch.int64, device=td["count_depot"].device)
-
-        # `agent_idx` is added by 1 if the current agent comes back to depot
-        agent_idx = (td["count_depot"] + 1) * torch.ones(
-            selected.size(0), 1, dtype=torch.long, device=td["count_depot"].device
-        )
-        visited = td["visited"].scatter(-1, selected.unsqueeze(-1), 1)
-        to_delivery = td["to_delivery"].scatter(-1, new_to_delivery[:, :, None], 1)
+    @abc.abstractmethod
+    def _step(
+        self,
+        logprobs: torch.Tensor,
+        mask: torch.Tensor,
+        td: TensorDict,
+        action: torch.Tensor = None,
+        **kwargs,
+    ) -> Tuple[torch.Tensor, torch.Tensor, TensorDict]:
+        """Main decoding operation. This method should be called in a loop until all sequences are done.
 
-        # Get done and reward
-        done = visited.all(dim=-1, keepdim=True).squeeze(-1)
-        reward = torch.zeros_like(done)
-
-        td.update(
-            {
-                "visited": visited,
-                "agent_idx": agent_idx,
-                "cur_coord": cur_coord,
-                "to_delivery": to_delivery,
-                "depot_distance": depot_distance,
-                "remain_sum_paired_distance": remain_sum_paired_distance,
-                "remain_pickup_max_distance": remain_pickup_max_distance,
-                "remain_delivery_max_distance": remain_delivery_max_distance,
-                "i": td["i"] + 1,
-                "done": done,
-                "reward": reward,
-            }
-        )
-        td.set("action_mask", self.get_action_mask(td))
-        return td
+        Args:
+            logprobs: Log probabilities processed from logits of the model.
+            mask: Action mask. 1 if feasible, 0 otherwise (so we keep if 1 as done in PyTorch).
+            td: TensorDict containing the current state of the environment.
+            action: Optional action to use, e.g. for evaluating log probabilities.
+        """
+        raise NotImplementedError("Must be implemented by subclass")
 
-    def _reset(
+    def pre_decoder_hook(
+        self, td: TensorDict, env: RL4COEnvBase, action: torch.Tensor = None
+    ):
+        """Pre decoding hook. This method is called before the main decoding operation."""
+        # Multi-start decoding. If num_starts is None, we use the number of actions in the action mask
+        if self.multistart:
+            if self.num_starts is None:
+                self.num_starts = env.get_num_starts(td)
+        else:
+            if self.num_starts is not None:
+                if self.num_starts >= 1:
+                    log.warn(
+                        f"num_starts={self.num_starts} is ignored for decode_type={self.name}"
+                    )
+
+            self.num_starts = 0
+
+        # Multi-start decoding: first action is chosen by ad-hoc node selection
+        if self.num_starts >= 1:
+            if action is None:  # if action is provided, we use it as the first action
+                if self.select_start_nodes_fn is not None:
+                    action = self.select_start_nodes_fn(td, env, self.num_starts)
+                else:
+                    action = env.select_start_nodes(td, num_starts=self.num_starts)
+
+            # Expand td to batch_size * num_starts
+            td = batchify(td, self.num_starts)
+
+            td.set("action", action)
+            td = env.step(td)["next"]
+            logprobs = torch.zeros_like(
+                td["action_mask"], device=td.device
+            )  # first logprobs is 0, so p = logprobs.exp() = 1
+
+            self.logprobs.append(logprobs)
+            self.actions.append(action)
+
+        return td, env, self.num_starts
+
+    def post_decoder_hook(
+        self, td: TensorDict, env: RL4COEnvBase
+    ) -> Tuple[torch.Tensor, torch.Tensor, TensorDict, RL4COEnvBase]:
+        assert (
+            len(self.logprobs) > 0
+        ), "No logprobs were collected because all environments were done. Check your initial state"
+
+        return torch.stack(self.logprobs, 1), torch.stack(self.actions, 1), td, env
+
+    def step(
         self,
-        td: Optional[TensorDict] = None,
-        batch_size: Optional[list] = None,
-        agent_num: Optional[int] = None,  # NOTE hardcoded from ET
+        logits: torch.Tensor,
+        mask: torch.Tensor,
+        td: TensorDict,
+        action: torch.Tensor = None,
+        **kwargs,
     ) -> TensorDict:
-        if batch_size is None:
-            batch_size = self.batch_size if td is None else td["locs"].shape[:-2]
+        """Main decoding operation. This method should be called in a loop until all sequences are done.
 
-        if td is None or td.is_empty():
-            td = self.generate_data(batch_size=batch_size)
+        Args:
+            logits: Logits from the model.
+            mask: Action mask. 1 if feasible, 0 otherwise (so we keep if 1 as done in PyTorch).
+            td: TensorDict containing the current state of the environment.
+            action: Optional action to use, e.g. for evaluating log probabilities.
+        """
+        if not self.mask_logits:  # set mask_logit to None if mask_logits is False
+            mask = None
+
+        logprobs = process_logits(
+            logits,
+            mask,
+            temperature=self.temperature,
+            top_p=self.top_p,
+            top_k=self.top_k,
+            tanh_clipping=self.tanh_clipping,
+            mask_logits=self.mask_logits,
+        )
+        logprobs, selected_action, td = self._step(
+            logprobs, mask, td, action=action, **kwargs
+        )
+        td.set("action", selected_action)
+        self.actions.append(selected_action)
+        self.logprobs.append(logprobs)
+        return td
 
-        self.to(td.device)
+    @staticmethod
+    def greedy(logprobs, mask=None):
+        """Select the action with the highest probability."""
+        # [BS], [BS]
+        selected = logprobs.argmax(dim=-1)
+        if mask is not None:
+            assert (
+                not (~mask).gather(1, selected.unsqueeze(-1)).data.any()
+            ), "infeasible action selected"
 
-        # NOTE: this is a hack to get the agent_num
-        # agent_num = td["agent_num"][0].item() if agent_num is None else agent_num
-        # agent_num = agent_num if agent_num is not None else td["agent_num"][0].item()
-
-        depot = td["depot"]
-        depot = depot.repeat(1, agent_num + 1, 1)
-        loc = td["locs"]
-        left_request = loc.size(1) // 2
-        whole_instance = torch.cat((depot, loc), dim=1)
-
-        # Distance from all nodes between each other
-        distance = torch.cdist(whole_instance, whole_instance, p=2)
-        index = torch.arange(left_request, 2 * left_request, device=depot.device)[
-            None, :, None
-        ]
-        index = index.repeat(distance.shape[0], 1, 1)
-        add_pd_distance = distance[
-            :, agent_num + 1 : agent_num + 1 + left_request, agent_num + 1 :
-        ].gather(-1, index)
-        add_pd_distance = add_pd_distance.squeeze(-1)
-
-        remain_pickup_max_distance = distance[:, 0, : agent_num + 1 + left_request].max(
-            dim=-1, keepdim=True
-        )[0]
-        remain_delivery_max_distance = distance[:, 0, agent_num + 1 + left_request :].max(
-            dim=-1, keepdim=True
-        )[0]
-        remain_sum_paired_distance = add_pd_distance.sum(dim=-1, keepdim=True)
-
-        # Distance from depot to all nodes
-        # Delivery nodes should consider the sum of distance from depot to paired pickup nodes and pickup nodes to delivery nodes
-        distance[:, 0, agent_num + 1 : agent_num + 1 + left_request] = (
-            distance[:, 0, agent_num + 1 : agent_num + 1 + left_request]
-            + distance[:, 0, agent_num + 1 + left_request :]
-        )
+        return selected
 
-        # Distance from depot to all nodes
-        depot_distance = distance[:, 0, :]
-        depot_distance[:, agent_num + 1 : agent_num + 1 + left_request] = depot_distance[
-            :, agent_num + 1 : agent_num + 1 + left_request
-        ]  # + add_pd_distance
-
-        batch_size, n_loc, _ = loc.size()
-        to_delivery = torch.cat(
-            [
-                torch.ones(
-                    batch_size,
-                    1,
-                    n_loc // 2 + agent_num + 1,
-                    dtype=torch.uint8,
-                    device=loc.device,
-                ),
-                torch.zeros(
-                    batch_size, 1, n_loc // 2, dtype=torch.uint8, device=loc.device
-                ),
-            ],
-            dim=-1,
-        )
+    @staticmethod
+    def sampling(logprobs, mask=None):
+        """Sample an action with a multinomial distribution given by the log probabilities."""
+        probs = logprobs.exp()
+        selected = torch.multinomial(probs, 1).squeeze(1)
 
-        # Create reset TensorDict
-        td_reset = TensorDict(
-            {
-                "locs": torch.cat((depot, loc), -2),
-                "visited": torch.zeros(
-                    batch_size,
-                    1,
-                    n_loc + agent_num + 1,
-                    dtype=torch.uint8,
-                    device=loc.device,
-                ),
-                "lengths": torch.zeros(batch_size, agent_num, device=loc.device),
-                "longest_lengths": torch.zeros(batch_size, agent_num, device=loc.device),
-                "cur_coord": td["depot"]
-                if len(td["depot"].shape) == 2
-                else td["depot"].squeeze(1),
-                "i": torch.zeros(
-                    batch_size, dtype=torch.int64, device=loc.device
-                ),  # Vector with length num_steps
-                "to_delivery": to_delivery,
-                "count_depot": torch.zeros(
-                    batch_size, 1, dtype=torch.int64, device=loc.device
-                ),
-                "agent_idx": torch.ones(
-                    batch_size, 1, dtype=torch.long, device=loc.device
-                ),
-                "left_request": left_request
-                * torch.ones(batch_size, 1, dtype=torch.long, device=loc.device),
-                "remain_pickup_max_distance": remain_pickup_max_distance,
-                "remain_delivery_max_distance": remain_delivery_max_distance,
-                "depot_distance": depot_distance,
-                "remain_sum_paired_distance": remain_sum_paired_distance,
-                "add_pd_distance": add_pd_distance,
-            },
-            batch_size=batch_size,
-        )
-        td_reset.set("action_mask", self.get_action_mask(td_reset))
-        return td_reset
+        if mask is not None:
+            while (~mask).gather(1, selected.unsqueeze(-1)).data.any():
+                log.info("Sampled bad values, resampling!")
+                selected = probs.multinomial(1).squeeze(1)
+            assert (
+                not (~mask).gather(1, selected.unsqueeze(-1)).data.any()
+            ), "infeasible action selected"
 
-    @staticmethod
-    def get_action_mask(td: TensorDict) -> torch.Tensor:
-        """Get the action mask for the current state."""
+        return selected
 
-        visited_loc = td["visited"].clone()
 
-        agent_num = td["lengths"].size(1)
-        n_loc = visited_loc.size(-1) - agent_num - 1  # num of customers
-        batch_size = visited_loc.size(0)
-        agent_idx = td["agent_idx"][:, None, :]
-        mask_loc = visited_loc.to(td["to_delivery"].device) | (1 - td["to_delivery"])
-
-        # depot
-        if td["i"][0].item() != 0:
-            mask_loc[:, :, : agent_num + 1] = 1
-
-            # if deliver nodes which is assigned agent is complete, then agent can go to depot
-            no_item_to_delivery = (
-                visited_loc[:, :, n_loc // 2 + agent_num + 1 :]
-                == td["to_delivery"][:, :, n_loc // 2 + agent_num + 1 :]
-            ).all(dim=-1)
-            mask_loc[no_item_to_delivery.squeeze(-1), :, :] = mask_loc[
-                no_item_to_delivery.squeeze(-1), :, :
-            ].scatter_(-1, agent_idx[no_item_to_delivery.squeeze(-1), :, :], 0)
-
-            condition = (td["count_depot"] == agent_num - 1) & (
-                (visited_loc[:, :, agent_num + 1 :] == 0).sum(dim=-1) != 0
-            )
+class Greedy(DecodingStrategy):
+    name = "greedy"
 
-            mask_loc[..., agent_num][condition] = 1
+    def _step(
+        self, logprobs: torch.Tensor, mask: torch.Tensor, td: TensorDict, **kwargs
+    ) -> Tuple[torch.Tensor, torch.Tensor, TensorDict]:
+        """Select the action with the highest log probability"""
+        selected = self.greedy(logprobs, mask)
+        return logprobs, selected, td
 
-        else:
-            return (
-                torch.cat(
-                    [
-                        torch.zeros(
-                            batch_size, 1, 1, dtype=torch.uint8, device=mask_loc.device
-                        ),
-                        torch.ones(
-                            batch_size,
-                            1,
-                            n_loc + agent_num,
-                            dtype=torch.uint8,
-                            device=mask_loc.device,
-                        ),
-                    ],
-                    dim=-1,
-                )
-                > 0
-            )
-        action_mask = mask_loc == 0  # action_mask gets feasible actions
-        return action_mask
-
-    def get_reward(self, td: TensorDict, actions: TensorDict) -> TensorDict:
-        # Check that the solution is valid
-        if self.check_solution:
-            self.check_solution_validity(td, actions)
-
-        # Calculate the reward (negative tour length)
-        if self.objective == "minmax":
-            return -td["lengths"].max(dim=-1, keepdim=True)[0].squeeze(-1)
-        elif self.objective == "minsum":
-            return -td["lengths"].sum(dim=-1, keepdim=True).squeeze(-1)
-        else:
-            raise ValueError(f"Unknown objective {self.objective}")
 
-    @staticmethod
-    def check_solution_validity(td: TensorDict, actions: torch.Tensor):
-        assert True, "Not implemented"
+class Sampling(DecodingStrategy):
+    name = "sampling"
 
-    def generate_data(self, batch_size) -> TensorDict:
-        # Batch size input check
-        batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
-
-        # Initialize the locations (including the depot which is always the first node)
-        locs_with_depot = (
-            torch.FloatTensor(*batch_size, self.num_loc + 1, 2)
-            .uniform_(self.min_loc, self.max_loc)
-            .to(self.device)
-        )
+    def _step(
+        self, logprobs: torch.Tensor, mask: torch.Tensor, td: TensorDict, **kwargs
+    ) -> Tuple[torch.Tensor, torch.Tensor, TensorDict]:
+        """Sample an action with a multinomial distribution given by the log probabilities."""
+        selected = self.sampling(logprobs, mask)
+        return logprobs, selected, td
 
-        return TensorDict(
-            {
-                "locs": locs_with_depot[..., 1:, :],
-                "depot": locs_with_depot[..., 0, :],
-            },
-            batch_size=batch_size,
-        )
 
-    def _make_spec(self, td_params: TensorDict):
-        """Make the observation and action specs from the parameters."""
-        max_nodes = self.num_loc + self.max_num_agents + 1
-        self.observation_spec = CompositeSpec(
-            locs=BoundedTensorSpec(
-                low=self.min_loc,
-                high=self.max_loc,
-                shape=(max_nodes, 2),
-                dtype=torch.float32,
-            ),
-            current_node=UnboundedDiscreteTensorSpec(
-                shape=(1),
-                dtype=torch.int64,
-            ),
-            action_mask=UnboundedDiscreteTensorSpec(
-                shape=(max_nodes, 1),
-                dtype=torch.bool,
-            ),
-            visited=UnboundedDiscreteTensorSpec(
-                shape=(1, max_nodes),
-                dtype=torch.bool,
-            ),
-            lengths=UnboundedContinuousTensorSpec(
-                shape=(self.max_num_agents,),
-                dtype=torch.float32,
-            ),
-            longest_lengths=UnboundedContinuousTensorSpec(
-                shape=(self.max_num_agents,),
-                dtype=torch.float32,
-            ),
-            cur_coord=BoundedTensorSpec(
-                low=self.min_loc,
-                high=self.max_loc,
-                shape=(2,),
-                dtype=torch.float32,
-            ),
-            to_delivery=UnboundedDiscreteTensorSpec(
-                shape=(max_nodes, 1),
-                dtype=torch.bool,
-            ),
-            count_depot=UnboundedDiscreteTensorSpec(
-                shape=(1,),
-                dtype=torch.int64,
-            ),
-            agent_idx=UnboundedDiscreteTensorSpec(
-                shape=(1,),
-                dtype=torch.int64,
-            ),
-            left_request=UnboundedDiscreteTensorSpec(
-                shape=(1,),
-                dtype=torch.int64,
-            ),
-            remain_pickup_max_distance=UnboundedContinuousTensorSpec(
-                shape=(1,),
-                dtype=torch.float32,
-            ),
-            remain_delivery_max_distance=UnboundedContinuousTensorSpec(
-                shape=(1,),
-                dtype=torch.float32,
-            ),
-            depot_distance=UnboundedContinuousTensorSpec(
-                shape=(max_nodes,),
-                dtype=torch.float32,
-            ),
-            remain_sum_paired_distance=UnboundedContinuousTensorSpec(
-                shape=(1,),
-                dtype=torch.float32,
-            ),
-            add_pd_distance=UnboundedContinuousTensorSpec(
-                shape=(max_nodes,),
-                dtype=torch.float32,
-            ),
-            ## NOTE: we should have a vectorized implementation for agent_num
-            # agent_num=UnboundedDiscreteTensorSpec(
-            #     shape=(1,),
-            #     dtype=torch.int64,
-            # ),
-            i=UnboundedDiscreteTensorSpec(
-                shape=(1,),
-                dtype=torch.int64,
-            ),
-        )
-        self.action_spec = BoundedTensorSpec(
-            shape=(1,),
-            dtype=torch.int64,
-            low=0,
-            high=max_nodes,
-        )
-        self.reward_spec = UnboundedContinuousTensorSpec(shape=(1,))
-        self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
+class Evaluate(DecodingStrategy):
+    name = "evaluate"
 
-    @staticmethod
-    def render(td: TensorDict, actions=None, ax=None):
-        # TODO: color switch with new agents; add pickup and delivery nodes as in `PDPEnv.render`
+    def _step(
+        self,
+        logprobs: torch.Tensor,
+        mask: torch.Tensor,
+        td: TensorDict,
+        action: torch.Tensor,
+        **kwargs,
+    ) -> Tuple[torch.Tensor, torch.Tensor, TensorDict]:
+        """The action is provided externally, so we just return the action"""
+        selected = action
+        return logprobs, selected, td
 
-        import matplotlib.pyplot as plt
-        import numpy as np
 
-        from matplotlib import cm, colormaps
+class BeamSearch(DecodingStrategy):
+    name = "beam_search"
 
-        num_routine = (actions == 0).sum().item() + 2
-        base = colormaps["nipy_spectral"]
-        color_list = base(np.linspace(0, 1, num_routine))
-        cmap_name = base.name + str(num_routine)
-        out = base.from_list(cmap_name, color_list, num_routine)
+    def __init__(self, beam_width=None, select_best=True, **kwargs) -> None:
+        super().__init__(**kwargs)
+        self.beam_width = beam_width
+        self.select_best = select_best
+        self.parent_beam_logprobs = None
+        self.beam_path = []
+
+    def _step(
+        self, logprobs: torch.Tensor, mask: torch.Tensor, td: TensorDict, **kwargs
+    ) -> Tuple[torch.Tensor, torch.Tensor, TensorDict]:
+        selected, batch_beam_idx = self._make_beam_step(logprobs)
+        # select the correct state representation, logprobs and mask according to beam parent
+        td = td[batch_beam_idx]
+        logprobs = logprobs[batch_beam_idx]
+        mask = mask[batch_beam_idx]
+
+        assert (
+            not (~mask).gather(1, selected.unsqueeze(-1)).data.any()
+        ), "infeasible action selected"
+
+        return logprobs, selected, td
+
+    def pre_decoder_hook(self, td: TensorDict, env: RL4COEnvBase, **kwargs):
+        if self.beam_width is None:
+            self.beam_width = env.get_num_starts(td)
+        assert self.beam_width > 1, "beam width must be larger than 1"
+
+        # select start nodes. TODO: include first step in beam search as well
+        if self.select_start_nodes_fn is not None:
+            action = self.select_start_nodes_fn(td, env, self.beam_width)
+        else:
+            action = env.select_start_nodes(td, num_starts=self.beam_width)
 
-        if ax is None:
-            # Create a plot of the nodes
-            _, ax = plt.subplots()
+        # Expand td to batch_size * beam_width
+        td = batchify(td, self.beam_width)
 
-        td = td.detach().cpu()
+        td.set("action", action)
+        td = env.step(td)["next"]
 
-        if actions is None:
-            actions = td.get("action", None)
+        logprobs = torch.zeros_like(td["action_mask"], device=td.device)
+        beam_parent = torch.zeros(logprobs.size(0), device=td.device, dtype=torch.int32)
 
-        # if batch_size greater than 0 , we need to select the first batch element
-        if td.batch_size != torch.Size([]):
-            td = td[0]
-            actions = actions[0]
+        self.logprobs.append(logprobs)
+        self.actions.append(action)
+        self.parent_beam_logprobs = logprobs.gather(1, action[..., None])
+        self.beam_path.append(beam_parent)
 
-        locs = td["locs"]
+        return td, env, self.beam_width
 
-        # add the depot at the first action and the end action
-        actions = torch.cat([torch.tensor([0]), actions, torch.tensor([0])])
+    def post_decoder_hook(self, td, env):
+        # [BS*BW, seq_len]
+        aligned_sequences, aligned_logprobs = self._backtrack()
 
-        # gather locs in order of action if available
-        if actions is None:
-            log.warning("No action in TensorDict, rendering unsorted locs")
+        if self.select_best:
+            return self._select_best_beam(aligned_logprobs, aligned_sequences, td, env)
         else:
-            locs = locs
+            return aligned_logprobs, aligned_sequences, td, env
+
+    def _backtrack(self):
+        # [BS*BW, seq_len]
+        actions = torch.stack(self.actions, 1)
+        # [BS*BW, seq_len]
+        logprobs = torch.stack(self.logprobs, 1)
+        assert actions.size(1) == len(
+            self.beam_path
+        ), "action idx shape and beam path shape dont match"
 
-        # Cat the first node to the end to complete the tour
-        x, y = locs[:, 0], locs[:, 1]
+        # [BS*BW]
+        cur_parent = self.beam_path[-1]
+        # [BS*BW]
+        reversed_aligned_sequences = [actions[:, -1]]
+        reversed_aligned_logprobs = [logprobs[:, -1]]
 
-        # plot depot
-        ax.scatter(
-            locs[0, 0],
-            locs[0, 1],
-            edgecolors=cm.Set2(2),
-            facecolors="none",
-            s=100,
-            linewidths=2,
-            marker="s",
-            alpha=1,
+        aug_batch_size = actions.size(0)
+        batch_size = aug_batch_size // self.beam_width
+        batch_beam_sequence = (
+            torch.arange(0, batch_size).repeat(self.beam_width).to(actions.device)
         )
 
-        # plot visited nodes
-        ax.scatter(
-            x[1:],
-            y[1:],
-            edgecolors=cm.Set2(0),
-            facecolors="none",
-            s=50,
-            linewidths=2,
-            marker="o",
-            alpha=1,
+        for k in reversed(range(len(self.beam_path) - 1)):
+            batch_beam_idx = batch_beam_sequence + cur_parent * batch_size
+
+            reversed_aligned_sequences.append(actions[batch_beam_idx, k])
+            reversed_aligned_logprobs.append(logprobs[batch_beam_idx, k])
+            cur_parent = self.beam_path[k][batch_beam_idx]
+
+        # [BS*BW, seq_len*num_targets]
+        actions = torch.stack(list(reversed(reversed_aligned_sequences)), dim=1)
+        logprobs = torch.stack(list(reversed(reversed_aligned_logprobs)), dim=1)
+
+        return actions, logprobs
+
+    def _select_best_beam(self, logprobs, actions, td: TensorDict, env: RL4COEnvBase):
+        aug_batch_size = logprobs.size(0)  # num nodes
+        batch_size = aug_batch_size // self.beam_width
+        rewards = env.get_reward(td, actions)
+        _, idx = torch.cat(rewards.unsqueeze(1).split(batch_size), 1).max(1)
+        flat_idx = torch.arange(batch_size, device=rewards.device) + idx * batch_size
+        return logprobs[flat_idx], actions[flat_idx], td[flat_idx], env
+
+    def _make_beam_step(self, logprobs: torch.Tensor):
+        aug_batch_size, num_nodes = logprobs.shape  # num nodes
+        batch_size = aug_batch_size // self.beam_width
+        batch_beam_sequence = (
+            torch.arange(0, batch_size).repeat(self.beam_width).to(logprobs.device)
         )
 
-        # text depot
-        ax.text(
-            locs[0, 0],
-            locs[0, 1] - 0.025,
-            "Depot",
-            horizontalalignment="center",
-            verticalalignment="top",
-            fontsize=10,
-            color=cm.Set2(2),
+        # [BS*BW, num_nodes] + [BS*BW, 1] -> [BS*BW, num_nodes]
+        log_beam_prob = logprobs + self.parent_beam_logprobs  #
+
+        # [BS, num_nodes * BW]
+        log_beam_prob_hstacked = torch.cat(log_beam_prob.split(batch_size), dim=1)
+        # [BS, BW]
+        topk_logprobs, topk_ind = torch.topk(
+            log_beam_prob_hstacked, self.beam_width, dim=1
         )
 
-        # plot actions
-        color_idx = 0
-        for action_idx in range(len(actions) - 1):
-            if actions[action_idx] == 0:
-                color_idx += 1
-            from_loc = locs[actions[action_idx]]
-            to_loc = locs[actions[action_idx + 1]]
-            ax.plot(
-                [from_loc[0], to_loc[0]],
-                [from_loc[1], to_loc[1]],
-                color=out(color_idx),
-                lw=1,
-            )
-            ax.annotate(
-                "",
-                xy=(to_loc[0], to_loc[1]),
-                xytext=(from_loc[0], from_loc[1]),
-                arrowprops=dict(arrowstyle="-|>", color=out(color_idx)),
-                size=15,
-                annotation_clip=False,
-            )
-
-        # Setup limits and show
-        ax.set_xlim(-0.05, 1.05)
-        ax.set_ylim(-0.05, 1.05)
+        # [BS*BW, 1]
+        logprobs_selected = torch.hstack(torch.unbind(topk_logprobs, 1)).unsqueeze(1)
+
+        # [BS*BW, 1]
+        topk_ind = torch.hstack(torch.unbind(topk_ind, 1))
+
+        # since we stack the logprobs from the distinct branches, the indices in
+        # topk dont correspond to node indices directly and need to be translated
+        selected = topk_ind % num_nodes  # determine node index
+
+        # calc parent this branch comes from
+        beam_parent = (topk_ind // num_nodes).int()
+
+        batch_beam_idx = batch_beam_sequence + beam_parent * batch_size
+
+        self.parent_beam_logprobs = logprobs_selected
+        self.beam_path.append(beam_parent)
+
+        return selected, batch_beam_idx
```

### Comparing `rl4co-0.3.3/rl4co/envs/routing/pdp.py` & `rl4co-0.4.0/rl4co/envs/routing/mtsp/env.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,292 +1,246 @@
 from typing import Optional
 
+import numpy as np
 import torch
 
 from tensordict.tensordict import TensorDict
 from torchrl.data import (
     BoundedTensorSpec,
     CompositeSpec,
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
 from rl4co.envs.common.base import RL4COEnvBase
-from rl4co.utils.ops import gather_by_index, get_tour_length
+from rl4co.envs.common.utils import batch_to_scalar
+from rl4co.utils.ops import gather_by_index, get_distance, get_tour_length
 
+from .generator import MTSPGenerator
+from .render import render
 
-class PDPEnv(RL4COEnvBase):
-    """Pickup and Delivery Problem (PDP) environment.
-    The environment is made of num_loc + 1 locations (cities):
-        - 1 depot
-        - `num_loc` / 2 pickup locations
-        - `num_loc` / 2 delivery locations
-    The goal is to visit all the pickup and delivery locations in the shortest path possible starting from the depot
-    The conditions is that the agent must visit a pickup location before visiting its corresponding delivery location
+
+class MTSPEnv(RL4COEnvBase):
+    """Multiple Traveling Salesman Problem environment
+    At each step, an agent chooses to visit a city. A maximum of `num_agents` agents can be employed to visit the cities.
+    The cost can be defined in two ways:
+        - `minmax`: (default) the reward is the maximum of the path lengths of all the agents
+        - `sum`: the cost is the sum of the path lengths of all the agents
+    Reward is - cost, so the goal is to maximize the reward (minimize the cost).
+
+    Observations:
+        - locations of the depot and each customer.
+        - number of agents.
+        - the current agent index.
+        - the current location of the vehicle.
+
+    Constrains:
+        - each agent's tour starts and ends at the depot.
+        - each customer must be visited exactly once.
+
+    Finish condition:
+        - all customers are visited and all agents back to the depot.
+
+    Reward:
+        There are two ways to calculate the cost (-reward):
+        - `minmax`: (default) the cost is the maximum of the path lengths of all the agents.
+        - `sum`: the cost is the sum of the path lengths of all the agents.
 
     Args:
-        num_loc: number of locations (cities) in the TSP
-        td_params: parameters of the environment
-        seed: seed for the environment
-        device: device to use.  Generally, no need to set as tensors are updated on the fly
+        cost_type: type of cost to use, either `minmax` or `sum`
+        generator: MTSPGenerator instance as the data generator
+        generator_params: parameters for the generator
     """
 
-    name = "pdp"
+    name = "mtsp"
 
     def __init__(
         self,
-        num_loc: int = 20,
-        min_loc: float = 0,
-        max_loc: float = 1,
-        td_params: TensorDict = None,
+        generator: MTSPGenerator = None,
+        generator_params: dict = {},
+        cost_type: str = "minmax",
         **kwargs,
     ):
         super().__init__(**kwargs)
-        self.num_loc = num_loc
-        self.min_loc = min_loc
-        self.max_loc = max_loc
-        self._make_spec(td_params)
+        if generator is None:
+            generator = MTSPGenerator(**generator_params)
+        self.generator = generator
+        self.cost_type = cost_type
+        self._make_spec(self.generator)
 
     @staticmethod
     def _step(td: TensorDict) -> TensorDict:
-        current_node = td["action"].unsqueeze(-1)
+        # Initial variables
+        is_first_action = batch_to_scalar(td["i"]) == 0
+        current_node = td["action"]
+        first_node = current_node if is_first_action else td["first_node"]
 
-        num_loc = td["locs"].shape[-2] - 1  # except depot
+        # Get the locations of the current node and the previous node and the depot
+        cur_loc = gather_by_index(td["locs"], current_node)
+        prev_loc = gather_by_index(
+            td["locs"], td["current_node"]
+        )  # current_node is the previous node
+        depot_loc = td["locs"][..., 0, :]
 
-        # Pickup and delivery node pair of selected node
-        new_to_deliver = (current_node + num_loc // 2) % (num_loc + 1)
+        # If current_node is the depot, then increment agent_idx
+        cur_agent_idx = td["agent_idx"] + (current_node == 0).long()
 
-        # Set available to 0 (i.e., we visited the node)
-        available = td["available"].scatter(
-            -1, current_node.expand_as(td["action_mask"]), 0
+        # Set not visited to 0 (i.e., we visited the node)
+        available = td["action_mask"].scatter(
+            -1, current_node[..., None].expand_as(td["action_mask"]), 0
+        )
+        # Available[..., 0] is the depot, which is always available unless:
+        # - current_node is the depot
+        # - agent_idx greater than num_agents -1
+        available[..., 0] = torch.logical_and(
+            current_node != 0, td["agent_idx"] < td["num_agents"] - 1
         )
 
-        to_deliver = td["to_deliver"].scatter(
-            -1, new_to_deliver.expand_as(td["to_deliver"]), 1
+        # We are done there are no unvisited locations except the depot
+        done = torch.count_nonzero(available[..., 1:], dim=-1) == 0
+
+        # If done is True, then we make the depot available again, so that it will be selected as the next node with prob 1
+        available[..., 0] = torch.logical_or(done, available[..., 0])
+
+        # Update the current length
+        current_length = td["current_length"] + get_distance(cur_loc, prev_loc)
+
+        # If done, we add the distance from the current_node to the depot as well
+        current_length = torch.where(
+            done, current_length + get_distance(cur_loc, depot_loc), current_length
         )
 
-        # Action is feasible if the node is not visited and is to deliver
-        # action_mask = torch.logical_and(available, to_deliver)
-        action_mask = available & to_deliver
+        # We update the max_subtour_length and reset the current_length
+        max_subtour_length = torch.where(
+            current_length > td["max_subtour_length"],
+            current_length,
+            td["max_subtour_length"],
+        )
 
-        # We are done there are no unvisited locations
-        done = torch.count_nonzero(available, dim=-1) == 0
+        # If current agent is different from previous agent, then we have a new subtour and reset the length
+        current_length *= (cur_agent_idx == td["agent_idx"]).float()
 
-        # The reward is calculated outside via get_reward for efficiency, so we set it to 0 here
-        reward = torch.zeros_like(done)
+        # The reward is the negative of the max_subtour_length (minmax objective)
+        reward = -max_subtour_length
 
-        # Update step
         td.update(
             {
+                "max_subtour_length": max_subtour_length,
+                "current_length": current_length,
+                "agent_idx": cur_agent_idx,
+                "first_node": first_node,
                 "current_node": current_node,
-                "available": available,
-                "to_deliver": to_deliver,
                 "i": td["i"] + 1,
-                "action_mask": action_mask,
+                "action_mask": available,
                 "reward": reward,
                 "done": done,
             }
         )
+
         return td
 
     def _reset(self, td: Optional[TensorDict] = None, batch_size=None) -> TensorDict:
-        if batch_size is None:
-            batch_size = self.batch_size if td is None else td.batch_size
-
-        if td is None or td.is_empty():
-            td = self.generate_data(batch_size=batch_size)
+        device = td.device
 
-        self.to(td.device)
-
-        locs = torch.cat((td["depot"][:, None, :], td["locs"]), -2)
-
-        # Pick is 1, deliver is 0 [batch_size, graph_size+1], [1,1...1, 0...0]
-        to_deliver = torch.cat(
-            [
-                torch.ones(
-                    *batch_size,
-                    self.num_loc // 2 + 1,
-                    dtype=torch.bool,
-                    device=self.device,
-                ),
-                torch.zeros(
-                    *batch_size, self.num_loc // 2, dtype=torch.bool, device=self.device
-                ),
-            ],
-            dim=-1,
-        )
+        # Keep track of the agent number to know when to stop
+        agent_idx = torch.zeros((*batch_size,), dtype=torch.int64, device=device)
 
-        # Cannot visit depot at first step # [0,1...1] so set not available
-        available = torch.ones(
-            (*batch_size, self.num_loc + 1), dtype=torch.bool, device=self.device
-        )
-        action_mask = ~available.contiguous()  # [batch_size, graph_size+1]
-        action_mask[..., 0] = 1  # First step is always the depot
+        # Make variable for max_subtour_length between subtours
+        max_subtour_length = torch.zeros(batch_size, dtype=torch.float32, device=device)
+        current_length = torch.zeros(batch_size, dtype=torch.float32, device=device)
 
         # Other variables
-        current_node = torch.zeros(
-            (*batch_size, 1), dtype=torch.int64, device=self.device
-        )
-        i = torch.zeros((*batch_size, 1), dtype=torch.int64, device=self.device)
+        current_node = torch.zeros((*batch_size,), dtype=torch.int64, device=device)
+        available = torch.ones(
+            (*batch_size, self.generator.num_loc), dtype=torch.bool, device=device
+        )  # 1 means not visited, i.e. action is allowed
+        available[..., 0] = 0  # Depot is not available as first node
+        i = torch.zeros((*batch_size,), dtype=torch.int64, device=device)
 
         return TensorDict(
             {
-                "locs": locs,
+                "locs": td["locs"],  # depot is first node
+                "num_agents": td["num_agents"],
+                "max_subtour_length": max_subtour_length,
+                "current_length": current_length,
+                "agent_idx": agent_idx,
+                "first_node": current_node,
                 "current_node": current_node,
-                "to_deliver": to_deliver,
-                "available": available,
                 "i": i,
-                "action_mask": action_mask,
+                "action_mask": available,
             },
             batch_size=batch_size,
         )
 
-    def _make_spec(self, td_params: TensorDict):
+    def _make_spec(self, generator: MTSPGenerator):
         """Make the observation and action specs from the parameters."""
         self.observation_spec = CompositeSpec(
             locs=BoundedTensorSpec(
-                low=self.min_loc,
-                high=self.max_loc,
-                shape=(self.num_loc + 1, 2),
+                low=generator.min_loc,
+                high=generator.max_loc,
+                shape=(generator.num_loc, 2),
                 dtype=torch.float32,
             ),
-            current_node=UnboundedDiscreteTensorSpec(
+            num_agents=UnboundedDiscreteTensorSpec(
                 shape=(1),
                 dtype=torch.int64,
             ),
-            to_deliver=UnboundedDiscreteTensorSpec(
+            agent_idx=UnboundedDiscreteTensorSpec(
+                shape=(1),
+                dtype=torch.int64,
+            ),
+            current_length=UnboundedContinuousTensorSpec(
+                shape=(1),
+                dtype=torch.float32,
+            ),
+            max_subtour_length=UnboundedContinuousTensorSpec(
+                shape=(1),
+                dtype=torch.float32,
+            ),
+            first_node=UnboundedDiscreteTensorSpec(
+                shape=(1),
+                dtype=torch.int64,
+            ),
+            current_node=UnboundedDiscreteTensorSpec(
                 shape=(1),
                 dtype=torch.int64,
             ),
             i=UnboundedDiscreteTensorSpec(
                 shape=(1),
                 dtype=torch.int64,
             ),
             action_mask=UnboundedDiscreteTensorSpec(
-                shape=(self.num_loc + 1),
+                shape=(generator.num_loc),
                 dtype=torch.bool,
             ),
             shape=(),
         )
         self.action_spec = BoundedTensorSpec(
             shape=(1,),
             dtype=torch.int64,
             low=0,
-            high=self.num_loc + 1,
+            high=generator.num_loc,
         )
-        self.reward_spec = UnboundedContinuousTensorSpec(shape=(1,))
-        self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
+        self.reward_spec = UnboundedContinuousTensorSpec()
+        self.done_spec = UnboundedDiscreteTensorSpec(dtype=torch.bool)
 
-    @staticmethod
-    def get_reward(td, actions) -> TensorDict:
-        # assert (actions[:, 0] == 0).all(), "Not starting at depot"
-        assert (
-            torch.arange(actions.size(1), out=actions.data.new())
-            .view(1, -1)
-            .expand_as(actions)
-            == actions.data.sort(1)[0]
-        ).all(), "Not visiting all nodes"
-
-        visited_time = torch.argsort(
-            actions, 1
-        )  # index of pickup less than index of delivery
-        assert (
-            visited_time[:, 1 : actions.size(1) // 2 + 1]
-            < visited_time[:, actions.size(1) // 2 + 1 :]
-        ).all(), "Deliverying without pick-up"
-
-        # Gather locations in the order of actions and get reward = -(total distance)
-        locs_ordered = gather_by_index(td["locs"], actions)  # [batch, graph_size+1, 2]
-        return -get_tour_length(locs_ordered)
-
-    def generate_data(self, batch_size) -> TensorDict:
-        batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
-
-        # Initialize the locations (including the depot which is always the first node)
-        locs_with_depot = (
-            torch.FloatTensor(*batch_size, self.num_loc + 1, 2)
-            .uniform_(self.min_loc, self.max_loc)
-            .to(self.device)
-        )
+    def _get_reward(self, td, actions=None) -> TensorDict:
+        # With minmax, get the maximum distance among subtours, calculated in the model
+        if self.cost_type == "minmax":
+            return td["reward"].squeeze(-1)
+
+        # With distance, same as TSP
+        elif self.cost_type == "sum":
+            locs = td["locs"]
+            locs_ordered = locs.gather(1, actions.unsqueeze(-1).expand_as(locs))
+            return -get_tour_length(locs_ordered)
 
-        return TensorDict(
-            {
-                "locs": locs_with_depot[..., 1:, :],
-                "depot": locs_with_depot[..., 0, :],
-            },
-            batch_size=batch_size,
-        )
+        else:
+            raise ValueError(f"Cost type {self.cost_type} not supported")
 
     @staticmethod
-    def render(td: TensorDict, actions=None, ax=None):
-        import matplotlib.pyplot as plt
+    def check_solution_validity(td: TensorDict, actions: torch.Tensor):
+        assert True, "Not implemented"
 
-        markersize = 8
-
-        td = td.detach().cpu()
-        # if batch_size greater than 0 , we need to select the first batch element
-        if td.batch_size != torch.Size([]):
-            td = td[0]
-            if actions is not None:
-                actions = actions[0]
-
-        # Variables
-        init_deliveries = td["to_deliver"][1:]
-        delivery_locs = td["locs"][1:][~init_deliveries.bool()]
-        pickup_locs = td["locs"][1:][init_deliveries.bool()]
-        depot_loc = td["locs"][0]
-        actions = actions if actions is not None else td["action"]
-
-        fig, ax = plt.subplots()
-
-        # Plot the actions in order
-        for i in range(len(actions)):
-            from_node = actions[i]
-            to_node = (
-                actions[i + 1] if i < len(actions) - 1 else actions[0]
-            )  # last goes back to depot
-            from_loc = td["locs"][from_node]
-            to_loc = td["locs"][to_node]
-            ax.plot([from_loc[0], to_loc[0]], [from_loc[1], to_loc[1]], "k-")
-            ax.annotate(
-                "",
-                xy=(to_loc[0], to_loc[1]),
-                xytext=(from_loc[0], from_loc[1]),
-                arrowprops=dict(arrowstyle="->", color="black"),
-                annotation_clip=False,
-            )
-
-        # Plot the depot location
-        ax.plot(
-            depot_loc[0],
-            depot_loc[1],
-            "g",
-            marker="s",
-            markersize=markersize,
-            label="Depot",
-        )
-
-        # Plot the pickup locations
-        for i, pickup_loc in enumerate(pickup_locs):
-            ax.plot(
-                pickup_loc[0],
-                pickup_loc[1],
-                "r",
-                marker="^",
-                markersize=markersize,
-                label="Pickup" if i == 0 else None,
-            )
-
-        # Plot the delivery locations
-        for i, delivery_loc in enumerate(delivery_locs):
-            ax.plot(
-                delivery_loc[0],
-                delivery_loc[1],
-                "b",
-                marker="v",
-                markersize=markersize,
-                label="Delivery" if i == 0 else None,
-            )
-
-        # Setup limits and show
-        ax.set_xlim(-0.05, 1.05)
-        ax.set_ylim(-0.05, 1.05)
+    @staticmethod
+    def render(td, actions=None, ax=None):
+        return render(td, actions, ax)
```

### Comparing `rl4co-0.3.3/rl4co/envs/routing/sdvrp.py` & `rl4co-0.4.0/rl4co/envs/routing/sdvrp/env.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,63 +9,60 @@
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
 from rl4co.utils.ops import gather_by_index
 from rl4co.utils.pylogger import get_pylogger
 
-from .cvrp import CVRPEnv
+from ..cvrp.env import CVRPEnv
+from ..cvrp.generator import CVRPGenerator
 
 log = get_pylogger(__name__)
 
 
 class SDVRPEnv(CVRPEnv):
     """Split Delivery Vehicle Routing Problem (SDVRP) environment.
     SDVRP is a generalization of CVRP, where nodes can be visited multiple times and a fraction of the demand can be met.
     At each step, the agent chooses a customer to visit depending on the current location and the remaining capacity.
     When the agent visits a customer, the remaining capacity is updated. If the remaining capacity is not enough to
-    visit any customer, the agent must go back to the depot. The reward is the -infinite unless the agent visits all the cities.
+    visit any customer, the agent must go back to the depot. The reward is the -infinite unless the agent visits all the customers.
     In that case, the reward is (-)length of the path: maximizing the reward is equivalent to minimizing the path length.
 
+    Observations:
+        - location of the depot.
+        - locations and demand/remaining demand of each customer 
+        - current location of the vehicle.
+        - the remaining capacity of the vehicle.
+
+    Constraints:
+        - the tour starts and ends at the depot.
+        - each customer can be visited multiple times.
+        - the vehicle cannot visit customers exceed the remaining capacity.
+        - the vehicle can return to the depot to refill the capacity.
+
+    Finish Condition:
+        - the vehicle has finished all customers demand and returned to the depot.
+
+    Reward:
+        - (minus) the negative length of the path.
+
     Args:
-        num_loc: number of locations (cities) in the VRP, without the depot. (e.g. 10 means 10 locs + 1 depot)
-        min_loc: minimum value for the location coordinates
-        max_loc: maximum value for the location coordinates
-        min_demand: minimum value for the demand of each customer
-        max_demand: maximum value for the demand of each customer
-        vehicle_capacity: capacity of the vehicle
-        capacity: capacity of the vehicle
-        td_params: parameters of the environment
+        generator: CVRPGenerator instance as the data generator
+        generator_params: parameters for the generator
     """
 
     name = "sdvrp"
 
     def __init__(
         self,
-        num_loc: int = 20,
-        min_loc: float = 0,
-        max_loc: float = 1,
-        min_demand: float = 1,
-        max_demand: float = 10,
-        vehicle_capacity: float = 1.0,
-        capacity: float = None,
-        td_params: TensorDict = None,
+        generator: CVRPGenerator = None,
+        generator_params: dict = {},
         **kwargs,
     ):
-        super().__init__(
-            num_loc=num_loc,
-            min_loc=min_loc,
-            max_loc=max_loc,
-            min_demand=min_demand,
-            max_demand=max_demand,
-            vehicle_capacity=vehicle_capacity,
-            capacity=capacity,
-            td_params=td_params,
-            **kwargs,
-        )
+        super().__init__(generator, generator_params, **kwargs)
 
     def _step(self, td: TensorDict) -> TensorDict:
         # Update the state
         current_node = td["action"][:, None]  # Add dimension for step
 
         # Not selected_demand is demand of first node (by clamp) so incorrect for nodes that visit depot!
         selected_demand = gather_by_index(
@@ -105,36 +102,30 @@
         return td
 
     def _reset(
         self,
         td: Optional[TensorDict] = None,
         batch_size: Optional[list] = None,
     ) -> TensorDict:
-        if batch_size is None:
-            batch_size = self.batch_size if td is None else td["locs"].shape[:-2]
-
-        if td is None or td.is_empty():
-            td = self.generate_data(batch_size=batch_size)
-
-        self.to(td.device)
+        device = td.device
 
         # Create reset TensorDict
         reset_td = TensorDict(
             {
                 "locs": torch.cat((td["depot"][..., None, :], td["locs"]), -2),
                 "demand": td["demand"],
                 "demand_with_depot": torch.cat(
                     (torch.zeros_like(td["demand"][..., 0:1]), td["demand"]), -1
                 ),
                 "current_node": torch.zeros(
-                    *batch_size, 1, dtype=torch.long, device=self.device
+                    *batch_size, 1, dtype=torch.long, device=device
                 ),
-                "used_capacity": torch.zeros((*batch_size, 1), device=self.device),
+                "used_capacity": torch.zeros((*batch_size, 1), device=device),
                 "vehicle_capacity": torch.full(
-                    (*batch_size, 1), self.vehicle_capacity, device=self.device
+                    (*batch_size, 1), self.generator.vehicle_capacity, device=device
                 ),
             },
             batch_size=batch_size,
         )
         reset_td.set("action_mask", self.get_action_mask(reset_td))
         return reset_td
 
@@ -168,52 +159,52 @@
             d = torch.min(demands[rng, a], td["vehicle_capacity"].squeeze(-1) - used_cap)
             demands[rng, a] -= d
             used_cap += d
             used_cap[a == 0] = 0
             a_prev = a
         assert (demands == 0).all(), "All demand must be satisfied"
 
-    def _make_spec(self, td_params: TensorDict):
+    def _make_spec(self, generator):
         """Make the observation and action specs from the parameters."""
         self.observation_spec = CompositeSpec(
             locs=BoundedTensorSpec(
-                low=self.min_loc,
-                high=self.max_loc,
-                shape=(self.num_loc + 1, 2),
+                low=generator.min_loc,
+                high=generator.max_loc,
+                shape=(generator.num_loc + 1, 2),
                 dtype=torch.float32,
             ),
             current_node=UnboundedDiscreteTensorSpec(
                 shape=(1),
                 dtype=torch.int64,
             ),
             demand=BoundedTensorSpec(
-                low=self.min_demand,
-                high=self.max_demand,
-                shape=(self.num_loc, 1),  # demand is only for customers
+                low=generator.min_demand,
+                high=generator.max_demand,
+                shape=(generator.num_loc, 1),  # demand is only for customers
                 dtype=torch.float32,
             ),
             demand_with_depot=BoundedTensorSpec(
-                low=self.min_demand,
-                high=self.max_demand,
-                shape=(self.num_loc + 1, 1),
+                low=generator.min_demand,
+                high=generator.max_demand,
+                shape=(generator.num_loc + 1, 1),
                 dtype=torch.float32,
             ),
             used_capacity=BoundedTensorSpec(
                 low=0,
-                high=self.vehicle_capacity,
+                high=generator.vehicle_capacity,
                 shape=(1,),
                 dtype=torch.float32,
             ),
             action_mask=UnboundedDiscreteTensorSpec(
-                shape=(self.num_loc + 1, 1),
+                shape=(generator.num_loc + 1, 1),
                 dtype=torch.bool,
             ),
             shape=(),
         )
         self.action_spec = BoundedTensorSpec(
             shape=(1,),
             dtype=torch.int64,
             low=0,
-            high=self.num_loc + 1,
+            high=generator.num_loc + 1,
         )
         self.reward_spec = UnboundedContinuousTensorSpec(shape=(1,))
         self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
```

### Comparing `rl4co-0.3.3/rl4co/envs/routing/spctsp.py` & `rl4co-0.4.0/rl4co/envs/routing/spctsp/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from rl4co.utils.pylogger import get_pylogger
 
-from .pctsp import PCTSPEnv
+from ..pctsp.env import PCTSPEnv
 
 log = get_pylogger(__name__)
 
 
 class SPCTSPEnv(PCTSPEnv):
     """Stochastic Prize Collecting Traveling Salesman Problem (SPCTSP) environment.
```

### Comparing `rl4co-0.3.3/rl4co/envs/routing/tsp.py` & `rl4co-0.4.0/rl4co/envs/routing/pdp/env.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,208 +8,204 @@
     CompositeSpec,
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
 from rl4co.envs.common.base import RL4COEnvBase
 from rl4co.utils.ops import gather_by_index, get_tour_length
-from rl4co.utils.pylogger import get_pylogger
 
-log = get_pylogger(__name__)
+from .generator import PDPGenerator
+from .render import render
 
 
-class TSPEnv(RL4COEnvBase):
-    """
-    Traveling Salesman Problem environment
-    At each step, the agent chooses a city to visit. The reward is 0 unless the agent visits all the cities.
-    In that case, the reward is (-)length of the path: maximizing the reward is equivalent to minimizing the path length.
+class PDPEnv(RL4COEnvBase):
+    """Pickup and Delivery Problem (PDP) environment.
+    The environment is made of num_loc + 1 locations (cities):
+        - 1 depot
+        - `num_loc` / 2 pickup locations
+        - `num_loc` / 2 delivery locations
+    The goal is to visit all the pickup and delivery locations in the shortest path possible starting from the depot
+    The conditions is that the agent must visit a pickup location before visiting its corresponding delivery location
+
+    Observations:
+        - locations of the depot, pickup, and delivery locations
+        - current location of the vehicle
+        - the remaining locations to deliver
+        - the visited locations
+        - the current step
+
+    Constraints:
+        - the tour starts and ends at the depot
+        - each pickup location must be visited before its corresponding delivery location
+        - the vehicle cannot visit the same location twice
+
+    Finish Condition:
+        - the vehicle has visited all locations
+
+    Reward:
+        - (minus) the negative length of the path
 
     Args:
-        num_loc: number of locations (cities) in the TSP
-        td_params: parameters of the environment
-        seed: seed for the environment
-        device: device to use.  Generally, no need to set as tensors are updated on the fly
+        generator: PDPGenerator instance as the data generator
+        generator_params: parameters for the generator
     """
 
-    name = "tsp"
+    name = "pdp"
 
     def __init__(
         self,
-        num_loc: int = 20,
-        min_loc: float = 0,
-        max_loc: float = 1,
-        td_params: TensorDict = None,
+        generator: PDPGenerator = None,
+        generator_params: dict = {},
         **kwargs,
     ):
         super().__init__(**kwargs)
-        self.num_loc = num_loc
-        self.min_loc = min_loc
-        self.max_loc = max_loc
-        self._make_spec(td_params)
+        if generator is None:
+            generator = PDPGenerator(**generator_params)
+        self.generator = generator
+        self._make_spec(self.generator)
 
     @staticmethod
     def _step(td: TensorDict) -> TensorDict:
-        current_node = td["action"]
-        first_node = current_node if td["i"].all() == 0 else td["first_node"]
+        current_node = td["action"].unsqueeze(-1)
+
+        num_loc = td["locs"].shape[-2] - 1  # except depot
+
+        # Pickup and delivery node pair of selected node
+        new_to_deliver = (current_node + num_loc // 2) % (num_loc + 1)
+
+        # Set available to 0 (i.e., we visited the node)
+        available = td["available"].scatter(
+            -1, current_node.expand_as(td["action_mask"]), 0
+        )
 
-        # # Set not visited to 0 (i.e., we visited the node)
-        available = td["action_mask"].scatter(
-            -1, current_node.unsqueeze(-1).expand_as(td["action_mask"]), 0
+        to_deliver = td["to_deliver"].scatter(
+            -1, new_to_deliver.expand_as(td["to_deliver"]), 1
         )
 
+        # Action is feasible if the node is not visited and is to deliver
+        # action_mask = torch.logical_and(available, to_deliver)
+        action_mask = available & to_deliver
+
         # We are done there are no unvisited locations
-        done = torch.sum(available, dim=-1) == 0
+        done = torch.count_nonzero(available, dim=-1) == 0
 
         # The reward is calculated outside via get_reward for efficiency, so we set it to 0 here
         reward = torch.zeros_like(done)
 
+        # Update step
         td.update(
             {
-                "first_node": first_node,
                 "current_node": current_node,
+                "available": available,
+                "to_deliver": to_deliver,
                 "i": td["i"] + 1,
-                "action_mask": available,
+                "action_mask": action_mask,
                 "reward": reward,
                 "done": done,
-            },
+            }
         )
         return td
 
     def _reset(self, td: Optional[TensorDict] = None, batch_size=None) -> TensorDict:
-        # Initialize locations
-        init_locs = td["locs"] if td is not None else None
-        if batch_size is None:
-            batch_size = self.batch_size if init_locs is None else init_locs.shape[:-2]
-        device = init_locs.device if init_locs is not None else self.device
-        self.to(device)
-        if init_locs is None:
-            init_locs = self.generate_data(batch_size=batch_size).to(device)["locs"]
-        batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
+        device = td.device
 
-        # We do not enforce loading from self for flexibility
-        num_loc = init_locs.shape[-2]
+        locs = torch.cat((td["depot"][:, None, :], td["locs"]), -2)
 
-        # Other variables
-        current_node = torch.zeros((batch_size), dtype=torch.int64, device=device)
+        # Pick is 1, deliver is 0 [batch_size, graph_size+1], [1,1...1, 0...0]
+        to_deliver = torch.cat(
+            [
+                torch.ones(
+                    *batch_size,
+                    self.generator.num_loc // 2 + 1,
+                    dtype=torch.bool,
+                    device=device,
+                ),
+                torch.zeros(
+                    *batch_size, self.generator.num_loc // 2, dtype=torch.bool, device=device
+                ),
+            ],
+            dim=-1,
+        )
+
+        # Cannot visit depot at first step # [0,1...1] so set not available
         available = torch.ones(
-            (*batch_size, num_loc), dtype=torch.bool, device=device
-        )  # 1 means not visited, i.e. action is allowed
+            (*batch_size, self.generator.num_loc + 1), dtype=torch.bool, device=device
+        )
+        action_mask = ~available.contiguous()  # [batch_size, graph_size+1]
+        action_mask[..., 0] = 1  # First step is always the depot
+
+        # Other variables
+        current_node = torch.zeros(
+            (*batch_size, 1), dtype=torch.int64, device=device
+        )
         i = torch.zeros((*batch_size, 1), dtype=torch.int64, device=device)
 
         return TensorDict(
             {
-                "locs": init_locs,
-                "first_node": current_node,
+                "locs": locs,
                 "current_node": current_node,
+                "to_deliver": to_deliver,
+                "available": available,
                 "i": i,
-                "action_mask": available,
-                "reward": torch.zeros((*batch_size, 1), dtype=torch.float32),
+                "action_mask": action_mask,
             },
             batch_size=batch_size,
         )
 
-    def _make_spec(self, td_params):
-        """Make the observation and action specs from the parameters"""
+    def _make_spec(self, generator: PDPGenerator):
+        """Make the observation and action specs from the parameters."""
         self.observation_spec = CompositeSpec(
             locs=BoundedTensorSpec(
-                low=self.min_loc,
-                high=self.max_loc,
-                shape=(self.num_loc, 2),
+                low=generator.min_loc,
+                high=generator.max_loc,
+                shape=(generator.num_loc + 1, 2),
                 dtype=torch.float32,
             ),
-            first_node=UnboundedDiscreteTensorSpec(
+            current_node=UnboundedDiscreteTensorSpec(
                 shape=(1),
                 dtype=torch.int64,
             ),
-            current_node=UnboundedDiscreteTensorSpec(
+            to_deliver=UnboundedDiscreteTensorSpec(
                 shape=(1),
                 dtype=torch.int64,
             ),
             i=UnboundedDiscreteTensorSpec(
                 shape=(1),
                 dtype=torch.int64,
             ),
             action_mask=UnboundedDiscreteTensorSpec(
-                shape=(self.num_loc),
+                shape=(generator.num_loc + 1),
                 dtype=torch.bool,
             ),
             shape=(),
         )
         self.action_spec = BoundedTensorSpec(
             shape=(1,),
             dtype=torch.int64,
             low=0,
-            high=self.num_loc,
+            high=generator.num_loc + 1,
         )
         self.reward_spec = UnboundedContinuousTensorSpec(shape=(1,))
         self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
 
-    def get_reward(self, td, actions) -> TensorDict:
-        if self.check_solution:
-            self.check_solution_validity(td, actions)
-
-        # Gather locations in order of tour and return distance between them (i.e., -reward)
-        locs_ordered = gather_by_index(td["locs"], actions)
+    @staticmethod
+    def _get_reward(td, actions) -> TensorDict:
+        # Gather locations in the order of actions and get reward = -(total distance)
+        locs_ordered = gather_by_index(td["locs"], actions)  # [batch, graph_size+1, 2]
         return -get_tour_length(locs_ordered)
 
-    @staticmethod
-    def check_solution_validity(td: TensorDict, actions: torch.Tensor):
-        """Check that solution is valid: nodes are visited exactly once"""
+    def check_solution_validity(self, td, actions):
+        # assert (actions[:, 0] == 0).all(), "Not starting at depot"
         assert (
             torch.arange(actions.size(1), out=actions.data.new())
             .view(1, -1)
             .expand_as(actions)
             == actions.data.sort(1)[0]
-        ).all(), "Invalid tour"
-
-    def generate_data(self, batch_size) -> TensorDict:
-        batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
-        locs = (
-            torch.rand((*batch_size, self.num_loc, 2), generator=self.rng)
-            * (self.max_loc - self.min_loc)
-            + self.min_loc
-        )
-        return TensorDict({"locs": locs}, batch_size=batch_size)
+        ).all(), "Not visiting all nodes"
 
-    @staticmethod
-    def render(td, actions=None, ax=None):
-        import matplotlib.pyplot as plt
-        import numpy as np
-
-        if ax is None:
-            # Create a plot of the nodes
-            _, ax = plt.subplots()
-
-        td = td.detach().cpu()
-
-        if actions is None:
-            actions = td.get("action", None)
-        # if batch_size greater than 0 , we need to select the first batch element
-        if td.batch_size != torch.Size([]):
-            td = td[0]
-            actions = actions[0]
-
-        locs = td["locs"]
-
-        # gather locs in order of action if available
-        if actions is None:
-            log.warning("No action in TensorDict, rendering unsorted locs")
-        else:
-            actions = actions.detach().cpu()
-            locs = gather_by_index(locs, actions, dim=0)
-
-        # Cat the first node to the end to complete the tour
-        locs = torch.cat((locs, locs[0:1]))
-        x, y = locs[:, 0], locs[:, 1]
-
-        # Plot the visited nodes
-        ax.scatter(x, y, color="tab:blue")
-
-        # Add arrows between visited nodes as a quiver plot
-        dx, dy = np.diff(x), np.diff(y)
-        ax.quiver(
-            x[:-1], y[:-1], dx, dy, scale_units="xy", angles="xy", scale=1, color="k"
-        )
-
-        # Setup limits and show
-        ax.set_xlim(-0.05, 1.05)
-        ax.set_ylim(-0.05, 1.05)
+        visited_time = torch.argsort(
+            actions, 1
+        )  # index of pickup less than index of delivery
+        assert (
+            visited_time[:, 1 : actions.size(1) // 2 + 1]
+            < visited_time[:, actions.size(1) // 2 + 1 :]
+        ).all(), "Deliverying without pick-up"
```

### Comparing `rl4co-0.3.3/rl4co/envs/scheduling/smtwtp.py` & `rl4co-0.4.0/rl4co/envs/scheduling/smtwtp/env.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,62 +9,71 @@
     UnboundedContinuousTensorSpec,
     UnboundedDiscreteTensorSpec,
 )
 
 from rl4co.envs.common.base import RL4COEnvBase
 from rl4co.utils.pylogger import get_pylogger
 
+from .generator import SMTWTPGenerator
+from .render import render
+
 log = get_pylogger(__name__)
 
 
 class SMTWTPEnv(RL4COEnvBase):
     """
     Single Machine Total Weighted Tardiness Problem environment as described in DeepACO (https://arxiv.org/pdf/2309.14032.pdf)
     SMTWTP is a scheduling problem in which a set of jobs must be processed on a single machine.
     Each job i has a processing time, a weight, and a due date. The objective is to minimize the sum of the weighted tardiness of all jobs,
     where the weighted tardiness of a job is defined as the product of its weight and the duration by which its completion time exceeds its due date.
     At each step, the agent chooses a job to process. The reward is 0 unless the agent processes all the jobs.
     In that case, the reward is (-)objective value of the processing order: maximizing the reward is equivalent to minimizing the objective.
 
+    Observation:
+        - job_due_time: the due time of each job
+        - job_weight: the weight of each job
+        - job_process_time: the process time of each job
+        - current_node: the current node
+        - action_mask: a mask of available actions
+        - current_time: the current time
+
+    Constants:
+        - num_job: number of jobs
+        - min_time_span: lower bound of jobs' due time. By default, jobs' due time is uniformly sampled from (min_time_span, max_time_span)
+        - max_time_span: upper bound of jobs' due time. By default, it will be set to num_job / 2
+        - min_job_weight: lower bound of jobs' weights. By default, jobs' weights are uniformly sampled from (min_job_weight, max_job_weight)
+        - max_job_weight: upper bound of jobs' weights
+        - min_process_time: lower bound of jobs' process time. By default, jobs' process time is uniformly sampled from (min_process_time, max_process_time)
+        - max_process_time: upper bound of jobs' process time
+
+    Finishing condition:
+        - All jobs are processed
+    
+    Reward:
+        - The reward is 0 unless the agent processes all the jobs.
+        - In that case, the reward is (-)objective value of the processing order: maximizing the reward is equivalent to minimizing the objective.
+
     Args:
-        num_job: number of jobs
-        min_time_span: lower bound of jobs' due time. By default, jobs' due time is uniformly sampled from (min_time_span, max_time_span)
-        max_time_span: upper bound of jobs' due time. By default, it will be set to num_job / 2
-        min_job_weight: lower bound of jobs' weights. By default, jobs' weights are uniformly sampled from (min_job_weight, max_job_weight)
-        max_job_weight: upper bound of jobs' weights
-        min_process_time: lower bound of jobs' process time. By default, jobs' process time is uniformly sampled from (min_process_time, max_process_time)
-        max_process_time: upper bound of jobs' process time
-        td_params: parameters of the environment
-        seed: seed for the environment
-        device: device to use.  Generally, no need to set as tensors are updated on the fly
+        generator: FFSPGenerator instance as the data generator
+        generator_params: parameters for the generator
     """
 
     name = "smtwtp"
 
     def __init__(
         self,
-        num_job: int = 10,
-        min_time_span: float = 0,
-        max_time_span: float = None,  # will be set to num_job/2 by default. In DeepACO, it is set to num_job, which would be too simple
-        min_job_weight: float = 0,
-        max_job_weight: float = 1,
-        min_process_time: float = 0,
-        max_process_time: float = 1,
-        td_params: TensorDict = None,
+        generator: SMTWTPGenerator = None,
+        generator_params: dict = {},
         **kwargs,
     ):
         super().__init__(**kwargs)
-        self.num_job = num_job
-        self.min_time_span = min_time_span
-        self.max_time_span = num_job / 2 if max_time_span is None else max_time_span
-        self.min_job_weight = min_job_weight
-        self.max_job_weight = max_job_weight
-        self.min_process_time = min_process_time
-        self.max_process_time = max_process_time
-        self._make_spec(td_params)
+        if generator is None:
+            generator = SMTWTPGenerator(**generator_params)
+        self.generator = generator
+        self._make_spec(self.generator)
 
     @staticmethod
     def _step(td: TensorDict) -> TensorDict:
         current_job = td["action"]
 
         # Set not visited to 0 (i.e., we visited the node)
         available = td["action_mask"].scatter(
@@ -91,33 +100,25 @@
                 "reward": reward,
                 "done": done,
             }
         )
         return td
 
     def _reset(self, td: Optional[TensorDict] = None, batch_size=None) -> TensorDict:
-        # Initialization
-        if batch_size is None:
-            batch_size = self.batch_size if td is None else td["job_due_time"].shape[:-1]
-        batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
-
-        device = td["job_due_time"].device if td is not None else self.device
-        self.to(device)
-
-        td = self.generate_data(batch_size) if td is None else td
+        device = td.device
 
         init_job_due_time = td["job_due_time"]
         init_job_process_time = td["job_process_time"]
         init_job_weight = td["job_weight"]
 
         # Other variables
         current_job = torch.zeros((*batch_size, 1), dtype=torch.int64, device=device)
         current_time = torch.zeros((*batch_size, 1), dtype=torch.int64, device=device)
         available = torch.ones(
-            (*batch_size, self.num_job + 1), dtype=torch.bool, device=device
+            (*batch_size, self.generator.num_job + 1), dtype=torch.bool, device=device
         )
         available[:, 0] = 0  # mask the starting dummy node
 
         return TensorDict(
             {
                 "job_due_time": init_job_due_time,
                 "job_weight": init_job_weight,
@@ -125,58 +126,58 @@
                 "current_job": current_job,
                 "current_time": current_time,
                 "action_mask": available,
             },
             batch_size=batch_size,
         )
 
-    def _make_spec(self, td_params: TensorDict = None):
+    def _make_spec(self, generator: SMTWTPGenerator) -> None:
         self.observation_spec = CompositeSpec(
             job_due_time=BoundedTensorSpec(
-                low=self.min_time_span,
-                high=self.max_time_span,
-                shape=(self.num_job + 1,),
+                low=generator.min_time_span,
+                high=generator.max_time_span,
+                shape=(generator.num_job + 1,),
                 dtype=torch.float32,
             ),
             job_weight=BoundedTensorSpec(
-                low=self.min_job_weight,
-                high=self.max_job_weight,
-                shape=(self.num_job + 1,),
+                low=generator.min_job_weight,
+                high=generator.max_job_weight,
+                shape=(generator.num_job + 1,),
                 dtype=torch.float32,
             ),
             job_process_time=BoundedTensorSpec(
-                low=self.min_process_time,
-                high=self.max_process_time,
-                shape=(self.num_job + 1,),
+                low=generator.min_process_time,
+                high=generator.max_process_time,
+                shape=(generator.num_job + 1,),
                 dtype=torch.float32,
             ),
             current_node=UnboundedDiscreteTensorSpec(
                 shape=(1,),
                 dtype=torch.int64,
             ),
             action_mask=UnboundedDiscreteTensorSpec(
-                shape=(self.num_job + 1,),
+                shape=(generator.num_job + 1,),
                 dtype=torch.bool,
             ),
             current_time=UnboundedContinuousTensorSpec(
                 shape=(1,),
                 dtype=torch.float32,
             ),
             shape=(),
         )
         self.action_spec = BoundedTensorSpec(
             shape=(1,),
             dtype=torch.int64,
             low=0,
-            high=self.num_job + 1,
+            high=generator.num_job + 1,
         )
         self.reward_spec = UnboundedContinuousTensorSpec(shape=(1,))
         self.done_spec = UnboundedDiscreteTensorSpec(shape=(1,), dtype=torch.bool)
 
-    def get_reward(self, td, actions) -> TensorDict:
+    def _get_reward(self, td, actions) -> TensorDict:
         job_due_time = td["job_due_time"]
         job_weight = td["job_weight"]
         job_process_time = td["job_process_time"]
 
         batch_idx = torch.arange(
             job_process_time.shape[0], device=job_process_time.device
         ).unsqueeze(1)
@@ -189,43 +190,14 @@
         )  # ending time of each job
         job_tardiness = presum_process_time - ordered_due_time
         job_tardiness[job_tardiness < 0] = 0
         job_weighted_tardiness = ordered_job_weight * job_tardiness
 
         return -job_weighted_tardiness.sum(-1)
 
-    def generate_data(self, batch_size) -> TensorDict:
-        batch_size = [batch_size] if isinstance(batch_size, int) else batch_size
-        # Sampling according to Ye et al. (2023)
-        job_due_time = (
-            torch.FloatTensor(*batch_size, self.num_job + 1)
-            .uniform_(self.min_time_span, self.max_time_span)
-            .to(self.device)
-        )
-        job_weight = (
-            torch.FloatTensor(*batch_size, self.num_job + 1)
-            .uniform_(self.min_job_weight, self.max_job_weight)
-            .to(self.device)
-        )
-        job_process_time = (
-            torch.FloatTensor(*batch_size, self.num_job + 1)
-            .uniform_(self.min_process_time, self.max_process_time)
-            .to(self.device)
-        )
-
-        # Rollouts begin at dummy node 0, whose features are set to 0
-        job_due_time[:, 0] = 0
-        job_weight[:, 0] = 0
-        job_process_time[:, 0] = 0
-
-        return TensorDict(
-            {
-                "job_due_time": job_due_time,
-                "job_weight": job_weight,
-                "job_process_time": job_process_time,
-            },
-            batch_size=batch_size,
-        )
+    def check_solution_validity(self, td, actions):
+        log.warning("Checking solution validity is not implemented for SMTWTP")
+        pass
 
     @staticmethod
     def render(td, actions=None, ax=None):
-        raise NotImplementedError("TODO: render is not implemented yet")
+        raise render(td, actions, ax)
```

### Comparing `rl4co-0.3.3/rl4co/models/__init__.py` & `rl4co-0.4.0/rl4co/models/zoo/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
+from rl4co.models.common.constructive.autoregressive import AutoregressivePolicy
+from rl4co.models.common.constructive.nonautoregressive import NonAutoregressivePolicy
+from rl4co.models.common.transductive import TransductiveModel
 from rl4co.models.zoo.active_search import ActiveSearch
 from rl4co.models.zoo.am import AttentionModel, AttentionModelPolicy
-from rl4co.models.zoo.common.autoregressive import (
-    AutoregressiveDecoder,
-    AutoregressivePolicy,
-    GraphAttentionEncoder,
-)
-from rl4co.models.zoo.common.search import SearchBase
+from rl4co.models.zoo.amppo import AMPPO
+from rl4co.models.zoo.deepaco import DeepACO, DeepACOPolicy
 from rl4co.models.zoo.eas import EAS, EASEmb, EASLay
 from rl4co.models.zoo.ham import (
     HeterogeneousAttentionModel,
     HeterogeneousAttentionModelPolicy,
 )
 from rl4co.models.zoo.matnet import MatNet, MatNetPolicy
 from rl4co.models.zoo.mdam import MDAM, MDAMPolicy
-from rl4co.models.zoo.pomo import POMO, POMOPolicy
-from rl4co.models.zoo.ppo import PPOModel, PPOPolicy
+from rl4co.models.zoo.nargnn import NARGNNPolicy
+from rl4co.models.zoo.pomo import POMO
 from rl4co.models.zoo.ptrnet import PointerNetwork, PointerNetworkPolicy
 from rl4co.models.zoo.symnco import SymNCO, SymNCOPolicy
```

### Comparing `rl4co-0.3.3/rl4co/models/nn/attention.py` & `rl4co-0.4.0/rl4co/models/nn/attention.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+import warnings
 
 from typing import Callable, Optional
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
@@ -70,15 +71,15 @@
         embed_dim: total dimension of the model
         num_heads: number of heads
         bias: whether to use bias
         attention_dropout: dropout rate for attention weights
         causal: whether to apply causal mask to attention scores
         device: torch device
         dtype: torch dtype
-        sdpa_fn: scaled dot product attention function (SDPA)
+        sdpa_fn: scaled dot product attention function (SDPA) implementation
     """
 
     def __init__(
         self,
         embed_dim: int,
         num_heads: int,
         bias: bool = True,
@@ -89,19 +90,15 @@
         sdpa_fn: Optional[Callable] = None,
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         super().__init__()
         self.embed_dim = embed_dim
         self.causal = causal
         self.attention_dropout = attention_dropout
-
-        # Default to `scaled_dot_product_attention` if `sdpa_fn` is not provided
-        if sdpa_fn is None:
-            sdpa_fn = scaled_dot_product_attention
-        self.sdpa_fn = sdpa_fn
+        self.sdpa_fn = sdpa_fn if sdpa_fn is not None else scaled_dot_product_attention
 
         self.num_heads = num_heads
         assert self.embed_dim % num_heads == 0, "self.kdim must be divisible by num_heads"
         self.head_dim = self.embed_dim // num_heads
         assert (
             self.head_dim % 8 == 0 and self.head_dim <= 128
         ), "Only support head_dim <= 128 and divisible by 8"
@@ -125,101 +122,103 @@
             v,
             attn_mask=key_padding_mask,
             dropout_p=self.attention_dropout,
         )
         return self.out_proj(rearrange(out, "b h s d -> b s (h d)"))
 
 
-class LogitAttention(nn.Module):
+class PointerAttention(nn.Module):
     """Calculate logits given query, key and value and logit key.
+    This follows the pointer mechanism of Vinyals et al. (2015) (https://arxiv.org/abs/1506.03134).
 
     Note:
         With Flash Attention, masking is not supported
 
-    Perform the following:
+    Performs the following:
         1. Apply cross attention to get the heads
         2. Project heads to get glimpse
         3. Compute attention score between glimpse and logit key
-        4. Normalize and mask
 
     Args:
         embed_dim: total dimension of the model
         num_heads: number of heads
-        tanh_clipping: tanh clipping value
         mask_inner: whether to mask inner attention
-        mask_logits: whether to mask logits
-        normalize: whether to normalize logits
-        softmax_temp: softmax temperature
         linear_bias: whether to use bias in linear projection
-        sdp_fn: scaled dot product attention function (SDPA)
+        check_nan: whether to check for NaNs in logits
+        sdpa_fn: scaled dot product attention function (SDPA) implementation
     """
 
     def __init__(
         self,
         embed_dim: int,
         num_heads: int,
-        tanh_clipping: float = 10.0,
         mask_inner: bool = True,
-        mask_logits: bool = True,
-        normalize: bool = True,
-        softmax_temp: float = 1.0,
-        linear_bias: bool = False,
-        sdp_fn=scaled_dot_product_attention,
+        out_bias: bool = False,
+        check_nan: bool = True,
+        sdpa_fn: Optional[Callable] = None,
     ):
-        super(LogitAttention, self).__init__()
+        super(PointerAttention, self).__init__()
         self.num_heads = num_heads
-        self.mask_logits = mask_logits
         self.mask_inner = mask_inner
-        self.tanh_clipping = tanh_clipping
-        self.normalize = normalize
-        self.softmax_temp = softmax_temp
 
         # Projection - query, key, value already include projections
-        self.project_out = nn.Linear(embed_dim, embed_dim, bias=linear_bias)
-        self.sdp_fn = sdp_fn
-
-    def forward(self, query, key, value, logit_key, mask, softmax_temp=None):
+        self.project_out = nn.Linear(embed_dim, embed_dim, bias=out_bias)
+        self.sdpa_fn = sdpa_fn if sdpa_fn is not None else scaled_dot_product_attention
+        self.check_nan = check_nan
+
+    def forward(self, query, key, value, logit_key, attn_mask=None):
+        """Compute attention logits given query, key, value, logit key and attention mask.
+
+        Args:
+            query: query tensor of shape [B, ..., L, E]
+            key: key tensor of shape [B, ..., S, E]
+            value: value tensor of shape [B, ..., S, E]
+            logit_key: logit key tensor of shape [B, ..., S, E]
+            attn_mask: attention mask tensor of shape [B, ..., S]. Note that `True` means that the value _should_ take part in attention
+                as described in the [PyTorch Documentation](https://pytorch.org/docs/stable/generated/torch.nn.functional.scaled_dot_product_attention.html)
+        """
         # Compute inner multi-head attention with no projections.
-        heads = self._inner_mha(query, key, value, mask)
+        heads = self._inner_mha(query, key, value, attn_mask)
         glimpse = self.project_out(heads)
 
         # Batch matrix multiplication to compute logits (batch_size, num_steps, graph_size)
         # bmm is slightly faster than einsum and matmul
-        logits = (
-            torch.bmm(glimpse, logit_key.squeeze(1).transpose(-2, -1))
-            / math.sqrt(glimpse.size(-1))
-        ).squeeze(1)
-
-        # From the logits compute the probabilities by clipping, masking and softmax
-        if self.tanh_clipping > 0:
-            logits = torch.tanh(logits) * self.tanh_clipping
-
-        if self.mask_logits:
-            logits[mask] = float("-inf")
-
-        # Normalize with softmax and apply temperature
-        if self.normalize:
-            softmax_temp = softmax_temp if softmax_temp is not None else self.softmax_temp
-            logits = torch.log_softmax(logits / softmax_temp, dim=-1)
+        logits = (torch.bmm(glimpse, logit_key.squeeze(-2).transpose(-2, -1))).squeeze(
+            -2
+        ) / math.sqrt(glimpse.size(-1))
 
-        assert not torch.isnan(logits).any(), "Logits contain NaNs"
+        if self.check_nan:
+            assert not torch.isnan(logits).any(), "Logits contain NaNs"
 
         return logits
 
-    def _inner_mha(self, query, key, value, mask):
+    def _inner_mha(self, query, key, value, attn_mask):
         q = self._make_heads(query)
         k = self._make_heads(key)
         v = self._make_heads(value)
-
         if self.mask_inner:
-            # need to invert mask: (N L S) -> (N 1 L S)
+            # make mask the same number of dimensions as q
             attn_mask = (
-                ~mask.unsqueeze(1) if mask.ndim == 3 else ~mask.unsqueeze(1).unsqueeze(2)
+                attn_mask.unsqueeze(1)
+                if attn_mask.ndim == 3
+                else attn_mask.unsqueeze(1).unsqueeze(2)
             )
         else:
             attn_mask = None
-
-        heads = self.sdp_fn(q, k, v, attn_mask=attn_mask)
+        heads = self.sdpa_fn(q, k, v, attn_mask=attn_mask)
         return rearrange(heads, "... h n g -> ... n (h g)", h=self.num_heads)
 
     def _make_heads(self, v):
         return rearrange(v, "... g (h s) -> ... h g s", h=self.num_heads)
+
+
+# Deprecated
+class LogitAttention(PointerAttention):
+    def __init__(self, *args, **kwargs):
+        warnings.simplefilter("always", DeprecationWarning)
+        warnings.warn(
+            "LogitAttention is deprecated and will be removed in a future release. "
+            "Please use PointerAttention instead."
+            "Note that several components of the previous LogitAttention have moved to `rl4co.models.nn.dec_strategies`.",
+            category=DeprecationWarning,
+        )
+        super(LogitAttention, self).__init__(*args, **kwargs)
```

### Comparing `rl4co-0.3.3/rl4co/models/nn/env_embeddings/context.py` & `rl4co-0.4.0/rl4co/models/nn/env_embeddings/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import torch
 import torch.nn as nn
 
+from tensordict import TensorDict
+
 from rl4co.utils.ops import gather_by_index
 
 
 def env_context_embedding(env_name: str, config: dict) -> nn.Module:
     """Get environment context embedding. The context embedding is used to modify the
     query embedding of the problem node of the current partial solution.
     Usually consists of a projection of gathered node embeddings and features to the embedding space.
@@ -14,24 +16,26 @@
         config: A dictionary of configuration options for the environment.
     """
     embedding_registry = {
         "tsp": TSPContext,
         "atsp": TSPContext,
         "cvrp": VRPContext,
         "cvrptw": VRPTWContext,
+        "ffsp": FFSPContext,
         "svrp": SVRPContext,
         "sdvrp": VRPContext,
         "pctsp": PCTSPContext,
         "spctsp": PCTSPContext,
         "op": OPContext,
         "dpp": DPPContext,
         "mdpp": DPPContext,
         "pdp": PDPContext,
         "mtsp": MTSPContext,
         "smtwtp": SMTWTPContext,
+        "mdcpdp": MDCPDPContext,
     }
 
     if env_name not in embedding_registry:
         raise ValueError(
             f"Unknown environment name '{env_name}'. Available context embeddings: {embedding_registry.keys()}"
         )
 
@@ -39,23 +43,19 @@
 
 
 class EnvContext(nn.Module):
     """Base class for environment context embeddings. The context embedding is used to modify the
     query embedding of the problem node of the current partial solution.
     Consists of a linear layer that projects the node features to the embedding space."""
 
-    def __init__(self, embedding_dim, step_context_dim=None, linear_bias=False):
+    def __init__(self, embed_dim, step_context_dim=None, linear_bias=False):
         super(EnvContext, self).__init__()
-        self.embedding_dim = embedding_dim
-        step_context_dim = (
-            step_context_dim if step_context_dim is not None else embedding_dim
-        )
-        self.project_context = nn.Linear(
-            step_context_dim, embedding_dim, bias=linear_bias
-        )
+        self.embed_dim = embed_dim
+        step_context_dim = step_context_dim if step_context_dim is not None else embed_dim
+        self.project_context = nn.Linear(step_context_dim, embed_dim, bias=linear_bias)
 
     def _cur_node_embedding(self, embeddings, td):
         """Get embedding of current node"""
         cur_node_embedding = gather_by_index(embeddings, td["current_node"])
         return cur_node_embedding
 
     def _state_embedding(self, embeddings, td):
@@ -65,25 +65,53 @@
     def forward(self, embeddings, td):
         cur_node_embedding = self._cur_node_embedding(embeddings, td)
         state_embedding = self._state_embedding(embeddings, td)
         context_embedding = torch.cat([cur_node_embedding, state_embedding], -1)
         return self.project_context(context_embedding)
 
 
+class FFSPContext(EnvContext):
+    def __init__(self, embed_dim, stage_cnt=None):
+        self.has_stage_emb = stage_cnt is not None
+        step_context_dim = (1 + int(self.has_stage_emb)) * embed_dim
+        super().__init__(embed_dim=embed_dim, step_context_dim=step_context_dim)
+        if self.has_stage_emb:
+            self.stage_emb = nn.Parameter(torch.rand(stage_cnt, embed_dim))
+
+    def _cur_node_embedding(self, embeddings: TensorDict, td):
+        cur_node_embedding = gather_by_index(
+            embeddings["machine_embeddings"], td["stage_machine_idx"]
+        )
+        return cur_node_embedding
+
+    def forward(self, embeddings, td):
+        cur_node_embedding = self._cur_node_embedding(embeddings, td)
+        if self.has_stage_emb:
+            state_embedding = self._state_embedding(embeddings, td)
+            context_embedding = torch.cat([cur_node_embedding, state_embedding], -1)
+            return self.project_context(context_embedding)
+        else:
+            return self.project_context(cur_node_embedding)
+
+    def _state_embedding(self, _, td):
+        cur_stage_emb = self.stage_emb[td["stage_idx"]]
+        return cur_stage_emb
+
+
 class TSPContext(EnvContext):
     """Context embedding for the Traveling Salesman Problem (TSP).
     Project the following to the embedding space:
         - first node embedding
         - current node embedding
     """
 
-    def __init__(self, embedding_dim):
-        super(TSPContext, self).__init__(embedding_dim, 2 * embedding_dim)
+    def __init__(self, embed_dim):
+        super(TSPContext, self).__init__(embed_dim, 2 * embed_dim)
         self.W_placeholder = nn.Parameter(
-            torch.Tensor(2 * self.embedding_dim).uniform_(-1, 1)
+            torch.Tensor(2 * self.embed_dim).uniform_(-1, 1)
         )
 
     def forward(self, embeddings, td):
         batch_size = embeddings.size(0)
         # By default, node_dim = -1 (we only have one node embedding per node)
         node_dim = (
             (-1,) if td["first_node"].dim() == 1 else (td["first_node"].size(-1), -1)
@@ -105,17 +133,17 @@
 class VRPContext(EnvContext):
     """Context embedding for the Capacitated Vehicle Routing Problem (CVRP).
     Project the following to the embedding space:
         - current node embedding
         - remaining capacity (vehicle_capacity - used_capacity)
     """
 
-    def __init__(self, embedding_dim):
+    def __init__(self, embed_dim):
         super(VRPContext, self).__init__(
-            embedding_dim=embedding_dim, step_context_dim=embedding_dim + 1
+            embed_dim=embed_dim, step_context_dim=embed_dim + 1
         )
 
     def _state_embedding(self, embeddings, td):
         state_embedding = td["vehicle_capacity"] - td["used_capacity"]
         return state_embedding
 
 
@@ -123,17 +151,17 @@
     """Context embedding for the Capacitated Vehicle Routing Problem (CVRP).
     Project the following to the embedding space:
         - current node embedding
         - remaining capacity (vehicle_capacity - used_capacity)
         - current time
     """
 
-    def __init__(self, embedding_dim):
+    def __init__(self, embed_dim):
         super(VRPContext, self).__init__(
-            embedding_dim=embedding_dim, step_context_dim=embedding_dim + 2
+            embed_dim=embed_dim, step_context_dim=embed_dim + 2
         )
 
     def _cur_node_embedding(self, embeddings, td):
         return super()._cur_node_embedding(embeddings, td).reshape(embeddings.size(0), -1)
 
     def _state_embedding(self, embeddings, td):
         capacity = super()._state_embedding(embeddings, td)
@@ -144,33 +172,31 @@
 class SVRPContext(EnvContext):
     """Context embedding for the Skill Vehicle Routing Problem (SVRP).
     Project the following to the embedding space:
         - current node embedding
         - current technician
     """
 
-    def __init__(self, embedding_dim):
-        super(SVRPContext, self).__init__(
-            embedding_dim=embedding_dim, step_context_dim=embedding_dim
-        )
+    def __init__(self, embed_dim):
+        super(SVRPContext, self).__init__(embed_dim=embed_dim, step_context_dim=embed_dim)
 
     def forward(self, embeddings, td):
         cur_node_embedding = self._cur_node_embedding(embeddings, td).squeeze()
         return self.project_context(cur_node_embedding)
 
 
 class PCTSPContext(EnvContext):
     """Context embedding for the Prize Collecting TSP (PCTSP).
     Project the following to the embedding space:
         - current node embedding
         - remaining prize (prize_required - cur_total_prize)
     """
 
-    def __init__(self, embedding_dim):
-        super(PCTSPContext, self).__init__(embedding_dim, embedding_dim + 1)
+    def __init__(self, embed_dim):
+        super(PCTSPContext, self).__init__(embed_dim, embed_dim + 1)
 
     def _state_embedding(self, embeddings, td):
         state_embedding = torch.clamp(
             td["prize_required"] - td["cur_total_prize"], min=0
         )[..., None]
         return state_embedding
 
@@ -178,46 +204,46 @@
 class OPContext(EnvContext):
     """Context embedding for the Orienteering Problem (OP).
     Project the following to the embedding space:
         - current node embedding
         - remaining distance (max_length - tour_length)
     """
 
-    def __init__(self, embedding_dim):
-        super(OPContext, self).__init__(embedding_dim, embedding_dim + 1)
+    def __init__(self, embed_dim):
+        super(OPContext, self).__init__(embed_dim, embed_dim + 1)
 
     def _state_embedding(self, embeddings, td):
         state_embedding = td["max_length"][..., 0] - td["tour_length"]
         return state_embedding[..., None]
 
 
 class DPPContext(EnvContext):
     """Context embedding for the Decap Placement Problem (DPP), EDA (electronic design automation).
     Project the following to the embedding space:
         - current cell embedding
     """
 
-    def __init__(self, embedding_dim):
-        super(DPPContext, self).__init__(embedding_dim)
+    def __init__(self, embed_dim):
+        super(DPPContext, self).__init__(embed_dim)
 
     def forward(self, embeddings, td):
         """Context cannot be defined by a single node embedding for DPP, hence 0.
         We modify the dynamic embedding instead to capture placed items
         """
-        return embeddings.new_zeros(embeddings.size(0), self.embedding_dim)
+        return embeddings.new_zeros(embeddings.size(0), self.embed_dim)
 
 
 class PDPContext(EnvContext):
     """Context embedding for the Pickup and Delivery Problem (PDP).
     Project the following to the embedding space:
         - current node embedding
     """
 
-    def __init__(self, embedding_dim):
-        super(PDPContext, self).__init__(embedding_dim, embedding_dim)
+    def __init__(self, embed_dim):
+        super(PDPContext, self).__init__(embed_dim, embed_dim)
 
     def forward(self, embeddings, td):
         cur_node_embedding = self._cur_node_embedding(embeddings, td).squeeze()
         return self.project_context(cur_node_embedding)
 
 
 class MTSPContext(EnvContext):
@@ -226,20 +252,20 @@
         - current node embedding
         - remaining_agents
         - current_length
         - max_subtour_length
         - distance_from_depot
     """
 
-    def __init__(self, embedding_dim, linear_bias=False):
-        super(MTSPContext, self).__init__(embedding_dim, 2 * embedding_dim)
+    def __init__(self, embed_dim, linear_bias=False):
+        super(MTSPContext, self).__init__(embed_dim, 2 * embed_dim)
         proj_in_dim = (
             4  # remaining_agents, current_length, max_subtour_length, distance_from_depot
         )
-        self.proj_dynamic_feats = nn.Linear(proj_in_dim, embedding_dim, bias=linear_bias)
+        self.proj_dynamic_feats = nn.Linear(proj_in_dim, embed_dim, bias=linear_bias)
 
     def _cur_node_embedding(self, embeddings, td):
         cur_node_embedding = gather_by_index(embeddings, td["current_node"])
         return cur_node_embedding.squeeze()
 
     def _state_embedding(self, embeddings, td):
         dynamic_feats = torch.stack(
@@ -262,17 +288,31 @@
 class SMTWTPContext(EnvContext):
     """Context embedding for the Single Machine Total Weighted Tardiness Problem (SMTWTP).
     Project the following to the embedding space:
         - current node embedding
         - current time
     """
 
-    def __init__(self, embedding_dim):
-        super(SMTWTPContext, self).__init__(embedding_dim, embedding_dim + 1)
+    def __init__(self, embed_dim):
+        super(SMTWTPContext, self).__init__(embed_dim, embed_dim + 1)
 
     def _cur_node_embedding(self, embeddings, td):
         cur_node_embedding = gather_by_index(embeddings, td["current_job"])
         return cur_node_embedding
 
     def _state_embedding(self, embeddings, td):
         state_embedding = td["current_time"]
         return state_embedding
+
+
+class MDCPDPContext(EnvContext):
+    """Context embedding for the MDCPDP.
+    Project the following to the embedding space:
+        - current node embedding
+    """
+
+    def __init__(self, embed_dim):
+        super(MDCPDPContext, self).__init__(embed_dim, embed_dim)
+
+    def forward(self, embeddings, td):
+        cur_node_embedding = self._cur_node_embedding(embeddings, td).squeeze()
+        return self.project_context(cur_node_embedding)
```

### Comparing `rl4co-0.3.3/rl4co/models/nn/env_embeddings/dynamic.py` & `rl4co-0.4.0/rl4co/models/nn/env_embeddings/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         config: A dictionary of configuration options for the environment.
     """
     embedding_registry = {
         "tsp": StaticEmbedding,
         "atsp": StaticEmbedding,
         "cvrp": StaticEmbedding,
         "cvrptw": StaticEmbedding,
+        "ffsp": StaticEmbedding,
         "svrp": StaticEmbedding,
         "sdvrp": SDVRPDynamicEmbedding,
         "pctsp": StaticEmbedding,
         "spctsp": StaticEmbedding,
         "op": StaticEmbedding,
         "dpp": StaticEmbedding,
         "mdpp": StaticEmbedding,
@@ -55,17 +56,17 @@
     """Dynamic embedding for the Split Delivery Vehicle Routing Problem (SDVRP).
     Embed the following node features to the embedding space:
         - demand_with_depot: demand of the customers and the depot
     The demand with depot is used to modify the query, key and value vectors of the attention mechanism
     based on the current state of the environment (which is changing during the rollout).
     """
 
-    def __init__(self, embedding_dim, linear_bias=False):
+    def __init__(self, embed_dim, linear_bias=False):
         super(SDVRPDynamicEmbedding, self).__init__()
-        self.projection = nn.Linear(1, 3 * embedding_dim, bias=linear_bias)
+        self.projection = nn.Linear(1, 3 * embed_dim, bias=linear_bias)
 
     def forward(self, td):
         demands_with_depot = td["demand_with_depot"][..., None].clone()
         demands_with_depot[..., 0, :] = 0
         glimpse_key_dynamic, glimpse_val_dynamic, logit_key_dynamic = self.projection(
             demands_with_depot
         ).chunk(3, dim=-1)
```

### Comparing `rl4co-0.3.3/rl4co/models/nn/flash_attention.py` & `rl4co-0.4.0/rl4co/models/nn/flash_attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/models/nn/graph/attnnet.py` & `rl4co-0.4.0/rl4co/models/nn/graph/attnnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,75 +11,75 @@
 log = get_pylogger(__name__)
 
 
 class MultiHeadAttentionLayer(nn.Sequential):
     """Multi-Head Attention Layer with normalization and feed-forward layer
 
     Args:
-        num_heads: number of heads in the MHA
         embed_dim: dimension of the embeddings
-        feed_forward_hidden: dimension of the hidden layer in the feed-forward layer
+        num_heads: number of heads in the MHA
+        feedforward_hidden: dimension of the hidden layer in the feed-forward layer
         normalization: type of normalization to use (batch, layer, none)
         sdpa_fn: scaled dot product attention function (SDPA)
     """
 
     def __init__(
         self,
-        num_heads: int,
         embed_dim: int,
-        feed_forward_hidden: int = 512,
+        num_heads: int = 8,
+        feedforward_hidden: int = 512,
         normalization: Optional[str] = "batch",
         sdpa_fn: Optional[Callable] = None,
     ):
         super(MultiHeadAttentionLayer, self).__init__(
             SkipConnection(MultiHeadAttention(embed_dim, num_heads, sdpa_fn=sdpa_fn)),
             Normalization(embed_dim, normalization),
             SkipConnection(
                 nn.Sequential(
-                    nn.Linear(embed_dim, feed_forward_hidden),
+                    nn.Linear(embed_dim, feedforward_hidden),
                     nn.ReLU(),
-                    nn.Linear(feed_forward_hidden, embed_dim),
+                    nn.Linear(feedforward_hidden, embed_dim),
                 )
-                if feed_forward_hidden > 0
+                if feedforward_hidden > 0
                 else nn.Linear(embed_dim, embed_dim)
             ),
             Normalization(embed_dim, normalization),
         )
 
 
 class GraphAttentionNetwork(nn.Module):
     """Graph Attention Network to encode embeddings with a series of MHA layers consisting of a MHA layer,
     normalization, feed-forward layer, and normalization. Similar to Transformer encoder, as used in Kool et al. (2019).
 
     Args:
         num_heads: number of heads in the MHA
-        embedding_dim: dimension of the embeddings
+        embed_dim: dimension of the embeddings
         num_layers: number of MHA layers
         normalization: type of normalization to use (batch, layer, none)
-        feed_forward_hidden: dimension of the hidden layer in the feed-forward layer
+        feedforward_hidden: dimension of the hidden layer in the feed-forward layer
         sdpa_fn: scaled dot product attention function (SDPA)
     """
 
     def __init__(
         self,
         num_heads: int,
-        embedding_dim: int,
+        embed_dim: int,
         num_layers: int,
         normalization: str = "batch",
-        feed_forward_hidden: int = 512,
+        feedforward_hidden: int = 512,
         sdpa_fn: Optional[Callable] = None,
     ):
         super(GraphAttentionNetwork, self).__init__()
 
         self.layers = nn.Sequential(
             *(
                 MultiHeadAttentionLayer(
+                    embed_dim,
                     num_heads,
-                    embedding_dim,
-                    feed_forward_hidden=feed_forward_hidden,
+                    feedforward_hidden=feedforward_hidden,
                     normalization=normalization,
                     sdpa_fn=sdpa_fn,
                 )
                 for _ in range(num_layers)
             )
         )
```

### Comparing `rl4co-0.3.3/rl4co/models/nn/graph/gcn.py` & `rl4co-0.4.0/rl4co/models/nn/graph/gcn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,61 @@
 from typing import Tuple, Union
 
-import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from tensordict import TensorDict
 from torch import Tensor
 from torch_geometric.data import Batch, Data
 from torch_geometric.nn import GCNConv
 
 from rl4co.models.nn.env_embeddings import env_init_embedding
+from rl4co.utils.ops import get_full_graph_edge_index
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class GCNEncoder(nn.Module):
     """Graph Convolutional Network to encode embeddings with a series of GCN layers
 
     Args:
-        embedding_dim: dimension of the embeddings
+        embed_dim: dimension of the embeddings
         num_nodes: number of nodes in the graph
         num_gcn_layer: number of GCN layers
         self_loop: whether to add self loop in the graph
         residual: whether to use residual connection
     """
 
     def __init__(
         self,
         env_name: str,
-        embedding_dim: int,
+        embed_dim: int,
         num_nodes: int,
         num_layers: int,
         init_embedding: nn.Module = None,
         self_loop: bool = False,
         residual: bool = True,
     ):
         super(GCNEncoder, self).__init__()
 
         self.env_name = env_name
 
         self.init_embedding = (
-            env_init_embedding(self.env_name, {"embedding_dim": embedding_dim})
+            env_init_embedding(self.env_name, {"embed_dim": embed_dim})
             if init_embedding is None
             else init_embedding
         )
 
         # Generate edge index for a fully connected graph
-        adj_matrix = torch.ones(num_nodes, num_nodes)
-        if self_loop:
-            adj_matrix.fill_diagonal_(0)  # No self-loops
-        self.edge_index = torch.permute(torch.nonzero(adj_matrix), (1, 0))
+        self.edge_index = get_full_graph_edge_index(num_nodes, self_loop)
 
         # Define the GCN layers
         self.gcn_layers = nn.ModuleList(
-            [GCNConv(embedding_dim, embedding_dim) for _ in range(num_layers)]
+            [GCNConv(embed_dim, embed_dim) for _ in range(num_layers)]
         )
 
         # Record parameters
         self.residual = residual
         self.self_loop = self_loop
 
     # def forward(self, x, node_feature, mask=None):
@@ -78,19 +75,17 @@
         """
         # Transfer to embedding space
         init_h = self.init_embedding(td)
         num_node = init_h.size(-2)
 
         # Check to update the edge index with different number of node
         if num_node != self.edge_index.max().item() + 1:
-            adj_matrix = torch.ones(num_node, num_node)
-            if self.self_loop:
-                adj_matrix.fill_diagonal_(0)
-            edge_index = torch.permute(torch.nonzero(adj_matrix), (1, 0))
-            edge_index = edge_index.to(init_h.device)
+            edge_index = get_full_graph_edge_index(num_node, self.self_loop).to(
+                init_h.device
+            )
         else:
             edge_index = self.edge_index.to(init_h.device)
 
         # Create the batched graph
         data_list = [Data(x=x, edge_index=edge_index) for x in init_h]
         data_batch = Batch.from_data_list(data_list)
```

### Comparing `rl4co-0.3.3/rl4co/models/nn/graph/mpnn.py` & `rl4co-0.4.0/rl4co/models/nn/graph/mpnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         return unf
 
 
 class MessagePassingEncoder(nn.Module):
     def __init__(
         self,
         env_name: str,
-        embedding_dim: int,
+        embed_dim: int,
         num_nodes: int,
         num_layers: int,
         init_embedding: nn.Module = None,
         aggregation: str = "add",
         self_loop: bool = False,
         residual: bool = True,
     ):
@@ -80,31 +80,31 @@
             - Support fully connected graph for now.
         """
         super(MessagePassingEncoder, self).__init__()
 
         self.env_name = env_name
 
         self.init_embedding = (
-            env_init_embedding(self.env_name, {"embedding_dim": embedding_dim})
+            env_init_embedding(self.env_name, {"embed_dim": embed_dim})
             if init_embedding is None
             else init_embedding
         )
 
         # Generate edge index for a fully connected graph
         adj_matrix = torch.ones(num_nodes, num_nodes)
         if self_loop:
             adj_matrix.fill_diagonal_(0)  # No self-loops
         self.edge_index = torch.permute(torch.nonzero(adj_matrix), (1, 0))
 
         # Init message passing models
         self.mpnn_layers = nn.ModuleList(
             [
                 MessagePassingLayer(
-                    node_indim=embedding_dim,
-                    node_outdim=embedding_dim,
+                    node_indim=embed_dim,
+                    node_outdim=embed_dim,
                     edge_indim=1,
                     edge_outdim=1,
                     aggregation=aggregation,
                     residual=residual,
                 )
                 for _ in range(num_layers)
             ]
```

### Comparing `rl4co-0.3.3/rl4co/models/nn/mlp.py` & `rl4co-0.4.0/rl4co/models/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/models/nn/ops.py` & `rl4co-0.4.0/rl4co/models/nn/ops.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/models/rl/common/base.py` & `rl4co-0.4.0/rl4co/models/rl/common/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import abc
+
 from functools import partial
 from typing import Any, Iterable, Union
 
 import torch
 import torch.nn as nn
 
 from lightning import LightningModule
@@ -11,15 +13,15 @@
 from rl4co.envs.common.base import RL4COEnvBase
 from rl4co.utils.optim_helpers import create_optimizer, create_scheduler
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
-class RL4COLitModule(LightningModule):
+class RL4COLitModule(LightningModule, metaclass=abc.ABCMeta):
     """Base class for Lightning modules for RL4CO. This defines the general training loop in terms of
     RL algorithms. Subclasses should implement mainly the `shared_step` to define the specific
     loss functions and optimization routines.
 
     Args:
         env: RL4CO environment
         policy: policy network (actor)
```

### Comparing `rl4co-0.3.3/rl4co/models/rl/common/critic.py` & `rl4co-0.4.0/rl4co/models/zoo/am/encoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from typing import Callable, Optional, Union
+from typing import Tuple, Union
+
+import torch.nn as nn
 
 from tensordict import TensorDict
-from torch import Tensor, nn
+from torch import Tensor
 
 from rl4co.envs import RL4COEnvBase
+from rl4co.models.common.constructive import AutoregressiveEncoder
 from rl4co.models.nn.env_embeddings import env_init_embedding
 from rl4co.models.nn.graph.attnnet import GraphAttentionNetwork
 
 
-class CriticNetwork(nn.Module):
-    """We make the critic network compatible with any problem by using encoder for any environment
-    Refactored from Kool et al. (2019) which only worked for TSP. In our case, we make it
-    compatible with any problem by using the environment init embedding. Note that if no environment
-    name and no init embedding are provided, the critic network does not transform the input (i.e.
-    it should be a tensor of shape (batch_size, embedding_dim)).
+class AttentionModelEncoder(AutoregressiveEncoder):
+    """Graph Attention Encoder as in Kool et al. (2019).
+    First embed the input and then process it with a Graph Attention Network.
 
     Args:
-        env_name: environment name to solve
-        encoder: Encoder to use for the critic
-        init_embedding: Initial embedding to use for the critic
-        embedding_dim: Dimension of the embeddings
-        hidden_dim: Hidden dimension for the feed-forward network
-        num_layers: Number of layers for the encoder
-        num_heads: Number of heads for the attention
-        normalization: Normalization to use for the attention
-        sdpa_fn: Scaled dot product function to use for the attention
+        embed_dim: Dimension of the embedding space
+        init_embedding: Module to use for the initialization of the embeddings
+        env_name: Name of the environment used to initialize embeddings
+        num_heads: Number of heads in the attention layers
+        num_layers: Number of layers in the attention network
+        normalization: Normalization type in the attention layers
+        feedforward_hidden: Hidden dimension in the feedforward layers
+        net: Graph Attention Network to use
+        sdpa_fn: Function to use for the scaled dot product attention
     """
 
     def __init__(
         self,
-        env_name: str = None,
-        encoder: nn.Module = None,
+        embed_dim: int = 128,
         init_embedding: nn.Module = None,
-        embedding_dim: int = 128,
-        hidden_dim: int = 512,
-        num_layers: int = 3,
+        env_name: str = "tsp",
         num_heads: int = 8,
+        num_layers: int = 3,
         normalization: str = "batch",
-        sdpa_fn: Optional[Callable] = None,
-        **unused_kwargs,
+        feedforward_hidden: int = 512,
+        net: nn.Module = None,
+        sdpa_fn=None,
     ):
-        super(CriticNetwork, self).__init__()
+        super(AttentionModelEncoder, self).__init__()
 
         if isinstance(env_name, RL4COEnvBase):
             env_name = env_name.name
         self.env_name = env_name
 
-        if env_name is None and init_embedding is None:
-            self.init_embedding = nn.Identity()  # No embedding
-        else:
-            self.init_embedding = (
-                env_init_embedding(self.env_name, {"embedding_dim": embedding_dim})
-                if init_embedding is None
-                else init_embedding
-            )
+        self.init_embedding = (
+            env_init_embedding(self.env_name, {"embed_dim": embed_dim})
+            if init_embedding is None
+            else init_embedding
+        )
 
-        self.encoder = (
+        self.net = (
             GraphAttentionNetwork(
-                num_heads=num_heads,
-                embedding_dim=embedding_dim,
-                num_layers=num_layers,
-                normalization=normalization,
-                feed_forward_hidden=hidden_dim,
+                num_heads,
+                embed_dim,
+                num_layers,
+                normalization,
+                feedforward_hidden,
                 sdpa_fn=sdpa_fn,
             )
-            if encoder is None
-            else encoder
-        )
-
-        self.value_head = nn.Sequential(
-            nn.Linear(embedding_dim, hidden_dim), nn.ReLU(), nn.Linear(hidden_dim, 1)
+            if net is None
+            else net
         )
 
-    def forward(self, x: Union[Tensor, TensorDict]) -> Tensor:
-        """Forward pass of the critic network: encode the imput in embedding space and return the value
+    def forward(
+        self, td: TensorDict, mask: Union[Tensor, None] = None
+    ) -> Tuple[Tensor, Tensor]:
+        """Forward pass of the encoder.
+        Transform the input TensorDict into a latent representation.
 
         Args:
-            x: Input containing the environment state. Can be a Tensor or a TensorDict
+            td: Input TensorDict containing the environment state
+            mask: Mask to apply to the attention
 
         Returns:
-            Value of the input state
+            h: Latent representation of the input
+            init_h: Initial embedding of the input
         """
+        # Transfer to embedding space
+        init_h = self.init_embedding(td)
+
+        # Process embedding
+        h = self.net(init_h, mask)
 
-        # Initial embedding of x. This is the identity function if env_name is None.
-        x = self.init_embedding(x)
-        x = self.encoder(x)
-        return self.value_head(x).mean(1)
+        # Return latent representation and initial embedding
+        return h, init_h
```

### Comparing `rl4co-0.3.3/rl4co/models/rl/ppo/ppo.py` & `rl4co-0.4.0/rl4co/models/rl/ppo/ppo.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import torch.nn as nn
 import torch.nn.functional as F
 
 from torch.utils.data import DataLoader
 
 from rl4co.envs.common.base import RL4COEnvBase
 from rl4co.models.rl.common.base import RL4COLitModule
+from rl4co.models.rl.common.critic import CriticNetwork, create_critic_from_actor
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class PPO(RL4COLitModule):
     """
@@ -57,29 +58,34 @@
     (e.g., https://github.com/lucidrains/PaLM-rlhf-pytorch).
     """
 
     def __init__(
         self,
         env: RL4COEnvBase,
         policy: nn.Module,
-        critic: nn.Module,
+        critic: CriticNetwork = None,
+        critic_kwargs: dict = {},
         clip_range: float = 0.2,  # epsilon of PPO
         ppo_epochs: int = 2,  # inner epoch, K
         mini_batch_size: Union[int, float] = 0.25,  # 0.25,
         vf_lambda: float = 0.5,  # lambda of Value function fitting
         entropy_lambda: float = 0.0,  # lambda of entropy bonus
         normalize_adv: bool = False,  # whether to normalize advantage
         max_grad_norm: float = 0.5,  # max gradient norm
         metrics: dict = {
             "train": ["loss", "surrogate_loss", "value_loss", "entropy"],
         },
         **kwargs,
     ):
         super().__init__(env, policy, metrics=metrics, **kwargs)
         self.automatic_optimization = False  # PPO uses custom optimization routine
+
+        if critic is None:
+            log.info("Creating critic network for {}".format(env.name))
+            critic = create_critic_from_actor(policy, **critic_kwargs)
         self.critic = critic
 
         if isinstance(mini_batch_size, float) and (
             mini_batch_size <= 0 or mini_batch_size > 1
         ):
             default_mini_batch_fraction = 0.25
             log.warning(
@@ -138,36 +144,42 @@
             else:
                 raise ValueError("mini_batch_size must be an integer or a float.")
 
             if mini_batch_size > batch_size:
                 mini_batch_size = batch_size
 
             # Todo: Add support for multi dimensional batches
-            td.set("log_prob", out["log_likelihood"])
+            td.set("logprobs", out["log_likelihood"])
             td.set("reward", out["reward"])
             td.set("action", out["actions"])
 
             # Inherit the dataset class from the environment for efficiency
             dataset = self.env.dataset_cls(td)
             dataloader = DataLoader(
                 dataset,
                 batch_size=mini_batch_size,
                 shuffle=True,
                 collate_fn=dataset.collate_fn,
             )
 
             for _ in range(self.ppo_cfg["ppo_epochs"]):  # PPO inner epoch, K
                 for sub_td in dataloader:
+                    sub_td = sub_td.to(td.device)
                     previous_reward = sub_td["reward"].view(-1, 1)
-                    ll, entropy = self.policy.evaluate_action(
-                        sub_td, action=sub_td["action"]
+                    out = self.policy(  # note: remember to clone to avoid in-place replacements!
+                        sub_td.clone(),
+                        actions=sub_td["action"],
+                        env=self.env,
+                        return_entropy=True,
+                        return_sum_log_likelihood=False,
                     )
+                    ll, entropy = out["log_likelihood"], out["entropy"]
 
                     # Compute the ratio of probabilities of new and old actions
-                    ratio = torch.exp(ll.sum(dim=-1) - sub_td["log_prob"]).view(
+                    ratio = torch.exp(ll.sum(dim=-1) - sub_td["logprobs"]).view(
                         -1, 1
                     )  # [batch, 1]
 
                     # Compute the advantage
                     value_pred = self.critic(sub_td)  # [batch, 1]
                     adv = previous_reward - value_pred.detach()
```

### Comparing `rl4co-0.3.3/rl4co/models/rl/reinforce/baselines.py` & `rl4co-0.4.0/rl4co/models/rl/reinforce/baselines.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,42 @@
+import abc
 import copy
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from scipy.stats import ttest_rel
-from torch.utils.data import DataLoader
+from tensordict import TensorDict
+from torch.utils.data import DataLoader, Dataset
 
-from rl4co import utils
-from rl4co.models.rl.common.critic import CriticNetwork
+from rl4co.envs.common.base import RL4COEnvBase
+from rl4co.models.rl.common.critic import CriticNetwork, create_critic_from_actor
+from rl4co.utils.pylogger import get_pylogger
 
-log = utils.get_pylogger(__name__)
+log = get_pylogger(__name__)
 
 
-class REINFORCEBaseline(nn.Module):
+class REINFORCEBaseline(nn.Module, metaclass=abc.ABCMeta):
     """Base class for REINFORCE baselines"""
 
     def __init__(self, *args, **kw):
         super().__init__()
         pass
 
-    def wrap_dataset(self, dataset, *args, **kw):
+    def wrap_dataset(self, dataset: Dataset, *args, **kw):
         """Wrap dataset with baseline-specific functionality"""
         return dataset
 
-    def eval(self, td, reward, env=None):
+    @abc.abstractmethod
+    def eval(
+        self, td: TensorDict, reward: torch.Tensor, env: RL4COEnvBase = None, **kwargs
+    ):
         """Evaluate baseline"""
-        pass
+        raise NotImplementedError
 
     def epoch_callback(self, *args, **kw):
         """Callback at the end of each epoch
         For example, update baseline parameters and obtain baseline values
         """
         pass
 
@@ -114,41 +120,42 @@
         if self.alpha == 1:
             return self.baseline.eval(td, reward, env)
         if self.alpha == 0:
             return self.warmup_baseline.eval(td, reward, env)
         v_b, l_b = self.baseline.eval(td, reward, env)
         v_wb, l_wb = self.warmup_baseline.eval(td, reward, env)
         # Return convex combination of baseline and of loss
-        return self.alpha * v_b + (1 - self.alpha) * v_wb, self.alpha * l_b + (
-            1 - self.alpha * l_wb
+        return (
+            self.alpha * v_b + (1 - self.alpha) * v_wb,
+            self.alpha * l_b + (1 - self.alpha) * l_wb,
         )
 
     def epoch_callback(self, *args, **kw):
-        # Need to call epoch callback of inner model (also after first epoch if we have not used it)
+        # Need to call epoch callback of inner policy (also after first epoch if we have not used it)
         self.baseline.epoch_callback(*args, **kw)
-        self.alpha = (kw["epoch"] + 1) / float(self.n_epochs)
         if kw["epoch"] < self.n_epochs:
+            self.alpha = (kw["epoch"] + 1) / float(self.n_epochs)
             log.info("Set warmup alpha = {}".format(self.alpha))
 
 
 class CriticBaseline(REINFORCEBaseline):
     """Critic baseline: use critic network as baseline
 
     Args:
         critic: Critic network to use as baseline. If None, create a new critic network based on the environment
     """
 
-    def __init__(self, critic: nn.Module = None, **unused_kw):
+    def __init__(self, critic: CriticNetwork = None, **unused_kw):
         super(CriticBaseline, self).__init__()
         self.critic = critic
 
-    def setup(self, model, env, **kwargs):
+    def setup(self, policy, env, **kwargs):
         if self.critic is None:
-            log.info("Creating critic network for {}".format(env.name))
-            self.critic = CriticNetwork(env.name, **kwargs)
+            log.info("Critic not found. Creating critic network for {}".format(env.name))
+            self.critic = create_critic_from_actor(policy)
 
     def eval(self, x, c, env=None):
         v = self.critic(x).squeeze(-1)
         # detach v since actor should not backprop through baseline, only for neg_loss
         return v.detach(), -F.mse_loss(v, c.detach())
 
 
@@ -160,48 +167,48 @@
     """
 
     def __init__(self, bl_alpha=0.05, **kw):
         super(RolloutBaseline, self).__init__()
         self.bl_alpha = bl_alpha
 
     def setup(self, *args, **kw):
-        self._update_model(*args, **kw)
+        self._update_policy(*args, **kw)
 
-    def _update_model(
-        self, model, env, batch_size=64, device="cpu", dataset_size=None, dataset=None
+    def _update_policy(
+        self, policy, env, batch_size=64, device="cpu", dataset_size=None, dataset=None
     ):
-        """Update model and rollout baseline values"""
-        self.model = copy.deepcopy(model).to(device)
+        """Update policy (=actor) and rollout baseline values"""
+        self.policy = copy.deepcopy(policy).to(device)
         if dataset is None:
             log.info("Creating evaluation dataset for rollout baseline")
             self.dataset = env.dataset(batch_size=[dataset_size])
 
-        log.info("Evaluating baseline model on evaluation dataset")
+        log.info("Evaluating baseline policy on evaluation dataset")
         self.bl_vals = (
-            self.rollout(self.model, env, batch_size, device, self.dataset).cpu().numpy()
+            self.rollout(self.policy, env, batch_size, device, self.dataset).cpu().numpy()
         )
         self.mean = self.bl_vals.mean()
 
     def eval(self, td, reward, env):
         """Evaluate rollout baseline
 
         Warning:
             This is not differentiable and should only be used for evaluation.
             Also, it is recommended to use the `rollout` method directly instead of this method.
         """
         with torch.inference_mode():
-            reward = self.model(td, env)["reward"]
+            reward = self.policy(td, env)["reward"]
         return reward, 0
 
     def epoch_callback(
-        self, model, env, batch_size=64, device="cpu", epoch=None, dataset_size=None
+        self, policy, env, batch_size=64, device="cpu", epoch=None, dataset_size=None
     ):
-        """Challenges the current baseline with the model and replaces the baseline model if it is improved"""
-        log.info("Evaluating candidate model on evaluation dataset")
-        candidate_vals = self.rollout(model, env, batch_size, device).cpu().numpy()
+        """Challenges the current baseline with the policy and replaces the baseline policy if it is improved"""
+        log.info("Evaluating candidate policy on evaluation dataset")
+        candidate_vals = self.rollout(policy, env, batch_size, device).cpu().numpy()
         candidate_mean = candidate_vals.mean()
 
         log.info(
             "Candidate mean: {:.3f}, Baseline mean: {:.3f}".format(
                 candidate_mean, self.mean
             )
         )
@@ -210,45 +217,45 @@
             t, p = ttest_rel(-candidate_vals, -self.bl_vals)
 
             p_val = p / 2  # one-sided
             assert t < 0, "T-statistic should be negative"
             log.info("p-value: {:.3f}".format(p_val))
             if p_val < self.bl_alpha:
                 log.info("Updating baseline")
-                self._update_model(model, env, batch_size, device, dataset_size)
+                self._update_policy(policy, env, batch_size, device, dataset_size)
 
-    def rollout(self, model, env, batch_size=64, device="cpu", dataset=None):
-        """Rollout the model on the given dataset"""
+    def rollout(self, policy, env, batch_size=64, device="cpu", dataset=None):
+        """Rollout the policy on the given dataset"""
 
         # if dataset is None, use the dataset of the baseline
         dataset = self.dataset if dataset is None else dataset
 
-        model.eval()
-        model = model.to(device)
+        policy.eval()
+        policy = policy.to(device)
 
-        def eval_model(batch):
+        def eval_policy(batch):
             with torch.inference_mode():
                 batch = env.reset(batch.to(device))
-                return model(batch, env, decode_type="greedy")["reward"]
+                return policy(batch, env, decode_type="greedy")["reward"]
 
         dl = DataLoader(dataset, batch_size=batch_size, collate_fn=dataset.collate_fn)
 
-        rewards = torch.cat([eval_model(batch) for batch in dl], 0)
+        rewards = torch.cat([eval_policy(batch) for batch in dl], 0)
         return rewards
 
     def wrap_dataset(self, dataset, env, batch_size=64, device="cpu", **kw):
         """Wrap the dataset in a baseline dataset
 
         Note:
-            This is an alternative to `eval` that does not require the model to be passed
+            This is an alternative to `eval` that does not require the policy to be passed
             at every call but just once. Values are added to the dataset. This also allows for
-            larger batch sizes since we evauate the model without gradients.
+            larger batch sizes since we evauate the policy without gradients.
         """
         rewards = (
-            self.rollout(self.model, env, batch_size, device, dataset=dataset)
+            self.rollout(self.policy, env, batch_size, device, dataset=dataset)
             .detach()
             .cpu()
         )
         return dataset.add_key("extra", rewards)
 
     def __getstate__(self):
         """Do not include datasets in state to avoid pickling issues"""
@@ -289,16 +296,16 @@
     elif name == "rollout":
         warmup_epochs = kw.get("n_epochs", 1)
         warmup_exp_beta = kw.get("exp_beta", 0.8)
         bl_alpha = kw.get("bl_alpha", 0.05)
         return WarmupBaseline(
             RolloutBaseline(bl_alpha=bl_alpha), warmup_epochs, warmup_exp_beta
         )
-    
+
     if name is None:
-        name = "no" # default to no baseline
+        name = "no"  # default to no baseline
     baseline_cls = REINFORCE_BASELINES_REGISTRY.get(name, None)
     if baseline_cls is None:
         raise ValueError(
             f"Unknown baseline {baseline_cls}. Available baselines: {REINFORCE_BASELINES_REGISTRY.keys()}"
         )
     return baseline_cls(**kw)
```

### Comparing `rl4co-0.3.3/rl4co/models/rl/reinforce/reinforce.py` & `rl4co-0.4.0/rl4co/models/rl/reinforce/reinforce.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/models/zoo/active_search/search.py` & `rl4co-0.4.0/rl4co/models/zoo/active_search/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 import torch
 
 from lightning.pytorch.utilities.types import STEP_OUTPUT
 from torch.utils.data import Dataset
 
 from rl4co.data.transforms import StateAugmentation
-from rl4co.models.zoo.common.search import SearchBase
-from rl4co.utils.ops import batchify, get_num_starts, unbatchify
+from rl4co.models.common.transductive import TransductiveModel
+from rl4co.utils.ops import batchify, unbatchify
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
-class ActiveSearch(SearchBase):
+class ActiveSearch(TransductiveModel):
     """Active Search for Neural Combination Optimization from Bello et al. (2016).
     Fine-tunes the whole policy network (encoder + decoder) on a batch of instances.
     Reference: https://arxiv.org/abs/1611.09940
 
     Args:
         env: RL4CO environment to be solved
         policy: policy network
@@ -77,17 +77,16 @@
         - original policy state dict
         """
         log.info("Setting up active search...")
         super(ActiveSearch, self).setup(stage)
 
         # Instantiate augmentation
         self.augmentation = StateAugmentation(
-            self.env.name,
             num_augment=self.hparams.augment_size,
-            use_dihedral_8=self.hparams.augment_dihedral,
+            augment_fn="dihedral8" if self.hparams.augment_dihedral else "symmetric",
         )
 
         # Store original policy state dict
         self.original_policy_state = self.policy.state_dict()
 
         # Get dataset size and problem size
         dataset_size = len(self.dataset)
@@ -108,15 +107,15 @@
     def training_step(self, batch, batch_idx):
         """Main search loop. We use the training step to effectively adapt to a `batch` of instances."""
         # Augment state
         batch_size = batch.shape[0]
         td_init = self.env.reset(batch)
         n_aug, n_start, n_runs = (
             self.augmentation.num_augment,
-            get_num_starts(td_init, self.env.name),
+            self.env.get_num_starts(td_init),
             self.hparams.num_parallel_runs,
         )
         td_init = self.augmentation(td_init)
         td_init = batchify(td_init, n_runs)
 
         # Solution and reward buffer
         max_reward = torch.full((batch_size,), -float("inf"), device=batch.device)
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/am/model.py` & `rl4co-0.4.0/rl4co/models/zoo/am/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from rl4co.models.rl import REINFORCE
 from rl4co.models.rl.reinforce.baselines import REINFORCEBaseline
 from rl4co.models.zoo.am.policy import AttentionModelPolicy
 
 
 class AttentionModel(REINFORCE):
     """Attention Model based on REINFORCE: https://arxiv.org/abs/1803.08475.
+    Check :class:`REINFORCE` and :class:`rl4co.models.RL4COLitModule` for more details such as additional parameters  including batch size.
 
     Args:
         env: Environment to use for the algorithm
         policy: Policy to use for the algorithm
         baseline: REINFORCE baseline. Defaults to rollout (1 epoch of exponential, then greedy rollout baseline)
         policy_kwargs: Keyword arguments for policy
         baseline_kwargs: Keyword arguments for baseline
@@ -24,10 +25,10 @@
         policy: AttentionModelPolicy = None,
         baseline: Union[REINFORCEBaseline, str] = "rollout",
         policy_kwargs={},
         baseline_kwargs={},
         **kwargs,
     ):
         if policy is None:
-            policy = AttentionModelPolicy(env.name, **policy_kwargs)
+            policy = AttentionModelPolicy(env_name=env.name, **policy_kwargs)
 
         super().__init__(env, policy, baseline, baseline_kwargs, **kwargs)
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/common/autoregressive/encoder.py` & `rl4co-0.4.0/rl4co/models/zoo/symnco/policy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,91 @@
-from typing import Tuple, Union
+from typing import Union
 
 import torch.nn as nn
 
-from tensordict import TensorDict
-from torch import Tensor
+from tensordict.tensordict import TensorDict
+from torchrl.modules.models import MLP
 
 from rl4co.envs import RL4COEnvBase
-from rl4co.models.nn.env_embeddings import env_init_embedding
-from rl4co.models.nn.graph.attnnet import GraphAttentionNetwork
+from rl4co.models.zoo.am import AttentionModelPolicy
+from rl4co.utils.pylogger import get_pylogger
 
+log = get_pylogger(__name__)
 
-class GraphAttentionEncoder(nn.Module):
-    """Graph Attention Encoder as in Kool et al. (2019).
+
+class SymNCOPolicy(AttentionModelPolicy):
+    """SymNCO Policy based on AutoregressivePolicy.
+    This differs from the default :class:`AutoregressivePolicy` in that it
+    projects the initial embeddings to a lower dimension using a projection head and
+    returns it. This is used in the SymNCO algorithm to compute the invariance loss.
+    Based on Kim et al. (2022) https://arxiv.org/abs/2205.13209.
 
     Args:
-        env_name: environment name to solve
-        num_heads: Number of heads for the attention
-        embedding_dim: Dimension of the embeddings
-        num_layers: Number of layers for the encoder
-        normalization: Normalization to use for the attention
-        feed_forward_hidden: Hidden dimension for the feed-forward network
-        init_embedding: Model to use for the initial embedding. If None, use the default embedding for the environment
-        sdpa_fn: Scaled dot product function to use for the attention
+        embed_dim: Dimension of the embedding
+        env_name: Name of the environment
+        num_encoder_layers: Number of layers in the encoder
+        num_heads: Number of heads in the encoder
+        normalization: Normalization to use in the encoder
+        projection_head: Projection head to use
+        use_projection_head: Whether to use projection head
+        **kwargs: Keyword arguments passed to the superclass
     """
 
     def __init__(
         self,
-        env_name: [str, RL4COEnvBase],
-        num_heads: int,
-        embedding_dim: int,
-        num_layers: int,
+        embed_dim: int = 128,
+        env_name: str = "tsp",
+        num_encoder_layers: int = 3,
+        num_heads: int = 8,
         normalization: str = "batch",
-        feed_forward_hidden: int = 512,
-        init_embedding: nn.Module = None,
-        sdpa_fn=None,
+        projection_head: nn.Module = None,
+        use_projection_head: bool = True,
+        **kwargs,
     ):
-        super(GraphAttentionEncoder, self).__init__()
-
-        if isinstance(env_name, RL4COEnvBase):
-            env_name = env_name.name
-        self.env_name = env_name
-
-        self.init_embedding = (
-            env_init_embedding(self.env_name, {"embedding_dim": embedding_dim})
-            if init_embedding is None
-            else init_embedding
+        super(SymNCOPolicy, self).__init__(
+            env_name=env_name,
+            embed_dim=embed_dim,
+            num_encoder_layers=num_encoder_layers,
+            num_heads=num_heads,
+            normalization=normalization,
+            **kwargs,
         )
 
-        self.net = GraphAttentionNetwork(
-            num_heads,
-            embedding_dim,
-            num_layers,
-            normalization,
-            feed_forward_hidden,
-            sdpa_fn=sdpa_fn,
-        )
+        self.use_projection_head = use_projection_head
+
+        if self.use_projection_head:
+            self.projection_head = (
+                MLP(embed_dim, embed_dim, 1, embed_dim, nn.ReLU)
+                if projection_head is None
+                else projection_head
+            )
 
     def forward(
-        self, td: TensorDict, mask: Union[Tensor, None] = None
-    ) -> Tuple[Tensor, Tensor]:
-        """Forward pass of the encoder.
-        Transform the input TensorDict into a latent representation.
-
-        Args:
-            td: Input TensorDict containing the environment state
-            mask: Mask to apply to the attention
-
-        Returns:
-            h: Latent representation of the input
-            init_h: Initial embedding of the input
-        """
-        # Transfer to embedding space
-        init_h = self.init_embedding(td)
+        self,
+        td: TensorDict,
+        env: Union[str, RL4COEnvBase] = None,
+        phase: str = "train",
+        return_actions: bool = False,
+        return_init_embeds: bool = True,
+        **kwargs,
+    ) -> dict:
+        super().forward.__doc__  # trick to get docs from parent class
+
+        # Ensure that if use_projection_head is True, then return_init_embeds is True
+        assert not (
+            self.use_projection_head and not return_init_embeds
+        ), "If `use_projection_head` is True, then we must `return_init_embeds`"
+
+        out = super().forward(
+            td,
+            env,
+            phase,
+            return_actions=return_actions,
+            return_init_embeds=return_init_embeds,
+            **kwargs,
+        )
 
-        # Process embedding
-        h = self.net(init_h, mask)
+        # Project initial embeddings
+        if self.use_projection_head:
+            out["proj_embeddings"] = self.projection_head(out["init_embeds"])
 
-        # Return latent representation and initial embedding
-        return h, init_h
+        return out
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/common/autoregressive/policy.py` & `rl4co-0.4.0/rl4co/models/zoo/matnet/policy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,190 +1,209 @@
-from typing import Callable, Optional, Tuple, Union
+from math import factorial
+from typing import List
 
+import torch
 import torch.nn as nn
 
 from tensordict import TensorDict
-from torch import Tensor
 
-from rl4co.envs import RL4COEnvBase, get_env
-from rl4co.models.nn.utils import get_log_likelihood
-from rl4co.models.zoo.common.autoregressive.decoder import AutoregressiveDecoder
-from rl4co.models.zoo.common.autoregressive.encoder import GraphAttentionEncoder
-from rl4co.utils.ops import select_start_nodes
+from rl4co.envs.scheduling.ffsp.env import FFSPEnv
+from rl4co.models.common.constructive.autoregressive import AutoregressivePolicy
+from rl4co.models.zoo.matnet.decoder import (
+    MatNetDecoder,
+    MatNetFFSPDecoder,
+    MultiStageFFSPDecoder,
+)
+from rl4co.models.zoo.matnet.encoder import MatNetEncoder
+from rl4co.utils.ops import batchify
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
-class AutoregressivePolicy(nn.Module):
-    """Base Auto-regressive policy for NCO construction methods.
-    The policy performs the following steps:
-        1. Encode the environment initial state into node embeddings
-        2. Decode (autoregressively) to construct the solution to the NCO problem
-    Based on the policy from Kool et al. (2019) and extended for common use on multiple models in RL4CO.
-
-    Note:
-        We recommend to provide the decoding method as a keyword argument to the
-        decoder during actual testing. The `{phase}_decode_type` arguments are only
-        meant to be used during the main training loop. You may have a look at the
-        evaluation scripts for examples.
+class MatNetPolicy(AutoregressivePolicy):
+    """MatNet Policy from Kwon et al., 2021.
+    Reference: https://arxiv.org/abs/2106.11113
+
+    Warning:
+        This implementation is under development and subject to change.
 
     Args:
         env_name: Name of the environment used to initialize embeddings
-        encoder: Encoder module. Can be passed by sub-classes.
-        decoder: Decoder module. Can be passed by sub-classes.
-        init_embedding: Model to use for the initial embedding. If None, use the default embedding for the environment
-        context_embedding: Model to use for the context embedding. If None, use the default embedding for the environment
-        dynamic_embedding: Model to use for the dynamic embedding. If None, use the default embedding for the environment
-        select_start_nodes_fn: Function to select the start nodes for multi-start decoding
-        embedding_dim: Dimension of the node embeddings
+        embed_dim: Dimension of the node embeddings
         num_encoder_layers: Number of layers in the encoder
         num_heads: Number of heads in the attention layers
         normalization: Normalization type in the attention layers
-        mask_inner: Whether to mask the inner diagonal in the attention layers
-        use_graph_context: Whether to use the initial graph context to modify the query
-        sdpa_fn: Scaled dot product function to use for the attention
-        train_decode_type: Type of decoding during training
-        val_decode_type: Type of decoding during validation
-        test_decode_type: Type of decoding during testing
-        **unused_kw: Unused keyword arguments
+        **kwargs: keyword arguments passed to the `AutoregressivePolicy`
+
+    Default paarameters are adopted from the original implementation.
     """
 
     def __init__(
         self,
-        env_name: Union[str, RL4COEnvBase] = "tsp",
-        encoder: nn.Module = None,
-        decoder: nn.Module = None,
-        init_embedding: nn.Module = None,
-        context_embedding: nn.Module = None,
-        dynamic_embedding: nn.Module = None,
-        select_start_nodes_fn: Callable = select_start_nodes,
-        embedding_dim: int = 128,
-        num_encoder_layers: int = 3,
-        num_heads: int = 8,
-        normalization: str = "batch",
-        mask_inner: bool = True,
-        use_graph_context: bool = True,
-        sdpa_fn: Optional[Callable] = None,
-        train_decode_type: str = "sampling",
-        val_decode_type: str = "greedy",
-        test_decode_type: str = "greedy",
-        **unused_kw,
+        env_name: str = "atsp",
+        embed_dim: int = 256,
+        num_encoder_layers: int = 5,
+        num_heads: int = 16,
+        normalization: str = "instance",
+        init_embedding_kwargs: dict = {"mode": "RandomOneHot"},
+        use_graph_context: bool = False,
+        bias: bool = False,
+        **kwargs,
     ):
-        super(AutoregressivePolicy, self).__init__()
-
-        if len(unused_kw) > 0:
-            log.warn(f"Unused kwargs: {unused_kw}")
+        if env_name not in ["atsp", "ffsp"]:
+            log.error(f"env_name {env_name} is not originally implemented in MatNet")
 
-        if isinstance(env_name, RL4COEnvBase):
-            env_name = env_name.name
-        self.env_name = env_name
-
-        if encoder is None:
-            log.info("Initializing default GraphAttentionEncoder")
-            self.encoder = GraphAttentionEncoder(
-                env_name=self.env_name,
+        if env_name == "ffsp":
+            decoder = MatNetFFSPDecoder(
+                embed_dim=embed_dim,
                 num_heads=num_heads,
-                embedding_dim=embedding_dim,
-                num_layers=num_encoder_layers,
-                normalization=normalization,
-                init_embedding=init_embedding,
-                sdpa_fn=sdpa_fn,
+                use_graph_context=use_graph_context,
+                out_bias=True,
             )
-        else:
-            self.encoder = encoder
 
-        if decoder is None:
-            log.info("Initializing default AutoregressiveDecoder")
-            self.decoder = AutoregressiveDecoder(
-                env_name=self.env_name,
-                embedding_dim=embedding_dim,
+        else:
+            decoder = MatNetDecoder(
+                env_name=env_name,
+                embed_dim=embed_dim,
                 num_heads=num_heads,
                 use_graph_context=use_graph_context,
-                select_start_nodes_fn=select_start_nodes_fn,
-                mask_inner=mask_inner,
-                context_embedding=context_embedding,
-                dynamic_embedding=dynamic_embedding,
             )
-        else:
-            self.decoder = decoder
+
+        super(MatNetPolicy, self).__init__(
+            env_name=env_name,
+            encoder=MatNetEncoder(
+                embed_dim=embed_dim,
+                num_heads=num_heads,
+                num_layers=num_encoder_layers,
+                normalization=normalization,
+                init_embedding_kwargs=init_embedding_kwargs,
+                bias=bias,
+            ),
+            decoder=decoder,
+            embed_dim=embed_dim,
+            num_encoder_layers=num_encoder_layers,
+            num_heads=num_heads,
+            normalization=normalization,
+            **kwargs,
+        )
+
+
+class MultiStageFFSPPolicy(nn.Module):
+    """Policy for solving the FFSP using a seperate encoder and decoder for each
+    stage. This requires the 'while not td["done"].all()'-loop to be on policy level
+    (instead of decoder level)."""
+
+    def __init__(
+        self,
+        stage_cnt: int,
+        embed_dim: int = 256,
+        num_heads: int = 16,
+        num_encoder_layers: int = 3,
+        use_graph_context: bool = False,
+        normalization: str = "instance",
+        feedforward_hidden: int = 512,
+        bias: bool = False,
+        train_decode_type: str = "sampling",
+        val_decode_type: str = "sampling",  # authors report better results for sampling
+        test_decode_type: str = "sampling",
+    ):
+        super().__init__()
+        self.stage_cnt = stage_cnt
+
+        self.encoders: List[MatNetEncoder] = nn.ModuleList(
+            [
+                MatNetEncoder(
+                    embed_dim=embed_dim,
+                    num_heads=num_heads,
+                    num_layers=num_encoder_layers,
+                    normalization=normalization,
+                    feedforward_hidden=feedforward_hidden,
+                    bias=bias,
+                    init_embedding_kwargs={"mode": "RandomOneHot"},
+                )
+                for _ in range(self.stage_cnt)
+            ]
+        )
+        self.decoders: List[MultiStageFFSPDecoder] = nn.ModuleList(
+            [
+                MultiStageFFSPDecoder(embed_dim, num_heads, use_graph_context)
+                for _ in range(self.stage_cnt)
+            ]
+        )
 
         self.train_decode_type = train_decode_type
         self.val_decode_type = val_decode_type
         self.test_decode_type = test_decode_type
 
+    def pre_forward(self, td: TensorDict, env: FFSPEnv, num_starts: int):
+        for stage_idx in range(self.stage_cnt):
+            td["cost_matrix"] = td["run_time"][:, :, :, stage_idx]
+            encoder = self.encoders[stage_idx]
+            embeddings, _ = encoder(td)
+            decoder = self.decoders[stage_idx]
+            decoder._precompute_cache(embeddings, td)
+
+        if num_starts > 1:
+            # repeat num_start times
+            td = batchify(td, num_starts)
+            # update machine idx and action mask
+            td = env.pre_step(td)
+
+        return td
+
     def forward(
         self,
         td: TensorDict,
-        env: Union[str, RL4COEnvBase] = None,
-        phase: str = "train",
+        env: FFSPEnv,
+        phase="train",
+        num_starts=1,
         return_actions: bool = False,
-        return_entropy: bool = False,
-        return_init_embeds: bool = False,
         **decoder_kwargs,
-    ) -> dict:
-        """Forward pass of the policy.
-
-        Args:
-            td: TensorDict containing the environment state
-            env: Environment to use for decoding
-            phase: Phase of the algorithm (train, val, test)
-            return_actions: Whether to return the actions
-            return_entropy: Whether to return the entropy
-            decoder_kwargs: Keyword arguments for the decoder. See :class:`rl4co.models.zoo.common.autoregressive.decoder.AutoregressiveDecoder`
-
-        Returns:
-            out: Dictionary containing the reward, log likelihood, and optionally the actions and entropy
-        """
-
-        # ENCODER: get embeddings from initial state
-        embeddings, init_embeds = self.encoder(td)
-
-        # Instantiate environment if needed
-        if isinstance(env, str) or env is None:
-            env_name = self.env_name if env is None else env
-            log.info(f"Instantiated environment not provided; instantiating {env_name}")
-            env = get_env(env_name)
+    ):
+        assert not env.flatten_stages, "Multistage model only supports unflattened env"
+        assert num_starts <= factorial(env.num_machine)
 
         # Get decode type depending on phase
-        if decoder_kwargs.get("decode_type", None) is None:
-            decoder_kwargs["decode_type"] = getattr(self, f"{phase}_decode_type")
+        decode_type = getattr(self, f"{phase}_decode_type")
+        device = td.device
 
-        # DECODER: main rollout with autoregressive decoding
-        log_p, actions, td_out = self.decoder(td, embeddings, env, **decoder_kwargs)
+        td = self.pre_forward(td, env, num_starts)
 
-        # Log likelihood is calculated within the model
-        log_likelihood = get_log_likelihood(log_p, actions, td_out.get("mask", None))
+        # NOTE: this must come after pre_forward due to batchify op
+        batch_size = td.size(0)
+        prob_list = torch.zeros(size=(batch_size, 0), device=device)
+        action_list = []
+
+        while not td["done"].all():
+            action_stack = torch.empty(
+                size=(batch_size, self.stage_cnt), dtype=torch.long, device=device
+            )
+            prob_stack = torch.empty(size=(batch_size, self.stage_cnt), device=device)
+
+            for stage_idx in range(self.stage_cnt):
+                decoder = self.decoders[stage_idx]
+                action, prob = decoder(td, decode_type, num_starts, **decoder_kwargs)
+                action_stack[:, stage_idx] = action
+                prob_stack[:, stage_idx] = prob
+
+            gathering_index = td["stage_idx"][:, None]
+            # shape: (batch, 1)
+            action = action_stack.gather(dim=1, index=gathering_index).squeeze(dim=1)
+            prob = prob_stack.gather(dim=1, index=gathering_index).squeeze(dim=1)
+            # shape: (batch)
+            action_list.append(action)
+            # transition
+            td.set("action", action)
+            td = env.step(td)["next"]
+
+            prob_list = torch.cat((prob_list, prob[:, None]), dim=1)
 
         out = {
-            "reward": td_out["reward"],
-            "log_likelihood": log_likelihood,
+            "reward": td["reward"],
+            "log_likelihood": prob_list.log().sum(1),
         }
-        if return_actions:
-            out["actions"] = actions
-
-        if return_entropy:
-            entropy = -(log_p.exp() * log_p).nansum(dim=1)  # [batch, decoder steps]
-            entropy = entropy.sum(dim=1)  # [batch]
-            out["entropy"] = entropy
 
-        if return_init_embeds:
-            out["init_embeds"] = init_embeds
+        if return_actions:
+            out["actions"] = torch.stack(action_list, 1)
 
         return out
-
-    def evaluate_action(
-        self,
-        td: TensorDict,
-        action: Tensor,
-        env: Union[str, RL4COEnvBase] = None,
-    ) -> Tuple[Tensor, Tensor]:
-        """Evaluate the action probability and entropy under the current policy
-
-        Args:
-            td: TensorDict containing the current state
-            action: Action to evaluate
-            env: Environment to evaluate the action in.
-        """
-        embeddings, _ = self.encoder(td)
-        ll, entropy = self.decoder.evaluate_action(td, embeddings, action, env)
-        return ll, entropy
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/common/search/base.py` & `rl4co-0.4.0/rl4co/models/common/transductive/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,35 @@
+import abc
+
 from typing import Any, Optional, Union
 
 from lightning.pytorch.utilities.types import STEP_OUTPUT
 from torch.utils.data import Dataset
 
 from rl4co.models.rl.common.base import RL4COLitModule
 
 
-class SearchBase(RL4COLitModule):
-    """Base class for search algorithms. Search algorithms
-    are used onlin to find better solutions for a given dataset, i.e.
+class TransductiveModel(RL4COLitModule, metaclass=abc.ABCMeta):
+    """Base class for transductive algorithms (i.e. that optimize policy parameters for
+    specific instances, see https://en.wikipedia.org/wiki/Transduction_(machine_learning)).
+    Transductive algorithms are used online to find better solutions for a given dataset, i.e.
     given a policy, improve (a part of) its parameters such that
     the policy performs better on the given dataset.
 
     Note:
         By default, we use manual optimization to handle the search.
 
     Args:
         env: RL4CO environment
         policy: policy network
         dataset: dataset to use for training
         batch_size: batch size
+        max_iters: maximum number of iterations
+        max_runtime: maximum runtime in seconds
+        save_path: path to save the model
         **kwargs: additional arguments
     """
 
     def __init__(
         self,
         env,
         policy,
@@ -57,14 +63,15 @@
 
     def on_train_batch_start(self, batch: Any, batch_idx: int):
         """Called before training (i.e. search) for a new batch begins.
         This can be used to perform changes to the model or optimizer at the start of each batch.
         """
         pass  # Implement in subclass
 
+    @abc.abstractmethod
     def training_step(self, batch, batch_idx):
         """Main search loop. We use the training step to effectively adapt to a `batch` of instances."""
         raise NotImplementedError("Implement in subclass")
 
     def on_train_batch_end(
         self, outputs: STEP_OUTPUT, batch: Any, batch_idx: int
     ) -> None:
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/eas/nn.py` & `rl4co-0.4.0/rl4co/models/zoo/eas/nn.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/models/zoo/eas/search.py` & `rl4co-0.4.0/rl4co/models/zoo/eas/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 import torch
 
 from lightning.pytorch.utilities.types import STEP_OUTPUT
 from torch.nn.utils.rnn import pad_sequence
 from torch.utils.data import Dataset
 
 from rl4co.data.transforms import StateAugmentation
-from rl4co.models.nn.utils import get_log_likelihood
-from rl4co.models.zoo.common.search import SearchBase
-from rl4co.models.zoo.eas.decoder import forward_eas, forward_logit_attn_eas_lay
+from rl4co.models.common.transductive import TransductiveModel
+from rl4co.models.zoo.eas.decoder import forward_eas, forward_pointer_attn_eas_lay
 from rl4co.models.zoo.eas.nn import EASLayerNet
-from rl4co.utils.ops import batchify, gather_by_index, get_num_starts, unbatchify
+from rl4co.utils.decoding import get_log_likelihood
+from rl4co.utils.ops import batchify, gather_by_index, unbatchify
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
-class EAS(SearchBase):
+class EAS(TransductiveModel):
     """Efficient Active Search for Neural Combination Optimization from Hottung et al. (2022).
     Fine-tunes a subset of parameters (such as node embeddings or newly added layers) thus avoiding
     expensive re-encoding of the problem.
     Reference: https://openreview.net/pdf?id=nO5caZwFwYu
 
     Args:
         env: RL4CO environment to be solved
@@ -105,17 +105,16 @@
             f"- EAS Embedding: {self.hparams.use_eas_embedding} \n"
             f"- EAS Layer: {self.hparams.use_eas_layer} \n"
         )
         super(EAS, self).setup(stage)
 
         # Instantiate augmentation
         self.augmentation = StateAugmentation(
-            self.env.name,
             num_augment=self.hparams.augment_size,
-            use_dihedral_8=self.hparams.augment_dihedral,
+            augment_fn="dihedral8" if self.hparams.augment_dihedral else "symmetric",
         )
 
         # Store original policy state dict
         self.original_policy_state = self.policy.state_dict()
 
         # Get dataset size and problem size
         len(self.dataset)
@@ -138,15 +137,15 @@
     def training_step(self, batch, batch_idx):
         """Main search loop. We use the training step to effectively adapt to a `batch` of instances."""
         # Augment state
         batch_size = batch.shape[0]
         td_init = self.env.reset(batch)
         n_aug, n_start, n_runs = (
             self.augmentation.num_augment,
-            get_num_starts(td_init, self.env.name),
+            self.env.get_num_starts(td_init),
             self.hparams.num_parallel_runs,
         )
         td_init = self.augmentation(td_init)
         td_init = batchify(td_init, n_runs)
         num_instances = batch_size * n_aug * n_runs  # NOTE: no num_starts!
         # batch_r = n_runs * batch_size # effective batch size
         group_s = (
@@ -161,57 +160,64 @@
         embeddings, _ = encoder(td_init)
         cached_embeds = decoder._precompute_cache(embeddings)
 
         # Collect optimizer parameters
         opt_params = []
         if self.hparams.use_eas_layer:
             # EASLay: replace forward of logit attention computation. EASLayer
-            eas_layer = EASLayerNet(num_instances, decoder.embedding_dim).to(batch.device)
-            decoder.logit_attention.eas_layer = partial(
-                eas_layer, decoder.logit_attention
-            )
-            decoder.logit_attention.forward = partial(
-                forward_logit_attn_eas_lay, decoder.logit_attention
+            eas_layer = EASLayerNet(num_instances, decoder.embed_dim).to(batch.device)
+            decoder.pointer.eas_layer = partial(eas_layer, decoder.pointer)
+            decoder.pointer.forward = partial(
+                forward_pointer_attn_eas_lay, decoder.pointer
             )
             for param in eas_layer.parameters():
                 opt_params.append(param)
         if self.hparams.use_eas_embedding:
             # EASEmb: set gradient of emb_key to True
             # for all the keys, wrap the embedding in a nn.Parameter
             for key in self.hparams.eas_emb_cache_keys:
                 setattr(
                     cached_embeds, key, torch.nn.Parameter(getattr(cached_embeds, key))
                 )
                 opt_params.append(getattr(cached_embeds, key))
-        decoder.forward = partial(forward_eas, decoder)
+        decoder.forward_eas = partial(forward_eas, decoder)
+
+        # We pass attributes saved in policy too
+        def set_attr_if_exists(attr):
+            if hasattr(self.policy, attr):
+                setattr(decoder, attr, getattr(self.policy, attr))
+
+        for attr in ["temperature", "tanh_clipping", "mask_logits"]:
+            set_attr_if_exists(attr)
+
         self.configure_optimizers(opt_params)
 
         # Solution and reward buffer
         max_reward = torch.full((batch_size,), -float("inf"), device=batch.device)
         best_solutions = torch.zeros(
             batch_size, self.problem_size * 2, device=batch.device, dtype=int
         )  # i.e. incumbent solutions
 
         # Init search
         t_start = time.time()
         for iter_count in range(self.hparams.max_iters):
             # Evaluate policy with sampling multistarts passing the cached embeddings
             best_solutions_expanded = best_solutions.repeat(n_aug, 1).repeat(n_runs, 1)
-            log_p, actions, td_out, reward = decoder(
+            logprobs, actions, td_out, reward = decoder.forward_eas(
                 td_init.clone(),
                 cached_embeds=cached_embeds,
                 best_solutions=best_solutions_expanded,
                 iter_count=iter_count,
                 env=self.env,
                 decode_type="multistart_sampling",
                 num_starts=n_start,
             )
 
             # Unbatchify to get correct dimensions
-            ll = get_log_likelihood(log_p, actions, td_out.get("mask", None))
+            ll = get_log_likelihood(logprobs, actions, td_out.get("mask", None))
             ll = unbatchify(ll, (n_runs * batch_size, n_aug, group_s)).squeeze()
             reward = unbatchify(reward, (n_runs * batch_size, n_aug, group_s)).squeeze()
             actions = unbatchify(actions, (n_runs * batch_size, n_aug, group_s)).squeeze()
 
             # Compute REINFORCE loss with shared baselines
             # compared to original EAS, we also support symmetric and full baselines
             group_reward = reward[..., :-1]  # exclude incumbent solution
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/equity_transformer/positional_encoding.py` & `rl4co-0.4.0/rl4co/models/zoo/equity_transformer/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/models/zoo/ham/attention.py` & `rl4co-0.4.0/rl4co/models/zoo/ham/attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,16 @@
 
     def forward(self, q, h=None, mask=None):
         """
         Args:
             q: queries (batch_size, n_query, input_dim)
             h: data (batch_size, graph_size, input_dim)
             mask: mask (batch_size, n_query, graph_size) or viewable as that (i.e. can be 2 dim if n_query == 1)
-            Mask should contain 1 if attention is not possible (i.e. mask is negative adjacency)
+            
+        Mask should contain 1 if attention is not possible (i.e. mask is negative adjacency)
         """
         if h is None:
             h = q  # compute self-attention
 
         # h should be (batch_size, graph_size, input_dim)
         batch_size, graph_size, input_dim = h.size()
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/ham/encoder.py` & `rl4co-0.4.0/rl4co/models/zoo/ham/encoder.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,59 +6,62 @@
 
 
 class HeterogeneuousMHALayer(nn.Sequential):
     def __init__(
         self,
         num_heads,
         embed_dim,
-        feed_forward_hidden=512,
+        feedforward_hidden=512,
         normalization="batch",
     ):
         super(HeterogeneuousMHALayer, self).__init__(
             SkipConnection(HeterogenousMHA(num_heads, embed_dim, embed_dim)),
             Normalization(embed_dim, normalization),
             SkipConnection(
                 nn.Sequential(
-                    nn.Linear(embed_dim, feed_forward_hidden),
+                    nn.Linear(embed_dim, feedforward_hidden),
                     nn.ReLU(),
-                    nn.Linear(feed_forward_hidden, embed_dim),
+                    nn.Linear(feedforward_hidden, embed_dim),
                 )
-                if feed_forward_hidden > 0
+                if feedforward_hidden > 0
                 else nn.Linear(embed_dim, embed_dim)
             ),
             Normalization(embed_dim, normalization),
         )
 
 
 class GraphHeterogeneousAttentionEncoder(nn.Module):
     def __init__(
         self,
+        init_embedding=None,
         num_heads=8,
-        embedding_dim=128,
+        embed_dim=128,
         num_encoder_layers=3,
         env_name=None,
         normalization="batch",
-        feed_forward_hidden=512,
+        feedforward_hidden=512,
         sdpa_fn=None,
     ):
         super(GraphHeterogeneousAttentionEncoder, self).__init__()
+
         # substitute env_name with pdp if none
         if env_name is None:
             env_name = "pdp"
         # Map input to embedding space
-        self.init_embedding = env_init_embedding(
-            env_name, {"embedding_dim": embedding_dim}
-        )
+        if init_embedding is None:
+            self.init_embedding = env_init_embedding(env_name, {"embed_dim": embed_dim})
+        else:
+            self.init_embedding = init_embedding
 
         self.layers = nn.Sequential(
             *(
                 HeterogeneuousMHALayer(
                     num_heads,
-                    embedding_dim,
-                    feed_forward_hidden,
+                    embed_dim,
+                    feedforward_hidden,
                     normalization,
                 )
                 for _ in range(num_encoder_layers)
             )
         )
 
     def forward(self, x, mask=None):
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/ham/model.py` & `rl4co-0.4.0/rl4co/models/zoo/ham/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,10 +28,10 @@
         baseline_kwargs={},
         **kwargs,
     ):
         assert (
             env.name == "pdp"
         ), "HeterogeneousAttentionModel only works for PDP (Pickup and Delivery Problem)"
         if policy is None:
-            policy = HeterogeneousAttentionModelPolicy(env.name, **policy_kwargs)
+            policy = HeterogeneousAttentionModelPolicy(env_name=env.name, **policy_kwargs)
 
         super().__init__(env, policy, baseline, baseline_kwargs, **kwargs)
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/matnet/encoder.py` & `rl4co-0.4.0/rl4co/models/zoo/matnet/encoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import math
+
 from typing import Optional
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+
 from einops import rearrange
+
+from rl4co.models.nn.env_embeddings import env_init_embedding
 from rl4co.models.nn.ops import Normalization
-from tensordict import TensorDict
 
 
 class MatNetCrossMHA(nn.Module):
     def __init__(
         self,
-        embedding_dim: int,
+        embed_dim: int,
         num_heads: int,
-        bias: bool = True,
+        bias: bool = False,
         mixer_hidden_dim: int = 16,
         mix1_init: float = (1 / 2) ** (1 / 2),
         mix2_init: float = (1 / 16) ** (1 / 2),
     ):
         super().__init__()
-        self.embedding_dim = embedding_dim
+        self.embed_dim = embed_dim
         self.num_heads = num_heads
-        assert (
-            self.embedding_dim % num_heads == 0
-        ), "embedding_dim must be divisible by num_heads"
-        self.head_dim = self.embedding_dim // num_heads
+        assert self.embed_dim % num_heads == 0, "embed_dim must be divisible by num_heads"
+        self.head_dim = self.embed_dim // num_heads
 
-        self.Wq = nn.Linear(embedding_dim, embedding_dim, bias=bias)
-        self.Wkv = nn.Linear(embedding_dim, 2 * embedding_dim, bias=bias)
+        self.Wq = nn.Linear(embed_dim, embed_dim, bias=bias)
+        self.Wkv = nn.Linear(embed_dim, 2 * embed_dim, bias=bias)
 
         # Score mixer
         # Taken from the official MatNet implementation
         # https://github.com/yd-kwon/MatNet/blob/main/ATSP/ATSP_MatNet/ATSPModel_LIB.py#L72
         mix_W1 = torch.torch.distributions.Uniform(low=-mix1_init, high=mix1_init).sample(
             (num_heads, 2, mixer_hidden_dim)
         )
@@ -47,15 +48,15 @@
         )
         mix_b2 = torch.torch.distributions.Uniform(low=-mix2_init, high=mix2_init).sample(
             (num_heads, 1)
         )
         self.mix_W2 = nn.Parameter(mix_W2)
         self.mix_b2 = nn.Parameter(mix_b2)
 
-        self.out_proj = nn.Linear(embedding_dim, embedding_dim, bias=bias)
+        self.out_proj = nn.Linear(embed_dim, embed_dim, bias=bias)
 
     def forward(self, q_input, kv_input, dmat):
         """
 
         Args:
             q_input (Tensor): [b, m, d]
             kv_input (Tensor): [b, n, d]
@@ -99,18 +100,18 @@
 
         attn_probs = F.softmax(mix_attn_scores, dim=-1)
         out = torch.matmul(attn_probs, v)
         return self.out_proj(rearrange(out, "b h s d -> b s (h d)"))
 
 
 class MatNetMHA(nn.Module):
-    def __init__(self, embedding_dim: int, num_heads: int, bias: bool = True):
+    def __init__(self, embed_dim: int, num_heads: int, bias: bool = False):
         super().__init__()
-        self.row_encoding_block = MatNetCrossMHA(embedding_dim, num_heads, bias)
-        self.col_encoding_block = MatNetCrossMHA(embedding_dim, num_heads, bias)
+        self.row_encoding_block = MatNetCrossMHA(embed_dim, num_heads, bias)
+        self.col_encoding_block = MatNetCrossMHA(embed_dim, num_heads, bias)
 
     def forward(self, row_emb, col_emb, dmat):
         """
         Args:
             row_emb (Tensor): [b, m, d]
             col_emb (Tensor): [b, n, d]
             dmat (Tensor): [b, m, n]
@@ -126,44 +127,44 @@
         )
         return updated_row_emb, updated_col_emb
 
 
 class MatNetMHALayer(nn.Module):
     def __init__(
         self,
-        embedding_dim: int,
+        embed_dim: int,
         num_heads: int,
-        bias: bool = True,
-        feed_forward_hidden: int = 512,
+        bias: bool = False,
+        feedforward_hidden: int = 512,
         normalization: Optional[str] = "instance",
     ):
         super().__init__()
-        self.MHA = MatNetMHA(embedding_dim, num_heads, bias)
+        self.MHA = MatNetMHA(embed_dim, num_heads, bias)
 
         self.F_a = nn.ModuleDict(
             {
-                "norm1": Normalization(embedding_dim, normalization),
+                "norm1": Normalization(embed_dim, normalization),
                 "ffn": nn.Sequential(
-                    nn.Linear(embedding_dim, feed_forward_hidden),
+                    nn.Linear(embed_dim, feedforward_hidden),
                     nn.ReLU(),
-                    nn.Linear(feed_forward_hidden, embedding_dim),
+                    nn.Linear(feedforward_hidden, embed_dim),
                 ),
-                "norm2": Normalization(embedding_dim, normalization),
+                "norm2": Normalization(embed_dim, normalization),
             }
         )
 
         self.F_b = nn.ModuleDict(
             {
-                "norm1": Normalization(embedding_dim, normalization),
+                "norm1": Normalization(embed_dim, normalization),
                 "ffn": nn.Sequential(
-                    nn.Linear(embedding_dim, feed_forward_hidden),
+                    nn.Linear(embed_dim, feedforward_hidden),
                     nn.ReLU(),
-                    nn.Linear(feed_forward_hidden, embedding_dim),
+                    nn.Linear(feedforward_hidden, embed_dim),
                 ),
-                "norm2": Normalization(embedding_dim, normalization),
+                "norm2": Normalization(embed_dim, normalization),
             }
         )
 
     def forward(self, row_emb, col_emb, dmat):
         """
         Args:
             row_emb (Tensor): [b, m, d]
@@ -184,28 +185,30 @@
         col_emb_out = self.F_b["norm2"](col_emb_out + self.F_b["ffn"](col_emb_out))
         return row_emb_out, col_emb_out
 
 
 class MatNetMHANetwork(nn.Module):
     def __init__(
         self,
-        embedding_dim: int = 128,
+        embed_dim: int = 128,
         num_heads: int = 8,
         num_layers: int = 3,
         normalization: str = "batch",
-        feed_forward_hidden: int = 512,
+        feedforward_hidden: int = 512,
+        bias: bool = False,
     ):
         super().__init__()
         self.layers = nn.ModuleList(
             [
                 MatNetMHALayer(
                     num_heads=num_heads,
-                    embedding_dim=embedding_dim,
-                    feed_forward_hidden=feed_forward_hidden,
+                    embed_dim=embed_dim,
+                    feedforward_hidden=feedforward_hidden,
                     normalization=normalization,
+                    bias=bias,
                 )
                 for _ in range(num_layers)
             ]
         )
 
     def forward(self, row_emb, col_emb, dmat):
         """
@@ -220,88 +223,41 @@
         """
 
         for layer in self.layers:
             row_emb, col_emb = layer(row_emb, col_emb, dmat)
         return row_emb, col_emb
 
 
-class MatNetATSPInitEmbedding(nn.Module):
-    """
-    Preparing the initial row and column embeddings for ATSP.
-
-    Reference:
-    https://github.com/yd-kwon/MatNet/blob/782698b60979effe2e7b61283cca155b7cdb727f/ATSP/ATSP_MatNet/ATSPModel.py#L51
-
-
-    """
-
-    def __init__(self, embedding_dim: int, mode: str = "RandomOneHot") -> None:
-        super().__init__()
-
-        self.embedding_dim = embedding_dim
-        assert mode in {
-            "RandomOneHot",
-            "Random",
-        }, "mode must be one of ['RandomOneHot', 'Random']"
-        self.mode = mode
-
-        self.dmat_proj = nn.Linear(1, 2 * embedding_dim, bias=False)
-        self.row_proj = nn.Linear(embedding_dim * 4, embedding_dim, bias=False)
-        self.col_proj = nn.Linear(embedding_dim * 4, embedding_dim, bias=False)
-
-    def forward(self, td: TensorDict):
-        dmat = td["cost_matrix"]  # [b, n, n]
-        b, n, _ = dmat.shape
-
-        row_emb = torch.zeros(b, n, self.embedding_dim, device=dmat.device)
-
-        if self.mode == "RandomOneHot":
-            # MatNet uses one-hot encoding for column embeddings
-            # https://github.com/yd-kwon/MatNet/blob/782698b60979effe2e7b61283cca155b7cdb727f/ATSP/ATSP_MatNet/ATSPModel.py#L60
-
-            col_emb = torch.zeros(b, n, self.embedding_dim, device=dmat.device)
-            rand = torch.rand(b, n)
-            rand_idx = rand.argsort(dim=1)
-            b_idx = torch.arange(b)[:, None].expand(b, n)
-            n_idx = torch.arange(n)[None, :].expand(b, n)
-            col_emb[b_idx, n_idx, rand_idx] = 1.0
-
-        elif self.mode == "Random":
-            col_emb = torch.rand(b, n, self.embedding_dim, device=dmat.device)
-        else:
-            raise NotImplementedError
-
-        return row_emb, col_emb, dmat
-
-
 class MatNetEncoder(nn.Module):
     def __init__(
         self,
-        embedding_dim: int = 256,
+        embed_dim: int = 256,
         num_heads: int = 16,
         num_layers: int = 5,
         normalization: str = "instance",
-        feed_forward_hidden: int = 512,
+        feedforward_hidden: int = 512,
         init_embedding: nn.Module = None,
         init_embedding_kwargs: dict = None,
+        bias: bool = False,
     ):
         super().__init__()
 
         if init_embedding is None:
-            init_embedding = MatNetATSPInitEmbedding(
-                embedding_dim, **init_embedding_kwargs
+            init_embedding = env_init_embedding(
+                "matnet", {"embed_dim": embed_dim, **init_embedding_kwargs}
             )
 
         self.init_embedding = init_embedding
         self.net = MatNetMHANetwork(
-            embedding_dim=embedding_dim,
+            embed_dim=embed_dim,
             num_heads=num_heads,
             num_layers=num_layers,
             normalization=normalization,
-            feed_forward_hidden=feed_forward_hidden,
+            feedforward_hidden=feedforward_hidden,
+            bias=bias,
         )
 
     def forward(self, td):
         row_emb, col_emb, dmat = self.init_embedding(td)
         row_emb, col_emb = self.net(row_emb, col_emb, dmat)
 
         embedding = (row_emb, col_emb)
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/matnet/policy.py` & `rl4co-0.4.0/rl4co/models/zoo/ham/policy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,62 @@
-from rl4co.models.zoo.common.autoregressive import AutoregressivePolicy
-from rl4co.models.zoo.matnet.encoder import MatNetEncoder
-from rl4co.models.zoo.matnet.decoder import MatNetDecoder
-from rl4co.utils.pylogger import get_pylogger
+from typing import Callable, Optional
 
-log = get_pylogger(__name__)
+import torch.nn as nn
 
+from rl4co.models.zoo.am import AttentionModelPolicy
+from rl4co.models.zoo.ham.encoder import GraphHeterogeneousAttentionEncoder
 
-class MatNetPolicy(AutoregressivePolicy):
-    """MatNet Policy from Kwon et al., 2021.
-    Reference: https://arxiv.org/abs/2106.11113
 
-    Warning:
-        This implementation is under development and subject to change.
+class HeterogeneousAttentionModelPolicy(AttentionModelPolicy):
+    """Heterogeneous Attention Model Policy based on https://ieeexplore.ieee.org/document/9352489.
+    We re-declare the most important arguments here for convenience as in the paper.
+    See :class:`rl4co.models.zoo.am.AttentionModelPolicy` for more details.
 
     Args:
+        encoder: Encoder module. Can be passed by sub-classes
         env_name: Name of the environment used to initialize embeddings
-        embedding_dim: Dimension of the node embeddings
+        init_embedding: Model to use for the initial embedding. If None, use the default embedding for the environment
+        embed_dim: Dimension of the embeddings
         num_encoder_layers: Number of layers in the encoder
-        num_heads: Number of heads in the attention layers
-        normalization: Normalization type in the attention layers
-        **kwargs: keyword arguments passed to the `AutoregressivePolicy`
-
-    Default paarameters are adopted from the original implementation.
+        num_heads: Number of heads for the attention in encoder
+        normalization: Normalization to use for the attention layers
+        feedforward_hidden: Dimension of the hidden layer in the feedforward network
+        sdpa_fn: Function to use for the scaled dot product attention
+        **kwargs: keyword arguments passed to the :class:`rl4co.models.zoo.am.AttentionModelPolicy`
     """
 
     def __init__(
         self,
-        env_name: str,
-        embedding_dim: int = 256,
-        num_encoder_layers: int = 5,
-        num_heads: int = 16,
-        normalization: str = "instance",
-        init_embedding_kwargs: dict = {"mode": "RandomOneHot"},
-        use_graph_context: bool = False,
+        encoder: nn.Module = None,
+        env_name: str = "pdp",
+        init_embedding: nn.Module = None,
+        embed_dim: int = 128,
+        num_encoder_layers: int = 3,
+        num_heads: int = 8,
+        normalization: str = "batch",
+        feedforward_hidden: int = 512,
+        sdpa_fn: Optional[Callable] = None,
         **kwargs,
     ):
-        if env_name not in ["atsp"]:
-            log.error(f"env_name {env_name} is not originally implemented in MatNet")
-
-        super(MatNetPolicy, self).__init__(
-            env_name=env_name,
-            encoder=MatNetEncoder(
-                embedding_dim=embedding_dim,
+        if encoder is None:
+            encoder = GraphHeterogeneousAttentionEncoder(
+                init_embedding=init_embedding,
                 num_heads=num_heads,
-                num_layers=num_encoder_layers,
-                normalization=normalization,
-                init_embedding_kwargs=init_embedding_kwargs,
-            ),
-            decoder=MatNetDecoder(
+                embed_dim=embed_dim,
+                num_encoder_layers=num_encoder_layers,
                 env_name=env_name,
-                embedding_dim=embedding_dim,
-                num_heads=num_heads,
-                use_graph_context=use_graph_context,
-            ),
-            embedding_dim=embedding_dim,
+                normalization=normalization,
+                feedforward_hidden=feedforward_hidden,
+                sdpa_fn=sdpa_fn,
+            )
+        else:
+            encoder = encoder
+
+        super(HeterogeneousAttentionModelPolicy, self).__init__(
+            env_name=env_name,
+            encoder=encoder,
+            embed_dim=embed_dim,
             num_encoder_layers=num_encoder_layers,
             num_heads=num_heads,
             normalization=normalization,
             **kwargs,
         )
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/mdam/decoder.py` & `rl4co-0.4.0/rl4co/models/zoo/mdam/decoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,99 +2,95 @@
 
 from dataclasses import dataclass
 from typing import Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+
 from tensordict import TensorDict
 
 from rl4co.envs import RL4COEnvBase
-from rl4co.models.nn.attention import LogitAttention
+from rl4co.models.nn.attention import PointerAttention
 from rl4co.models.nn.env_embeddings import env_context_embedding, env_dynamic_embedding
-from rl4co.models.nn.utils import decode_probs, get_log_likelihood
+from rl4co.utils.decoding import decode_logprobs, get_log_likelihood
 
 
 @dataclass
 class PrecomputedCache:
     node_embeddings: torch.Tensor
     graph_context: torch.Tensor
     glimpse_key: torch.Tensor
     glimpse_val: torch.Tensor
     logit_key: torch.Tensor
 
 
-class Decoder(nn.Module):
+class MDAMDecoder(nn.Module):
     def __init__(
         self,
-        env_name,
-        embedding_dim,
-        num_heads,
+        embed_dim: int = 128,
+        num_heads: int = 8,
         num_paths: int = 5,
+        env_name: str = "tsp",
         mask_inner: bool = True,
         mask_logits: bool = True,
         eg_step_gap: int = 200,
         tanh_clipping: float = 10.0,
-        force_flash_attn: bool = False,
         shrink_size=None,
         train_decode_type: str = "sampling",
         val_decode_type: str = "greedy",
         test_decode_type: str = "greedy",
     ):
-        super(Decoder, self).__init__()
-        self.dynamic_embedding = env_dynamic_embedding(
-            env_name, {"embedding_dim": embedding_dim}
-        )
+        super(MDAMDecoder, self).__init__()
+        self.dynamic_embedding = env_dynamic_embedding(env_name, {"embed_dim": embed_dim})
 
         self.train_decode_type = train_decode_type
         self.val_decode_type = val_decode_type
         self.test_decode_type = test_decode_type
 
-        self.W_placeholder = nn.Parameter(torch.Tensor(2 * embedding_dim))
+        self.W_placeholder = nn.Parameter(torch.Tensor(2 * embed_dim))
         self.W_placeholder.data.uniform_(
             -1, 1
         )  # Placeholder should be in range of activations
 
-        self.context = [
-            env_context_embedding(env_name, {"embedding_dim": embedding_dim})
-            for _ in range(num_paths)
-        ]
+        self.context = nn.ModuleList(
+            [
+                env_context_embedding(env_name, {"embed_dim": embed_dim})
+                for _ in range(num_paths)
+            ]
+        )
 
         self.project_node_embeddings = [
-            nn.Linear(embedding_dim, 3 * embedding_dim, bias=False)
-            for _ in range(num_paths)
+            nn.Linear(embed_dim, 3 * embed_dim, bias=False) for _ in range(num_paths)
         ]
         self.project_node_embeddings = nn.ModuleList(self.project_node_embeddings)
 
         self.project_fixed_context = [
-            nn.Linear(embedding_dim, embedding_dim, bias=False) for _ in range(num_paths)
+            nn.Linear(embed_dim, embed_dim, bias=False) for _ in range(num_paths)
         ]
         self.project_fixed_context = nn.ModuleList(self.project_fixed_context)
 
         self.project_step_context = [
-            nn.Linear(2 * embedding_dim, embedding_dim, bias=False)
-            for _ in range(num_paths)
+            nn.Linear(2 * embed_dim, embed_dim, bias=False) for _ in range(num_paths)
         ]
         self.project_step_context = nn.ModuleList(self.project_step_context)
 
         self.project_out = [
-            nn.Linear(embedding_dim, embedding_dim, bias=False) for _ in range(num_paths)
+            nn.Linear(embed_dim, embed_dim, bias=False) for _ in range(num_paths)
         ]
         self.project_out = nn.ModuleList(self.project_out)
 
-        self.dynamic_embedding = env_dynamic_embedding(
-            env_name, {"embedding_dim": embedding_dim}
-        )
+        self.dynamic_embedding = env_dynamic_embedding(env_name, {"embed_dim": embed_dim})
 
-        self.logit_attention = [
-            LogitAttention(
-                embedding_dim,
+        # MHA with Pointer mechanism (https://arxiv.org/abs/1506.03134)
+        self.pointer = [
+            PointerAttention(
+                embed_dim,
                 num_heads,
                 mask_inner=mask_inner,
-                force_flash_attn=force_flash_attn,
             )
             for _ in range(num_paths)
         ]
 
         self.env_name = env_name
         self.mask_inner = mask_inner
         self.mask_logits = mask_logits
@@ -108,30 +104,32 @@
         self,
         td: TensorDict,
         encoded_inputs: torch.Tensor,
         env: Union[str, RL4COEnvBase],
         attn,
         V,
         h_old,
+        encoder,  # note: used because of different paths, could be better modularized
         **decoder_kwargs,
     ):
         # SECTION: Decoder first step: calculate for the decoder divergence loss
         # Cost list and log likelihood list along with path
         output_list = []
-        td_list = [env.reset(td) for i in range(self.num_paths)]
+        # td_list = [env.reset(td) for i in range(self.num_paths)]
+        td_list = [td.clone() for i in range(self.num_paths)]
         for i in range(self.num_paths):
             # Clone the encoded features for this path
             _encoded_inputs = encoded_inputs.clone()
 
             # Compute keys, values for the glimpse and keys for the logits once as they can be reused in every step
             fixed = self._precompute(_encoded_inputs, path_index=i)
-            log_p, _ = self._get_log_p(fixed, td_list[i], i)
+            logprobs, _ = self._get_logprobs(fixed, td_list[i], i)
 
             # Collect output of step
-            output_list.append(log_p[:, 0, :])
+            output_list.append(logprobs[:, 0, :])
             output_list[-1] = torch.max(
                 output_list[-1],
                 torch.ones(
                     output_list[-1].shape,
                     dtype=output_list[-1].dtype,
                     device=output_list[-1].device,
                 )
@@ -153,15 +151,16 @@
 
         # SECTION: Decoder rest step: calculate for other decoder divergence loss
         # Cost list and log likelihood list along with path
         reward_list = []
         output_list = []
         action_list = []
         ll_list = []
-        td_list = [env.reset(td) for _ in range(self.num_paths)]
+        # td_list = [env.reset(td) for _ in range(self.num_paths)]
+        td_list = [td.clone() for i in range(self.num_paths)]
         for i in range(self.num_paths):
             # Clone the encoded features for this path
             _encoded_inputs = encoded_inputs.clone()
             _attn = attn.clone()
             _V = V.clone()
             _h_old = h_old.clone()
 
@@ -169,51 +168,53 @@
             fixed = self._precompute(_encoded_inputs, path_index=i)
 
             j = 0
             mask, mask_first = None, None  # dummy, we get them during the steps
             while not (self.shrink_size is None and td_list[i]["done"].all()):
                 if j > 1 and j % self.eg_step_gap == 0:
                     if not self.is_vrp:
+                        # TODO: modularize
                         mask_attn = mask ^ mask_first
                     else:
                         mask_attn = mask
-                    _encoded_inputs, _ = self.embedder.change(
-                        _attn, _V, _h_old, mask_attn, self.is_tsp
-                    )
+
+                    # TODO: decoder
+                    _encoded_inputs, _ = encoder.change(_attn, _V, _h_old, mask_attn)
                     fixed = self._precompute(_encoded_inputs, path_index=i)
-                log_p, mask = self._get_log_p(fixed, td_list[i], i)
+                logprobs, mask = self._get_logprobs(fixed, td_list[i], i)
                 if j == 0:
                     pass
 
                 # Select the indices of the next nodes in the sequences, result (batch_size) long
-                action = decode_probs(
-                    log_p.exp()[:, 0, :],
+                action = decode_logprobs(
+                    logprobs[:, 0, :],
                     mask,
                     decode_type=decoder_kwargs["decode_type"],
                 )
 
                 td_list[i].set("action", action)
                 td_list[i] = env.step(td_list[i])["next"]
 
                 # Collect output of step
-                outputs.append(log_p[:, 0, :])
+                outputs.append(logprobs[:, 0, :])
                 actions.append(action)
                 j += 1
 
+            assert len(outputs) > 0, "No outputs were generated, check if envs were done"
             outputs, actions = torch.stack(outputs, 1), torch.stack(actions, 1)
             reward = env.get_reward(td, actions)
-            ll = get_log_likelihood(outputs, actions, mask)
+            ll = get_log_likelihood(outputs, actions, mask=None)
 
             reward_list.append(reward)
             output_list.append(outputs)
             action_list.append(actions)
             ll_list.append(ll)
 
-        reward = torch.stack(reward_list, 0)
-        log_likelihood = torch.stack(ll_list, 0)
+        reward = torch.stack(reward_list, 1)
+        log_likelihood = torch.stack(ll_list, 1)
         return reward, log_likelihood, loss_kl_divergence, actions
 
     def _precompute(self, embeddings, num_steps=1, path_index=None):
         # The fixed context projection of the graph embedding is calculated only once for efficiency
         graph_embed = embeddings.mean(1)
 
         # Fixed context = (batch_size, 1, embed_dim) to make broadcastable with parallel timesteps
@@ -250,15 +251,15 @@
                 -1,
             )
             .permute(
                 3, 0, 1, 2, 4
             )  # (n_heads, batch_size, num_steps, graph_size, head_dim)
         )
 
-    def _get_log_p(self, fixed, td, path_index, normalize=True):
+    def _get_logprobs(self, fixed, td, path_index, normalize=True):
         step_context = self.context[path_index](
             fixed.node_embeddings, td
         )  # [batch, embed_dim]
         glimpse_q = fixed.graph_context + step_context.unsqueeze(1).to(
             fixed.graph_context.device
         )
 
@@ -268,23 +269,23 @@
             glimpse_val_dynamic,
             logit_key_dynamic,
         ) = self.dynamic_embedding(td)
         glimpse_k = fixed.glimpse_key + glimpse_key_dynamic
         glimpse_v = fixed.glimpse_val + glimpse_val_dynamic
         logit_k = fixed.logit_key + logit_key_dynamic
 
-        # Compute the mask
-        mask = ~td["action_mask"]
+        # Compute the action mask
+        mask = td["action_mask"]
 
-        # Compute logits (unnormalized log_p)
-        # log_p, _ = self.logit_attention[path_index](glimpse_q, glimpse_k, glimpse_v, logit_k, mask, path_index)
-        log_p, _ = self._one_to_many_logits(
+        # Compute logits (unnormalized logprobs)
+        # logprobs, _ = self.logit_attention[path_index](glimpse_q, glimpse_k, glimpse_v, logit_k, mask, path_index)
+        logprobs, _ = self._one_to_many_logits(
             glimpse_q, glimpse_k, glimpse_v, logit_k, mask, path_index
         )
-        return log_p, mask
+        return logprobs, mask
 
     def _one_to_many_logits(self, query, glimpse_K, glimpse_V, logit_K, mask, path_index):
         batch_size, num_steps, embed_dim = query.size()
         key_size = val_size = embed_dim // self.num_heads
 
         # Compute the glimpse, rearrange dimensions so the dimensions are (n_heads, batch_size, num_steps, 1, key_size)
         glimpse_Q = query.view(
@@ -294,21 +295,21 @@
         # Batch matrix multiplication to compute compatibilities (n_heads, batch_size, num_steps, graph_size)
         compatibility = torch.matmul(glimpse_Q, glimpse_K.transpose(-2, -1)) / math.sqrt(
             glimpse_Q.size(-1)
         )
         if self.mask_inner:
             assert self.mask_logits, "Cannot mask inner without masking logits"
             compatibility[
-                mask[None, :, None, None, :].expand_as(compatibility)
+                ~mask[None, :, None, None, :].expand_as(compatibility)
             ] = -math.inf
 
         # Batch matrix multiplication to compute heads (n_heads, batch_size, num_steps, val_size)
         heads = torch.matmul(F.softmax(compatibility, dim=-1), glimpse_V)
 
-        # Project to get glimpse/updated context node embedding (batch_size, num_steps, embedding_dim)
+        # Project to get glimpse/updated context node embedding (batch_size, num_steps, embed_dim)
         glimpse = self.project_out[path_index](
             heads.permute(1, 2, 3, 0, 4)
             .contiguous()
             .view(-1, num_steps, 1, self.num_heads * val_size)
         )
 
         # Now projecting the glimpse is not needed since this can be absorbed into project_out
@@ -321,10 +322,10 @@
             final_Q.size(-1)
         )
 
         # From the logits compute the probabilities by clipping, masking and softmax
         if self.tanh_clipping > 0:
             logits = F.tanh(logits) * self.tanh_clipping
         if self.mask_logits:
-            logits[mask[:, None, :]] = -math.inf
+            logits[~mask[:, None, :]] = -math.inf
 
         return logits, glimpse.squeeze(-2)
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/mdam/encoder.py` & `rl4co-0.4.0/rl4co/models/zoo/mdam/encoder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 from typing import Callable, Optional
 
 import torch
-
-from torch import nn
+import torch.nn as nn
 
 from rl4co.models.nn.graph.attnnet import (
-    MultiHeadAttention,
     MultiHeadAttentionLayer,
     Normalization,
     SkipConnection,
 )
+from rl4co.models.zoo.mdam.mha import MultiHeadAttentionMDAM
 
 
-class GraphAttentionEncoder(nn.Module):
+class MDAMGraphAttentionEncoder(nn.Module):
     def __init__(
         self,
         num_heads,
         embed_dim,
         num_layers,
         node_dim=None,
         normalization="batch",
-        feed_forward_hidden=512,
+        feedforward_hidden=512,
         sdpa_fn: Optional[Callable] = None,
     ):
-        super(GraphAttentionEncoder, self).__init__()
+        super(MDAMGraphAttentionEncoder, self).__init__()
 
         # To map input to embedding space
         self.init_embed = nn.Linear(node_dim, embed_dim) if node_dim is not None else None
 
-        self.layers = MultiHeadAttentionLayer(
-            num_heads,
-            embed_dim,
-            num_layers - 1,
-            feed_forward_hidden,
-            normalization,
-            sdpa_fn=sdpa_fn,
+        self.layers = nn.Sequential(
+            *(
+                MultiHeadAttentionLayer(
+                    embed_dim,
+                    num_heads,
+                    feedforward_hidden,
+                    normalization,
+                    sdpa_fn=sdpa_fn,
+                )
+                for _ in range(num_layers - 1)  # because last layer is different
+            )
         )
-        self.attention_layer = MultiHeadAttention(
-            num_heads, input_dim=embed_dim, embed_dim=embed_dim, sdpa_fn=sdpa_fn
+        self.attention_layer = MultiHeadAttentionMDAM(
+            embed_dim, num_heads, sdpa_fn=sdpa_fn, last_one=True
         )
         self.BN1 = Normalization(embed_dim, normalization)
         self.projection = SkipConnection(
             nn.Sequential(
-                nn.Linear(embed_dim, feed_forward_hidden),
+                nn.Linear(embed_dim, feedforward_hidden),
                 nn.ReLU(),
-                nn.Linear(feed_forward_hidden, embed_dim),
+                nn.Linear(feedforward_hidden, embed_dim),
             )
-            if feed_forward_hidden > 0
+            if feedforward_hidden > 0
             else nn.Linear(embed_dim, embed_dim)
         )
         self.BN2 = Normalization(embed_dim, normalization)
 
     def forward(self, x, mask=None, return_transform_loss=False):
         """
         Returns:
@@ -67,27 +70,25 @@
         h = h_new + h_old
         h = self.BN1(h)
         h = self.projection(h)
         h = self.BN2(h)
 
         return (h, h.mean(dim=1), attn, V, h_old)
 
-    def change(self, attn, V, h_old, mask, is_tsp=False):
+    def change(self, attn, V, h_old, mask):
         num_heads, batch_size, graph_size, feat_size = V.size()
-        attn = (1 - mask.float()).view(1, batch_size, 1, graph_size).repeat(
-            num_heads, 1, graph_size, 1
-        ) * attn
-        if is_tsp:
-            attn = attn / (
-                torch.sum(attn, dim=-1).view(num_heads, batch_size, graph_size, 1)
-            )
-        else:
-            attn = attn / (
-                torch.sum(attn, dim=-1).view(num_heads, batch_size, graph_size, 1) + 1e-9
-            )
+        attn = (
+            mask.float()
+            .view(1, batch_size, 1, graph_size)
+            .repeat(num_heads, 1, graph_size, 1)
+            * attn
+        )
+        attn = attn / (
+            torch.sum(attn, dim=-1).view(num_heads, batch_size, graph_size, 1) + 1e-9
+        )
         heads = torch.matmul(attn, V)
 
         h_new = torch.mm(
             heads.permute(1, 2, 0, 3)
             .contiguous()
             .view(-1, self.attention_layer.num_heads * self.attention_layer.val_dim),
             self.attention_layer.W_out.view(-1, self.attention_layer.embed_dim),
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/mdam/model.py` & `rl4co-0.4.0/rl4co/models/zoo/ptrnet/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from typing import Union
 
 from rl4co.envs.common.base import RL4COEnvBase
 from rl4co.models.rl import REINFORCE
 from rl4co.models.rl.reinforce.baselines import REINFORCEBaseline
-from rl4co.models.zoo.mdam.policy import MDAMPolicy
+from rl4co.models.zoo.ptrnet.policy import PointerNetworkPolicy
 
 
-class MDAM(REINFORCE):
-    """Multi-Decoder Attention Model (MDAM) is a model
-    to train multiple diverse policies, which effectively increases the chance of finding
-    good solutions compared with existing methods that train only one policy.
-    Reference link: https://arxiv.org/abs/2012.10638;
-    Implementation reference: https://github.com/liangxinedu/MDAM.
+class PointerNetwork(REINFORCE):
+    """Pointer Network for neural combinatorial optimization based on REINFORCE
+    Based on Vinyals et al. (2015) https://arxiv.org/abs/1506.03134
+    Refactored from reference implementation: https://github.com/wouterkool/attention-learn-to-route
 
     Args:
         env: Environment to use for the algorithm
         policy: Policy to use for the algorithm
         baseline: REINFORCE baseline. Defaults to rollout (1 epoch of exponential, then greedy rollout baseline)
         policy_kwargs: Keyword arguments for policy
         baseline_kwargs: Keyword arguments for baseline
         **kwargs: Keyword arguments passed to the superclass
     """
 
     def __init__(
         self,
         env: RL4COEnvBase,
-        policy: MDAMPolicy = None,
+        policy: PointerNetworkPolicy = None,
         baseline: Union[REINFORCEBaseline, str] = "rollout",
         policy_kwargs={},
         baseline_kwargs={},
         **kwargs,
     ):
-        if policy is None:
-            policy = MDAMPolicy(env.name, **policy_kwargs)
-
+        policy = (
+            PointerNetworkPolicy(env=env, **policy_kwargs) if policy is None else policy
+        )
         super().__init__(env, policy, baseline, baseline_kwargs, **kwargs)
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/mdam/policy.py` & `rl4co-0.4.0/rl4co/models/zoo/mdam/policy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 from typing import Union
 
 from tensordict import TensorDict
 
 from rl4co.envs import RL4COEnvBase, get_env
+from rl4co.models.common.constructive.autoregressive import AutoregressivePolicy
 from rl4co.models.nn.env_embeddings import env_init_embedding
-from rl4co.models.zoo.common.autoregressive import AutoregressivePolicy
-from rl4co.models.zoo.mdam.decoder import Decoder
-from rl4co.models.zoo.mdam.encoder import GraphAttentionEncoder
+from rl4co.models.zoo.mdam.decoder import MDAMDecoder
+from rl4co.models.zoo.mdam.encoder import MDAMGraphAttentionEncoder
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class MDAMPolicy(AutoregressivePolicy):
     """Multi-Decoder Attention Model (MDAM) policy.
     Args:
 
     """
 
     def __init__(
         self,
-        env_name: str,
-        embedding_dim: int = 128,
+        encoder: MDAMGraphAttentionEncoder = None,
+        decoder: MDAMDecoder = None,
+        embed_dim: int = 128,
+        env_name: str = "tsp",
         num_encoder_layers: int = 3,
         num_heads: int = 8,
         normalization: str = "batch",
-        **kwargs,
+        **decoder_kwargs,
     ):
-        super(MDAMPolicy, self).__init__(
-            env_name=env_name,
-            encoder=GraphAttentionEncoder(
+        encoder = (
+            MDAMGraphAttentionEncoder(
                 num_heads=num_heads,
-                embed_dim=embedding_dim,
+                embed_dim=embed_dim,
                 num_layers=num_encoder_layers,
                 normalization=normalization,
-                **kwargs,
-            ),
-            decoder=Decoder(
+            )
+            if encoder is None
+            else encoder
+        )
+
+        decoder = (
+            MDAMDecoder(
                 env_name=env_name,
-                embedding_dim=embedding_dim,
+                embed_dim=embed_dim,
                 num_heads=num_heads,
-                **kwargs,
-            ),
-            embedding_dim=embedding_dim,
-            num_encoder_layers=num_encoder_layers,
-            num_heads=num_heads,
-            normalization=normalization,
-            **kwargs,
+                **decoder_kwargs,
+            )
+            if decoder is None
+            else decoder
         )
 
-        self.init_embedding = env_init_embedding(
-            env_name, {"embedding_dim": embedding_dim}
+        super(MDAMPolicy, self).__init__(
+            env_name=env_name, encoder=encoder, decoder=decoder
         )
 
+        self.init_embedding = env_init_embedding(env_name, {"embed_dim": embed_dim})
+
     def forward(
         self,
         td: TensorDict,
         env: Union[str, RL4COEnvBase] = None,
         phase: str = "train",
         return_actions: bool = False,
         **decoder_kwargs,
@@ -71,15 +75,15 @@
             env = get_env(env_name)
 
         # Get decode type depending on phase
         if decoder_kwargs.get("decode_type", None) is None:
             decoder_kwargs["decode_type"] = getattr(self, f"{phase}_decode_type")
 
         reward, log_likelihood, kl_divergence, actions = self.decoder(
-            td, encoded_inputs, env, attn, V, h_old, **decoder_kwargs
+            td, encoded_inputs, env, attn, V, h_old, self.encoder, **decoder_kwargs
         )
         out = {
             "reward": reward,
             "log_likelihood": log_likelihood,
             "entropy": kl_divergence,
             "actions": actions if return_actions else None,
         }
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/pomo/model.py` & `rl4co-0.4.0/rl4co/models/zoo/pomo/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,122 +1,133 @@
 from typing import Any, Union
 
 import torch.nn as nn
 
 from rl4co.data.transforms import StateAugmentation
 from rl4co.envs.common.base import RL4COEnvBase
 from rl4co.models.rl.reinforce.reinforce import REINFORCE
-from rl4co.models.zoo.pomo.policy import POMOPolicy
-from rl4co.utils.ops import (
-    gather_by_index,
-    get_num_starts,
-    select_start_nodes,
-    unbatchify,
-)
+from rl4co.models.zoo.am import AttentionModelPolicy
+from rl4co.utils.ops import gather_by_index, unbatchify
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class POMO(REINFORCE):
     """POMO Model for neural combinatorial optimization based on REINFORCE
     Based on Kwon et al. (2020) http://arxiv.org/abs/2010.16011.
 
+    Note:
+        If no policy kwargs is passed, we use the Attention Model policy with the following arguments:
+        Differently to the base class:
+        - `num_encoder_layers=6` (instead of 3)
+        - `normalization="instance"` (instead of "batch")
+        - `use_graph_context=False` (instead of True)
+        The latter is due to the fact that the paper does not use the graph context in the policy, which seems to be
+        helpful in overfitting to the training graph size.
+
     Args:
         env: TorchRL Environment
         policy: Policy to use for the algorithm
         policy_kwargs: Keyword arguments for policy
         baseline: Baseline to use for the algorithm. Note that POMO only supports shared baseline,
             so we will throw an error if anything else is passed.
         num_augment: Number of augmentations (used only for validation and test)
-        use_dihedral_8: Whether to use dihedral 8 augmentation
+        augment_fn: Function to use for augmentation, defaulting to dihedral8
+        first_aug_identity: Whether to include the identity augmentation in the first position
+        feats: List of features to augment
         num_starts: Number of starts for multi-start. If None, use the number of available actions
-        select_start_nodes_fn: Function to select the start nodes for the environment defaulting to :func:`select_start_nodes`
         **kwargs: Keyword arguments passed to the superclass
     """
 
     def __init__(
         self,
         env: RL4COEnvBase,
-        policy: Union[nn.Module, POMOPolicy] = None,
+        policy: nn.Module = None,
         policy_kwargs={},
         baseline: str = "shared",
         num_augment: int = 8,
-        use_dihedral_8: bool = True,
+        augment_fn: Union[str, callable] = "dihedral8",
+        first_aug_identity: bool = True,
+        feats: list = None,
         num_starts: int = None,
-        select_start_nodes_fn: callable = select_start_nodes,
         **kwargs,
     ):
         self.save_hyperparameters(logger=False)
 
-        # If select_start_nodes_fn is provided in policy_kwargs, we use that instead
-        if "select_start_nodes_fn" in policy_kwargs:
-            log.info(
-                "Overriding select_start_nodes_fn in POMO with the one provided in policy_kwargs"
-            )
-        policy_kwargs["select_start_nodes_fn"] = select_start_nodes_fn
-
         if policy is None:
-            policy = POMOPolicy(env.name, **policy_kwargs)
+            policy_kwargs_with_defaults = {
+                "num_encoder_layers": 6,
+                "normalization": "instance",
+                "use_graph_context": False,
+            }
+            policy_kwargs_with_defaults.update(policy_kwargs)
+            policy = AttentionModelPolicy(env_name=env.name, **policy_kwargs_with_defaults)
 
         assert baseline == "shared", "POMO only supports shared baseline"
 
         # Initialize with the shared baseline
         super(POMO, self).__init__(env, policy, baseline, **kwargs)
 
         self.num_starts = num_starts
         self.num_augment = num_augment
         if self.num_augment > 1:
             self.augment = StateAugmentation(
-                self.env.name, num_augment=self.num_augment, use_dihedral_8=use_dihedral_8
+                num_augment=self.num_augment,
+                augment_fn=augment_fn,
+                first_aug_identity=first_aug_identity,
+                feats=feats,
             )
         else:
             self.augment = None
 
         # Add `_multistart` to decode type for train, val and test in policy
         for phase in ["train", "val", "test"]:
             self.set_decode_type_multistart(phase)
 
     def shared_step(
         self, batch: Any, batch_idx: int, phase: str, dataloader_idx: int = None
     ):
         td = self.env.reset(batch)
         n_aug, n_start = self.num_augment, self.num_starts
-        n_start = get_num_starts(td, self.env.name) if n_start is None else n_start
+        n_start = self.env.get_num_starts(td) if n_start is None else n_start
 
         # During training, we do not augment the data
         if phase == "train":
             n_aug = 0
         elif n_aug > 1:
             td = self.augment(td)
 
         # Evaluate policy
-        out = self.policy(td, self.env, phase=phase, num_starts=n_start)
+        out = self.policy(
+            td, self.env, phase=phase, num_starts=n_start, return_actions=True
+        )
 
         # Unbatchify reward to [batch_size, num_augment, num_starts].
         reward = unbatchify(out["reward"], (n_aug, n_start))
 
         # Training phase
         if phase == "train":
             assert n_start > 1, "num_starts must be > 1 during training"
             log_likelihood = unbatchify(out["log_likelihood"], (n_aug, n_start))
             self.calculate_loss(td, batch, out, reward, log_likelihood)
-
+            max_reward, max_idxs = reward.max(dim=-1)
+            out.update({"max_reward": max_reward})
         # Get multi-start (=POMO) rewards and best actions only during validation and test
         else:
             if n_start > 1:
                 # max multi-start reward
                 max_reward, max_idxs = reward.max(dim=-1)
                 out.update({"max_reward": max_reward})
 
                 if out.get("actions", None) is not None:
                     # Reshape batch to [batch_size, num_augment, num_starts, ...]
                     actions = unbatchify(out["actions"], (n_aug, n_start))
                     out.update(
-                        {"best_multistart_actions": gather_by_index(actions, max_idxs)}
+                        {"best_multistart_actions": gather_by_index(actions, max_idxs, dim=max_idxs.dim())}
                     )
                     out["actions"] = actions
 
             # Get augmentation score only during inference
             if n_aug > 1:
                 # If multistart is enabled, we use the best multistart rewards
                 reward_ = max_reward if n_start > 1 else reward
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/ptrnet/critic.py` & `rl4co-0.4.0/rl4co/models/zoo/ptrnet/critic.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 
 
 class CriticNetworkLSTM(nn.Module):
     """Useful as a baseline in REINFORCE updates"""
 
     def __init__(
         self,
-        embedding_dim,
+        embed_dim,
         hidden_dim,
         n_process_block_iters,
         tanh_exploration,
         use_tanh,
     ):
         super(CriticNetworkLSTM, self).__init__()
 
         self.hidden_dim = hidden_dim
         self.n_process_block_iters = n_process_block_iters
 
-        self.encoder = Encoder(embedding_dim, hidden_dim)
+        self.encoder = Encoder(embed_dim, hidden_dim)
 
         self.process_block = SimpleAttention(
             hidden_dim, use_tanh=use_tanh, C=tanh_exploration
         )
         self.sm = nn.Softmax(dim=1)
         self.decoder = nn.Sequential(
             nn.Linear(hidden_dim, hidden_dim), nn.ReLU(), nn.Linear(hidden_dim, 1)
         )
 
     def forward(self, inputs):
         """
         Args:
-            inputs: [embedding_dim x batch_size x sourceL] of embedded inputs
+            inputs: [embed_dim x batch_size x sourceL] of embedded inputs
         """
         inputs = inputs.transpose(0, 1).contiguous()
 
         encoder_hx = (
             self.encoder.init_hx.unsqueeze(0).repeat(inputs.size(1), 1).unsqueeze(0)
         )
         encoder_cx = (
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/ptrnet/decoder.py` & `rl4co-0.4.0/rl4co/models/zoo/ptrnet/decoder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-from rl4co.models.nn.utils import decode_probs
+from rl4co.utils.decoding import decode_logprobs
 
 
 class SimpleAttention(nn.Module):
     """A generic attention module for a decoder in seq2seq"""
 
     def __init__(self, dim, use_tanh=False, C=10):
         super(SimpleAttention, self).__init__()
@@ -45,56 +45,55 @@
             logits = u
         return e, logits
 
 
 class Decoder(nn.Module):
     def __init__(
         self,
-        embedding_dim: int = 128,
+        embed_dim: int = 128,
         hidden_dim: int = 128,
         tanh_exploration: float = 10.0,
         use_tanh: bool = True,
         num_glimpses=1,
         mask_glimpses=True,
         mask_logits=True,
     ):
         super(Decoder, self).__init__()
 
-        self.embedding_dim = embedding_dim
+        self.embed_dim = embed_dim
         self.hidden_dim = hidden_dim
         self.num_glimpses = num_glimpses
         self.mask_glimpses = mask_glimpses
         self.mask_logits = mask_logits
         self.use_tanh = use_tanh
         self.tanh_exploration = tanh_exploration
 
-        self.lstm = nn.LSTMCell(embedding_dim, hidden_dim)
+        self.lstm = nn.LSTMCell(embed_dim, hidden_dim)
         self.pointer = SimpleAttention(hidden_dim, use_tanh=use_tanh, C=tanh_exploration)
         self.glimpse = SimpleAttention(hidden_dim, use_tanh=False)
 
     def update_mask(self, mask, selected):
-        return mask.clone().scatter_(1, selected.unsqueeze(-1), True)
+        return mask.clone().scatter_(1, selected.unsqueeze(-1), False)
 
     def recurrence(self, x, h_in, prev_mask, prev_idxs, step, context):
         logit_mask = (
             self.update_mask(prev_mask, prev_idxs) if prev_idxs is not None else prev_mask
         )
 
         logits, h_out = self.calc_logits(
             x, h_in, logit_mask, context, self.mask_glimpses, self.mask_logits
         )
 
         # Calculate log_softmax for better numerical stability
         log_p = torch.log_softmax(logits, dim=1)
-        probs = log_p.exp()
 
         if not self.mask_logits:
-            probs[logit_mask] = 0.0
+            log_p[~logit_mask] = float("-inf")
 
-        return h_out, log_p, probs, logit_mask
+        return h_out, log_p, logit_mask
 
     def calc_logits(
         self, x, h_in, logit_mask, context, mask_glimpses=None, mask_logits=None
     ):
         if mask_glimpses is None:
             mask_glimpses = self.mask_glimpses
 
@@ -104,23 +103,23 @@
         hy, cy = self.lstm(x, h_in)
         g_l, h_out = hy, (hy, cy)
 
         for i in range(self.num_glimpses):
             ref, logits = self.glimpse(g_l, context)
             # For the glimpses, only mask before softmax so we have always an L1 norm 1 readout vector
             if mask_glimpses:
-                logits[logit_mask] = float("-inf")
+                logits[~logit_mask] = float("-inf")
             # [batch_size x h_dim x sourceL] * [batch_size x sourceL x 1] =
             # [batch_size x h_dim x 1]
             g_l = torch.bmm(ref, F.softmax(logits, dim=1).unsqueeze(2)).squeeze(2)
         _, logits = self.pointer(g_l, context)
 
         # Masking before softmax makes probs sum to one
         if mask_logits:
-            logits[logit_mask] = float("-inf")
+            logits[~logit_mask] = float("-inf")
 
         return logits, h_out
 
     def forward(
         self,
         decoder_input,
         embedded_inputs,
@@ -128,40 +127,40 @@
         context,
         decode_type="sampling",
         eval_tours=None,
     ):
         """
         Args:
             decoder_input: The initial input to the decoder
-                size is [batch_size x embedding_dim]. Trainable parameter.
-            embedded_inputs: [sourceL x batch_size x embedding_dim]
+                size is [batch_size x embed_dim]. Trainable parameter.
+            embedded_inputs: [sourceL x batch_size x embed_dim]
             hidden: the prev hidden state, size is [batch_size x hidden_dim].
                 Initially this is set to (enc_h[-1], enc_c[-1])
             context: encoder outputs, [sourceL x batch_size x hidden_dim]
         """
 
         batch_size = context.size(1)
         outputs = []
         selections = []
         steps = range(embedded_inputs.size(0))
         idxs = None
-        mask = torch.zeros(
+        mask = torch.ones(
             embedded_inputs.size(1),
             embedded_inputs.size(0),
             dtype=torch.bool,
             device=embedded_inputs.device,
         )
 
         for i in steps:
-            hidden, log_p, probs, mask = self.recurrence(
+            hidden, log_p, mask = self.recurrence(
                 decoder_input, hidden, mask, idxs, i, context
             )
             # select the next inputs for the decoder [batch_size x hidden_dim]
             idxs = (
-                decode_probs(probs, mask, decode_type=decode_type)
+                decode_logprobs(log_p, mask, decode_type=decode_type)
                 if eval_tours is None
                 else eval_tours[:, i]
             )
 
             idxs = (
                 idxs.detach()
             )  # Otherwise pytorch complains it want's a reward, todo implement this more properly?
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/ptrnet/encoder.py` & `rl4co-0.4.0/rl4co/models/zoo/ptrnet/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/models/zoo/ptrnet/model.py` & `rl4co-0.4.0/rl4co/models/zoo/deepaco/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-from typing import Union
+from typing import Optional, Union
 
 from rl4co.envs.common.base import RL4COEnvBase
 from rl4co.models.rl import REINFORCE
 from rl4co.models.rl.reinforce.baselines import REINFORCEBaseline
-from rl4co.models.zoo.ptrnet.policy import PointerNetworkPolicy
+from rl4co.models.zoo.deepaco.policy import DeepACOPolicy
 
 
-class PointerNetwork(REINFORCE):
-    """Pointer Network for neural combinatorial optimization based on REINFORCE
-    Based on Vinyals et al. (2015) https://arxiv.org/abs/1506.03134
-    Refactored from reference implementation: https://github.com/wouterkool/attention-learn-to-route
+class DeepACO(REINFORCE):
+    """Implements DeepACO: https://arxiv.org/abs/2309.14032.
 
     Args:
         env: Environment to use for the algorithm
         policy: Policy to use for the algorithm
-        baseline: REINFORCE baseline. Defaults to rollout (1 epoch of exponential, then greedy rollout baseline)
+        baseline: REINFORCE baseline. Defaults to exponential
         policy_kwargs: Keyword arguments for policy
         baseline_kwargs: Keyword arguments for baseline
         **kwargs: Keyword arguments passed to the superclass
     """
 
     def __init__(
         self,
         env: RL4COEnvBase,
-        policy: PointerNetworkPolicy = None,
-        baseline: Union[REINFORCEBaseline, str] = "rollout",
-        policy_kwargs={},
-        baseline_kwargs={},
+        policy: Optional[DeepACOPolicy] = None,
+        baseline: Union[REINFORCEBaseline, str] = "exponential",
+        policy_kwargs: dict = {},
+        baseline_kwargs: dict = {},
         **kwargs,
     ):
-        self.policy = (
-            PointerNetworkPolicy(self.env, **policy_kwargs) if policy is None else policy
-        )
+        if policy is None:
+            policy = DeepACOPolicy(env_name=env.name, **policy_kwargs)
+
         super().__init__(env, policy, baseline, baseline_kwargs, **kwargs)
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/ptrnet/policy.py` & `rl4co-0.4.0/rl4co/models/zoo/ptrnet/policy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 import math
 
 import torch
 import torch.nn as nn
 
-from rl4co.models.nn.utils import get_log_likelihood
 from rl4co.models.zoo.ptrnet.decoder import Decoder
 from rl4co.models.zoo.ptrnet.encoder import Encoder
+from rl4co.utils.decoding import get_log_likelihood
 from rl4co.utils.pylogger import get_pylogger
 
 log = get_pylogger(__name__)
 
 
 class PointerNetworkPolicy(nn.Module):
     def __init__(
         self,
-        env_name,
-        embedding_dim: int = 128,
+        env_name: str = "tsp",
+        embed_dim: int = 128,
         hidden_dim: int = 128,
         tanh_clipping=10.0,
         mask_inner=True,
         mask_logits=True,
         **kwargs,
     ):
         super(PointerNetworkPolicy, self).__init__()
 
-        # torch.backends.cudnn.enabled=False
-        assert env_name == "tsp", "Only the Euclidean TSP env supported"
+        assert env_name == "tsp", "Only the Euclidean TSP env is implemented"
         self.env_name = env_name
-
         self.input_dim = 2
 
-        self.encoder = Encoder(embedding_dim, hidden_dim)
+        self.encoder = Encoder(embed_dim, hidden_dim)
 
         self.decoder = Decoder(
-            embedding_dim,
+            embed_dim,
             hidden_dim,
             tanh_exploration=tanh_clipping,
             use_tanh=tanh_clipping > 0,
             num_glimpses=1,
             mask_glimpses=mask_inner,
             mask_logits=mask_logits,
         )
 
         # Trainable initial hidden states
-        std = 1.0 / math.sqrt(embedding_dim)
-        self.decoder_in_0 = nn.Parameter(torch.FloatTensor(embedding_dim))
+        std = 1.0 / math.sqrt(embed_dim)
+        self.decoder_in_0 = nn.Parameter(torch.FloatTensor(embed_dim))
         self.decoder_in_0.data.uniform_(-std, std)
 
-        self.embedding = nn.Parameter(torch.FloatTensor(self.input_dim, embedding_dim))
+        self.embedding = nn.Parameter(torch.FloatTensor(self.input_dim, embed_dim))
         self.embedding.data.uniform_(-std, std)
 
     def forward(
         self,
         td,
         env,
         phase: str = "train",
@@ -74,21 +72,21 @@
         embedded_inputs = torch.mm(
             td["locs"].transpose(0, 1).contiguous().view(-1, input_dim),
             self.embedding,
         ).view(graph_size, batch_size, -1)
 
         # query the actor net for the input indices
         # making up the output, and the pointer attn
-        _log_p, actions = self._inner(embedded_inputs, decode_type, eval_tours)
+        _logprobs, actions = self._inner(embedded_inputs, decode_type, eval_tours)
 
         reward = env.get_reward(td, actions)
 
         # Log likelyhood is calculated within the model since returning it per action does not work well with
         # DataParallel since sequences can be of different lengths
-        ll = get_log_likelihood(_log_p, actions, td.get("mask", None))
+        ll = get_log_likelihood(_logprobs, actions, td.get("mask", None))
 
         out = {"reward": reward, "log_likelihood": ll, "actions": actions}
         return out
 
     def _inner(self, inputs, decode_type="sampling", eval_tours=None):
         encoder_hx = encoder_cx = torch.zeros(
             1, *inputs.shape[1:], device=inputs.device
```

### Comparing `rl4co-0.3.3/rl4co/models/zoo/symnco/losses.py` & `rl4co-0.4.0/rl4co/models/zoo/symnco/losses.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/models/zoo/symnco/model.py` & `rl4co-0.4.0/rl4co/models/zoo/symnco/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,46 +22,52 @@
     Based on Kim et al. (2022) https://arxiv.org/abs/2205.13209.
 
     Args:
         env: TorchRL environment to use for the algorithm
         policy: Policy to use for the algorithm
         policy_kwargs: Keyword arguments for policy
         num_augment: Number of augmentations
+        augment_fn: Function to use for augmentation, defaulting to dihedral_8_augmentation
+        feats: List of features to augment
         alpha: weight for invariance loss
         beta: weight for solution symmetricity loss
         num_starts: Number of starts for multi-start. If None, use the number of available actions
         **kwargs: Keyword arguments passed to the superclass
     """
 
     def __init__(
         self,
         env: RL4COEnvBase,
         policy: Union[nn.Module, SymNCOPolicy] = None,
         policy_kwargs: dict = {},
         baseline: str = "symnco",
         num_augment: int = 4,
+        augment_fn: Union[str, callable] = "symmetric",
+        feats: list = None,
         alpha: float = 0.2,
         beta: float = 1,
         num_starts: int = 0,
         **kwargs,
     ):
         self.save_hyperparameters(logger=False)
 
         if policy is None:
-            policy = SymNCOPolicy(env.name, **policy_kwargs)
+            policy = SymNCOPolicy(env_name=env.name, **policy_kwargs)
 
         assert baseline == "symnco", "SymNCO only supports custom-symnco baseline"
         baseline = "no"  # Pass no baseline to superclass since there are multiple custom baselines
 
         # Pass no baseline to superclass since there are multiple custom baselines
         super().__init__(env, policy, baseline, **kwargs)
 
         self.num_starts = num_starts
         self.num_augment = num_augment
-        self.augment = StateAugmentation(self.env.name, num_augment=self.num_augment)
+        self.augment = StateAugmentation(
+            num_augment=self.num_augment, augment_fn=augment_fn, feats=feats
+        )
         self.alpha = alpha  # weight for invariance loss
         self.beta = beta  # weight for solution symmetricity loss
 
         # Add `_multistart` to decode type for train, val and test in policy if num_starts > 1
         if self.num_starts > 1:
             for phase in ["train", "val", "test"]:
                 self.set_decode_type_multistart(phase)
```

### Comparing `rl4co-0.3.3/rl4co/tasks/eval.py` & `rl4co-0.4.0/rl4co/tasks/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,19 +116,19 @@
     Args:
         num_augment (int): Number of state augmentations
         force_dihedral_8 (bool): Whether to force the use of 8 augmentations
     """
 
     name = "augmentation"
 
-    def __init__(self, env, num_augment=8, force_dihedral_8=False, **kwargs):
+    def __init__(self, env, num_augment=8, force_dihedral_8=False, feats=None, **kwargs):
         check_unused_kwargs(self, kwargs)
         super().__init__(env, kwargs.get("progress", True))
         self.augmentation = StateAugmentation(
-            env.name, num_augment=num_augment, use_dihedral_8=force_dihedral_8
+            num_augment=num_augment, augment_fn='dihedral8' if force_dihedral_8 else 'symmetric', feats=feats
         )
 
     def _inner(self, policy, td, num_augment=None):
         if num_augment is None:
             num_augment = self.augmentation.num_augment
         td_init = td.clone()
         td = self.augmentation(td)
@@ -235,26 +235,26 @@
         num_augment: Number of augmentations per sample
         force_dihedral_8: If True, force the use of 8 augmentations (rotations and flips) as in POMO
     """
 
     name = "multistart_greedy_augment"
 
     def __init__(
-        self, env, num_starts=None, num_augment=8, force_dihedral_8=False, **kwargs
+        self, env, num_starts=None, num_augment=8, force_dihedral_8=False, feats=None, **kwargs
     ):
         check_unused_kwargs(self, kwargs)
         super().__init__(env, kwargs.get("progress", True))
 
         assert num_starts is not None, "Must specify num_starts"
         self.num_starts = num_starts
         assert not (
             num_augment != 8 and force_dihedral_8
         ), "Cannot force dihedral 8 when num_augment != 8"
         self.augmentation = StateAugmentation(
-            env.name, num_augment=num_augment, use_dihedral_8=force_dihedral_8
+            num_augment=num_augment, augment_fn='dihedral8' if force_dihedral_8 else 'symmetric', feats=feats
         )
 
     def _inner(self, policy, td, num_augment=None):
         if num_augment is None:
             num_augment = self.augmentation.num_augment
 
         td_init = td.clone()
```

### Comparing `rl4co-0.3.3/rl4co/tasks/train.py` & `rl4co-0.4.0/rl4co/tasks/train.py`

 * *Files 9% similar despite different names*

```diff
@@ -92,15 +92,14 @@
     # merge train and test metrics
     metric_dict = {**train_metrics, **test_metrics}
 
     return metric_dict, object_dict
 
 
 @hydra.main(version_base="1.3", config_path="../../configs", config_name="main.yaml")
-# @hydra.main(version_base="1.3", config_path="configs", config_name="experiment/tsp/am-ppo.yaml")
 def train(cfg: DictConfig) -> Optional[float]:
     # apply extra utilities
     # (e.g. ask for tags if none are provided in cfg, print cfg tree, etc.)
     utils.extras(cfg)
 
     # train the model
     metric_dict, _ = run(cfg)
```

### Comparing `rl4co-0.3.3/rl4co/utils/callbacks/speed_monitor.py` & `rl4co-0.4.0/rl4co/utils/callbacks/speed_monitor.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/utils/instantiators.py` & `rl4co-0.4.0/rl4co/utils/instantiators.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/utils/lightning.py` & `rl4co-0.4.0/rl4co/utils/lightning.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/utils/optim_helpers.py` & `rl4co-0.4.0/rl4co/utils/optim_helpers.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/utils/param_grouping.py` & `rl4co-0.4.0/rl4co/utils/param_grouping.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/utils/pylogger.py` & `rl4co-0.4.0/rl4co/utils/pylogger.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/utils/rich_utils.py` & `rl4co-0.4.0/rl4co/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/utils/test_utils.py` & `rl4co-0.4.0/rl4co/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.3.3/rl4co/utils/trainer.py` & `rl4co-0.4.0/rl4co/utils/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Iterable, List, Optional, Union
 
 import lightning.pytorch as pl
 import torch
+
 from lightning import Callback, Trainer
 from lightning.fabric.accelerators.cuda import num_cuda_devices
 from lightning.pytorch.accelerators import Accelerator
 from lightning.pytorch.core.datamodule import LightningDataModule
 from lightning.pytorch.loggers import Logger
 from lightning.pytorch.strategies import DDPStrategy, Strategy
 from lightning.pytorch.utilities.types import EVAL_DATALOADERS, TRAIN_DATALOADERS
@@ -35,15 +36,15 @@
         gradient_clip_val: 0 means don't clip. Defaults to 1.0 for stability.
         precision: allows for mixed precision training. Can be specified as a string (e.g., '16').
             This also allows to use `FlashAttention` by default.
         disable_profiling_executor: Disable JIT profiling executor. This reduces memory and increases speed.
         auto_configure_ddp: Automatically configure DDP strategy if multiple GPUs are available.
         reload_dataloaders_every_n_epochs: Set to a value different than 1 to reload dataloaders every n epochs.
         matmul_precision: Set matmul precision for faster inference https://pytorch.org/docs/stable/generated/torch.set_float32_matmul_precision.html#torch.set_float32_matmul_precision
-        **kwargs: Additional keyword arguments passed to the Lightning Trainer. See :class:`~lightning.pytorch.trainer.Trainer` for details.
+        **kwargs: Additional keyword arguments passed to the Lightning Trainer. See :class:`lightning.pytorch.trainer.Trainer` for details.
     """
 
     def __init__(
         self,
         accelerator: Union[str, Accelerator] = "auto",
         callbacks: Optional[List[Callback]] = None,
         logger: Optional[Union[Logger, Iterable[Logger]]] = None,
```

### Comparing `rl4co-0.3.3/rl4co/utils/utils.py` & `rl4co-0.4.0/rl4co/utils/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,26 @@
+import importlib
+import platform
+import sys
 import warnings
 
 from importlib.util import find_spec
 from typing import Callable, List
 
 import hydra
 
+from lightning import Callback
 from lightning.pytorch.loggers.logger import Logger
+
+# Import the necessary PyTorch Lightning component
+from lightning.pytorch.trainer.connectors.accelerator_connector import (
+    _AcceleratorConnector,
+)
 from lightning.pytorch.utilities.rank_zero import rank_zero_only
 from omegaconf import DictConfig
-from pytorch_lightning import Callback
 
 from rl4co.utils import pylogger, rich_utils
 
 log = pylogger.get_pylogger(__name__)
 
 
 def task_wrapper(task_func: Callable) -> Callable:
@@ -206,7 +214,74 @@
 
 
 @rank_zero_only
 def save_file(path: str, content: str) -> None:
     """Save file in rank zero mode (only on one process in multi-GPU setup)."""
     with open(path, "w+") as file:
         file.write(content)
+
+
+def merge_with_defaults(_config=None, **defaults) -> dict:
+    """Merge configuration with default values.
+
+    This function merges a provided configuration dictionary with default values.
+    If no configuration is provided (`_config` is None), it returns the default values.
+    If a dictionary is provided, it updates the defaults dictionary with the values from the provided dictionary.
+    Otherwise, it sets all keys in the defaults dictionary to `_config`.
+
+    Args:
+        _config: Configuration to merge. Defaults to None.
+        **defaults: Default values to merge with the configuration.
+
+    Returns:
+        dict: Merged configuration with default values.
+    """
+    if _config is None:
+        return defaults
+    elif isinstance(_config, (DictConfig, dict)):
+        defaults.update(dict(**_config))  # type: ignore
+        return defaults
+    else:
+        return {key: _config for key in defaults.keys()}
+
+
+def show_versions():
+    """
+    This function prints version information that is useful when filing bug
+    reports. Inspired by https://github.com/PyVRP/PyVRP
+    """
+
+    modules = {
+        "rl4co": "rl4co",
+        "torch": "torch",
+        "lightning": "pytorch_lightning",  # Updated module name if necessary
+        "torchrl": "torchrl",
+        "tensordict": "tensordict",
+        "numpy": "numpy",
+        "pytorch_geometric": "torch_geometric",
+        "hydra-core": "hydra",
+        "omegaconf": "omegaconf",
+        "matplotlib": "matplotlib",
+    }
+
+    # Find the longest module name for formatting
+    longest_name = max(len(name) for name in modules.keys())
+
+    print("INSTALLED VERSIONS")
+    print("-" * (longest_name + 20))
+    # modules
+    for name, module in modules.items():
+        try:
+            imported_module = importlib.import_module(module)
+            version = imported_module.__version__
+        except ImportError:
+            version = "Not installed"
+        print(f"{name.rjust(longest_name)} : {version}")
+    # platform information
+    print(f'{"Python".rjust(longest_name)} : {sys.version.split()[0]}')
+    print(f'{"Platform".rjust(longest_name)} : {platform.platform()}')
+    try:
+        lightning_auto_device = _AcceleratorConnector()._choose_auto_accelerator(None)
+    except Exception:
+        lightning_auto_device = _AcceleratorConnector()._choose_auto_accelerator()
+    # lightning hardware accelerators
+    print(f'{"Lightning device".rjust(longest_name)} : {lightning_auto_device}')
```

### Comparing `rl4co-0.3.3/tests/test_envs.py` & `rl4co-0.4.0/tests/test_envs.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 
 from rl4co.envs import (
     ATSPEnv,
     CVRPEnv,
     CVRPTWEnv,
     DPPEnv,
     FFSPEnv,
+    MDCPDPEnv,
     MDPPEnv,
     MTSPEnv,
     OPEnv,
     PCTSPEnv,
     PDPEnv,
     SDVRPEnv,
-    SVRPEnv,
     SMTWTPEnv,
     SPCTSPEnv,
+    SVRPEnv,
     TSPEnv,
 )
-from rl4co.models.nn.utils import random_policy, rollout
+from rl4co.utils.decoding import random_policy, rollout
 
 # Switch to non-GUI backend for testing
 plt.switch_backend("Agg")
 warnings.filterwarnings("ignore", "Matplotlib is currently using agg")
 
 
 @pytest.mark.parametrize(
@@ -38,42 +39,35 @@
         SDVRPEnv,
         PCTSPEnv,
         SPCTSPEnv,
         OPEnv,
         PDPEnv,
         MTSPEnv,
         ATSPEnv,
+        MDCPDPEnv,
     ],
 )
 def test_routing(env_cls, batch_size=2, size=20):
     env = env_cls(num_loc=size)
     reward, td, actions = rollout(env, env.reset(batch_size=[batch_size]), random_policy)
-    env.render(td, actions)
     assert reward.shape == (batch_size,)
 
 
 @pytest.mark.parametrize("env_cls", [DPPEnv, MDPPEnv])
 def test_eda(env_cls, batch_size=2, max_decaps=5):
     env = env_cls(max_decaps=max_decaps)
     reward, td, actions = rollout(env, env.reset(batch_size=[batch_size]), random_policy)
-    ## Note: we skip rendering for now because we need to collect extra data. TODO
-    # env.render(td, actions)
     assert reward.shape == (batch_size,)
 
 
 @pytest.mark.parametrize("env_cls", [FFSPEnv])
 def test_scheduling(env_cls, batch_size=2):
-    env = env_cls(
-        num_stage=2,
-        num_machine=3,
-        num_job=4,
-        batch_size=[batch_size],
-    )
-    td = env.reset()
-    td["job_idx"] = torch.tensor([1, 1])
+    env = env_cls()
+    td = env.reset(batch_size=[batch_size])
+    td["action"] = torch.tensor([1, 1])
     td = env._step(td)
 
 
 @pytest.mark.parametrize("env_cls", [SMTWTPEnv])
 def test_smtwtp(env_cls, batch_size=2):
     env = env_cls(num_job=4)
     reward, td, actions = rollout(env, env.reset(batch_size=[batch_size]), random_policy)
```

### Comparing `rl4co-0.3.3/tests/test_policy.py` & `rl4co-0.4.0/tests/test_policy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import pytest
 
-from rl4co.models import AutoregressivePolicy, PointerNetworkPolicy
-from rl4co.utils.test_utils import generate_env_data
+from rl4co.models import AttentionModelPolicy, PointerNetworkPolicy
 from rl4co.utils.ops import select_start_nodes
+from rl4co.utils.test_utils import generate_env_data
 
 
 # Main autorergressive policy: rollout over multiple envs since it is the base
 @pytest.mark.parametrize(
     "env_name",
     ["tsp", "cvrp", "sdvrp", "mtsp", "op", "pctsp", "spctsp", "dpp", "mdpp", "smtwtp"],
 )
-def test_base_policy(env_name, size=20, batch_size=2):
+def test_am_policy(env_name, size=20, batch_size=2):
     env, x = generate_env_data(env_name, size, batch_size)
     td = env.reset(x)
-    policy = AutoregressivePolicy(env.name)
+    policy = AttentionModelPolicy(env_name=env.name)
     out = policy(td, env, decode_type="greedy")
     assert out["reward"].shape == (batch_size,)
 
 
 @pytest.mark.parametrize(
     "env_name", ["tsp", "cvrp", "pctsp", "spctsp", "sdvrp", "op", "pdp"]
 )
-def test_base_policy_multistart(env_name, size=20, batch_size=2):
+@pytest.mark.parametrize("policy_cls", [AttentionModelPolicy])
+def test_policy_multistart(env_name, policy_cls, size=20, batch_size=2):
     env, x = generate_env_data(env_name, size, batch_size)
     td = env.reset(x)
-    policy = AutoregressivePolicy(env.name)
+    policy = policy_cls(env_name=env.name)
     num_starts = size // 2 if env.name in ["pdp"] else size
     out = policy(
         td,
         env,
         decode_type="multistart_greedy",
         num_starts=num_starts,
         select_start_nodes_fn=select_start_nodes,
@@ -39,18 +40,18 @@
 
 
 @pytest.mark.parametrize(
     "env_name",
     ["tsp", "cvrp", "pctsp", "spctsp", "sdvrp", "op", "pdp"],
 )
 @pytest.mark.parametrize("select_best", [True, False])
-def test_base_policy_beam_search(env_name, select_best, size=20, batch_size=2):
+def test_beam_search(env_name, select_best, size=20, batch_size=2):
     env, x = generate_env_data(env_name, size, batch_size)
     td = env.reset(x)
-    policy = AutoregressivePolicy(env.name)
+    policy = AttentionModelPolicy(env_name=env.name)
     beam_width = size // 2 if env.name in ["pdp"] else size
     out = policy(
         td, env, decode_type="beam_search", beam_width=beam_width, select_best=select_best
     )
 
     if select_best:
         expected_shape = (batch_size,)
@@ -58,10 +59,10 @@
         expected_shape = (batch_size * beam_width,)
     assert out["reward"].shape == expected_shape
 
 
 def test_pointer_network(size=20, batch_size=2):
     env, x = generate_env_data("tsp", size, batch_size)
     td = env.reset(x)
-    policy = PointerNetworkPolicy(env.name)
+    policy = PointerNetworkPolicy(env_name=env.name)
     out = policy(td, env, decode_type="greedy")
     assert out["reward"].shape == (batch_size,)
```

### Comparing `rl4co-0.3.3/tests/test_utils.py` & `rl4co-0.4.0/tests/test_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 import torch
 
 from tensordict import TensorDict
 
+from rl4co.utils.decoding import process_logits
 from rl4co.utils.ops import batchify, unbatchify
 
 
 @pytest.mark.parametrize(
     "a",
     [
         torch.randn(10, 20, 2),
@@ -21,7 +22,16 @@
     # unbatchify: [b * prod(shape), ...] -> [b, shape[0], shape[1], ...]
     a_batch = batchify(a, shape)
     a_unbatch = unbatchify(a_batch, shape)
     if isinstance(a, TensorDict):
         a, a_unbatch = a["a"], a_unbatch["a"]
     index = (slice(None),) + (0,) * len(shape)  # (slice(None), 0, 0, ..., 0)
     assert torch.allclose(a, a_unbatch[index])
+
+
+@pytest.mark.parametrize("top_p", [0.0, 0.5, 1.0])
+@pytest.mark.parametrize("top_k", [0, 5, 10])
+def test_top_k_top_p_sampling(top_p, top_k):
+    logits = torch.randn(8, 10)
+    mask = torch.ones(8, 10).bool()
+    logprobs = process_logits(logits, mask, top_p=top_p, top_k=top_k)
+    assert len(logprobs) == logits.size(0)
```

