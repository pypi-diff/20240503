# Comparing `tmp/telliot_core-0.3.4.tar.gz` & `tmp/telliot_core-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telliot_core-0.3.4.tar", last modified: Wed Apr 17 15:39:13 2024, max compression
+gzip compressed data, was "telliot_core-0.3.5.tar", last modified: Fri May  3 16:24:31 2024, max compression
```

## Comparing `telliot_core-0.3.4.tar` & `telliot_core-0.3.5.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.546697 telliot_core-0.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.522698 telliot_core-0.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.526698 telliot_core-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-17 15:39:08.000000 telliot_core-0.3.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-17 15:39:08.000000 telliot_core-0.3.4/.github/workflows/py39.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-17 15:39:08.000000 telliot_core-0.3.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-17 15:39:08.000000 telliot_core-0.3.4/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-17 15:39:08.000000 telliot_core-0.3.4/.github/workflows/typing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-17 15:39:08.000000 telliot_core-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-17 15:39:08.000000 telliot_core-0.3.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-17 15:39:08.000000 telliot_core-0.3.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-17 15:39:08.000000 telliot_core-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-17 15:39:13.546697 telliot_core-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-17 15:39:08.000000 telliot_core-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 15:39:08.000000 telliot_core-0.3.4/brownie-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.526698 telliot_core-0.3.4/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.526698 telliot_core-0.3.4/contracts/Integrations/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-17 15:39:08.000000 telliot_core-0.3.4/contracts/Integrations/DIVAOracleMock.sol
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-17 15:39:08.000000 telliot_core-0.3.4/contracts/Integrations/DIVAProtocolMock.sol
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-17 15:39:08.000000 telliot_core-0.3.4/contracts/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.530698 telliot_core-0.3.4/contracts/TellorFlex/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-17 15:39:08.000000 telliot_core-0.3.4/contracts/TellorFlex/AutopayMock.sol
--rw-r--r--   0 runner    (1001) docker     (127)    20244 2024-04-17 15:39:08.000000 telliot_core-0.3.4/contracts/TellorFlex/TellorFlex.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.530698 telliot_core-0.3.4/contracts/TellorFlex/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-17 15:39:08.000000 telliot_core-0.3.4/contracts/TellorFlex/testing/StakingToken.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.530698 telliot_core-0.3.4/contracts/TellorX/
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-17 15:39:08.000000 telliot_core-0.3.4/contracts/TellorX/TellorXMasterMock.sol
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-17 15:39:08.000000 telliot_core-0.3.4/contracts/TellorX/TellorXOracleMock.sol
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.530698 telliot_core-0.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-17 15:39:08.000000 telliot_core-0.3.4/docs/add-chain.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.530698 telliot_core-0.3.4/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-17 15:39:08.000000 telliot_core-0.3.4/docs/assets/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)   160315 2024-04-17 15:39:08.000000 telliot_core-0.3.4/docs/assets/tellor_swoosh.png
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-17 15:39:08.000000 telliot_core-0.3.4/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-17 15:39:08.000000 telliot_core-0.3.4/docs/documentation.md
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-17 15:39:08.000000 telliot_core-0.3.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.530698 telliot_core-0.3.4/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-17 15:39:08.000000 telliot_core-0.3.4/interfaces/IERC20.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-17 15:39:08.000000 telliot_core-0.3.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-17 15:39:08.000000 telliot_core-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-17 15:39:08.000000 telliot_core-0.3.4/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.530698 telliot_core-0.3.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-17 15:39:08.000000 telliot_core-0.3.4/scripts/morphware_data_sizes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-04-17 15:39:08.000000 telliot_core-0.3.4/scripts/query_catalog.md
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-17 15:39:08.000000 telliot_core-0.3.4/scripts/query_catalog.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-17 15:39:13.550698 telliot_core-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:39:08.000000 telliot_core-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.522698 telliot_core-0.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.530698 telliot_core-0.3.4/src/telliot_core/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.534698 telliot_core-0.3.4/src/telliot_core/apps/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/apps/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/apps/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/apps/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/apps/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/apps/telliot_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/asset_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.534698 telliot_core-0.3.4/src/telliot_core/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.534698 telliot_core-0.3.4/src/telliot_core/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/cli/commands/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/cli/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/cli/commands/listen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/cli/commands/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.534698 telliot_core-0.3.4/src/telliot_core/contract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/contract/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/contract/listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.534698 telliot_core-0.3.4/src/telliot_core/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.538698 telliot_core-0.3.4/src/telliot_core/data/abi/
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/diva-oracle-tellor-abi.json
--rw-r--r--   0 runner    (1001) docker     (127)    28088 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/diva-protocol-abi.json
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/fuse-token-abi.json
--rw-r--r--   0 runner    (1001) docker     (127)    20737 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/tellor-governance-abi.json
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/tellor-mesosphere-abi.json
--rw-r--r--   0 runner    (1001) docker     (127)    35232 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/tellor360-autopay-abi.json
--rw-r--r--   0 runner    (1001) docker     (127)    26675 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/tellor360-oracle-abi.json
--rw-r--r--   0 runner    (1001) docker     (127)    21821 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/tellor360-playground.json
--rw-r--r--   0 runner    (1001) docker     (127)    21041 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/tellorflex-autopay-abi.json
--rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/tellorflex-oracle-abi.json
--rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/tellorx-governance-abi.json
--rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/tellorx-lens-abi.json
--rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/tellorx-master-abi.json
--rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/tellorx-oracle-abi.json
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/tellorx-treasury-abi.json
--rw-r--r--   0 runner    (1001) docker     (127)    13989 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/abi/trb-token-abi.json
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/assets.json
--rw-r--r--   0 runner    (1001) docker     (127)    15287 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/data/contract_directory.json
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.538698 telliot_core-0.3.4/src/telliot_core/gas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/gas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/gas/legacy_gas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.542698 telliot_core-0.3.4/src/telliot_core/model/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/model/api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/model/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8524 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/model/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)    11660 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/model/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/model/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/model/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.542698 telliot_core-0.3.4/src/telliot_core/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/reporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.542698 telliot_core-0.3.4/src/telliot_core/tellor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/tellor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.542698 telliot_core-0.3.4/src/telliot_core/tellor/tellor360/
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/tellor/tellor360/autopay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/tellor/tellor360/oracle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.542698 telliot_core-0.3.4/src/telliot_core/tellor/tellorflex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/tellor/tellorflex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/tellor/tellorflex/autopay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/tellor/tellorflex/oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/tellor/tellorflex/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.542698 telliot_core-0.3.4/src/telliot_core/tellor/tellorx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/tellor/tellorx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/tellor/tellorx/master.py
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/tellor/tellorx/oracle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.542698 telliot_core-0.3.4/src/telliot_core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/utils/home.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/utils/key_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/utils/pyutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/utils/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/utils/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-17 15:39:08.000000 telliot_core-0.3.4/src/telliot_core/utils/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.546697 telliot_core-0.3.4/src/telliot_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-17 15:39:13.000000 telliot_core-0.3.4/src/telliot_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-17 15:39:13.000000 telliot_core-0.3.4/src/telliot_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:39:13.000000 telliot_core-0.3.4/src/telliot_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-17 15:39:13.000000 telliot_core-0.3.4/src/telliot_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 15:39:13.000000 telliot_core-0.3.4/src/telliot_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 15:39:13.000000 telliot_core-0.3.4/src/telliot_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:39:13.546697 telliot_core-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_app_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_asset_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_autopay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_gas.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_master_read.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_model_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_oracle_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_rpc_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_telliot_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_tellorflex.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tests/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-17 15:39:08.000000 telliot_core-0.3.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.786684 telliot_core-0.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.758684 telliot_core-0.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.766684 telliot_core-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-03 16:24:27.000000 telliot_core-0.3.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-03 16:24:27.000000 telliot_core-0.3.5/.github/workflows/py39.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-03 16:24:27.000000 telliot_core-0.3.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-03 16:24:27.000000 telliot_core-0.3.5/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-03 16:24:27.000000 telliot_core-0.3.5/.github/workflows/typing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-03 16:24:27.000000 telliot_core-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-03 16:24:27.000000 telliot_core-0.3.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-03 16:24:27.000000 telliot_core-0.3.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-03 16:24:27.000000 telliot_core-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-03 16:24:31.786684 telliot_core-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-03 16:24:27.000000 telliot_core-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-03 16:24:27.000000 telliot_core-0.3.5/brownie-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.766684 telliot_core-0.3.5/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.766684 telliot_core-0.3.5/contracts/Integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-03 16:24:27.000000 telliot_core-0.3.5/contracts/Integrations/DIVAOracleMock.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-03 16:24:27.000000 telliot_core-0.3.5/contracts/Integrations/DIVAProtocolMock.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-03 16:24:27.000000 telliot_core-0.3.5/contracts/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.766684 telliot_core-0.3.5/contracts/TellorFlex/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-03 16:24:27.000000 telliot_core-0.3.5/contracts/TellorFlex/AutopayMock.sol
+-rw-r--r--   0 runner    (1001) docker     (127)    20244 2024-05-03 16:24:27.000000 telliot_core-0.3.5/contracts/TellorFlex/TellorFlex.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.766684 telliot_core-0.3.5/contracts/TellorFlex/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-03 16:24:27.000000 telliot_core-0.3.5/contracts/TellorFlex/testing/StakingToken.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.766684 telliot_core-0.3.5/contracts/TellorX/
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-03 16:24:27.000000 telliot_core-0.3.5/contracts/TellorX/TellorXMasterMock.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-03 16:24:27.000000 telliot_core-0.3.5/contracts/TellorX/TellorXOracleMock.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.766684 telliot_core-0.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-03 16:24:27.000000 telliot_core-0.3.5/docs/add-chain.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.766684 telliot_core-0.3.5/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-03 16:24:27.000000 telliot_core-0.3.5/docs/assets/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)   160315 2024-05-03 16:24:27.000000 telliot_core-0.3.5/docs/assets/tellor_swoosh.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-03 16:24:27.000000 telliot_core-0.3.5/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-03 16:24:27.000000 telliot_core-0.3.5/docs/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-03 16:24:27.000000 telliot_core-0.3.5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.766684 telliot_core-0.3.5/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-03 16:24:27.000000 telliot_core-0.3.5/interfaces/IERC20.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-03 16:24:27.000000 telliot_core-0.3.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-03 16:24:27.000000 telliot_core-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-03 16:24:27.000000 telliot_core-0.3.5/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.766684 telliot_core-0.3.5/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-03 16:24:27.000000 telliot_core-0.3.5/scripts/morphware_data_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7909 2024-05-03 16:24:27.000000 telliot_core-0.3.5/scripts/query_catalog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-03 16:24:27.000000 telliot_core-0.3.5/scripts/query_catalog.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-03 16:24:31.786684 telliot_core-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:24:27.000000 telliot_core-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.762684 telliot_core-0.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.770684 telliot_core-0.3.5/src/telliot_core/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.770684 telliot_core-0.3.5/src/telliot_core/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/apps/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/apps/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/apps/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/apps/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/apps/telliot_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/asset_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.770684 telliot_core-0.3.5/src/telliot_core/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.770684 telliot_core-0.3.5/src/telliot_core/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/cli/commands/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/cli/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/cli/commands/listen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/cli/commands/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.774684 telliot_core-0.3.5/src/telliot_core/contract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/contract/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/contract/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.774684 telliot_core-0.3.5/src/telliot_core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.774684 telliot_core-0.3.5/src/telliot_core/data/abi/
+-rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/diva-oracle-tellor-abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28088 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/diva-protocol-abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/fuse-token-abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20737 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/tellor-governance-abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/tellor-mesosphere-abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35232 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/tellor360-autopay-abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26675 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/tellor360-oracle-abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21821 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/tellor360-playground.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21041 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/tellorflex-autopay-abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/tellorflex-oracle-abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11824 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/tellorx-governance-abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/tellorx-lens-abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23746 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/tellorx-master-abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/tellorx-oracle-abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/tellorx-treasury-abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13989 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/abi/trb-token-abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/assets.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17123 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/data/contract_directory.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.778684 telliot_core-0.3.5/src/telliot_core/gas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/gas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/gas/legacy_gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.778684 telliot_core-0.3.5/src/telliot_core/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/model/api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/model/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/model/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13018 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/model/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/model/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/model/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.778684 telliot_core-0.3.5/src/telliot_core/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/reporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.778684 telliot_core-0.3.5/src/telliot_core/tellor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/tellor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.778684 telliot_core-0.3.5/src/telliot_core/tellor/tellor360/
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/tellor/tellor360/autopay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/tellor/tellor360/oracle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.778684 telliot_core-0.3.5/src/telliot_core/tellor/tellorflex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/tellor/tellorflex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/tellor/tellorflex/autopay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/tellor/tellorflex/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/tellor/tellorflex/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.778684 telliot_core-0.3.5/src/telliot_core/tellor/tellorx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/tellor/tellorx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/tellor/tellorx/master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/tellor/tellorx/oracle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.782684 telliot_core-0.3.5/src/telliot_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/utils/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/utils/key_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/utils/pyutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/utils/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/utils/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-03 16:24:27.000000 telliot_core-0.3.5/src/telliot_core/utils/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.782684 telliot_core-0.3.5/src/telliot_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-03 16:24:31.000000 telliot_core-0.3.5/src/telliot_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-05-03 16:24:31.000000 telliot_core-0.3.5/src/telliot_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:24:31.000000 telliot_core-0.3.5/src/telliot_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 16:24:31.000000 telliot_core-0.3.5/src/telliot_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-03 16:24:31.000000 telliot_core-0.3.5/src/telliot_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 16:24:31.000000 telliot_core-0.3.5/src/telliot_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:24:31.782684 telliot_core-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_app_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_asset_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_autopay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_master_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_model_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_oracle_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_rpc_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_telliot_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_tellorflex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tests/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-03 16:24:27.000000 telliot_core-0.3.5/tox.ini
```

### Comparing `telliot_core-0.3.4/.github/workflows/docs.yml` & `telliot_core-0.3.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/.github/workflows/py39.yml` & `telliot_core-0.3.5/.github/workflows/py39.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/.github/workflows/release.yml` & `telliot_core-0.3.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/.github/workflows/style.yml` & `telliot_core-0.3.5/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/.github/workflows/typing.yml` & `telliot_core-0.3.5/.github/workflows/typing.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/.gitignore` & `telliot_core-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/.pre-commit-config.yaml` & `telliot_core-0.3.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/.readthedocs.yaml` & `telliot_core-0.3.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/LICENSE` & `telliot_core-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/PKG-INFO` & `telliot_core-0.3.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telliot_core
-Version: 0.3.4
+Version: 0.3.5
 Summary: Telliot is a Python framework for interacting with the decentralized TellorX network.
 Home-page: https://github.com/tellor-io/telliot-core
 Author: Tellor Development Community
 Author-email: info@tellor.io
 License: MIT
 Keywords: oracle,etherium,blockchain
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `telliot_core-0.3.4/README.md` & `telliot_core-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/contracts/Integrations/DIVAProtocolMock.sol` & `telliot_core-0.3.5/contracts/Integrations/DIVAProtocolMock.sol`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/contracts/TellorFlex/TellorFlex.sol` & `telliot_core-0.3.5/contracts/TellorFlex/TellorFlex.sol`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/contracts/TellorX/TellorXMasterMock.sol` & `telliot_core-0.3.5/contracts/TellorX/TellorXMasterMock.sol`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/contracts/TellorX/TellorXOracleMock.sol` & `telliot_core-0.3.5/contracts/TellorX/TellorXOracleMock.sol`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/docs/add-chain.md` & `telliot_core-0.3.5/docs/add-chain.md`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/docs/assets/favicon-32x32.png` & `telliot_core-0.3.5/docs/assets/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/docs/assets/tellor_swoosh.png` & `telliot_core-0.3.5/docs/assets/tellor_swoosh.png`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/docs/contributing.md` & `telliot_core-0.3.5/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/docs/documentation.md` & `telliot_core-0.3.5/docs/documentation.md`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/mkdocs.yml` & `telliot_core-0.3.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/scripts/morphware_data_sizes.py` & `telliot_core-0.3.5/scripts/morphware_data_sizes.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/scripts/query_catalog.md` & `telliot_core-0.3.5/scripts/query_catalog.md`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/scripts/query_catalog.yaml` & `telliot_core-0.3.5/scripts/query_catalog.yaml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/setup.cfg` & `telliot_core-0.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/apps/app.py` & `telliot_core-0.3.5/src/telliot_core/apps/app.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/apps/config.py` & `telliot_core-0.3.5/src/telliot_core/apps/config.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/apps/core.py` & `telliot_core-0.3.5/src/telliot_core/apps/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,20 @@
     252: "Fraxtal Mainnet",
     1998: "Kyoto Testnet",
     1444673419: "Skale Europa Testnet",
     2046399126: "Skale Europa Mainnet",
     59141: "Linea Sepolia",
     324: "zkSync Era Mainnet",
     300: "zkSync Era Sepolia Testnet",
+    80002: "polygon-amoy",
+    11155420: "optimism-sepolia",
+    421614: "arbitrum-sepolia",
+    5003: "mantle-sepolia",
+    84532: "Base Sepolia",
+    111: "puff-bob-jznbxtoq7h",
 }
 
 LOGLEVEL_MAP = {
     "CRITICAL": logging.CRITICAL,
     "ERROR": logging.ERROR,
     "WARNING": logging.WARNING,
     "INFO": logging.INFO,
```

### Comparing `telliot_core-0.3.4/src/telliot_core/apps/session_manager.py` & `telliot_core-0.3.5/src/telliot_core/apps/session_manager.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/apps/telliot_config.py` & `telliot_core-0.3.5/src/telliot_core/apps/telliot_config.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/asset_registry.py` & `telliot_core-0.3.5/src/telliot_core/asset_registry.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/cli/commands/account.py` & `telliot_core-0.3.5/src/telliot_core/cli/commands/account.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/cli/commands/config.py` & `telliot_core-0.3.5/src/telliot_core/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/cli/commands/listen.py` & `telliot_core-0.3.5/src/telliot_core/cli/commands/listen.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/cli/commands/read.py` & `telliot_core-0.3.5/src/telliot_core/cli/commands/read.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/cli/main.py` & `telliot_core-0.3.5/src/telliot_core/cli/main.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/cli/utils.py` & `telliot_core-0.3.5/src/telliot_core/cli/utils.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/contract/contract.py` & `telliot_core-0.3.5/src/telliot_core/contract/contract.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/contract/listener.py` & `telliot_core-0.3.5/src/telliot_core/contract/listener.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/diva-oracle-tellor-abi.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/diva-oracle-tellor-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/diva-protocol-abi.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/diva-protocol-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/fuse-token-abi.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/fuse-token-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/tellor-governance-abi.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/tellor-governance-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/tellor-mesosphere-abi.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/tellor-mesosphere-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/tellor360-autopay-abi.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/tellor360-autopay-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/tellor360-oracle-abi.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/tellor360-oracle-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/tellor360-playground.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/tellor360-playground.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/tellorflex-autopay-abi.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/tellorflex-autopay-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/tellorflex-oracle-abi.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/tellorflex-oracle-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/tellorx-governance-abi.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/tellorx-governance-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/tellorx-lens-abi.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/tellorx-lens-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/tellorx-master-abi.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/tellorx-master-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/tellorx-oracle-abi.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/tellorx-oracle-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/tellorx-treasury-abi.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/tellorx-treasury-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/abi/trb-token-abi.json` & `telliot_core-0.3.5/src/telliot_core/data/abi/trb-token-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/assets.json` & `telliot_core-0.3.5/src/telliot_core/data/assets.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/data/contract_directory.json` & `telliot_core-0.3.5/src/telliot_core/data/contract_directory.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9941951746314629%*

 * *Differences: {'12': "{'address': {'1998': '0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc', '1444673419': "*

 * *       "'0x16d623f2f3AB1d58426f0402c313f1d3fdA14249', '59141': "*

 * *       "'0x34Fae97547E990ef0E05e05286c51E4645bf1A85 ', '80002': "*

 * *       "'0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81', '11155420': "*

 * *       "'0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc', '421614': "*

 * *       "'0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81', '5003': "*

 * *       "'0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc', '84532': "*

 * *       "'0x896419Ed2E0dC848 […]*

```diff
@@ -103,18 +103,20 @@
         "abi_file": "tellor360-oracle-abi.json",
         "address": {
             "1": "0x8cFc184c877154a8F9ffE0fe75649dbe5e2DBEbf",
             "10": "0x8cFc184c877154a8F9ffE0fe75649dbe5e2DBEbf",
             "100": "0x8cFc184c877154a8F9ffE0fe75649dbe5e2DBEbf",
             "10200": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "1101": "0x34Fae97547E990ef0E05e05286c51E4645bf1A85",
+            "111": "0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81",
             "11155111": "0xB19584Be015c04cf6CFBF6370Fe94a58b7A38830",
+            "11155420": "0x9EA18BFDB50E9bb4A18F9d3Df7804E398F8fE0dc",
             "137": "0x8cFc184c877154a8F9ffE0fe75649dbe5e2DBEbf",
-            "1444673419": "0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81",
-            "1998": "0xB3bB03eA894C609C8560Af3d8726556f52140a39",
+            "1444673419": "0x004B2b43AE9Eb84FE1A6d56229d4b7D12eED50dF",
+            "1998": "0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81",
             "2046399126": "0x004B2b43AE9Eb84FE1A6d56229d4b7D12eED50dF",
             "2442": "0x9EA18BFDB50E9bb4A18F9d3Df7804E398F8fE0dc",
             "252": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
             "2522": "0x6684E5DdbEe1b97E10847468cB5f4e38f3aB83FE",
             "300": "0xf46725B1aD707D6B7D5add3889C97856888a17D7",
             "314": "0x8cFc184c877154a8F9ffE0fe75649dbe5e2DBEbf",
             "3141": "0xb2CB696fE5244fB9004877e58dcB680cB86Ba444",
@@ -122,40 +124,46 @@
             "324": "0x61e3BE234D7EE7b1e2a1fA84027105c733b91545",
             "3441005": "0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81",
             "369": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "4": "0xDb7923FA7D8959A5aDCAA2B652508420f9E47541",
             "420": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "42161": "0x8cFc184c877154a8F9ffE0fe75649dbe5e2DBEbf",
             "421613": "0xb2CB696fE5244fB9004877e58dcB680cB86Ba444",
+            "421614": "0x6684E5DdbEe1b97E10847468cB5f4e38f3aB83FE",
             "5": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "5000": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "5001": "0xf9C672525284C76b9a7e83BE94849Af47624a2dd",
+            "5003": "0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81",
             "59140": "0x6684E5DdbEe1b97E10847468cB5f4e38f3aB83FE",
-            "59141": "0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81",
+            "59141": "0xC7199e0686DF9844B511fAf2796C518F6D7292EB",
             "59144": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
             "80001": "0xB0ff935b775a70504b810cf97c39987058e18550",
+            "80002": "0xe331Afe3a8D7836bEdF1F09bC91549f4bc8c60C9",
             "84531": "0x16d623f2f3AB1d58426f0402c313f1d3fdA14249",
+            "84532": "0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81",
             "943": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0"
         },
         "name": "tellor360-oracle",
         "org": "tellor",
         "type": "ContractInfo"
     },
     {
         "abi_file": "tellor360-autopay-abi.json",
         "address": {
             "1": "0x3b50dEc3CA3d34d5346228D86D29CF679EAA0Ccb",
             "10": "0x3b50dEc3CA3d34d5346228D86D29CF679EAA0Ccb",
             "100": "0x3b50dEc3CA3d34d5346228D86D29CF679EAA0Ccb",
             "10200": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "1101": "0x6684E5DdbEe1b97E10847468cB5f4e38f3aB83FE",
+            "111": "0x89e44099f5E80484dcF48995080481214b9c2D7c",
             "11155111": "0xB59a8085b4C360a3694396CA8E09441052656cF6",
+            "11155420": "0x5446397292854D92872eDf426eEaB8FdC6Bd2bEa",
             "137": "0x11cA06aa780ce89dbBF5D8F5fA8bf6965Be942c9",
-            "1444673419": "0x89e44099f5E80484dcF48995080481214b9c2D7c",
-            "1998": "0xcdf24BD1f51c7F1DA63F20877a284A19B4eAfde0",
+            "1444673419": "0x6CCB007bCdbCa8234e0D1A39a84453bFF79f95E2",
+            "1998": "0x89e44099f5E80484dcF48995080481214b9c2D7c",
             "2046399126": "0x6CCB007bCdbCa8234e0D1A39a84453bFF79f95E2",
             "2442": "0x5446397292854D92872eDf426eEaB8FdC6Bd2bEa",
             "252": "0x9EA18BFDB50E9bb4A18F9d3Df7804E398F8fE0dc",
             "2522": "0xe331Afe3a8D7836bEdF1F09bC91549f4bc8c60C9",
             "300": "0x40099d1fB3C8727aE6C25Bc9e209A3789e7d81A9",
             "314": "0x3b50dEc3CA3d34d5346228D86D29CF679EAA0Ccb",
             "3141": "0x60cBf3991F05a0671250e673Aa166e9D1A0C662E",
@@ -163,42 +171,48 @@
             "324": "0x13442df2611Ba2BE59116F0c8407dcdf3adaB0cA",
             "3441005": "0x89e44099f5E80484dcF48995080481214b9c2D7c",
             "369": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "4": "0xb4a418153039eECcaEE2d74D57766BF943aA8d53",
             "420": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "42161": "0x3b50dEc3CA3d34d5346228D86D29CF679EAA0Ccb",
             "421613": "0x60cBf3991F05a0671250e673Aa166e9D1A0C662E",
+            "421614": "0xe331Afe3a8D7836bEdF1F09bC91549f4bc8c60C9",
             "5": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "5000": "0x6C77f2c171C8cEe08F7A5645c34BB14A29b8532f",
             "5001": "0x10c9042C4BBD61E98bB2b3dfb90d127Be4328Aab",
+            "5003": "0x89e44099f5E80484dcF48995080481214b9c2D7c",
             "59140": "0xe331Afe3a8D7836bEdF1F09bC91549f4bc8c60C9",
-            "59141": "0x6CCB007bCdbCa8234e0D1A39a84453bFF79f95E2",
+            "59141": "0x02FB285409Cec68EE12183cc3035a090A456f66C",
             "59144": "0x9EA18BFDB50E9bb4A18F9d3Df7804E398F8fE0dc",
             "80001": "0xBfe8B0b5dBB521bdD1CF8E09432B41eD5328619a",
+            "80002": "0x004B2b43AE9Eb84FE1A6d56229d4b7D12eED50dF",
             "84531": "0xCEBae6f5398853e7cd1E68301dA77C4B95Ae197a",
+            "84532": "0x89e44099f5E80484dcF48995080481214b9c2D7c",
             "943": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0"
         },
         "name": "tellor360-autopay",
         "org": "tellor",
         "type": "ContractInfo"
     },
     {
         "abi_file": "trb-token-abi.json",
         "address": {
             "1": "0x88dF592F8eb5D7Bd38bFeF7dEb0fBc02cf3778a0",
             "10": "0xaf8cA653Fa2772d58f4368B0a71980e9E3cEB888",
             "100": "0xAAd66432d27737ecf6ED183160Adc5eF36aB99f2",
             "10200": "0xe7147C5Ed14F545B4B17251992D1DB2bdfa26B6d",
             "1101": "0x03346b2F4BC23fd7f4935f74E70c7a7FebC45313",
+            "111": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
             "11155111": "0x80fc34a2f9FfE86F41580F47368289C402DEc660",
+            "11155420": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
             "137": "0xE3322702BEdaaEd36CdDAb233360B939775ae5f1",
-            "1444673419": "0x34fae97547e990ef0e05e05286c51e4645bf1a85",
+            "1444673419": "0x92732c3E59aF2ea6Aa2E886DA5959Fe952Ce2D24",
             "1666600000": "0xd4b28ecb7b765C89F1e67dE3359d09A3520f794E",
             "1666700000": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
-            "1998": "0xCEBae6f5398853e7cd1E68301dA77C4B95Ae197a",
+            "1998": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
             "2046399126": "0x92732c3E59aF2ea6Aa2E886DA5959Fe952Ce2D24",
             "2442": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
             "252": "0xf4Fee0A3aa10abD90b2E03Cf9aB4C221d8348157",
             "2522": "0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81",
             "3": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
             "300": "0x61e3BE234D7EE7b1e2a1fA84027105c733b91545",
             "314": "0x045CE60839d108B43dF9e703d4b25402a6a28a0d",
@@ -208,23 +222,27 @@
             "3441005": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
             "369": "0x88dF592F8eb5D7Bd38bFeF7dEb0fBc02cf3778a0",
             "4": "0x88dF592F8eb5D7Bd38bFeF7dEb0fBc02cf3778a0",
             "420": "0xd71F72C18767083e4e3FE84F9c62b8038C1Ef4f6",
             "42161": "0xd58D345Fd9c82262E087d2D0607624B410D88242",
             "421611": "0x126f5C4802c10848Eb66ce2F74380B7ADeFF36Cb",
             "421613": "0x8d1bB5eDdFce08B92dD47c9871d1805211C3Eb3C",
+            "421614": "0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81",
             "5": "0x51c59c6cAd28ce3693977F2feB4CfAebec30d8a2",
             "5000": "0x35D48A789904E9b15705977192e5d95e2aF7f1D3",
             "5001": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
+            "5003": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
             "59140": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
             "59141": "0x34Fae97547E990ef0E05e05286c51E4645bf1A85",
             "59144": "0x35482B93941B439dEA2244Cc30A20D1Ed862DF86",
             "69": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
             "80001": "0x3251838bd813fdf6a97D32781e011cce8D225d59",
+            "80002": "0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81",
             "84531": "0x34Fae97547E990ef0E05e05286c51E4645bf1A85",
+            "84532": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
             "943": "0x88dF592F8eb5D7Bd38bFeF7dEb0fBc02cf3778a0"
         },
         "name": "trb-token",
         "org": "tellor",
         "type": "ContractInfo"
     },
     {
@@ -244,32 +262,38 @@
         "name": "tellor-mesosphere",
         "org": "tellor",
         "type": "ContractInfo"
     },
     {
         "address": {
             "10200": "0xe7147C5Ed14F545B4B17251992D1DB2bdfa26B6d",
-            "1444673419": "0x34fae97547e990ef0e05e05286c51e4645bf1a85",
+            "111": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
+            "11155420": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
+            "1444673419": "0x16d623f2f3AB1d58426f0402c313f1d3fdA14249",
             "1666700000": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
-            "1998": "0xCEBae6f5398853e7cd1E68301dA77C4B95Ae197a",
+            "1998": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
             "2442": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
             "2522": "0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81",
             "3": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
             "300": "0x61e3BE234D7EE7b1e2a1fA84027105c733b91545",
             "3441005": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
             "4": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
             "42": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
             "421611": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
+            "421614": "0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81",
             "5": "0x3251838bd813fdf6a97D32781e011cce8D225d59",
             "5001": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
+            "5003": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
             "59140": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
-            "59141": "0x34Fae97547E990ef0E05e05286c51E4645bf1A85",
+            "59141": "0x34Fae97547E990ef0E05e05286c51E4645bf1A85 ",
             "69": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
             "80001": "0x3251838bd813fdf6a97D32781e011cce8D225d59",
-            "84531": "0x34Fae97547E990ef0E05e05286c51E4645bf1A85"
+            "80002": "0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81",
+            "84531": "0x34Fae97547E990ef0E05e05286c51E4645bf1A85",
+            "84532": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc"
         },
         "name": "tellor-playground",
         "org": "tellor",
         "type": "ContractInfo"
     },
     {
         "address": {
@@ -320,40 +344,46 @@
         "abi_file": "tellor-governance-abi.json",
         "address": {
             "1": "0xB30b1B98d8276b80bC4f5aF9f9170ef3220EC27D",
             "10": "0xB30b1B98d8276b80bC4f5aF9f9170ef3220EC27D",
             "100": "0xB30b1B98d8276b80bC4f5aF9f9170ef3220EC27D",
             "10200": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "1101": "0x896419Ed2E0dC848a1f7d2814F4e5Df4b9B9bFcc",
+            "111": "0x6684E5DdbEe1b97E10847468cB5f4e38f3aB83FE",
             "11155111": "0xA192f62726ea27979146dfF94f886a8E4Eb6D7A5",
+            "11155420": "0x89e44099f5E80484dcF48995080481214b9c2D7c",
             "137": "0x4e9b7b5b49F7e72871526304d7ecb05D4836d67e",
             "1444673419": "0x6684E5DdbEe1b97E10847468cB5f4e38f3aB83FE",
-            "1998": "0x788070Db2084DeDFBD344Da4B14EABA44D83fd2e",
+            "1998": "0x6684E5DdbEe1b97E10847468cB5f4e38f3aB83FE",
             "2046399126": "0x16d623f2f3AB1d58426f0402c313f1d3fdA14249",
             "2442": "0x89e44099f5E80484dcF48995080481214b9c2D7c",
             "252": "0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81",
             "2522": "0x9EA18BFDB50E9bb4A18F9d3Df7804E398F8fE0dc",
             "300": "0x9f599b0044838397584CF181989a9A40d1aafD94",
             "314": "0xB30b1B98d8276b80bC4f5aF9f9170ef3220EC27D",
             "3141": "0xb55bB55f7D8b4F26Bd18198088C96488D95cab39",
             "314159": "0xb55bB55f7D8b4F26Bd18198088C96488D95cab39",
             "324": "0xDC94D5245B19661BD71a973788696D6D965236EA",
             "3441005": "0x6684E5DdbEe1b97E10847468cB5f4e38f3aB83FE",
             "369": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "420": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "42161": "0xB30b1B98d8276b80bC4f5aF9f9170ef3220EC27D",
             "421613": "0xb55bB55f7D8b4F26Bd18198088C96488D95cab39",
+            "421614": "0x9EA18BFDB50E9bb4A18F9d3Df7804E398F8fE0dc",
             "5": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "5000": "0x96918F58e0D34DC1f69d0ef724D5207C28919010",
             "5001": "0xFeAE6a8451e188b973F57be047d5aBE8814cC899",
+            "5003": "0x6684E5DdbEe1b97E10847468cB5f4e38f3aB83FE",
             "59140": "0x9EA18BFDB50E9bb4A18F9d3Df7804E398F8fE0dc",
-            "59141": "0x16d623f2f3AB1d58426f0402c313f1d3fdA14249",
+            "59141": "0xB3bB03eA894C609C8560Af3d8726556f52140a39",
             "59144": "0xC866DB9021fe81856fF6c5B3E3514BF9D1593D81",
             "80001": "0x11cA06aa780ce89dbBF5D8F5fA8bf6965Be942c9",
+            "80002": "0x5446397292854D92872eDf426eEaB8FdC6Bd2bEa",
             "84531": "0xAb0145d6aA4F799Bf7f4C0178e5393F6B5655dbf",
+            "84532": "0x6684E5DdbEe1b97E10847468cB5f4e38f3aB83FE",
             "943": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45"
         },
         "name": "tellor-governance",
         "org": "tellor",
         "type": "ContractInfo"
     }
 ]
```

### Comparing `telliot_core-0.3.4/src/telliot_core/directory.py` & `telliot_core-0.3.5/src/telliot_core/directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,19 +100,31 @@
                 elif chain_id == 1998:
                     url = "https://testnet.kyotoscan.io"
                 elif chain_id == 1444673419:
                     url = "https://juicy-low-small-testnet.explorer.testnet.skalenodes.com"
                 elif chain_id == 2046399126:
                     url = "https://elated-tan-skat.explorer.mainnet.skalenodes.com"
                 elif chain_id == 59141:
-                    url = "https://sepolia.lineascan.build"
+                    url = "https://api-sepolia.lineascan.build"
                 elif chain_id == 324:
                     url = "https://block-explorer-api.mainnet.zksync.io"
                 elif chain_id == 300:
                     url = "https://block-explorer-api.sepolia.zksync.io"
+                elif chain_id == 80002:
+                    url = "https://api-amoy.polygonscan.com/"
+                elif chain_id == 11155420:
+                    url = "https://api-sepolia-optimism.etherscan.io/"
+                elif chain_id == 421614:
+                    url = "https://api-sepolia.arbiscan.io/"
+                elif chain_id == 5003:
+                    url = "https://explorer.sepolia.mantle.xyz/"
+                elif chain_id == 84532:
+                    url = "https://api-sepolia.basescan.org/"
+                elif chain_id == 111:
+                    url = "https://testnet-explorer.gobob.xyz:443"
                 else:
                     raise ValueError(f"Could not retrieve ABI using chain_id {chain_id}")
 
                 url = url + f"/api?module=contract&action=getabi&address={address}&format=raw"
 
                 if api_key:
                     url = url + f"&apikey={api_key}"
```

### Comparing `telliot_core-0.3.4/src/telliot_core/gas/legacy_gas.py` & `telliot_core-0.3.5/src/telliot_core/gas/legacy_gas.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/logs.py` & `telliot_core-0.3.5/src/telliot_core/logs.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/model/api_keys.py` & `telliot_core-0.3.5/src/telliot_core/model/api_keys.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     ApiKey(
         name="bravenewcoin",
         key="",
         url="https://bravenewcoin.p.rapidapi.com/",
     ),
     ApiKey(name="nomics", key="", url="https://api.nomics.com/"),
     ApiKey(name="coinmarketcap", key="", url="https://pro-api.coinmarketcap.com/"),
+    ApiKey(name="coingecko", key="", url="https://pro-api.coingecko.com"),
 ]
 
 
 @dataclass
 class ApiKeyList(ConfigOptions):
     api_keys: List[ApiKey] = field(default_factory=lambda: default_api_keys)
```

### Comparing `telliot_core-0.3.4/src/telliot_core/model/chain.py` & `telliot_core-0.3.5/src/telliot_core/model/chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,14 +279,56 @@
     Chain(
         chain_id=300,
         name="zkSync Era Sepolia Testnet",
         chain="zkSync Era Sepolia Testnet",
         network="testnet",
         currency=EVMCurrency(name="Ether", symbol="ETH", decimals=18),
     ),
+    Chain(
+        chain_id=80002,
+        name="Polygon Amoy Testnet",
+        chain="polygon-amoy",
+        network="testnet",
+        currency=EVMCurrency(name="Matic", symbol="MATIC", decimals=18),
+    ),
+    Chain(
+        chain_id=11155420,
+        name="Optimism Sepolia Testnet",
+        chain="optimism-sepolia",
+        network="testnet",
+        currency=EVMCurrency(name="Ether", symbol="ETH", decimals=18),
+    ),
+    Chain(
+        chain_id=421614,
+        name="Arbitrum Sepolia Testnet",
+        chain="arbitrum-sepolia",
+        network="testnet",
+        currency=EVMCurrency(name="Ether", symbol="ETH", decimals=18),
+    ),
+    Chain(
+        chain_id=5003,
+        name="Mantle Sepolia Testnet",
+        chain="mantle-sepolia",
+        network="testnet",
+        currency=EVMCurrency(name="Mantle", symbol="MNT", decimals=18),
+    ),
+    Chain(
+        chain_id=84532,
+        name="Base Sepolia Testnet",
+        chain="base-sepolia",
+        network="testnet",
+        currency=EVMCurrency(name="Ether", symbol="ETH", decimals=18),
+    ),
+    Chain(
+        chain_id=111,
+        name="puff-bob-jznbxtoq7h",
+        chain="BOB",
+        network="testnet",
+        currency=EVMCurrency(name="Ether", symbol="ETH", decimals=18),
+    ),
 ]
 
 
 @dataclass
 class ChainList(ConfigOptions):
     chains: List[Chain] = field(default_factory=lambda: default_chain_list)
```

### Comparing `telliot_core-0.3.4/src/telliot_core/model/endpoints.py` & `telliot_core-0.3.5/src/telliot_core/model/endpoints.py`

 * *Files 14% similar despite different names*

```diff
@@ -298,29 +298,29 @@
         explorer="https://sepolia.lineascan.build",
     ),
     RPCEndpoint(
         chain_id=59144,
         provider="Linea",
         network="Linea",
         url="https://rpc.linea.build",
-        explorer="https://api.lineascan.build",
+        explorer="https://lineascan.build/",
     ),
     RPCEndpoint(
         chain_id=2522,
         provider="Fraxtal",
         network="Fraxtal Testnet",
         url="https://rpc.testnet.frax.com",
-        explorer="https://api-holesky.fraxscan.com",
+        explorer="https://holesky.fraxscan.com",
     ),
     RPCEndpoint(
         chain_id=252,
         provider="Fraxtal",
         network="Fraxtal Mainnet",
         url="https://rpc.frax.com",
-        explorer="https://api.fraxscan.com",
+        explorer="https://fraxscan.com",
     ),
     RPCEndpoint(
         chain_id=1998,
         provider="Kyoto",
         network="Kyoto Testnet",
         url="https://rpc.testnet.kyotoprotocol.io:8545",
         explorer="https://testnet.kyotoscan.io",
@@ -349,14 +349,56 @@
     RPCEndpoint(
         chain_id=300,
         provider="zksync",
         network="ZkSync Era Sepolia Testnet",
         url="https://zksync-era-sepolia.blockpi.network/v1/rpc/public",
         explorer="https://sepolia.explorer.zksync.io",
     ),
+    RPCEndpoint(
+        chain_id=80002,
+        provider="infura",
+        network="Polygon Amoy Testnet",
+        url="https://polygon-amoy.infura.io/v3/{INFURA_API_KEY}",
+        explorer="https://amoy.polygonscan.com/",
+    ),
+    RPCEndpoint(
+        chain_id=11155420,
+        provider="infura",
+        network="Optimism Sepolia Testnet",
+        url="https://optimism-sepolia.infura.io/v3/{INFURA_API_KEY}",
+        explorer="https://sepolia-optimism.etherscan.io/",
+    ),
+    RPCEndpoint(
+        chain_id=421614,
+        provider="infura",
+        network="Arbitrum Sepolia Testnet",
+        url="https://arbitrum-sepolia.infura.io/v3/{INFURA_API_KEY}",
+        explorer="https://sepolia.arbiscan.io/",
+    ),
+    RPCEndpoint(
+        chain_id=5003,
+        provider="Mantle",
+        network="Mantle Sepolia Testnet",
+        url="https://rpc.sepolia.mantle.xyz",
+        explorer="https://explorer.sepolia.mantle.xyz",
+    ),
+    RPCEndpoint(
+        chain_id=84532,
+        provider="Base",
+        network="Base Sepolia Testnet",
+        url="https://sepolia.base.org",
+        explorer="https://sepolia.basescan.org",
+    ),
+    RPCEndpoint(
+        chain_id=111,
+        provider="BOB",
+        network="puff-bob-jznbxtoq7h",
+        url="https://l2-puff-bob-jznbxtoq7h.t.conduit.xyz",
+        explorer="https://testnet-explorer.gobob.xyz:443",
+    ),
 ]
 
 
 @dataclass
 class EndpointList(ConfigOptions):
     endpoints: List[RPCEndpoint] = field(default_factory=lambda: default_endpoint_list)
```

### Comparing `telliot_core-0.3.4/src/telliot_core/model/tokens.py` & `telliot_core-0.3.5/src/telliot_core/model/tokens.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/tellor/tellor360/autopay.py` & `telliot_core-0.3.5/src/telliot_core/tellor/tellor360/autopay.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/tellor/tellor360/oracle.py` & `telliot_core-0.3.5/src/telliot_core/tellor/tellor360/oracle.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/tellor/tellorflex/autopay.py` & `telliot_core-0.3.5/src/telliot_core/tellor/tellorflex/autopay.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/tellor/tellorflex/oracle.py` & `telliot_core-0.3.5/src/telliot_core/tellor/tellorflex/oracle.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/tellor/tellorflex/token.py` & `telliot_core-0.3.5/src/telliot_core/tellor/tellorflex/token.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/tellor/tellorx/master.py` & `telliot_core-0.3.5/src/telliot_core/tellor/tellorx/master.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/tellor/tellorx/oracle.py` & `telliot_core-0.3.5/src/telliot_core/tellor/tellorx/oracle.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/utils/home.py` & `telliot_core-0.3.5/src/telliot_core/utils/home.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/utils/key_helpers.py` & `telliot_core-0.3.5/src/telliot_core/utils/key_helpers.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/utils/response.py` & `telliot_core-0.3.5/src/telliot_core/utils/response.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/utils/timestamp.py` & `telliot_core-0.3.5/src/telliot_core/utils/timestamp.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core/utils/versions.py` & `telliot_core-0.3.5/src/telliot_core/utils/versions.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/src/telliot_core.egg-info/PKG-INFO` & `telliot_core-0.3.5/src/telliot_core.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telliot_core
-Version: 0.3.4
+Version: 0.3.5
 Summary: Telliot is a Python framework for interacting with the decentralized TellorX network.
 Home-page: https://github.com/tellor-io/telliot-core
 Author: Tellor Development Community
 Author-email: info@tellor.io
 License: MIT
 Keywords: oracle,etherium,blockchain
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `telliot_core-0.3.4/src/telliot_core.egg-info/SOURCES.txt` & `telliot_core-0.3.5/src/telliot_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/conftest.py` & `telliot_core-0.3.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_app_core.py` & `telliot_core-0.3.5/tests/test_app_core.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_autopay.py` & `telliot_core-0.3.5/tests/test_autopay.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_cli.py` & `telliot_core-0.3.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_config.py` & `telliot_core-0.3.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_contract.py` & `telliot_core-0.3.5/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_directory.py` & `telliot_core-0.3.5/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_gas.py` & `telliot_core-0.3.5/tests/test_gas.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_listener.py` & `telliot_core-0.3.5/tests/test_listener.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_master_read.py` & `telliot_core-0.3.5/tests/test_master_read.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_model_chain.py` & `telliot_core-0.3.5/tests/test_model_chain.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_oracle_read.py` & `telliot_core-0.3.5/tests/test_oracle_read.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_rpc_endpoint.py` & `telliot_core-0.3.5/tests/test_rpc_endpoint.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_session_manager.py` & `telliot_core-0.3.5/tests/test_session_manager.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_telliot_config.py` & `telliot_core-0.3.5/tests/test_telliot_config.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_tellorflex.py` & `telliot_core-0.3.5/tests/test_tellorflex.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tests/test_token.py` & `telliot_core-0.3.5/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.3.4/tox.ini` & `telliot_core-0.3.5/tox.ini`

 * *Files identical despite different names*

