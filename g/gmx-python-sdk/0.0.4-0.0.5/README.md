# Comparing `tmp/gmx_python_sdk-0.0.4.tar.gz` & `tmp/gmx_python_sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmx_python_sdk-0.0.4.tar", max compression
+gzip compressed data, was "gmx_python_sdk-0.0.5.tar", max compression
```

## Comparing `gmx_python_sdk-0.0.4.tar` & `gmx_python_sdk-0.0.5.tar`

### file list

```diff
@@ -1,50 +1,77 @@
--rw-r--r--   0        0        0     1070 2024-03-03 20:24:20.328844 gmx_python_sdk-0.0.4/LICENSE
--rw-r--r--   0        0        0    19356 2024-03-03 20:24:20.328956 gmx_python_sdk-0.0.4/README.md
--rw-r--r--   0        0        0    16152 2024-03-04 11:04:19.368888 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/datastore.json
--rw-r--r--   0        0        0     2935 2024-03-04 11:04:19.368993 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/depositvault.json
--rw-r--r--   0        0        0    26628 2024-03-04 11:04:19.369071 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/eventemitter.json
--rw-r--r--   0        0        0    14130 2024-03-04 11:04:19.369177 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/exchangerouter.json
--rw-r--r--   0        0        0     2935 2024-03-04 11:04:19.369251 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/ordervault.json
--rw-r--r--   0        0        0   124378 2024-03-04 11:04:19.369410 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/syntheticsreader.json
--rw-r--r--   0        0        0      804 2024-03-04 11:04:19.369517 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/syntheticsrouter.json
--rw-r--r--   0        0        0     2935 2024-03-04 11:04:19.369591 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/withdrawalvault.json
--rw-r--r--   0        0        0    16152 2024-03-04 11:04:19.369720 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/datastore.json
--rw-r--r--   0        0        0     2935 2024-03-04 11:04:19.369798 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/depositvault.json
--rw-r--r--   0        0        0    26628 2024-03-04 11:04:19.369869 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/eventemitter.json
--rw-r--r--   0        0        0    14130 2024-03-04 11:04:19.369981 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/exchangerouter.json
--rw-r--r--   0        0        0     2935 2024-03-04 11:04:19.370047 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/ordervault.json
--rw-r--r--   0        0        0    46631 2024-03-04 11:04:19.370122 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/syntheticsreader.json
--rw-r--r--   0        0        0      804 2024-03-04 11:04:19.370203 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/syntheticsrouter.json
--rw-r--r--   0        0        0     2935 2024-03-04 11:04:19.370265 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/withdrawalvault.json
--rw-r--r--   0        0        0      518 2024-03-04 11:04:19.370333 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/balance_abi.json
--rw-r--r--   0        0        0     5575 2024-03-04 11:04:19.370561 gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/token_approval.json
--rw-r--r--   0        0        0       75 2024-03-04 11:04:19.370685 gmx_python_sdk-0.0.4/gmx_python_sdk/data_store/placeholder.txt
--rw-r--r--   0        0        0    10589 2024-03-04 11:04:19.370966 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/__pycache__/get_available_liquidity.cpython-311.pyc
--rw-r--r--   0        0        0     4470 2024-03-04 11:06:04.226134 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/approve_token_for_spend.py
--rw-r--r--   0        0        0      620 2024-03-04 11:04:19.371452 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/create_decrease_order.py
--rw-r--r--   0        0        0      634 2024-03-04 11:04:19.371521 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/create_deposit_order.py
--rw-r--r--   0        0        0      617 2024-03-04 11:04:19.371605 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/create_increase_order.py
--rw-r--r--   0        0        0     3200 2024-03-04 11:04:19.371685 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/create_swap_order.py
--rw-r--r--   0        0        0      643 2024-03-04 11:04:19.371756 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/create_withdrawal_order.py
--rw-r--r--   0        0        0    11220 2024-03-04 11:04:19.371909 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/deposit.py
--rw-r--r--   0        0        0     2762 2024-03-04 11:04:19.371980 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/gas_utils.py
--rw-r--r--   0        0        0    12066 2024-03-04 11:04:19.372115 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_available_liquidity.py
--rw-r--r--   0        0        0     6864 2024-03-04 11:04:19.372359 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_borrow_apr.py
--rw-r--r--   0        0        0     6210 2024-03-04 11:04:19.372615 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_claimable_fees.py
--rw-r--r--   0        0        0     5031 2024-03-04 11:04:19.372862 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_contract_balance.py
--rw-r--r--   0        0        0     9028 2024-03-04 11:04:19.372999 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_funding_apr.py
--rw-r--r--   0        0        0     7753 2024-03-04 11:04:19.373228 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_gm_prices.py
--rw-r--r--   0        0        0     4018 2024-03-05 21:44:34.667499 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_markets.py
--rw-r--r--   0        0        0     8078 2024-03-04 11:04:19.373529 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_open_interest.py
--rw-r--r--   0        0        0     5963 2024-03-04 11:04:19.373762 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_open_positions.py
--rw-r--r--   0        0        0     5961 2024-03-04 11:04:19.374014 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_open_positons.py
--rw-r--r--   0        0        0     1572 2024-03-04 11:04:19.374085 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_oracle_prices.py
--rw-r--r--   0        0        0     6364 2024-03-04 11:04:19.374338 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_pool_tvl.py
--rw-r--r--   0        0        0    20960 2024-03-05 21:44:34.668081 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/gmx_utils.py
--rw-r--r--   0        0        0     4202 2024-03-04 11:04:19.374727 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/keys.py
--rw-r--r--   0        0        0    10995 2024-03-04 11:04:19.374889 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/liquidity_argument_parser.py
--rw-r--r--   0        0        0    14657 2024-03-04 11:04:19.374970 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/order.py
--rw-r--r--   0        0        0    17903 2024-03-04 11:04:19.375030 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/order_argument_parser.py
--rw-r--r--   0        0        0     9037 2024-03-04 11:04:19.375360 gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/withdraw.py
--rw-r--r--   0        0        0      783 2024-03-05 21:45:08.931348 gmx_python_sdk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    20216 1970-01-01 00:00:00.000000 gmx_python_sdk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-03 20:24:20.328844 gmx_python_sdk-0.0.5/LICENSE
+-rw-r--r--   0        0        0    21068 2024-06-02 19:52:55.618840 gmx_python_sdk-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2024-06-02 19:52:55.620646 gmx_python_sdk-0.0.5/gmx_python_sdk/__init__.py
+-rw-r--r--   0        0        0    16152 2024-03-04 11:04:19.368888 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/datastore.json
+-rw-r--r--   0        0        0     2935 2024-03-04 11:04:19.368993 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/depositvault.json
+-rw-r--r--   0        0        0    26628 2024-03-04 11:04:19.369071 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/eventemitter.json
+-rw-r--r--   0        0        0    14130 2024-03-04 11:04:19.369177 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/exchangerouter.json
+-rw-r--r--   0        0        0     2935 2024-03-04 11:04:19.369251 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/ordervault.json
+-rw-r--r--   0        0        0   124378 2024-03-04 11:04:19.369410 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/syntheticsreader.json
+-rw-r--r--   0        0        0      804 2024-03-04 11:04:19.369517 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/syntheticsrouter.json
+-rw-r--r--   0        0        0     2935 2024-03-04 11:04:19.369591 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/withdrawalvault.json
+-rw-r--r--   0        0        0    16152 2024-03-04 11:04:19.369720 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/datastore.json
+-rw-r--r--   0        0        0     2935 2024-03-04 11:04:19.369798 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/depositvault.json
+-rw-r--r--   0        0        0    26628 2024-03-04 11:04:19.369869 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/eventemitter.json
+-rw-r--r--   0        0        0    14130 2024-03-04 11:04:19.369981 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/exchangerouter.json
+-rw-r--r--   0        0        0     2935 2024-03-04 11:04:19.370047 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/ordervault.json
+-rw-r--r--   0        0        0    46631 2024-03-04 11:04:19.370122 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/syntheticsreader.json
+-rw-r--r--   0        0        0      804 2024-03-04 11:04:19.370203 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/syntheticsrouter.json
+-rw-r--r--   0        0        0     2935 2024-03-04 11:04:19.370265 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/withdrawalvault.json
+-rw-r--r--   0        0        0      518 2024-03-04 11:04:19.370333 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/balance_abi.json
+-rw-r--r--   0        0        0     5575 2024-03-04 11:04:19.370561 gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/token_approval.json
+-rw-r--r--   0        0        0     1327 2024-06-02 19:52:55.621051 gmx_python_sdk-0.0.5/gmx_python_sdk/data_store/arbitrum_gm_prices.csv
+-rw-r--r--   0        0        0       75 2024-03-04 11:04:19.370685 gmx_python_sdk-0.0.5/gmx_python_sdk/data_store/placeholder.txt
+-rw-r--r--   0        0        0        0 2024-06-02 19:52:55.621078 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/__init__.py
+-rw-r--r--   0        0        0      196 2024-06-02 19:52:55.621190 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-06-02 19:52:55.621215 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/__init__.py
+-rw-r--r--   0        0        0      199 2024-06-02 19:52:55.621295 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6924 2024-06-02 19:52:55.621592 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     9690 2024-06-02 19:52:55.621938 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/__pycache__/get_available_liquidity.cpython-311.pyc
+-rw-r--r--   0        0        0     2871 2024-06-02 19:52:55.622154 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/__pycache__/get_borrow_apr.cpython-311.pyc
+-rw-r--r--   0        0        0     5813 2024-06-02 19:52:55.622298 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/__pycache__/get_claimable_fees.cpython-311.pyc
+-rw-r--r--   0        0        0     4755 2024-06-02 19:52:55.622492 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/__pycache__/get_funding_apr.cpython-311.pyc
+-rw-r--r--   0        0        0     6639 2024-06-02 19:52:55.622723 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/__pycache__/get_markets.cpython-311.pyc
+-rw-r--r--   0        0        0     4794 2024-06-02 19:52:55.622966 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/__pycache__/get_markets_legacy.cpython-311.pyc
+-rw-r--r--   0        0        0     5262 2024-06-02 19:52:55.623241 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/__pycache__/get_open_interest.cpython-311.pyc
+-rw-r--r--   0        0        0     8320 2024-06-02 19:52:55.623435 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/__pycache__/get_open_interest_legacy.cpython-311.pyc
+-rw-r--r--   0        0        0     2624 2024-06-02 19:52:55.623520 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/__pycache__/get_oracle_prices.cpython-311.pyc
+-rw-r--r--   0        0        0    25921 2024-06-02 19:52:55.624044 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/__pycache__/gmx_utils.cpython-311.pyc
+-rw-r--r--   0        0        0     5711 2024-06-02 19:52:55.624180 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/__pycache__/keys.cpython-311.pyc
+-rw-r--r--   0        0        0     6110 2024-06-02 19:52:55.624350 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/__pycache__/test.cpython-311.pyc
+-rw-r--r--   0        0        0     3997 2024-06-02 19:52:55.624462 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/approve_token_for_spend.py
+-rw-r--r--   0        0        0     2770 2024-06-02 19:52:55.624621 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/gas_utils.py
+-rw-r--r--   0        0        0     7038 2024-06-02 19:52:55.624850 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/__pycache__/get.cpython-311.pyc
+-rw-r--r--   0        0        0     9397 2024-06-02 19:52:55.625164 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/__pycache__/get_available_liquidity.cpython-311.pyc
+-rw-r--r--   0        0        0     7281 2024-06-02 19:52:55.625330 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/__pycache__/get_gm_prices.cpython-311.pyc
+-rw-r--r--   0        0        0     6630 2024-06-02 19:52:55.625481 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/__pycache__/get_markets.cpython-311.pyc
+-rw-r--r--   0        0        0     5267 2024-06-02 19:52:55.625653 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/__pycache__/get_open_interest.cpython-311.pyc
+-rw-r--r--   0        0        0     6494 2024-06-02 19:52:55.625831 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/__pycache__/get_open_positions.cpython-311.pyc
+-rw-r--r--   0        0        0     2630 2024-06-02 19:52:55.625989 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/__pycache__/get_oracle_prices.cpython-311.pyc
+-rw-r--r--   0        0        0     7578 2024-06-02 19:52:55.626203 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/__pycache__/test.cpython-311.pyc
+-rw-r--r--   0        0        0     6561 2024-06-02 19:52:55.626327 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get.py
+-rw-r--r--   0        0        0    10359 2024-06-02 19:52:55.626495 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_available_liquidity.py
+-rw-r--r--   0        0        0     1645 2024-06-02 19:52:55.626642 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_borrow_apr.py
+-rw-r--r--   0        0        0     4859 2024-06-02 19:52:55.626751 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_claimable_fees.py
+-rw-r--r--   0        0        0     5067 2024-06-02 19:52:55.626858 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_contract_balance.py
+-rw-r--r--   0        0        0     3897 2024-06-02 19:52:55.626937 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_funding_apr.py
+-rw-r--r--   0        0        0     6084 2024-06-02 19:52:55.627056 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_gm_prices.py
+-rw-r--r--   0        0        0     5242 2024-06-02 19:52:55.627163 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_markets.py
+-rw-r--r--   0        0        0     4532 2024-06-02 19:52:55.627271 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_open_interest.py
+-rw-r--r--   0        0        0     4975 2024-06-02 19:52:55.627377 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_open_positions.py
+-rw-r--r--   0        0        0     1514 2024-06-02 19:52:55.627445 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_oracle_prices.py
+-rw-r--r--   0        0        0     6383 2024-06-02 19:52:55.627558 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_pool_tvl.py
+-rw-r--r--   0        0        0     5952 2024-06-02 19:52:55.627740 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/test.py
+-rw-r--r--   0        0        0    19513 2024-06-02 19:52:55.627897 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/gmx_utils.py
+-rw-r--r--   0        0        0     4202 2024-03-04 11:04:19.374727 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/keys.py
+-rw-r--r--   0        0        0      621 2024-06-02 19:52:55.628034 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/create_decrease_order.py
+-rw-r--r--   0        0        0      635 2024-06-02 19:52:55.628100 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/create_deposit_order.py
+-rw-r--r--   0        0        0      618 2024-06-02 19:52:55.628162 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/create_increase_order.py
+-rw-r--r--   0        0        0     3213 2024-06-02 19:52:55.628229 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/create_swap_order.py
+-rw-r--r--   0        0        0      644 2024-06-02 19:52:55.628290 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/create_withdrawal_order.py
+-rw-r--r--   0        0        0    11687 2024-06-02 19:52:55.628455 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/deposit.py
+-rw-r--r--   0        0        0    10982 2024-06-02 19:52:55.628606 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/liquidity_argument_parser.py
+-rw-r--r--   0        0        0    14974 2024-06-02 19:52:55.628851 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/order.py
+-rw-r--r--   0        0        0    17844 2024-06-02 19:52:55.628911 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/order_argument_parser.py
+-rw-r--r--   0        0        0     9383 2024-06-02 19:52:55.629050 gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/withdraw.py
+-rw-r--r--   0        0        0      783 2024-06-02 20:04:57.225508 gmx_python_sdk-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    21928 1970-01-01 00:00:00.000000 gmx_python_sdk-0.0.5/PKG-INFO
```

### Comparing `gmx_python_sdk-0.0.4/LICENSE` & `gmx_python_sdk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/README.md` & `gmx_python_sdk-0.0.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 # GMX Python SDK
 
 A python based SDK developed for interacting with GMX v2
 
+- [Pip Install](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#pip-install)
 - [Requirements](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#requirements)
 - [Config File Setup](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#config-file-setup)
 - [Example Scripts](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#example-scripts)
 - [General Usage](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#general-usage)
     - [Increase Position](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#increase-position)
     - [Decrease Position](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#decrease-position)
     - [Swap Order](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#swap-order)
@@ -17,14 +18,21 @@
         - [Order Argument Parser](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#order-argument-parser)
         - [Liquidity Argument Parser](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#liquidity-argument-parser)
         - [Closing Positions](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#closing-positions)
     - [GMX Stats](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#gmx-stats)
     - [Debug Mode](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#debug-mode)
 - [Known Limitations](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#known-limitations)
 
+## Pip Install
+
+The SDK can be installed via pip:
+
+```
+pip install gmx-python-sdk
+```
 
 ## Requirements
 
 Developed using:
 ```python
   python=3.10.4
 ```
@@ -40,58 +48,60 @@
 pip install pandas==1.4.2
 pip install numerize
 ```
 
 The codebase is designed around the usage of web3py [6.10.0](https://web3py.readthedocs.io/en/stable/releases.html#web3-py-v6-10-0-2023-09-21), and will not work with older versions and has not been tested with the latest version.
 ## Config File Setup
 
-[Config file](https://github.com/snipermonke01/gmx_python_sdk/blob/main/config.yaml) must set up before usage. For stats based operations, you will need only an RPC but for execution you need to save both a wallet address and the private key of that wallet. 
+[Config file](https://github.com/snipermonke01/gmx_python_sdk/blob/main/config.yaml) can be set before usage by editing the yaml file. For stats based operations, you will need only an RPC but for execution you need to save both a wallet address and the private key of that wallet. 
 
 ```yaml
-arbitrum:
-  rpc: rpc_url
-  chain_id: chain_id
-avalanche:
-  rpc: rpc_url
-  chain_id: chain_id
+rpcs:
+  arbitrum: arbitrum_rpc
+  avalanche: avax_rpc
+chain_ids:
+  arbitrum: 42161
+  avalanche: 43114
 private_key: private_key
-user_wallet_address: wallet_address
+user_wallet_address: user_wallet_address
+
 ```
 
-The example script [setting_config.py](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/setting_config.py) can be viewed for demonstration on how to import config and update with new details from script.
+The example script [setting_config.py](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/setting_config.py) can be viewed for demonstration on how to import config and update with new details from within a script.
 
-There is an example in [create_increase_.py](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/setting_config.py) of how it is possible to [set config parameters](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/create_increase_order.py#L8-L19) within the py script, and then [reset these](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/create_increase_order.py#L71-L77) once the script has finished running.
+There is an example in all the example scripts of how to import the config and init the object to pass to functions and classes through the SDK.
 
 ## Example Scripts
 
 There are several example scripts which can be run and can be found in [example scripts.](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/) These are mostly for demonstration purposes on how to utilise the SDK, and can should be incoporated into your own scripts and strategies.
 
 
 ## General Usage
 
 ### [Increase Position](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/create_increase_order.py)
 
 The following block demonstrates how to open (or increase) a position:
 
 ```python
-from scripts.v2.create_increase_order import IncreaseOrder
+from gmx_python_sdk_scripts.v2.order.create_increase_order import IncreaseOrder
 
 order = IncreaseOrder(
-    chain,
-    market_key,
-    collateral_address,
-    index_token_address,
-    is_long,
-    size_delta_usd,
-    initial_collateral_delta_amount,
-    slippage_percent,
-    swap_path
+    config=config,
+    market_key=market_key,
+    collateral_address=collateral_address,
+    index_token_address=index_token_address,
+    is_long=is_long,
+    size_delta_usd=size_delta_usd,
+    initial_collateral_delta_amount=initial_collateral_delta_amount,
+    slippage_percent=slippage_percent,
+    swap_path=swap_path,
+    debug_mode=debug_mode
 )
 ```
-**chain** - *type str*: either 'arbitrum' or 'avalanche' (avalanche currently in testing still)
+**config** - *type obj*: an initialised config object (avalanche currently in testing still)
 
 **market_key** - *type str*: the contract address of the GMX market you want to increase a position on
 
 **collateral_address** - *type str*: the contract address of the token you want to use as collateral
 
 **index_token_address** - *type str*: the contract address of the token you want to trade
 
@@ -101,34 +111,37 @@
 
 **initial_collateral_delta_amount** - *type int*: the amount of token you want to use as collateral, 10^decimal of that token
 
 **slippage_percent** - *type float*: the percentage you want to allow slippage
 
 **swap_path** - *type list(str)*: a list of the GMX markets you will need to swap through if the starting token is different to the token you want to use as collateral
 
+**debug_mode** - *type bool*: set to true to create an order without submitting
+
 ### [Decrease Position](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/create_decrease_order.py)
 
 The following block demonstrates how to close (or decrease) a position:
 
 ```python
-from scripts.v2.create_decrease_order import DecreaseOrder
+from gmx_python_sdk_scripts.v2.order.create_decrease_order import DecreaseOrder
 
 order = DecreaseOrder(
-    chain,
-    market_key,
-    collateral_address,
-    index_token_address,
-    is_long,
-    size_delta_usd,
-    initial_collateral_delta_amount,
-    slippage_percent,
-    swap_path
+    config=config,
+    market_key=market_key,
+    collateral_address=collateral_address,
+    index_token_address=index_token_address,
+    is_long=is_long,
+    size_delta_usd=size_delta_usd,
+    initial_collateral_delta_amount=initial_collateral_delta_amount,
+    slippage_percent=slippage_percent,
+    swap_path=swap_path,
+    debug_mode=debug_mode
 )
 ```
-**chain** - *type str*: either 'arbitrum' or 'avalanche' (currently in testing still)
+**config** - *type obj*: an initialised config object (avalanche currently in testing still)
 
 **market_key** - *type str*: the contract address of the GMX market you want to decrease a position for
 
 **collateral_address** - *type str*: the contract address of the token you are using as collateral
 
 **index_token_address** - *type str*: the contract address of the token are trading
 
@@ -138,36 +151,39 @@
 
 **initial_collateral_delta_amount** - *type int*: the amount of collateral token you want to remove, 10^decimal of that token
 
 **slippage_percent** - *type float*: the percentage you want to allow slippage
 
 **swap_path** - *type list(str)*: a list of the GMX markets you will need to swap through to get your desired out token
 
+**debug_mode** - *type bool*: set to true to create an order without submitting
+
 ### [Swap Order](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/create_swap_order.py)
 
 The following block demonstrates how to make a swap:
 
 ```python
-from scripts.v2.create_swap_order import SwapOrder
+from gmx_python_sdk_scripts.v2.order.create_swap_order import SwapOrder
 
 order = SwapOrder(
-    chain,
-    market_key,
-    start_token,
-    out_token,
-    collateral_address,
-    index_token_address,
-    is_long,
-    size_delta,
-    initial_collateral_delta_amount,
-    slippage_percent,
-    swap_path
+    config=config,
+    market_key=market_key,
+    start_token=start_token,
+    out_token=out_token,
+    collateral_address=collateral_address,
+    index_token_address=index_token_address,
+    is_long=is_long,
+    size_delta=size_delta,
+    initial_collateral_delta_amount=initial_collateral_delta_amount,
+    slippage_percent=slippage_percent,
+    swap_path=swap_path,
+    debug_mode=debug_mode
 )
 ```
-**chain** - *type str*: either 'arbitrum' or 'avalanche' (currently in testing still)
+**config** - *type obj*: an initialised config object (avalanche currently in testing still)
 
 **market_key** - *type str*: the contract address of the GMX market you want to (first) market you want to swap through
 
 **start_token** - *type str*: the contract address of the token you start the swap with
 
 **out_token** - *type str*: the contract address of the token you want out
 
@@ -181,146 +197,118 @@
 
 **initial_collateral_delta_amount** - *type int*: the amount of start token you are swapping
 
 **slippage_percent** - *type float*: the percentage you want to allow slippage
 
 **swap_path** - *type list()*: list of gmx market address your swap will go through
 
+**debug_mode** - *type bool*: set to true to create an order without submitting
+
 ### [Deposit Order](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/create_deposit_order.py)
 
 The following block demonstrates how to make a deposit to a gm pool:
 
 ```python
-from scripts.v2.create_deposit_order import DepositOrder
+from gmx_python_sdk_scripts.v2.order.create_deposit_order import DepositOrder
 
 order = DepositOrder(
-    chain,
-    market_key,
-    initial_long_token,
-    initial_short_token,
-    long_token_amount,
-    short_token_amount
+    config=config,
+    market_key=market_key,
+    initial_long_token=initial_long_token,
+    initial_short_token=initial_short_token,
+    long_token_amount=long_token_amount,
+    short_token_amount=short_token_amount,
+    debug_mode=debug_mode
 )
 ```
-**chain** - *type str*: either 'arbitrum' or 'avalanche' (currently in testing still)
+**config** - *type obj*: an initialised config object (avalanche currently in testing still)
 
 **market_key** - *type str*: the contract address of the GMX market you want to deposit into
 
 **initial_long_token** - *type str*: the contract address of the token you want to use to deposit into long side, can be None
 
 **initial_short_token** - *type str*: the contract address of the token you want to use to deposit into short side, can be None
 
 **long_token_amount** - *type str*: the amount of token to add to long side, can be 0
 
 **short_token_amount** - *type str*: the amount of token to add to short side, can be 0
 
+**debug_mode** - *type bool*: set to true to create an order without submitting
+
 ### [Withdraw Order](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/create_withdraw_order.py)
 
 The following block demonstrates how to make a withdrawal from a gm pool:
 
 ```python
-from scripts.v2.create_withdrawal_order import WithdrawOrder
+from gmx_python_sdk_scripts.v2.order.create_withdrawal_order import WithdrawOrder
 
 order = WithdrawOrder(
-    chain,
-    market_key,
-    out_token,
-    gm_amount
+    config=config,
+    market_key=market_key,
+    out_token=out_token,
+    gm_amount=gm_amount,
+    debug_mode=debug_mode
 )
 ```
-**chain** - *type str*: either 'arbitrum' or 'avalanche' (currently in testing still)
+**config** - *type obj*: an initialised config object (avalanche currently in testing still)
 
 **market_key** - *type str*: the contract address of the GMX market you want to withdraw from
 
 **out_token** - *type str*: the contract address of the token you want to use to receive
 
 **gm_amount** - *type str*: amount of gm tokens to burn
 
-### Get Execution Price & Price Impact On Position Change
-
-
-```python
-from scripts.v2.gmx_utils import get_execution_price_and_price_impact
-
-chain = "arbitrum"
-estimated_swap_output_parameters = {
-    'data_store_address': (data_store_address),
-    'market_addresses': [
-        gmx_market_address,
-        index_token_address,
-        long_token_address,
-        short_token_address
-    ],
-    'token_prices_tuple': [
-        [
-            int(max_price_of_index_token),
-            int(min_price_of_index_token)
-        ],
-        [
-            int(max_price_of_long_token),
-            int(min_price_of_long_token)
-        ],
-        [
-            int(max_price_of_short_token),
-            int(min_price_of_short_token])
-        ],
-    ],
-    'token_in': in_token_address,
-    'token_amount_in': in_token_amount,
-    'ui_fee_receiver': "0x0000000000000000000000000000000000000000"
-}
-
-get_execution_price_and_price_impact(
-    chain,
-    estimated_swap_output_parameters,
-    decimals
-)
-
-```
+**debug_mode** - *type bool*: set to true to create an order without submitting
 
 ### Estimate Swap output
 
-Below shows an example of how to estimate swap output using the [EstimateSwapOutput](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/estimate_swap_output.py#L21) class in [estimate_swap_ouput.py](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/estimate_swap_output.py). One can provide either a token symbol or contract address for in and out tokens and the script will return a dictionary containing the estimate output number of tokens and price impact.
+Below shows an example of how to estimate swap output using the [EstimateSwapOutput](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/estimate_swap_output.py#L20) class in [estimate_swap_ouput.py](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/estimate_swap_output.py). One can provide either a token symbol or contract address for in and out tokens and the script will return a dictionary containing the estimate output number of tokens and price impact.
 
 ```python
-from estimate_swap_output import EstimateSwapOutput
+from gmx_python_sdk.example_scripts.estimate_swap_output import EstimateSwapOutput
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
+
+config = ConfigManager("arbitrum")
+config.set_config()
 
-chain = "arbitrum"
-in_token_symbol = "SOL"
+in_token_symbol = "GMX"
 out_token_symbol = "USDC"
-token_amount = 2
+token_amount = 10
 in_token_address = None
 out_token_address = None
 token_amount_expanded = None
 
-output = EstimateSwapOutput(chain=chain).get_swap_output(
-    in_token_symbol=in_token_symbol,
-    out_token_symbol=out_token_symbol,
-    token_amount=token_amount,
-    in_token_address=in_token_address,
-    out_token_address=out_token_address,
-    token_amount_expanded=token_amount_expanded
+output = EstimateSwapOutput(config=config).get_swap_output(
+     in_token_symbol=in_token_symbol,
+     out_token_symbol=out_token_symbol,
+     token_amount=token_amount,
+     in_token_address=in_token_address,
+     out_token_address=out_token_address,
+     token_amount_expanded=token_amount_expanded
 )
 
 ```
 
 ### Helper Scripts
 
 To assist in argument formatting, there are a few helper functions:
 
-#### [Order Argument Parser](https://github.com/snipermonke01/gmx_python_sdk/blob/main/scripts/v2/order_argument_parser.py)
+#### [Order Argument Parser](https://github.com/snipermonke01/gmx_python_sdk/blob/main/gmx_python_sdk/scripts/v2/order/order_argument_parser.py)
 
 Human readable numbers can be parsed in a dictionary with the following keys/values which are processed by a class, OrderArgumentParser. This class should initialised with a bool to indicate is_increase, is_decrease, or is_swap, calling the method: "process_parameters_dictionary". This will output a dictionary containing the user input parameters reformatted to allow for successful order creation.
 
 For increase:
 
 
 ```python
-from scripts.v2.order_argument_parser import OrderArgumentParser
+from gmx_python_sdk.scripts.v2.order.order_argument_parser import OrderArgumentParser
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
 
+config = ConfigManager("arbitrum")
+config.set_config()
 
 parameters = {
     "chain": 'arbitrum',
 
     # the market you want to trade on
     "index_token_symbol": "ARB",
 
@@ -340,21 +328,30 @@
     "leverage": 1,
 
     # as a percentage
     "slippage_percent": 0.03
 }
 
 
-order_parameters = OrderArgumentParser(is_increase=True).process_parameters_dictionary(parameters)
+order_parameters = OrderArgumentParser(
+     config=config,
+     is_increase=True
+).process_parameters_dictionary(
+     parameters
+)
 ```
 
 For decrease:
 
 ```python
-from scripts.v2.order_argument_parser import OrderArgumentParser
+from gmx_python_sdk.scripts.v2.order.order_argument_parser import OrderArgumentParser
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
+
+config = ConfigManager("arbitrum")
+config.set_config()
 
 parameters = {
     "chain": 'arbitrum',
     "index_token_symbol": "ARB",
 
     "collateral_token_symbol": "USDC",
 
@@ -370,20 +367,29 @@
     "initial_collateral_delta": 6,
 
     # as a percentage
     "slippage_percent": 0.03
 }
 
 
-order_parameters = OrderArgumentParser(is_decrease=True).process_parameters_dictionary(parameters)
+order_parameters = OrderArgumentParser(
+     config=config,
+     is_decrease=True
+).process_parameters_dictionary(
+     parameters
+)
 ```
 For Swap:
 
 ```python
-from scripts.v2.order_argument_parser import OrderArgumentParser
+from gmx_python_sdk.scripts.v2.order.order_argument_parser import OrderArgumentParser
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
+
+config = ConfigManager("arbitrum")
+config.set_config()
 
 parameters = {
     "chain": 'arbitrum',
 
     # token to use as collateral. Start token swaps into collateral token if different
     "out_token_symbol": "ETH",
 
@@ -400,133 +406,165 @@
     "initial_collateral_delta": 10,
 
     # as a percentage
     "slippage_percent": 0.03
 }
 
 
-order_parameters = OrderArgumentParser(is_swap=True).process_parameters_dictionary(parameters)
+order_parameters = OrderArgumentParser(
+     config=config,
+     is_swap=True
+).process_parameters_dictionary(
+     parameters
+)
 ```
-#### [Liquidity Argument Parser](https://github.com/snipermonke01/gmx_python_sdk/blob/main/scripts/v2/order_argument_parser.py)
+#### [Liquidity Argument Parser](https://github.com/snipermonke01/gmx_python_sdk/blob/main/gmx_python_sdk/scripts/v2/order/liquidity_argument_parser.py)
 
 Human readable numbers can be parsed in a dictionary with the following keys/values which are processed by a class, LiquidityArgumentParser. This class should initialised with a bool to indicate is_deposit or is_withdraw calling the method: "process_parameters_dictionary". This will output a dictionary containing the user input parameters reformatted to allow for successful deposit/withdrawal order creation.
 
 For Deposit:
 
 ```python
-from scripts.v2.liquidity_argument_parser import LiquidityArgumentParser
+from gmx_python_sdk.scripts.v2.order.liquidity_argument_parser import LiquidityArgumentParser
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
+
+config = ConfigManager("arbitrum")
+config.set_config()
 
 parameters = {
     "chain": "arbitrum",
     "market_token_symbol": "ETH",
     "long_token_symbol": "ETH",
     "short_token_symbol": USDC,
     "long_token_usd": 10,
     "short_token_usd": 10
 }
 
-output = LiquidityArgumentParser(is_deposit=True).process_parameters_dictionary(parameters)
+output = LiquidityArgumentParser(
+     config=config,
+     is_deposit=True
+).process_parameters_dictionary(
+     parameters
+)
 ```
 
 
 For Withdraw:
 
 ```python
-from scripts.v2.liquidity_argument_parser import LiquidityArgumentParser
+from gmx_python_sdk.scripts.v2.order.liquidity_argument_parser import LiquidityArgumentParser
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
 
 parameters = {
     "chain": "arbitrum",
     "market_token_symbol": "ETH",
     "out_token_symbol": "ETH",
     "gm_amount": 1
 }
 
-output = LiquidityArgumentParser(is_withdrawal=True).process_parameters_dictionary(parameters)
+output = LiquidityArgumentParser(
+     config=config,
+     is_withdraw=True
+).process_parameters_dictionary(
+     parameters
+)
 ```
 
 #### Closing positions
 
-Instead of passing the parameters to close a position, if you are aware of the market symbol and the direction of the trade you want to close you can pass these to [transform_open_position_to_order_parameters](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/get_positions.py#L46) after collecting all open positions using [get_positions](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/get_positions.py#L13). You can specify the amount of collateral or position size to remove/close as a decimal, eg 0.5 would close/remove 50% of size/collateral:
+Instead of passing the parameters to close a position, if you are aware of the market symbol and the direction of the trade you want to close you can pass these to [transform_open_position_to_order_parameters](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/get_positions.py#L51) after collecting all open positions using [get_positions](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/get_positions.py#L16). You can specify the amount of collateral or position size to remove/close as a decimal, eg 0.5 would close/remove 50% of size/collateral:
 
 ```python
-from get_positions import get_positions, transform_open_position_to_order_parameters
+from gmx_python_sdk.example_scripts.get_positions import get_positions, transform_open_position_to_order_parameters
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
 
-chain = "arbitrum"
+config = ConfigManager(chain='arbitrum')
+config.set_config()
+
+address = None
 market_symbol = "ETH"
 out_token = "ETH"
 is_long = False
 slippage_percent = 0.003
 amount_of_position_to_close = 1
 amount_of_collateral_to_remove = 1
 
 # gets all open positions as a dictionary, which the keys as each position
-positions = get_positions(chain)
+positions = get_positions(
+     config=config,
+     address=address
+)
 
 order_parameters = transform_open_position_to_order_parameters(
-    chain,
-    positions,
-    market_symbol,
-    is_long,
-    slippage_percent,
-    out_token,
-    amount_of_position_to_close,
-    amount_of_collateral_to_remove
+    config=config,
+    positions=positions,
+    market_symbol=market_symbol,
+    is_long=is_long,
+    slippage_percent=slippage_percent,
+    out_token=out_token,
+    amount_of_position_to_close=amount_of_position_to_close,
+    amount_of_collateral_to_remove=amount_of_collateral_to_remove
 )
 ```
 
 ### GMX Stats
 
-A number of stats can be obtained using a wide range of scripts. The overview on how to call these can be found in [get_gmx_stats](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/get_gmx_stats.py). Each method returns a dictionary containing long/short information for a given chain. When initialising the class, pass to_json or to_csv as True to save the output to the [data store](https://github.com/snipermonke01/gmx_python_sdk/tree/main/data_store): 
+A number of stats can be obtained using a wide range of scripts. The overview on how to call these can be found in [get_gmx_stats](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/get_gmx_stats.py). Each method returns a dictionary containing long/short information for a given chain. When initialising the class, pass to_json or to_csv as True to save the output to the [data store](https://github.com/snipermonke01/gmx_python_sdk/tree/main/gmx_python_sdk/data_store): 
 
 ```python
-from get_gmx_stats import GetGMXv2Stats
+from gmx_python_sdk.example_scripts.get_gmx_stats import GetGMXv2Stats
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
 
 to_json = False
 to_csv = False
-chain = "arbitrum"
+
+config = ConfigManager(chain='arbitrum')
+config.set_config()
 
 stats_object = GetGMXv2Stats(
-    to_json=to_json,
-    to_csv=to_csv
+     config=config,
+     to_json=to_json,
+     to_csv=to_csv
 )
 
-liquidity = stats_object.get_available_liquidity(chain=chain)
-borrow_apr = stats_object.get_borrow_apr(chain=chain)
-claimable_fees = stats_object.get_claimable_fees(chain=chain)
-contract_tvl = stats_object.get_contract_tvl(chain=chain)
-funding_apr = stats_object.get_funding_apr(chain=chain)
-gm_prices = stats_object.get_gm_price(chain=chain)
-markets = stats_object.get_available_markets(chain=chain)
-open_interest = stats_object.get_open_interest(chain=chain)
-oracle_prices = stats_object.get_oracle_prices(chain=chain)
-pool_tvl = stats_object.get_pool_tvl(chain=chain)
+liquidity = stats_object.get_available_liquidity()
+borrow_apr = stats_object.get_borrow_apr()
+claimable_fees = stats_object.get_claimable_fees()
+contract_tvl = stats_object.get_contract_tvl()
+funding_apr = stats_object.get_funding_apr()
+gm_prices = stats_object.get_gm_price()
+markets = stats_object.get_available_markets()
+open_interest = stats_object.get_open_interest()
+oracle_prices = stats_object.get_oracle_prices()
+pool_tvl = stats_object.get_pool_tvl()
 ```
 
 ### Debug Mode
 
 It is possible to call IncreaseOrder, DecreaseOrder, SwapOrder, DepositOrder, and WithdrawOrder in debug mode by passing debug_mode=True when initialising the class:
 
 ```python
-from scripts.v2.create_increase_order import IncreaseOrder
+from gmx_python_sdk.scripts.v2.order.create_increase_order import IncreaseOrder
 
 order = IncreaseOrder(
-    chain,
-    market_key,
-    collateral_address,
-    index_token_address,
-    is_long,
-    size_delta_usd,
-    initial_collateral_delta_amount,
-    slippage_percent,
-    swap_path
+    config=config,
+    market_key=market_key,
+    collateral_address=collateral_address,
+    index_token_address=index_token_address,
+    is_long=is_long,
+    size_delta_usd=size_delta_usd,
+    initial_collateral_delta_amount=initial_collateral_delta_amount,
+    slippage_percent=slippage_percent,
+    swap_path=swap_path,
     debug_mode=True
 )
 ```
 
 This will allow you to submit parameters to the order class and build your txn without executing it.
 
 ### Known Limitations
 
 - Avalanche chain not fully tested.
 - A high rate limit RPC is required to read multiple sets of stats successively.
 - Possible to specify out token not the long/short of the GM market when withdrawing,
   but it will fail and return GM tokens to users wallet.
+- Testnet is currently NOT supported
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/datastore.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/datastore.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/depositvault.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/depositvault.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/eventemitter.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/eventemitter.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/exchangerouter.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/exchangerouter.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/ordervault.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/ordervault.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/syntheticsreader.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/syntheticsreader.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/syntheticsrouter.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/syntheticsrouter.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/arbitrum/withdrawalvault.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/arbitrum/withdrawalvault.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/datastore.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/datastore.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/depositvault.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/depositvault.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/eventemitter.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/eventemitter.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/exchangerouter.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/exchangerouter.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/ordervault.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/ordervault.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/syntheticsreader.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/syntheticsreader.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/syntheticsrouter.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/syntheticsrouter.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/avalanche/withdrawalvault.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/avalanche/withdrawalvault.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/balance_abi.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/balance_abi.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/contracts/token_approval.json` & `gmx_python_sdk-0.0.5/gmx_python_sdk/contracts/token_approval.json`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/__pycache__/get_available_liquidity.cpython-311.pyc` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/__pycache__/get_available_liquidity.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,1109 +1,969 @@
 magic:    0xa70d0d0a
-moddate:  0xbf96e465 (Sun Mar  3 15:26:55 2024 UTC)
-files sz: 12066
+moddate:  0xd9940966 (Sun Mar 31 16:52:41 2024 UTC)
+files sz: 9708
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 4
+   stacksize : 5
    flags     : 0
    code
-      0x9700640064016c005a00640064016c015a01640064016c025a02640064
-      016c035a04640064026c056d055a050100640364046c066d075a07010064
-      0364056c086d095a096d0a5a0a6d0b5a0b6d0c5a0c6d0d5a0d0100640364
-      066c0e6d0f5a0f0100640364076c106d115a110100640364086c126d135a
-      136d145a146d155a156d165a1601000200470064098400640aa6020000ab
-      0200000000000000005a176518640b6b0200000000722302006517640c64
-      0dac0ea6020000ab020000000000000000a0190000000000000000000000
-      000000000000000000640dac0fa6010000ab0100000000000000005a1a64
-      01530064015300
+      0x9700640064016c005a00640064016c015a02640064026c036d035a0301
+      00640064036c046d055a056d065a060100640464056c076d085a08010064
+      0464066c096d0a5a0a0100640464076c0b6d0c5a0c0100640864096c0d6d
+      0e5a0e01006408640a6c0f6d105a106d115a116d125a126d135a13010002
+      004700640b8400640c6508a6030000ab0300000000000000005a14651564
+      0d6b0200000000722302006514640e640fac10a6020000ab020000000000
+      000000a0160000000000000000000000000000000000000000640fac11a6
+      010000ab0100000000000000005a176401530064015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
-                 6 IMPORT_NAME              0 (os)
-                 8 STORE_NAME               0 (os)
+                 6 IMPORT_NAME              0 (time)
+                 8 STORE_NAME               0 (time)
    
-     2          10 LOAD_CONST               0 (0)
+     3          10 LOAD_CONST               0 (0)
                 12 LOAD_CONST               1 (None)
-                14 IMPORT_NAME              1 (json)
-                16 STORE_NAME               1 (json)
+                14 IMPORT_NAME              1 (numpy)
+                16 STORE_NAME               2 (np)
    
-     3          18 LOAD_CONST               0 (0)
-                20 LOAD_CONST               1 (None)
-                22 IMPORT_NAME              2 (time)
-                24 STORE_NAME               2 (time)
-   
-     5          26 LOAD_CONST               0 (0)
-                28 LOAD_CONST               1 (None)
-                30 IMPORT_NAME              3 (numpy)
-                32 STORE_NAME               4 (np)
-   
-     7          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               2 (('numerize',))
-                38 IMPORT_NAME              5 (numerize)
-                40 IMPORT_FROM              5 (numerize)
-                42 STORE_NAME               5 (numerize)
+     4          18 LOAD_CONST               0 (0)
+                20 LOAD_CONST               2 (('numerize',))
+                22 IMPORT_NAME              3 (numerize)
+                24 IMPORT_FROM              3 (numerize)
+                26 STORE_NAME               3 (numerize)
+                28 POP_TOP
+   
+     5          30 LOAD_CONST               0 (0)
+                32 LOAD_CONST               3 (('Tuple', 'Any'))
+                34 IMPORT_NAME              4 (typing)
+                36 IMPORT_FROM              5 (Tuple)
+                38 STORE_NAME               5 (Tuple)
+                40 IMPORT_FROM              6 (Any)
+                42 STORE_NAME               6 (Any)
                 44 POP_TOP
    
-     9          46 LOAD_CONST               3 (1)
-                48 LOAD_CONST               4 (('GetMarkets',))
-                50 IMPORT_NAME              6 (get_markets)
-                52 IMPORT_FROM              7 (GetMarkets)
-                54 STORE_NAME               7 (GetMarkets)
+     7          46 LOAD_CONST               4 (1)
+                48 LOAD_CONST               5 (('GetData',))
+                50 IMPORT_NAME              7 (get)
+                52 IMPORT_FROM              8 (GetData)
+                54 STORE_NAME               8 (GetData)
                 56 POP_TOP
    
-    10          58 LOAD_CONST               3 (1)
-                60 LOAD_CONST               5 (('base_dir', 'execute_threading', 'save_json_file_to_datastore', 'make_timestamped_dataframe', 'save_csv_to_datastore'))
-                62 IMPORT_NAME              8 (gmx_utils)
-                64 IMPORT_FROM              9 (base_dir)
-                66 STORE_NAME               9 (base_dir)
-                68 IMPORT_FROM             10 (execute_threading)
-                70 STORE_NAME              10 (execute_threading)
-                72 IMPORT_FROM             11 (save_json_file_to_datastore)
-                74 STORE_NAME              11 (save_json_file_to_datastore)
-                76 IMPORT_FROM             12 (make_timestamped_dataframe)
-                78 STORE_NAME              12 (make_timestamped_dataframe)
-                80 IMPORT_FROM             13 (save_csv_to_datastore)
-                82 STORE_NAME              13 (save_csv_to_datastore)
-                84 POP_TOP
-   
-    15          86 LOAD_CONST               3 (1)
-                88 LOAD_CONST               6 (('GetOraclePrices',))
-                90 IMPORT_NAME             14 (get_oracle_prices)
-                92 IMPORT_FROM             15 (GetOraclePrices)
-                94 STORE_NAME              15 (GetOraclePrices)
-                96 POP_TOP
-   
-    16          98 LOAD_CONST               3 (1)
-               100 LOAD_CONST               7 (('OpenInterest',))
-               102 IMPORT_NAME             16 (get_open_interest)
-               104 IMPORT_FROM             17 (OpenInterest)
-               106 STORE_NAME              17 (OpenInterest)
-               108 POP_TOP
-   
-    17         110 LOAD_CONST               3 (1)
-               112 LOAD_CONST               8 (('get_datastore_contract', 'pool_amount_key', 'reserve_factor_key', 'open_interest_reserve_factor_key'))
-               114 IMPORT_NAME             18 (keys)
-               116 IMPORT_FROM             19 (get_datastore_contract)
-               118 STORE_NAME              19 (get_datastore_contract)
-               120 IMPORT_FROM             20 (pool_amount_key)
-               122 STORE_NAME              20 (pool_amount_key)
-               124 IMPORT_FROM             21 (reserve_factor_key)
-               126 STORE_NAME              21 (reserve_factor_key)
-               128 IMPORT_FROM             22 (open_interest_reserve_factor_key)
-               130 STORE_NAME              22 (open_interest_reserve_factor_key)
-               132 POP_TOP
-   
-    23         134 PUSH_NULL
-               136 LOAD_BUILD_CLASS
-               138 LOAD_CONST               9 (<code object GetAvailableLiquidity, file "/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk_2/scripts/v2/get_available_liquidity.py", line 23>)
-               140 MAKE_FUNCTION            0
-               142 LOAD_CONST              10 ('GetAvailableLiquidity')
-               144 PRECALL                  2
-               148 CALL                     2
-               158 STORE_NAME              23 (GetAvailableLiquidity)
-   
-   367         160 LOAD_NAME               24 (__name__)
-               162 LOAD_CONST              11 ('__main__')
-               164 COMPARE_OP               2 (==)
-               170 POP_JUMP_FORWARD_IF_FALSE    35 (to 242)
-   
-   368         172 PUSH_NULL
-               174 LOAD_NAME               23 (GetAvailableLiquidity)
+     8          58 LOAD_CONST               4 (1)
+                60 LOAD_CONST               6 (('OraclePrices',))
+                62 IMPORT_NAME              9 (get_oracle_prices)
+                64 IMPORT_FROM             10 (OraclePrices)
+                66 STORE_NAME              10 (OraclePrices)
+                68 POP_TOP
+   
+     9          70 LOAD_CONST               4 (1)
+                72 LOAD_CONST               7 (('OpenInterest',))
+                74 IMPORT_NAME             11 (get_open_interest)
+                76 IMPORT_FROM             12 (OpenInterest)
+                78 STORE_NAME              12 (OpenInterest)
+                80 POP_TOP
+   
+    10          82 LOAD_CONST               8 (2)
+                84 LOAD_CONST               9 (('execute_threading',))
+                86 IMPORT_NAME             13 (gmx_utils)
+                88 IMPORT_FROM             14 (execute_threading)
+                90 STORE_NAME              14 (execute_threading)
+                92 POP_TOP
+   
+    11          94 LOAD_CONST               8 (2)
+                96 LOAD_CONST              10 (('get_datastore_contract', 'pool_amount_key', 'reserve_factor_key', 'open_interest_reserve_factor_key'))
+                98 IMPORT_NAME             15 (keys)
+               100 IMPORT_FROM             16 (get_datastore_contract)
+               102 STORE_NAME              16 (get_datastore_contract)
+               104 IMPORT_FROM             17 (pool_amount_key)
+               106 STORE_NAME              17 (pool_amount_key)
+               108 IMPORT_FROM             18 (reserve_factor_key)
+               110 STORE_NAME              18 (reserve_factor_key)
+               112 IMPORT_FROM             19 (open_interest_reserve_factor_key)
+               114 STORE_NAME              19 (open_interest_reserve_factor_key)
+               116 POP_TOP
+   
+    17         118 PUSH_NULL
+               120 LOAD_BUILD_CLASS
+               122 LOAD_CONST              11 (<code object GetAvailableLiquidity, file "/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk/scripts/v2/get/get_available_liquidity.py", line 17>)
+               124 MAKE_FUNCTION            0
+               126 LOAD_CONST              12 ('GetAvailableLiquidity')
+               128 LOAD_NAME                8 (GetData)
+               130 PRECALL                  3
+               134 CALL                     3
+               144 STORE_NAME              20 (GetAvailableLiquidity)
+   
+   285         146 LOAD_NAME               21 (__name__)
+               148 LOAD_CONST              13 ('__main__')
+               150 COMPARE_OP               2 (==)
+               156 POP_JUMP_FORWARD_IF_FALSE    35 (to 228)
+   
+   286         158 PUSH_NULL
+               160 LOAD_NAME               20 (GetAvailableLiquidity)
+   
+   287         162 LOAD_CONST              14 ('arbitrum')
+   
+   288         164 LOAD_CONST              15 (False)
+   
+   286         166 KW_NAMES                16
+               168 PRECALL                  2
+               172 CALL                     2
+   
+   289         182 LOAD_METHOD             22 (get_data)
+   
+   290         204 LOAD_CONST              15 (False)
+   
+   289         206 KW_NAMES                17
+               208 PRECALL                  1
+               212 CALL                     1
+   
+   286         222 STORE_NAME              23 (data)
+               224 LOAD_CONST               1 (None)
+               226 RETURN_VALUE
    
-   369         176 LOAD_CONST              12 ('arbitrum')
-   
-   370         178 LOAD_CONST              13 (False)
-   
-   368         180 KW_NAMES                14
-               182 PRECALL                  2
-               186 CALL                     2
-   
-   371         196 LOAD_METHOD             25 (get_available_liquidity)
-   
-   372         218 LOAD_CONST              13 (False)
-   
-   371         220 KW_NAMES                15
-               222 PRECALL                  1
-               226 CALL                     1
-   
-   368         236 STORE_NAME              26 (data)
-               238 LOAD_CONST               1 (None)
-               240 RETURN_VALUE
-   
-   367     >>  242 LOAD_CONST               1 (None)
-               244 RETURN_VALUE
+   285     >>  228 LOAD_CONST               1 (None)
+               230 RETURN_VALUE
    consts
       0
       None
       ('numerize',)
+      ('Tuple', 'Any')
       1
-      ('GetMarkets',)
-      ('base_dir', 'execute_threading', 'save_json_file_to_datastore', 'make_timestamped_dataframe', 'save_csv_to_datastore')
-      ('GetOraclePrices',)
+      ('GetData',)
+      ('OraclePrices',)
       ('OpenInterest',)
+      2
+      ('execute_threading',)
       ('get_datastore_contract', 'pool_amount_key', 'reserve_factor_key', 'open_interest_reserve_factor_key')
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 6
+         stacksize : 11
          flags     : 0
          code
-            0x970065005a0164005a02640e64026503640365046604640484055a0509
-            00640f64056504640665046604640784055a06640884005a076409650364
-            0a6503640b65046606640c84045a08640d5300
-          23           0 RESUME                   0
-                       2 LOAD_NAME                0 (__name__)
-                       4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('GetAvailableLiquidity')
-                       8 STORE_NAME               2 (__qualname__)
-         
-          25          10 LOAD_CONST              14 ((False,))
-                      12 LOAD_CONST               2 ('chain')
-                      14 LOAD_NAME                3 (str)
-                      16 LOAD_CONST               3 ('use_local_datastore')
-                      18 LOAD_NAME                4 (bool)
-                      20 BUILD_TUPLE              4
-                      22 LOAD_CONST               4 (<code object __init__, file "/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk_2/scripts/v2/get_available_liquidity.py", line 25>)
-                      24 MAKE_FUNCTION            5 (defaults, annotations)
-                      26 STORE_NAME               5 (__init__)
+            0x8700970065005a0164005a02640b640265036403650466048800660164
+            04840d5a05640565066602640684045a0764076503640865036409650464
+            0565086509650965096603190000000000000000006608640a84045a0a88
+            0078015a0b5300
+                       0 MAKE_CELL                0 (__class__)
          
-          31          28 NOP
+          17           2 RESUME                   0
+                       4 LOAD_NAME                0 (__name__)
+                       6 STORE_NAME               1 (__module__)
+                       8 LOAD_CONST               0 ('GetAvailableLiquidity')
+                      10 STORE_NAME               2 (__qualname__)
          
-          30          30 LOAD_CONST              15 ((False, False))
-                      32 LOAD_CONST               5 ('to_json')
+          18          12 LOAD_CONST              11 ((False,))
+                      14 LOAD_CONST               2 ('chain')
+                      16 LOAD_NAME                3 (str)
+                      18 LOAD_CONST               3 ('use_local_datastore')
+                      20 LOAD_NAME                4 (bool)
+                      22 BUILD_TUPLE              4
+                      24 LOAD_CLOSURE             0 (__class__)
+                      26 BUILD_TUPLE              1
+                      28 LOAD_CONST               4 (<code object __init__, file "/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk/scripts/v2/get/get_available_liquidity.py", line 18>)
+                      30 MAKE_FUNCTION           13 (defaults, annotations, closure)
+                      32 STORE_NAME               5 (__init__)
          
-          31          34 LOAD_NAME                4 (bool)
+          21          34 LOAD_CONST               5 ('return')
+                      36 LOAD_NAME                6 (dict)
+                      38 BUILD_TUPLE              2
+                      40 LOAD_CONST               6 (<code object _get_data_processing, file "/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk/scripts/v2/get/get_available_liquidity.py", line 21>)
+                      42 MAKE_FUNCTION            4 (annotations)
+                      44 STORE_NAME               7 (_get_data_processing)
          
-          30          36 LOAD_CONST               6 ('to_csv')
+         222          46 LOAD_CONST               7 ('market')
+                      48 LOAD_NAME                3 (str)
+                      50 LOAD_CONST               8 ('token')
+                      52 LOAD_NAME                3 (str)
+                      54 LOAD_CONST               9 ('is_long')
+                      56 LOAD_NAME                4 (bool)
+                      58 LOAD_CONST               5 ('return')
          
-          31          38 LOAD_NAME                4 (bool)
+         223          60 LOAD_NAME                8 (Tuple)
+                      62 LOAD_NAME                9 (Any)
+                      64 LOAD_NAME                9 (Any)
+                      66 LOAD_NAME                9 (Any)
+                      68 BUILD_TUPLE              3
+                      70 BINARY_SUBSCR
          
-          30          40 BUILD_TUPLE              4
-                      42 LOAD_CONST               7 (<code object get_available_liquidity, file "/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk_2/scripts/v2/get_available_liquidity.py", line 30>)
-                      44 MAKE_FUNCTION            5 (defaults, annotations)
-                      46 STORE_NAME               6 (get_available_liquidity)
-         
-          74          48 LOAD_CONST               8 (<code object _available_liquidity, file "/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk_2/scripts/v2/get_available_liquidity.py", line 74>)
-                      50 MAKE_FUNCTION            0
-                      52 STORE_NAME               7 (_available_liquidity)
-         
-         309          54 LOAD_CONST               9 ('market')
-                      56 LOAD_NAME                3 (str)
-                      58 LOAD_CONST              10 ('token')
-                      60 LOAD_NAME                3 (str)
-                      62 LOAD_CONST              11 ('is_long')
-                      64 LOAD_NAME                4 (bool)
-                      66 BUILD_TUPLE              6
-                      68 LOAD_CONST              12 (<code object get_max_reserved_usd, file "/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk_2/scripts/v2/get_available_liquidity.py", line 309>)
-                      70 MAKE_FUNCTION            4 (annotations)
-                      72 STORE_NAME               8 (get_max_reserved_usd)
-                      74 LOAD_CONST              13 (None)
-                      76 RETURN_VALUE
+         222          80 BUILD_TUPLE              8
+                      82 LOAD_CONST              10 (<code object get_max_reserved_usd, file "/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk/scripts/v2/get/get_available_liquidity.py", line 222>)
+                      84 MAKE_FUNCTION            4 (annotations)
+                      86 STORE_NAME              10 (get_max_reserved_usd)
+                      88 LOAD_CLOSURE             0 (__class__)
+                      90 COPY                     1
+                      92 STORE_NAME              11 (__classcell__)
+                      94 RETURN_VALUE
          consts
             'GetAvailableLiquidity'
             False
             'chain'
             'use_local_datastore'
             code
                argcount  : 3
                nlocals   : 3
-               stacksize : 2
+               stacksize : 3
                flags     : 3
                code
-                  0x97007c017c005f0000000000000000007c027c005f0100000000000000
-                  0064005300
-                25           0 RESUME                   0
-               
-                27           2 LOAD_FAST                1 (chain)
-                             4 LOAD_FAST                0 (self)
-                             6 STORE_ATTR               0 (chain)
-               
-                28          16 LOAD_FAST                2 (use_local_datastore)
-                            18 LOAD_FAST                0 (self)
-                            20 STORE_ATTR               1 (use_local_datastore)
-                            30 LOAD_CONST               0 (None)
-                            32 RETURN_VALUE
+                  0x95019700740100000000000000000000a6000000ab0000000000000000
+                  00a00100000000000000000000000000000000000000007c01a6010000ab
+                  010000000000000000010064005300
+                             0 COPY_FREE_VARS           1
+               
+                18           2 RESUME                   0
+               
+                19           4 LOAD_GLOBAL              1 (NULL + super)
+                            16 PRECALL                  0
+                            20 CALL                     0
+                            30 LOAD_METHOD              1 (__init__)
+                            52 LOAD_FAST                1 (chain)
+                            54 PRECALL                  1
+                            58 CALL                     1
+                            68 POP_TOP
+                            70 LOAD_CONST               0 (None)
+                            72 RETURN_VALUE
                consts
                   None
-               names      ('chain', 'use_local_datastore')
+               names      ('super', '__init__')
                varnames   ('self', 'chain', 'use_local_datastore')
-               freevars   ()
+               freevars   ('__class__',)
                cellvars   ()
-               filename   '/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk_2/scripts/v2/get_available_liquidity.py'
+               filename   '/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk/scripts/v2/get/get_available_liquidity.py'
                name       '__init__'
-               firstlineno 25
-               lnotab 0x02020e01
-            'to_json'
-            'to_csv'
-            code
-               argcount  : 3
-               nlocals   : 6
-               stacksize : 5
-               flags     : 3
-               code
-                  0x97007c00a0000000000000000000000000000000000000000000a60000
-                  00ab0000000000000000007d037c01722874030000000000000000000064
-                  01a00200000000000000000000000000000000000000007c006a03000000
-                  0000000000a6010000ab0100000000000000007c03a6020000ab02000000
-                  000000000001007c02727c7409000000000000000000007c036402190000
-                  00000000000000a6010000ab0100000000000000007d0474090000000000
-                  00000000007c03640319000000000000000000a6010000ab010000000000
-                  0000007d05740b000000000000000000006404a002000000000000000000
-                  00000000000000000000007c006a030000000000000000a6010000ab0100
-                  000000000000007c04a6020000ab0200000000000000000100740b000000
-                  000000000000006405a00200000000000000000000000000000000000000
-                  007c006a030000000000000000a6010000ab0100000000000000007c05a6
-                  020000ab0200000000000000000100640653007c035300
-                30           0 RESUME                   0
-               
-                51           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (_available_liquidity)
-                            26 PRECALL                  0
-                            30 CALL                     0
-                            40 STORE_FAST               3 (data)
-               
-                53          42 LOAD_FAST                1 (to_json)
-                            44 POP_JUMP_FORWARD_IF_FALSE    40 (to 126)
-               
-                54          46 LOAD_GLOBAL              3 (NULL + save_json_file_to_datastore)
-               
-                55          58 LOAD_CONST               1 ('{}_available_liquidity.json')
-                            60 LOAD_METHOD              2 (format)
-                            82 LOAD_FAST                0 (self)
-                            84 LOAD_ATTR                3 (chain)
-                            94 PRECALL                  1
-                            98 CALL                     1
-               
-                56         108 LOAD_FAST                3 (data)
-               
-                54         110 PRECALL                  2
-                           114 CALL                     2
-                           124 POP_TOP
-               
-                59     >>  126 LOAD_FAST                2 (to_csv)
-                           128 POP_JUMP_FORWARD_IF_FALSE   124 (to 378)
-               
-                60         130 LOAD_GLOBAL              9 (NULL + make_timestamped_dataframe)
-                           142 LOAD_FAST                3 (data)
-                           144 LOAD_CONST               2 ('long')
-                           146 BINARY_SUBSCR
-                           156 PRECALL                  1
-                           160 CALL                     1
-                           170 STORE_FAST               4 (long_dataframe)
-               
-                61         172 LOAD_GLOBAL              9 (NULL + make_timestamped_dataframe)
-                           184 LOAD_FAST                3 (data)
-                           186 LOAD_CONST               3 ('short')
-                           188 BINARY_SUBSCR
-                           198 PRECALL                  1
-                           202 CALL                     1
-                           212 STORE_FAST               5 (short_dataframe)
-               
-                62         214 LOAD_GLOBAL             11 (NULL + save_csv_to_datastore)
-               
-                63         226 LOAD_CONST               4 ('{}_long_available_liquidity.csv')
-                           228 LOAD_METHOD              2 (format)
-                           250 LOAD_FAST                0 (self)
-                           252 LOAD_ATTR                3 (chain)
-                           262 PRECALL                  1
-                           266 CALL                     1
-               
-                64         276 LOAD_FAST                4 (long_dataframe)
-               
-                62         278 PRECALL                  2
-                           282 CALL                     2
-                           292 POP_TOP
-               
-                66         294 LOAD_GLOBAL             11 (NULL + save_csv_to_datastore)
-               
-                67         306 LOAD_CONST               5 ('{}_short_available_liquidity.csv')
-                           308 LOAD_METHOD              2 (format)
-                           330 LOAD_FAST                0 (self)
-                           332 LOAD_ATTR                3 (chain)
-                           342 PRECALL                  1
-                           346 CALL                     1
-               
-                68         356 LOAD_FAST                5 (short_dataframe)
-               
-                66         358 PRECALL                  2
-                           362 CALL                     2
-                           372 POP_TOP
-                           374 LOAD_CONST               6 (None)
-                           376 RETURN_VALUE
-               
-                72     >>  378 LOAD_FAST                3 (data)
-                           380 RETURN_VALUE
-               consts
-                  '\n        Call to get the available liquidity across all pools on a given\n        chain defined in class init. Pass either to_json or to_csv to save\n        locally in datastore\n\n        Parameters\n        ----------\n        to_json : bool, optional\n            save output to json file. The default is False.\n        to_csv : bool, optional\n            save out to csv file. The default is False.\n\n        Returns\n        -------\n        data : dict\n            dictionary of data.\n\n        '
-                  '{}_available_liquidity.json'
-                  'long'
-                  'short'
-                  '{}_long_available_liquidity.csv'
-                  '{}_short_available_liquidity.csv'
-                  None
-               names      ('_available_liquidity', 'save_json_file_to_datastore', 'format', 'chain', 'make_timestamped_dataframe', 'save_csv_to_datastore')
-               varnames   ('self', 'to_json', 'to_csv', 'data', 'long_dataframe', 'short_dataframe')
-               freevars   ()
-               cellvars   ()
-               filename   '/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk_2/scripts/v2/get_available_liquidity.py'
-               name       'get_available_liquidity'
-               firstlineno 30
-               lnotab
-                  0x0215280204010c01320102fe100504012a012a010c01320102fe10040c
-                  01320102fe1406
+               firstlineno 18
+               lnotab 0x0401
+            'return'
             code
                argcount  : 1
-               nlocals   : 45
+               nlocals   : 43
                stacksize : 14
                flags     : 3
                code
-                  0x97007c006a000000000000000000725e7403000000000000000000006a
-                  020000000000000000740700000000000000000000740800000000000000
-                  0000006a050000000000000000a006000000000000000000000000000000
-                  0000000000740e0000000000000000000064016402a00800000000000000
-                  000000000000000000000000007c006a090000000000000000a6010000ab
-                  010000000000000000a6030000ab030000000000000000a6010000ab0100
-                  00000000000000a6010000ab0100000000000000007d016e297415000000
-                  000000000000007c006a090000000000000000ac03a6010000ab01000000
-                  0000000000a00b00000000000000000000000000000000000000006404ac
-                  05a6010000ab0100000000000000007d017419000000000000000000007c
-                  006a090000000000000000ac03a6010000ab010000000000000000a00d00
-                  00000000000000000000000000000000000000a6000000ab000000000000
-                  0000007d026900690064069c027d03741d000000000000000000006407a6
-                  010000ab010000000000000000010067007d0467007d0567007d0667007d
-                  0767007d0867007d0967007d0a67007d0b67007d0c67007d0d67007d0e67
-                  007d0f7c02440090015d8b7d107c027c1019000000000000000000640819
-                  0000000000000000007d1164097c11760072018c167c077c1167017a0000
-                  007d077c027c1019000000000000000000640a190000000000000000007d
-                  127c00a00f00000000000000000000000000000000000000007c107c1264
-                  0ba6030000ab0300000000000000005c0300007d137d147d15640c640d7c
-                  027c1019000000000000000000640e19000000000000000000640f190000
-                  000000000000007a0000007a0800007d167c047c01641019000000000000
-                  0000007c111900000000000000000067017a0000007d047c087c1367017a
-                  0000007d087c097c1467017a0000007d097c0a7c1567017a0000007d0a7c
-                  0e7c1667017a0000007d0e7c027c10190000000000000000006411190000
-                  000000000000007d177c00a00f0000000000000000000000000000000000
-                  0000007c107c176404a6030000ab0300000000000000005c0300007d187d
-                  197d1a640c640d7c027c1019000000000000000000641219000000000000
-                  000000640f190000000000000000007a0000007a0800007d1b7c057c0164
-                  13190000000000000000007c111900000000000000000067017a0000007d
-                  057c0b7c1867017a0000007d0b7c0c7c1967017a0000007d0c7c0d7c1a67
-                  017a0000007d0d7c0f7c1b67017a0000007d0f7421000000000000000000
-                  007c006a090000000000000000ac03a6010000ab010000000000000000a0
-                  110000000000000000000000000000000000000000a6000000ab00000000
-                  00000000007d1c640c640d7c027c1019000000000000000000640e190000
-                  00000000000000640f190000000000000000007a0a00007a0800007d1d74
-                  25000000000000000000006a130000000000000000742900000000000000
-                  0000007c1c7c1219000000000000000000641419000000000000000000a6
-                  010000ab0100000000000000007c1d7a0b00007429000000000000000000
-                  007c1c7c1219000000000000000000641519000000000000000000a60100
-                  00ab0100000000000000007c1d7a0b00006702a6010000ab010000000000
-                  0000007d1e7c067c1e67017a0000007d0690018c8d742b00000000000000
-                  0000007c08a6010000ab0100000000000000007d1f742d00000000000000
-                  0000006a1700000000000000006416a6010000ab01000000000000000001
-                  00742b000000000000000000007c0ba6010000ab0100000000000000007d
-                  20742d000000000000000000006a1700000000000000006416a6010000ab
-                  0100000000000000000100742b000000000000000000007c09a6010000ab
-                  0100000000000000007d21742d000000000000000000006a170000000000
-                  0000006416a6010000ab0100000000000000000100742b00000000000000
-                  0000007c0ca6010000ab0100000000000000007d22742d00000000000000
-                  0000006a1700000000000000006416a6010000ab01000000000000000001
-                  00742b000000000000000000007c0aa6010000ab0100000000000000007d
-                  23742d000000000000000000006a1700000000000000006416a6010000ab
-                  0100000000000000000100742b000000000000000000007c0da6010000ab
-                  0100000000000000007d247431000000000000000000007c1f7c207c217c
-                  227c237c247c047c057c067c077c0e7c0fa60c0000ab0c00000000000000
-                  0044005de55c0c00007d137d187d147d197d157d1a7d257d267d1e7d277d
-                  167d1b741d000000000000000000007c27a6010000ab0100000000000000
-                  0001007c157c146b000000000072027c157d147c137c147a0500007d287c
-                  287c167a0b00007c1e7a0500007d297c297429000000000000000000007c
-                  25a6010000ab0100000000000000007a0a00007d2a741d00000000000000
-                  0000006417a0080000000000000000000000000000000000000000743300
-                  0000000000000000006a1900000000000000007c2aa6010000ab01000000
-                  0000000000a6010000ab010000000000000000a6010000ab010000000000
-                  00000001007c2a7c036410190000000000000000007c273c0000007c1a7c
-                  196b000000000072027c1a7d197c187c197a0500007d2b7c2b7c1b7a0b00
-                  007429000000000000000000007c26a6010000ab0100000000000000007a
-                  0a00007d2c741d000000000000000000006418a008000000000000000000
-                  00000000000000000000007433000000000000000000006a190000000000
-                  0000007c2ca6010000ab010000000000000000a6010000ab010000000000
-                  000000a6010000ab01000000000000000001007c2c7c0364131900000000
-                  00000000007c273c0000008ce67c035300
-                74           0 RESUME                   0
-               
-                84           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (use_local_datastore)
-                            14 POP_JUMP_FORWARD_IF_FALSE    94 (to 204)
-               
-                85          16 LOAD_GLOBAL              3 (NULL + json)
-                            28 LOAD_ATTR                2 (load)
-               
-                86          38 LOAD_GLOBAL              7 (NULL + open)
-               
-                87          50 LOAD_GLOBAL              8 (os)
-                            62 LOAD_ATTR                5 (path)
-                            72 LOAD_METHOD              6 (join)
-               
-                88          94 LOAD_GLOBAL             14 (base_dir)
-               
-                89         106 LOAD_CONST               1 ('data_store')
-               
-                90         108 LOAD_CONST               2 ('{}_open_interest.json')
-                           110 LOAD_METHOD              8 (format)
-                           132 LOAD_FAST                0 (self)
-                           134 LOAD_ATTR                9 (chain)
-                           144 PRECALL                  1
-                           148 CALL                     1
-               
-                87         158 PRECALL                  3
-                           162 CALL                     3
-               
-                86         172 PRECALL                  1
-                           176 CALL                     1
-               
-                85         186 PRECALL                  1
-                           190 CALL                     1
-                           200 STORE_FAST               1 (open_interest)
-                           202 JUMP_FORWARD            41 (to 286)
-               
-                95     >>  204 LOAD_GLOBAL             21 (NULL + OpenInterest)
-                           216 LOAD_FAST                0 (self)
-                           218 LOAD_ATTR                9 (chain)
-                           228 KW_NAMES                 3
-                           230 PRECALL                  1
-                           234 CALL                     1
-                           244 LOAD_METHOD             11 (call_open_interest)
-               
-                96         266 LOAD_CONST               4 (False)
-               
-                95         268 KW_NAMES                 5
-                           270 PRECALL                  1
-                           274 CALL                     1
-                           284 STORE_FAST               1 (open_interest)
-               
-                99     >>  286 LOAD_GLOBAL             25 (NULL + GetMarkets)
-                           298 LOAD_FAST                0 (self)
-                           300 LOAD_ATTR                9 (chain)
-                           310 KW_NAMES                 3
-                           312 PRECALL                  1
-                           316 CALL                     1
-                           326 LOAD_METHOD             13 (get_available_markets)
-                           348 PRECALL                  0
-                           352 CALL                     0
-                           362 STORE_FAST               2 (markets)
-               
-               101         364 BUILD_MAP                0
-               
-               103         366 BUILD_MAP                0
-               
-               100         368 LOAD_CONST               6 (('long', 'short'))
-                           370 BUILD_CONST_KEY_MAP      2
-                           372 STORE_FAST               3 (available_liquidity)
-               
-               107         374 LOAD_GLOBAL             29 (NULL + print)
-                           386 LOAD_CONST               7 ('\nGMX v2 Available Liquidity\n')
-                           388 PRECALL                  1
-                           392 CALL                     1
-                           402 POP_TOP
-               
-               109         404 BUILD_LIST               0
-                           406 STORE_FAST               4 (reserved_long_list)
-               
-               110         408 BUILD_LIST               0
-                           410 STORE_FAST               5 (reserved_short_list)
-               
-               111         412 BUILD_LIST               0
-                           414 STORE_FAST               6 (token_price_list)
-               
-               112         416 BUILD_LIST               0
-                           418 STORE_FAST               7 (mapper)
-               
-               113         420 BUILD_LIST               0
-                           422 STORE_FAST               8 (long_pool_amount_list)
-               
-               114         424 BUILD_LIST               0
-                           426 STORE_FAST               9 (long_reserve_factor_list)
-               
-               115         428 BUILD_LIST               0
-                           430 STORE_FAST              10 (long_open_interest_reserve_factor_list)
-               
-               116         432 BUILD_LIST               0
-                           434 STORE_FAST              11 (short_pool_amount_list)
-               
-               117         436 BUILD_LIST               0
-                           438 STORE_FAST              12 (short_reserve_factor_list)
-               
-               118         440 BUILD_LIST               0
-                           442 STORE_FAST              13 (short_open_interest_reserve_factor_list)
-               
-               119         444 BUILD_LIST               0
-                           446 STORE_FAST              14 (long_precision_list)
-               
-               120         448 BUILD_LIST               0
-                           450 STORE_FAST              15 (short_precision_list)
-               
-               122         452 LOAD_FAST                2 (markets)
-                           454 GET_ITER
-                       >>  456 EXTENDED_ARG             1
-                           458 FOR_ITER               395 (to 1250)
-                           460 STORE_FAST              16 (market_key)
-               
-               125         462 LOAD_FAST                2 (markets)
-                           464 LOAD_FAST               16 (market_key)
-                           466 BINARY_SUBSCR
-                           476 LOAD_CONST               8 ('market_symbol')
-                           478 BINARY_SUBSCR
-                           488 STORE_FAST              17 (market_symbol)
-               
-               126         490 LOAD_CONST               9 ('SWAP')
-                           492 LOAD_FAST               17 (market_symbol)
-                           494 CONTAINS_OP              0
-                           496 POP_JUMP_FORWARD_IF_FALSE     1 (to 500)
-               
-               127         498 JUMP_BACKWARD           22 (to 456)
-               
-               130     >>  500 LOAD_FAST                7 (mapper)
-                           502 LOAD_FAST               17 (market_symbol)
-                           504 BUILD_LIST               1
-                           506 BINARY_OP                0 (+)
-                           510 STORE_FAST               7 (mapper)
-               
-               133         512 LOAD_FAST                2 (markets)
-                           514 LOAD_FAST               16 (market_key)
-                           516 BINARY_SUBSCR
-                           526 LOAD_CONST              10 ('long_token_address')
-                           528 BINARY_SUBSCR
-                           538 STORE_FAST              18 (long_token_address)
-               
-               135         540 LOAD_FAST                0 (self)
-                           542 LOAD_METHOD             15 (get_max_reserved_usd)
-               
-               136         564 LOAD_FAST               16 (market_key)
-               
-               137         566 LOAD_FAST               18 (long_token_address)
-               
-               138         568 LOAD_CONST              11 (True)
-               
-               135         570 PRECALL                  3
-                           574 CALL                     3
-               
-               134         584 UNPACK_SEQUENCE          3
-                           588 STORE_FAST              19 (long_pool_amount)
-                           590 STORE_FAST              20 (long_reserve_factor)
-               
-               135         592 STORE_FAST              21 (long_open_interest_reserve_factor)
-               
-               140         594 LOAD_CONST              12 (10)
-               
-               141         596 LOAD_CONST              13 (30)
-                           598 LOAD_FAST                2 (markets)
-                           600 LOAD_FAST               16 (market_key)
-                           602 BINARY_SUBSCR
-                           612 LOAD_CONST              14 ('long_token_metadata')
-                           614 BINARY_SUBSCR
-                           624 LOAD_CONST              15 ('decimals')
-                           626 BINARY_SUBSCR
-                           636 BINARY_OP                0 (+)
-               
-               140         640 BINARY_OP                8 (**)
-                           644 STORE_FAST              22 (long_precision)
-               
-               146         646 LOAD_FAST                4 (reserved_long_list)
-                           648 LOAD_FAST                1 (open_interest)
-                           650 LOAD_CONST              16 ('long')
-                           652 BINARY_SUBSCR
-                           662 LOAD_FAST               17 (market_symbol)
-                           664 BINARY_SUBSCR
-                           674 BUILD_LIST               1
-                           676 BINARY_OP                0 (+)
-               
-               145         680 STORE_FAST               4 (reserved_long_list)
-               
-               148         682 LOAD_FAST                8 (long_pool_amount_list)
-                           684 LOAD_FAST               19 (long_pool_amount)
-                           686 BUILD_LIST               1
-                           688 BINARY_OP                0 (+)
-                           692 STORE_FAST               8 (long_pool_amount_list)
-               
-               150         694 LOAD_FAST                9 (long_reserve_factor_list)
-                           696 LOAD_FAST               20 (long_reserve_factor)
-                           698 BUILD_LIST               1
-                           700 BINARY_OP                0 (+)
-               
-               149         704 STORE_FAST               9 (long_reserve_factor_list)
-               
-               153         706 LOAD_FAST               10 (long_open_interest_reserve_factor_list)
-               
-               154         708 LOAD_FAST               21 (long_open_interest_reserve_factor)
-                           710 BUILD_LIST               1
-               
-               153         712 BINARY_OP                0 (+)
-               
-               152         716 STORE_FAST              10 (long_open_interest_reserve_factor_list)
-               
-               156         718 LOAD_FAST               14 (long_precision_list)
-                           720 LOAD_FAST               22 (long_precision)
-                           722 BUILD_LIST               1
-                           724 BINARY_OP                0 (+)
-                           728 STORE_FAST              14 (long_precision_list)
-               
-               159         730 LOAD_FAST                2 (markets)
-                           732 LOAD_FAST               16 (market_key)
-                           734 BINARY_SUBSCR
-                           744 LOAD_CONST              17 ('short_token_address')
-                           746 BINARY_SUBSCR
-                           756 STORE_FAST              23 (short_token_address)
-               
-               164         758 LOAD_FAST                0 (self)
-                           760 LOAD_METHOD             15 (get_max_reserved_usd)
-               
-               165         782 LOAD_FAST               16 (market_key)
-               
-               166         784 LOAD_FAST               23 (short_token_address)
-               
-               167         786 LOAD_CONST               4 (False)
-               
-               164         788 PRECALL                  3
-                           792 CALL                     3
-               
-               160         802 UNPACK_SEQUENCE          3
-               
-               161         806 STORE_FAST              24 (short_pool_amount)
-               
-               162         808 STORE_FAST              25 (short_reserve_factor)
-               
-               163         810 STORE_FAST              26 (short_open_interest_reserve_factor)
-               
-               169         812 LOAD_CONST              12 (10)
-               
-               170         814 LOAD_CONST              13 (30)
-                           816 LOAD_FAST                2 (markets)
-                           818 LOAD_FAST               16 (market_key)
-                           820 BINARY_SUBSCR
-                           830 LOAD_CONST              18 ('short_token_metadata')
-                           832 BINARY_SUBSCR
-                           842 LOAD_CONST              15 ('decimals')
-                           844 BINARY_SUBSCR
-                           854 BINARY_OP                0 (+)
-               
-               169         858 BINARY_OP                8 (**)
-                           862 STORE_FAST              27 (short_precision)
-               
-               175         864 LOAD_FAST                5 (reserved_short_list)
-                           866 LOAD_FAST                1 (open_interest)
-                           868 LOAD_CONST              19 ('short')
-                           870 BINARY_SUBSCR
-                           880 LOAD_FAST               17 (market_symbol)
-                           882 BINARY_SUBSCR
-                           892 BUILD_LIST               1
-                           894 BINARY_OP                0 (+)
-               
-               174         898 STORE_FAST               5 (reserved_short_list)
-               
-               178         900 LOAD_FAST               11 (short_pool_amount_list)
-                           902 LOAD_FAST               24 (short_pool_amount)
-                           904 BUILD_LIST               1
-                           906 BINARY_OP                0 (+)
-               
-               177         910 STORE_FAST              11 (short_pool_amount_list)
-               
-               181         912 LOAD_FAST               12 (short_reserve_factor_list)
-                           914 LOAD_FAST               25 (short_reserve_factor)
-                           916 BUILD_LIST               1
-                           918 BINARY_OP                0 (+)
-               
-               180         922 STORE_FAST              12 (short_reserve_factor_list)
-               
-               184         924 LOAD_FAST               13 (short_open_interest_reserve_factor_list)
-               
-               185         926 LOAD_FAST               26 (short_open_interest_reserve_factor)
-                           928 BUILD_LIST               1
-               
-               184         930 BINARY_OP                0 (+)
-               
-               183         934 STORE_FAST              13 (short_open_interest_reserve_factor_list)
-               
-               187         936 LOAD_FAST               15 (short_precision_list)
-                           938 LOAD_FAST               27 (short_precision)
-                           940 BUILD_LIST               1
-                           942 BINARY_OP                0 (+)
-                           946 STORE_FAST              15 (short_precision_list)
-               
-               190         948 LOAD_GLOBAL             33 (NULL + GetOraclePrices)
-                           960 LOAD_FAST                0 (self)
-                           962 LOAD_ATTR                9 (chain)
-                           972 KW_NAMES                 3
-                           974 PRECALL                  1
-                           978 CALL                     1
-                           988 LOAD_METHOD             17 (get_recent_prices)
-                          1010 PRECALL                  0
-                          1014 CALL                     0
-                          1024 STORE_FAST              28 (prices)
-               
-               191        1026 LOAD_CONST              12 (10)
-               
-               192        1028 LOAD_CONST              13 (30)
-                          1030 LOAD_FAST                2 (markets)
-                          1032 LOAD_FAST               16 (market_key)
-                          1034 BINARY_SUBSCR
-                          1044 LOAD_CONST              14 ('long_token_metadata')
-                          1046 BINARY_SUBSCR
-                          1056 LOAD_CONST              15 ('decimals')
-                          1058 BINARY_SUBSCR
-                          1068 BINARY_OP               10 (-)
-               
-               191        1072 BINARY_OP                8 (**)
-                          1076 STORE_FAST              29 (oracle_precision)
-               
-               195        1078 LOAD_GLOBAL             37 (NULL + np)
-                          1090 LOAD_ATTR               19 (median)
-               
-               197        1100 LOAD_GLOBAL             41 (NULL + float)
-               
-               198        1112 LOAD_FAST               28 (prices)
-                          1114 LOAD_FAST               18 (long_token_address)
-                          1116 BINARY_SUBSCR
-                          1126 LOAD_CONST              20 ('maxPriceFull')
-                          1128 BINARY_SUBSCR
-               
-               197        1138 PRECALL                  1
-                          1142 CALL                     1
-               
-               199        1152 LOAD_FAST               29 (oracle_precision)
-               
-               197        1154 BINARY_OP               11 (/)
-               
-               200        1158 LOAD_GLOBAL             41 (NULL + float)
-               
-               201        1170 LOAD_FAST               28 (prices)
-                          1172 LOAD_FAST               18 (long_token_address)
-                          1174 BINARY_SUBSCR
-                          1184 LOAD_CONST              21 ('minPriceFull')
-                          1186 BINARY_SUBSCR
-               
-               200        1196 PRECALL                  1
-                          1200 CALL                     1
-               
-               202        1210 LOAD_FAST               29 (oracle_precision)
-               
-               200        1212 BINARY_OP               11 (/)
-               
-               196        1216 BUILD_LIST               2
-               
-               195        1218 PRECALL                  1
-                          1222 CALL                     1
-                          1232 STORE_FAST              30 (token_price)
-               
-               207        1234 LOAD_FAST                6 (token_price_list)
-                          1236 LOAD_FAST               30 (token_price)
-                          1238 BUILD_LIST               1
-                          1240 BINARY_OP                0 (+)
-                          1244 STORE_FAST               6 (token_price_list)
-                          1246 EXTENDED_ARG             1
-                          1248 JUMP_BACKWARD          397 (to 456)
-               
-               211     >> 1250 LOAD_GLOBAL             43 (NULL + execute_threading)
-                          1262 LOAD_FAST                8 (long_pool_amount_list)
-                          1264 PRECALL                  1
-                          1268 CALL                     1
-                          1278 STORE_FAST              31 (long_pool_amount_output)
-               
-               212        1280 LOAD_GLOBAL             45 (NULL + time)
-                          1292 LOAD_ATTR               23 (sleep)
-                          1302 LOAD_CONST              22 (0.2)
-                          1304 PRECALL                  1
-                          1308 CALL                     1
-                          1318 POP_TOP
-               
-               214        1320 LOAD_GLOBAL             43 (NULL + execute_threading)
-                          1332 LOAD_FAST               11 (short_pool_amount_list)
-                          1334 PRECALL                  1
-                          1338 CALL                     1
-                          1348 STORE_FAST              32 (short_pool_amount_output)
-               
-               215        1350 LOAD_GLOBAL             45 (NULL + time)
-                          1362 LOAD_ATTR               23 (sleep)
-                          1372 LOAD_CONST              22 (0.2)
-                          1374 PRECALL                  1
-                          1378 CALL                     1
-                          1388 POP_TOP
-               
-               217        1390 LOAD_GLOBAL             43 (NULL + execute_threading)
-               
-               218        1402 LOAD_FAST                9 (long_reserve_factor_list)
-               
-               217        1404 PRECALL                  1
-                          1408 CALL                     1
-                          1418 STORE_FAST              33 (long_reserve_factor_list_output)
-               
-               220        1420 LOAD_GLOBAL             45 (NULL + time)
-                          1432 LOAD_ATTR               23 (sleep)
-                          1442 LOAD_CONST              22 (0.2)
-                          1444 PRECALL                  1
-                          1448 CALL                     1
-                          1458 POP_TOP
-               
-               222        1460 LOAD_GLOBAL             43 (NULL + execute_threading)
-               
-               223        1472 LOAD_FAST               12 (short_reserve_factor_list)
-               
-               222        1474 PRECALL                  1
-                          1478 CALL                     1
-                          1488 STORE_FAST              34 (short_reserve_factor_list_output)
-               
-               225        1490 LOAD_GLOBAL             45 (NULL + time)
-                          1502 LOAD_ATTR               23 (sleep)
-                          1512 LOAD_CONST              22 (0.2)
-                          1514 PRECALL                  1
-                          1518 CALL                     1
-                          1528 POP_TOP
-               
-               227        1530 LOAD_GLOBAL             43 (NULL + execute_threading)
-               
-               228        1542 LOAD_FAST               10 (long_open_interest_reserve_factor_list)
-               
-               227        1544 PRECALL                  1
-                          1548 CALL                     1
-                          1558 STORE_FAST              35 (long_open_interest_reserve_factor_list_output)
-               
-               230        1560 LOAD_GLOBAL             45 (NULL + time)
-                          1572 LOAD_ATTR               23 (sleep)
-                          1582 LOAD_CONST              22 (0.2)
-                          1584 PRECALL                  1
-                          1588 CALL                     1
-                          1598 POP_TOP
-               
-               232        1600 LOAD_GLOBAL             43 (NULL + execute_threading)
-               
-               233        1612 LOAD_FAST               13 (short_open_interest_reserve_factor_list)
-               
-               232        1614 PRECALL                  1
-                          1618 CALL                     1
-                          1628 STORE_FAST              36 (short_open_interest_reserve_factor_list_output)
-               
-               249        1630 LOAD_GLOBAL             49 (NULL + zip)
-               
-               250        1642 LOAD_FAST               31 (long_pool_amount_output)
-               
-               251        1644 LOAD_FAST               32 (short_pool_amount_output)
-               
-               252        1646 LOAD_FAST               33 (long_reserve_factor_list_output)
-               
-               253        1648 LOAD_FAST               34 (short_reserve_factor_list_output)
-               
-               254        1650 LOAD_FAST               35 (long_open_interest_reserve_factor_list_output)
-               
-               255        1652 LOAD_FAST               36 (short_open_interest_reserve_factor_list_output)
-               
-               256        1654 LOAD_FAST                4 (reserved_long_list)
-               
-               257        1656 LOAD_FAST                5 (reserved_short_list)
-               
-               258        1658 LOAD_FAST                6 (token_price_list)
-               
-               259        1660 LOAD_FAST                7 (mapper)
-               
-               260        1662 LOAD_FAST               14 (long_precision_list)
-               
-               261        1664 LOAD_FAST               15 (short_precision_list)
-               
-               249        1666 PRECALL                 12
-                          1670 CALL                    12
-               
-               236        1680 GET_ITER
-                       >> 1682 FOR_ITER               229 (to 2142)
-                          1684 UNPACK_SEQUENCE         12
-               
-               237        1688 STORE_FAST              19 (long_pool_amount)
-               
-               238        1690 STORE_FAST              24 (short_pool_amount)
-               
-               239        1692 STORE_FAST              20 (long_reserve_factor)
-               
-               240        1694 STORE_FAST              25 (short_reserve_factor)
-               
-               241        1696 STORE_FAST              21 (long_open_interest_reserve_factor)
-               
-               242        1698 STORE_FAST              26 (short_open_interest_reserve_factor)
-               
-               243        1700 STORE_FAST              37 (reserved_long)
-               
-               244        1702 STORE_FAST              38 (reserved_short)
-               
-               245        1704 STORE_FAST              30 (token_price)
-               
-               246        1706 STORE_FAST              39 (token_symbol)
-               
-               247        1708 STORE_FAST              22 (long_precision)
-               
-               248        1710 STORE_FAST              27 (short_precision)
-               
-               263        1712 LOAD_GLOBAL             29 (NULL + print)
-                          1724 LOAD_FAST               39 (token_symbol)
-                          1726 PRECALL                  1
-                          1730 CALL                     1
-                          1740 POP_TOP
-               
-               267        1742 LOAD_FAST               21 (long_open_interest_reserve_factor)
-                          1744 LOAD_FAST               20 (long_reserve_factor)
-                          1746 COMPARE_OP               0 (<)
-                          1752 POP_JUMP_FORWARD_IF_FALSE     2 (to 1758)
-               
-               268        1754 LOAD_FAST               21 (long_open_interest_reserve_factor)
-                          1756 STORE_FAST              20 (long_reserve_factor)
-               
-               271     >> 1758 LOAD_FAST               19 (long_pool_amount)
-                          1760 LOAD_FAST               20 (long_reserve_factor)
-                          1762 BINARY_OP                5 (*)
-               
-               270        1766 STORE_FAST              40 (long_max_reserved_tokens)
-               
-               275        1768 LOAD_FAST               40 (long_max_reserved_tokens)
-                          1770 LOAD_FAST               22 (long_precision)
-                          1772 BINARY_OP               11 (/)
-                          1776 LOAD_FAST               30 (token_price)
-                          1778 BINARY_OP                5 (*)
-               
-               274        1782 STORE_FAST              41 (long_max_reserved_usd)
-               
-               278        1784 LOAD_FAST               41 (long_max_reserved_usd)
-                          1786 LOAD_GLOBAL             41 (NULL + float)
-                          1798 LOAD_FAST               37 (reserved_long)
-                          1800 PRECALL                  1
-                          1804 CALL                     1
-                          1814 BINARY_OP               10 (-)
-                          1818 STORE_FAST              42 (long_liquidity)
-               
-               280        1820 LOAD_GLOBAL             29 (NULL + print)
-               
-               281        1832 LOAD_CONST              23 ('Available Long Liquidity: ${}')
-                          1834 LOAD_METHOD              8 (format)
-               
-               282        1856 LOAD_GLOBAL             51 (NULL + numerize)
-                          1868 LOAD_ATTR               25 (numerize)
-                          1878 LOAD_FAST               42 (long_liquidity)
-                          1880 PRECALL                  1
-                          1884 CALL                     1
-               
-               281        1894 PRECALL                  1
-                          1898 CALL                     1
-               
-               280        1908 PRECALL                  1
-                          1912 CALL                     1
-                          1922 POP_TOP
-               
-               285        1924 LOAD_FAST               42 (long_liquidity)
-                          1926 LOAD_FAST                3 (available_liquidity)
-                          1928 LOAD_CONST              16 ('long')
-                          1930 BINARY_SUBSCR
-                          1940 LOAD_FAST               39 (token_symbol)
-                          1942 STORE_SUBSCR
-               
-               289        1946 LOAD_FAST               26 (short_open_interest_reserve_factor)
-                          1948 LOAD_FAST               25 (short_reserve_factor)
-                          1950 COMPARE_OP               0 (<)
-                          1956 POP_JUMP_FORWARD_IF_FALSE     2 (to 1962)
-               
-               290        1958 LOAD_FAST               26 (short_open_interest_reserve_factor)
-                          1960 STORE_FAST              25 (short_reserve_factor)
-               
-               292     >> 1962 LOAD_FAST               24 (short_pool_amount)
-                          1964 LOAD_FAST               25 (short_reserve_factor)
-                          1966 BINARY_OP                5 (*)
-                          1970 STORE_FAST              43 (short_max_reserved_usd)
-               
-               295        1972 LOAD_FAST               43 (short_max_reserved_usd)
-                          1974 LOAD_FAST               27 (short_precision)
-                          1976 BINARY_OP               11 (/)
-                          1980 LOAD_GLOBAL             41 (NULL + float)
-               
-               296        1992 LOAD_FAST               38 (reserved_short)
-               
-               295        1994 PRECALL                  1
-                          1998 CALL                     1
-                          2008 BINARY_OP               10 (-)
-               
-               294        2012 STORE_FAST              44 (short_liquidity)
-               
-               299        2014 LOAD_GLOBAL             29 (NULL + print)
-               
-               300        2026 LOAD_CONST              24 ('Available Short Liquidity: ${}\n')
-                          2028 LOAD_METHOD              8 (format)
-               
-               301        2050 LOAD_GLOBAL             51 (NULL + numerize)
-                          2062 LOAD_ATTR               25 (numerize)
-                          2072 LOAD_FAST               44 (short_liquidity)
-                          2074 PRECALL                  1
-                          2078 CALL                     1
-               
-               300        2088 PRECALL                  1
-                          2092 CALL                     1
-               
-               299        2102 PRECALL                  1
-                          2106 CALL                     1
-                          2116 POP_TOP
-               
-               305        2118 LOAD_FAST               44 (short_liquidity)
-                          2120 LOAD_FAST                3 (available_liquidity)
-                          2122 LOAD_CONST              19 ('short')
-                          2124 BINARY_SUBSCR
-                          2134 LOAD_FAST               39 (token_symbol)
-                          2136 STORE_SUBSCR
-                          2140 JUMP_BACKWARD          230 (to 1682)
-               
-               307     >> 2142 LOAD_FAST                3 (available_liquidity)
-                          2144 RETURN_VALUE
+                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  000000000000006401a6010000ab01000000000000000001007405000000
+                  000000000000007c006a030000000000000000ac02a6010000ab01000000
+                  0000000000a00400000000000000000000000000000000000000006403ac
+                  04a6010000ab0100000000000000007d0167007d0267007d0367007d0467
+                  007d0567007d0667007d0767007d0867007d0967007d0a67007d0b67007d
+                  0c67007d0d7c006a0500000000000000006a010000000000000000440090
+                  025d6b7d0e7c00a0060000000000000000000000000000000000000000a6
+                  000000ab00000000000000000001007c00a0070000000000000000000000
+                  0000000000000000007c0ea6010000ab01000000000000000001007c006a
+                  050000000000000000a00800000000000000000000000000000000000000
+                  007c0ea6010000ab0100000000000000007d0f7c006a0500000000000000
+                  00a00900000000000000000000000000000000000000007c0e64056403ac
+                  06a6030000ab0300000000000000007d107c006a050000000000000000a0
+                  0900000000000000000000000000000000000000007c0e64036405ac06a6
+                  030000ab0300000000000000007d11640764087c107a0000007a0800007d
+                  12640764087c117a0000007a0800007d13640764087c107a0a00007a0800
+                  007d147c05a00a00000000000000000000000000000000000000007c0fa6
+                  010000ab01000000000000000001007c00a00b0000000000000000000000
+                  0000000000000000007c0e7c006a0c00000000000000006405a6030000ab
+                  0300000000000000005c0300007d157d167d177c02a00a00000000000000
+                  000000000000000000000000007c016409190000000000000000007c0f19
+                  000000000000000000a6010000ab01000000000000000001007c06a00a00
+                  000000000000000000000000000000000000007c15a6010000ab01000000
+                  000000000001007c07a00a00000000000000000000000000000000000000
+                  007c16a6010000ab01000000000000000001007c08a00a00000000000000
+                  000000000000000000000000007c17a6010000ab01000000000000000001
+                  007c0ca00a00000000000000000000000000000000000000007c12a60100
+                  00ab01000000000000000001007c00a00b00000000000000000000000000
+                  000000000000007c0e7c006a0d00000000000000006403a6030000ab0300
+                  000000000000005c0300007d187d197d1a7c03a00a000000000000000000
+                  00000000000000000000007c01640a190000000000000000007c0f190000
+                  00000000000000a6010000ab01000000000000000001007c09a00a000000
+                  00000000000000000000000000000000007c18a6010000ab010000000000
+                  00000001007c0aa00a00000000000000000000000000000000000000007c
+                  19a6010000ab01000000000000000001007c0ba00a000000000000000000
+                  00000000000000000000007c1aa6010000ab01000000000000000001007c
+                  0da00a00000000000000000000000000000000000000007c13a6010000ab
+                  0100000000000000000100741d000000000000000000007c006a03000000
+                  0000000000ac02a6010000ab010000000000000000a00f00000000000000
+                  00000000000000000000000000a6000000ab0000000000000000007d1b74
+                  21000000000000000000006a110000000000000000742500000000000000
+                  0000007c1b7c006a0c000000000000000019000000000000000000640b19
+                  000000000000000000a6010000ab0100000000000000007c147a0b000074
+                  25000000000000000000007c1b7c006a0c00000000000000001900000000
+                  0000000000640c19000000000000000000a6010000ab0100000000000000
+                  007c147a0b00006702a6010000ab0100000000000000007d1c7c04a00a00
+                  000000000000000000000000000000000000007c1ca6010000ab01000000
+                  0000000000010090028c6d7427000000000000000000007c06a6010000ab
+                  0100000000000000007d1d7429000000000000000000006a150000000000
+                  000000640da6010000ab0100000000000000000100742700000000000000
+                  0000007c09a6010000ab0100000000000000007d1e742900000000000000
+                  0000006a150000000000000000640da6010000ab01000000000000000001
+                  007427000000000000000000007c07a6010000ab0100000000000000007d
+                  1f7429000000000000000000006a150000000000000000640da6010000ab
+                  01000000000000000001007427000000000000000000007c0aa6010000ab
+                  0100000000000000007d207429000000000000000000006a150000000000
+                  000000640da6010000ab0100000000000000000100742700000000000000
+                  0000007c08a6010000ab0100000000000000007d21742900000000000000
+                  0000006a150000000000000000640da6010000ab01000000000000000001
+                  007427000000000000000000007c0ba6010000ab0100000000000000007d
+                  22742d000000000000000000007c1d7c1e7c1f7c207c217c227c027c037c
+                  047c057c0c7c0da60c0000ab0c0000000000000000440090015d245c0c00
+                  007d157d187d167d197d177d1a7d237d247d1c7d257d127d137c006a0000
+                  00000000000000a001000000000000000000000000000000000000000064
+                  0ea01700000000000000000000000000000000000000007c25a6010000ab
+                  010000000000000000a6010000ab01000000000000000001007c177c166b
+                  000000000072027c177d167c157c167a0500007d267c267c127a0b00007c
+                  1c7a0500007d277c277425000000000000000000007c23a6010000ab0100
+                  000000000000007a0a00007d287c006a000000000000000000a001000000
+                  0000000000000000000000000000000000640fa017000000000000000000
+                  00000000000000000000007431000000000000000000006a180000000000
+                  0000007c28a6010000ab010000000000000000a6010000ab010000000000
+                  000000a6010000ab01000000000000000001007c1a7c196b000000000072
+                  027c1a7d197c187c197a0500007d297c297c137a0b000074250000000000
+                  00000000007c24a6010000ab0100000000000000007a0a00007d2a7c006a
+                  000000000000000000a00100000000000000000000000000000000000000
+                  006410a01700000000000000000000000000000000000000007431000000
+                  000000000000006a1800000000000000007c2aa6010000ab010000000000
+                  000000a6010000ab010000000000000000a6010000ab0100000000000000
+                  0001007c287c006a1900000000000000006409190000000000000000007c
+                  253c0000007c2a7c006a190000000000000000640a190000000000000000
+                  007c253c00000090018c267c006a1900000000000000005300
+                21           0 RESUME                   0
+               
+                31           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (log)
+                            14 LOAD_METHOD              1 (info)
+                            36 LOAD_CONST               1 ('GMX v2 Available Liquidity')
+                            38 PRECALL                  1
+                            42 CALL                     1
+                            52 POP_TOP
+               
+                33          54 LOAD_GLOBAL              5 (NULL + OpenInterest)
+                            66 LOAD_FAST                0 (self)
+                            68 LOAD_ATTR                3 (chain)
+                            78 KW_NAMES                 2
+                            80 PRECALL                  1
+                            84 CALL                     1
+                            94 LOAD_METHOD              4 (get_data)
+               
+                34         116 LOAD_CONST               3 (False)
+               
+                33         118 KW_NAMES                 4
+                           120 PRECALL                  1
+                           124 CALL                     1
+                           134 STORE_FAST               1 (open_interest)
+               
+                37         136 BUILD_LIST               0
+                           138 STORE_FAST               2 (reserved_long_list)
+               
+                38         140 BUILD_LIST               0
+                           142 STORE_FAST               3 (reserved_short_list)
+               
+                39         144 BUILD_LIST               0
+                           146 STORE_FAST               4 (token_price_list)
+               
+                40         148 BUILD_LIST               0
+                           150 STORE_FAST               5 (mapper)
+               
+                41         152 BUILD_LIST               0
+                           154 STORE_FAST               6 (long_pool_amount_list)
+               
+                42         156 BUILD_LIST               0
+                           158 STORE_FAST               7 (long_reserve_factor_list)
+               
+                43         160 BUILD_LIST               0
+                           162 STORE_FAST               8 (long_open_interest_reserve_factor_list)
+               
+                44         164 BUILD_LIST               0
+                           166 STORE_FAST               9 (short_pool_amount_list)
+               
+                45         168 BUILD_LIST               0
+                           170 STORE_FAST              10 (short_reserve_factor_list)
+               
+                46         172 BUILD_LIST               0
+                           174 STORE_FAST              11 (short_open_interest_reserve_factor_list)
+               
+                47         176 BUILD_LIST               0
+                           178 STORE_FAST              12 (long_precision_list)
+               
+                48         180 BUILD_LIST               0
+                           182 STORE_FAST              13 (short_precision_list)
+               
+                50         184 LOAD_FAST                0 (self)
+                           186 LOAD_ATTR                5 (markets)
+                           196 LOAD_ATTR                1 (info)
+                           206 GET_ITER
+                       >>  208 EXTENDED_ARG             2
+                           210 FOR_ITER               619 (to 1450)
+                           212 STORE_FAST              14 (market_key)
+               
+                51         214 LOAD_FAST                0 (self)
+                           216 LOAD_METHOD              6 (_filter_swap_markets)
+                           238 PRECALL                  0
+                           242 CALL                     0
+                           252 POP_TOP
+               
+                52         254 LOAD_FAST                0 (self)
+                           256 LOAD_METHOD              7 (_get_token_addresses)
+                           278 LOAD_FAST               14 (market_key)
+                           280 PRECALL                  1
+                           284 CALL                     1
+                           294 POP_TOP
+               
+                53         296 LOAD_FAST                0 (self)
+                           298 LOAD_ATTR                5 (markets)
+                           308 LOAD_METHOD              8 (get_market_symbol)
+                           330 LOAD_FAST               14 (market_key)
+                           332 PRECALL                  1
+                           336 CALL                     1
+                           346 STORE_FAST              15 (market_symbol)
+               
+                54         348 LOAD_FAST                0 (self)
+                           350 LOAD_ATTR                5 (markets)
+                           360 LOAD_METHOD              9 (get_decimal_factor)
+               
+                55         382 LOAD_FAST               14 (market_key)
+               
+                56         384 LOAD_CONST               5 (True)
+               
+                57         386 LOAD_CONST               3 (False)
+               
+                54         388 KW_NAMES                 6
+                           390 PRECALL                  3
+                           394 CALL                     3
+                           404 STORE_FAST              16 (long_decimal_factor)
+               
+                59         406 LOAD_FAST                0 (self)
+                           408 LOAD_ATTR                5 (markets)
+                           418 LOAD_METHOD              9 (get_decimal_factor)
+               
+                60         440 LOAD_FAST               14 (market_key)
+               
+                61         442 LOAD_CONST               3 (False)
+               
+                62         444 LOAD_CONST               5 (True)
+               
+                59         446 KW_NAMES                 6
+                           448 PRECALL                  3
+                           452 CALL                     3
+                           462 STORE_FAST              17 (short_decimal_factor)
+               
+                64         464 LOAD_CONST               7 (10)
+                           466 LOAD_CONST               8 (30)
+                           468 LOAD_FAST               16 (long_decimal_factor)
+                           470 BINARY_OP                0 (+)
+                           474 BINARY_OP                8 (**)
+                           478 STORE_FAST              18 (long_precision)
+               
+                65         480 LOAD_CONST               7 (10)
+                           482 LOAD_CONST               8 (30)
+                           484 LOAD_FAST               17 (short_decimal_factor)
+                           486 BINARY_OP                0 (+)
+                           490 BINARY_OP                8 (**)
+                           494 STORE_FAST              19 (short_precision)
+               
+                66         496 LOAD_CONST               7 (10)
+                           498 LOAD_CONST               8 (30)
+                           500 LOAD_FAST               16 (long_decimal_factor)
+                           502 BINARY_OP               10 (-)
+                           506 BINARY_OP                8 (**)
+                           510 STORE_FAST              20 (oracle_precision)
+               
+                69         512 LOAD_FAST                5 (mapper)
+                           514 LOAD_METHOD             10 (append)
+                           536 LOAD_FAST               15 (market_symbol)
+                           538 PRECALL                  1
+                           542 CALL                     1
+                           552 POP_TOP
+               
+                76         554 LOAD_FAST                0 (self)
+                           556 LOAD_METHOD             11 (get_max_reserved_usd)
+               
+                77         578 LOAD_FAST               14 (market_key)
+               
+                78         580 LOAD_FAST                0 (self)
+                           582 LOAD_ATTR               12 (_long_token_address)
+               
+                79         592 LOAD_CONST               5 (True)
+               
+                76         594 PRECALL                  3
+                           598 CALL                     3
+               
+                72         608 UNPACK_SEQUENCE          3
+               
+                73         612 STORE_FAST              21 (long_pool_amount)
+               
+                74         614 STORE_FAST              22 (long_reserve_factor)
+               
+                75         616 STORE_FAST              23 (long_open_interest_reserve_factor)
+               
+                81         618 LOAD_FAST                2 (reserved_long_list)
+                           620 LOAD_METHOD             10 (append)
+                           642 LOAD_FAST                1 (open_interest)
+                           644 LOAD_CONST               9 ('long')
+                           646 BINARY_SUBSCR
+                           656 LOAD_FAST               15 (market_symbol)
+                           658 BINARY_SUBSCR
+                           668 PRECALL                  1
+                           672 CALL                     1
+                           682 POP_TOP
+               
+                82         684 LOAD_FAST                6 (long_pool_amount_list)
+                           686 LOAD_METHOD             10 (append)
+                           708 LOAD_FAST               21 (long_pool_amount)
+                           710 PRECALL                  1
+                           714 CALL                     1
+                           724 POP_TOP
+               
+                83         726 LOAD_FAST                7 (long_reserve_factor_list)
+                           728 LOAD_METHOD             10 (append)
+                           750 LOAD_FAST               22 (long_reserve_factor)
+                           752 PRECALL                  1
+                           756 CALL                     1
+                           766 POP_TOP
+               
+                84         768 LOAD_FAST                8 (long_open_interest_reserve_factor_list)
+                           770 LOAD_METHOD             10 (append)
+               
+                85         792 LOAD_FAST               23 (long_open_interest_reserve_factor)
+               
+                84         794 PRECALL                  1
+                           798 CALL                     1
+                           808 POP_TOP
+               
+                87         810 LOAD_FAST               12 (long_precision_list)
+                           812 LOAD_METHOD             10 (append)
+                           834 LOAD_FAST               18 (long_precision)
+                           836 PRECALL                  1
+                           840 CALL                     1
+                           850 POP_TOP
+               
+                94         852 LOAD_FAST                0 (self)
+                           854 LOAD_METHOD             11 (get_max_reserved_usd)
+               
+                95         876 LOAD_FAST               14 (market_key)
+               
+                96         878 LOAD_FAST                0 (self)
+                           880 LOAD_ATTR               13 (_short_token_address)
+               
+                97         890 LOAD_CONST               3 (False)
+               
+                94         892 PRECALL                  3
+                           896 CALL                     3
+               
+                90         906 UNPACK_SEQUENCE          3
+               
+                91         910 STORE_FAST              24 (short_pool_amount)
+               
+                92         912 STORE_FAST              25 (short_reserve_factor)
+               
+                93         914 STORE_FAST              26 (short_open_interest_reserve_factor)
+               
+                99         916 LOAD_FAST                3 (reserved_short_list)
+                           918 LOAD_METHOD             10 (append)
+                           940 LOAD_FAST                1 (open_interest)
+                           942 LOAD_CONST              10 ('short')
+                           944 BINARY_SUBSCR
+                           954 LOAD_FAST               15 (market_symbol)
+                           956 BINARY_SUBSCR
+                           966 PRECALL                  1
+                           970 CALL                     1
+                           980 POP_TOP
+               
+               100         982 LOAD_FAST                9 (short_pool_amount_list)
+                           984 LOAD_METHOD             10 (append)
+                          1006 LOAD_FAST               24 (short_pool_amount)
+                          1008 PRECALL                  1
+                          1012 CALL                     1
+                          1022 POP_TOP
+               
+               101        1024 LOAD_FAST               10 (short_reserve_factor_list)
+                          1026 LOAD_METHOD             10 (append)
+                          1048 LOAD_FAST               25 (short_reserve_factor)
+                          1050 PRECALL                  1
+                          1054 CALL                     1
+                          1064 POP_TOP
+               
+               102        1066 LOAD_FAST               11 (short_open_interest_reserve_factor_list)
+                          1068 LOAD_METHOD             10 (append)
+               
+               103        1090 LOAD_FAST               26 (short_open_interest_reserve_factor)
+               
+               102        1092 PRECALL                  1
+                          1096 CALL                     1
+                          1106 POP_TOP
+               
+               105        1108 LOAD_FAST               13 (short_precision_list)
+                          1110 LOAD_METHOD             10 (append)
+                          1132 LOAD_FAST               19 (short_precision)
+                          1134 PRECALL                  1
+                          1138 CALL                     1
+                          1148 POP_TOP
+               
+               108        1150 LOAD_GLOBAL             29 (NULL + OraclePrices)
+                          1162 LOAD_FAST                0 (self)
+                          1164 LOAD_ATTR                3 (chain)
+                          1174 KW_NAMES                 2
+                          1176 PRECALL                  1
+                          1180 CALL                     1
+                          1190 LOAD_METHOD             15 (get_recent_prices)
+                          1212 PRECALL                  0
+                          1216 CALL                     0
+                          1226 STORE_FAST              27 (prices)
+               
+               109        1228 LOAD_GLOBAL             33 (NULL + np)
+                          1240 LOAD_ATTR               17 (median)
+               
+               111        1250 LOAD_GLOBAL             37 (NULL + float)
+               
+               112        1262 LOAD_FAST               27 (prices)
+                          1264 LOAD_FAST                0 (self)
+                          1266 LOAD_ATTR               12 (_long_token_address)
+                          1276 BINARY_SUBSCR
+                          1286 LOAD_CONST              11 ('maxPriceFull')
+                          1288 BINARY_SUBSCR
+               
+               111        1298 PRECALL                  1
+                          1302 CALL                     1
+               
+               113        1312 LOAD_FAST               20 (oracle_precision)
+               
+               111        1314 BINARY_OP               11 (/)
+               
+               114        1318 LOAD_GLOBAL             37 (NULL + float)
+               
+               115        1330 LOAD_FAST               27 (prices)
+                          1332 LOAD_FAST                0 (self)
+                          1334 LOAD_ATTR               12 (_long_token_address)
+                          1344 BINARY_SUBSCR
+                          1354 LOAD_CONST              12 ('minPriceFull')
+                          1356 BINARY_SUBSCR
+               
+               114        1366 PRECALL                  1
+                          1370 CALL                     1
+               
+               116        1380 LOAD_FAST               20 (oracle_precision)
+               
+               114        1382 BINARY_OP               11 (/)
+               
+               110        1386 BUILD_LIST               2
+               
+               109        1388 PRECALL                  1
+                          1392 CALL                     1
+                          1402 STORE_FAST              28 (token_price)
+               
+               119        1404 LOAD_FAST                4 (token_price_list)
+                          1406 LOAD_METHOD             10 (append)
+                          1428 LOAD_FAST               28 (token_price)
+                          1430 PRECALL                  1
+                          1434 CALL                     1
+                          1444 POP_TOP
+                          1446 EXTENDED_ARG             2
+                          1448 JUMP_BACKWARD          621 (to 208)
+               
+               123     >> 1450 LOAD_GLOBAL             39 (NULL + execute_threading)
+                          1462 LOAD_FAST                6 (long_pool_amount_list)
+                          1464 PRECALL                  1
+                          1468 CALL                     1
+                          1478 STORE_FAST              29 (long_pool_amount_output)
+               
+               124        1480 LOAD_GLOBAL             41 (NULL + time)
+                          1492 LOAD_ATTR               21 (sleep)
+                          1502 LOAD_CONST              13 (0.2)
+                          1504 PRECALL                  1
+                          1508 CALL                     1
+                          1518 POP_TOP
+               
+               126        1520 LOAD_GLOBAL             39 (NULL + execute_threading)
+                          1532 LOAD_FAST                9 (short_pool_amount_list)
+                          1534 PRECALL                  1
+                          1538 CALL                     1
+                          1548 STORE_FAST              30 (short_pool_amount_output)
+               
+               127        1550 LOAD_GLOBAL             41 (NULL + time)
+                          1562 LOAD_ATTR               21 (sleep)
+                          1572 LOAD_CONST              13 (0.2)
+                          1574 PRECALL                  1
+                          1578 CALL                     1
+                          1588 POP_TOP
+               
+               129        1590 LOAD_GLOBAL             39 (NULL + execute_threading)
+               
+               130        1602 LOAD_FAST                7 (long_reserve_factor_list)
+               
+               129        1604 PRECALL                  1
+                          1608 CALL                     1
+                          1618 STORE_FAST              31 (long_reserve_factor_list_output)
+               
+               132        1620 LOAD_GLOBAL             41 (NULL + time)
+                          1632 LOAD_ATTR               21 (sleep)
+                          1642 LOAD_CONST              13 (0.2)
+                          1644 PRECALL                  1
+                          1648 CALL                     1
+                          1658 POP_TOP
+               
+               134        1660 LOAD_GLOBAL             39 (NULL + execute_threading)
+               
+               135        1672 LOAD_FAST               10 (short_reserve_factor_list)
+               
+               134        1674 PRECALL                  1
+                          1678 CALL                     1
+                          1688 STORE_FAST              32 (short_reserve_factor_list_output)
+               
+               137        1690 LOAD_GLOBAL             41 (NULL + time)
+                          1702 LOAD_ATTR               21 (sleep)
+                          1712 LOAD_CONST              13 (0.2)
+                          1714 PRECALL                  1
+                          1718 CALL                     1
+                          1728 POP_TOP
+               
+               139        1730 LOAD_GLOBAL             39 (NULL + execute_threading)
+               
+               140        1742 LOAD_FAST                8 (long_open_interest_reserve_factor_list)
+               
+               139        1744 PRECALL                  1
+                          1748 CALL                     1
+                          1758 STORE_FAST              33 (long_open_interest_reserve_factor_list_output)
+               
+               142        1760 LOAD_GLOBAL             41 (NULL + time)
+                          1772 LOAD_ATTR               21 (sleep)
+                          1782 LOAD_CONST              13 (0.2)
+                          1784 PRECALL                  1
+                          1788 CALL                     1
+                          1798 POP_TOP
+               
+               144        1800 LOAD_GLOBAL             39 (NULL + execute_threading)
+               
+               145        1812 LOAD_FAST               11 (short_open_interest_reserve_factor_list)
+               
+               144        1814 PRECALL                  1
+                          1818 CALL                     1
+                          1828 STORE_FAST              34 (short_open_interest_reserve_factor_list_output)
+               
+               161        1830 LOAD_GLOBAL             45 (NULL + zip)
+               
+               162        1842 LOAD_FAST               29 (long_pool_amount_output)
+               
+               163        1844 LOAD_FAST               30 (short_pool_amount_output)
+               
+               164        1846 LOAD_FAST               31 (long_reserve_factor_list_output)
+               
+               165        1848 LOAD_FAST               32 (short_reserve_factor_list_output)
+               
+               166        1850 LOAD_FAST               33 (long_open_interest_reserve_factor_list_output)
+               
+               167        1852 LOAD_FAST               34 (short_open_interest_reserve_factor_list_output)
+               
+               168        1854 LOAD_FAST                2 (reserved_long_list)
+               
+               169        1856 LOAD_FAST                3 (reserved_short_list)
+               
+               170        1858 LOAD_FAST                4 (token_price_list)
+               
+               171        1860 LOAD_FAST                5 (mapper)
+               
+               172        1862 LOAD_FAST               12 (long_precision_list)
+               
+               173        1864 LOAD_FAST               13 (short_precision_list)
+               
+               161        1866 PRECALL                 12
+                          1870 CALL                    12
+               
+               148        1880 GET_ITER
+                       >> 1882 EXTENDED_ARG             1
+                          1884 FOR_ITER               292 (to 2470)
+                          1886 UNPACK_SEQUENCE         12
+               
+               149        1890 STORE_FAST              21 (long_pool_amount)
+               
+               150        1892 STORE_FAST              24 (short_pool_amount)
+               
+               151        1894 STORE_FAST              22 (long_reserve_factor)
+               
+               152        1896 STORE_FAST              25 (short_reserve_factor)
+               
+               153        1898 STORE_FAST              23 (long_open_interest_reserve_factor)
+               
+               154        1900 STORE_FAST              26 (short_open_interest_reserve_factor)
+               
+               155        1902 STORE_FAST              35 (reserved_long)
+               
+               156        1904 STORE_FAST              36 (reserved_short)
+               
+               157        1906 STORE_FAST              28 (token_price)
+               
+               158        1908 STORE_FAST              37 (token_symbol)
+               
+               159        1910 STORE_FAST              18 (long_precision)
+               
+               160        1912 STORE_FAST              19 (short_precision)
+               
+               175        1914 LOAD_FAST                0 (self)
+                          1916 LOAD_ATTR                0 (log)
+                          1926 LOAD_METHOD              1 (info)
+                          1948 LOAD_CONST              14 ('Token: {}')
+                          1950 LOAD_METHOD             23 (format)
+                          1972 LOAD_FAST               37 (token_symbol)
+                          1974 PRECALL                  1
+                          1978 CALL                     1
+                          1988 PRECALL                  1
+                          1992 CALL                     1
+                          2002 POP_TOP
+               
+               179        2004 LOAD_FAST               23 (long_open_interest_reserve_factor)
+                          2006 LOAD_FAST               22 (long_reserve_factor)
+                          2008 COMPARE_OP               0 (<)
+                          2014 POP_JUMP_FORWARD_IF_FALSE     2 (to 2020)
+               
+               180        2016 LOAD_FAST               23 (long_open_interest_reserve_factor)
+                          2018 STORE_FAST              22 (long_reserve_factor)
+               
+               183     >> 2020 LOAD_FAST               21 (long_pool_amount)
+                          2022 LOAD_FAST               22 (long_reserve_factor)
+                          2024 BINARY_OP                5 (*)
+               
+               182        2028 STORE_FAST              38 (long_max_reserved_tokens)
+               
+               187        2030 LOAD_FAST               38 (long_max_reserved_tokens)
+                          2032 LOAD_FAST               18 (long_precision)
+                          2034 BINARY_OP               11 (/)
+                          2038 LOAD_FAST               28 (token_price)
+                          2040 BINARY_OP                5 (*)
+               
+               186        2044 STORE_FAST              39 (long_max_reserved_usd)
+               
+               190        2046 LOAD_FAST               39 (long_max_reserved_usd)
+                          2048 LOAD_GLOBAL             37 (NULL + float)
+                          2060 LOAD_FAST               35 (reserved_long)
+                          2062 PRECALL                  1
+                          2066 CALL                     1
+                          2076 BINARY_OP               10 (-)
+                          2080 STORE_FAST              40 (long_liquidity)
+               
+               192        2082 LOAD_FAST                0 (self)
+                          2084 LOAD_ATTR                0 (log)
+                          2094 LOAD_METHOD              1 (info)
+               
+               193        2116 LOAD_CONST              15 ('Available Long Liquidity: ${}')
+                          2118 LOAD_METHOD             23 (format)
+               
+               194        2140 LOAD_GLOBAL             49 (NULL + numerize)
+                          2152 LOAD_ATTR               24 (numerize)
+                          2162 LOAD_FAST               40 (long_liquidity)
+                          2164 PRECALL                  1
+                          2168 CALL                     1
+               
+               193        2178 PRECALL                  1
+                          2182 CALL                     1
+               
+               192        2192 PRECALL                  1
+                          2196 CALL                     1
+                          2206 POP_TOP
+               
+               200        2208 LOAD_FAST               26 (short_open_interest_reserve_factor)
+                          2210 LOAD_FAST               25 (short_reserve_factor)
+                          2212 COMPARE_OP               0 (<)
+                          2218 POP_JUMP_FORWARD_IF_FALSE     2 (to 2224)
+               
+               201        2220 LOAD_FAST               26 (short_open_interest_reserve_factor)
+                          2222 STORE_FAST              25 (short_reserve_factor)
+               
+               203     >> 2224 LOAD_FAST               24 (short_pool_amount)
+                          2226 LOAD_FAST               25 (short_reserve_factor)
+                          2228 BINARY_OP                5 (*)
+                          2232 STORE_FAST              41 (short_max_reserved_usd)
+               
+               206        2234 LOAD_FAST               41 (short_max_reserved_usd)
+                          2236 LOAD_FAST               19 (short_precision)
+                          2238 BINARY_OP               11 (/)
+                          2242 LOAD_GLOBAL             37 (NULL + float)
+               
+               207        2254 LOAD_FAST               36 (reserved_short)
+               
+               206        2256 PRECALL                  1
+                          2260 CALL                     1
+                          2270 BINARY_OP               10 (-)
+               
+               205        2274 STORE_FAST              42 (short_liquidity)
+               
+               211        2276 LOAD_FAST                0 (self)
+                          2278 LOAD_ATTR                0 (log)
+                          2288 LOAD_METHOD              1 (info)
+               
+               212        2310 LOAD_CONST              16 ('Available Short Liquidity: ${}')
+                          2312 LOAD_METHOD             23 (format)
+               
+               213        2334 LOAD_GLOBAL             49 (NULL + numerize)
+                          2346 LOAD_ATTR               24 (numerize)
+                          2356 LOAD_FAST               42 (short_liquidity)
+                          2358 PRECALL                  1
+                          2362 CALL                     1
+               
+               212        2372 PRECALL                  1
+                          2376 CALL                     1
+               
+               211        2386 PRECALL                  1
+                          2390 CALL                     1
+                          2400 POP_TOP
+               
+               217        2402 LOAD_FAST               40 (long_liquidity)
+                          2404 LOAD_FAST                0 (self)
+                          2406 LOAD_ATTR               25 (output)
+                          2416 LOAD_CONST               9 ('long')
+                          2418 BINARY_SUBSCR
+                          2428 LOAD_FAST               37 (token_symbol)
+                          2430 STORE_SUBSCR
+               
+               218        2434 LOAD_FAST               42 (short_liquidity)
+                          2436 LOAD_FAST                0 (self)
+                          2438 LOAD_ATTR               25 (output)
+                          2448 LOAD_CONST              10 ('short')
+                          2450 BINARY_SUBSCR
+                          2460 LOAD_FAST               37 (token_symbol)
+                          2462 STORE_SUBSCR
+                          2466 EXTENDED_ARG             1
+                          2468 JUMP_BACKWARD          294 (to 1882)
+               
+               220     >> 2470 LOAD_FAST                0 (self)
+                          2472 LOAD_ATTR               25 (output)
+                          2482 RETURN_VALUE
                consts
-                  '\n        Generate the dictionary of available liquidity\n\n        Returns\n        -------\n        funding_apr : dict\n            dictionary of available liquidity\n\n        '
-                  'data_store'
-                  '{}_open_interest.json'
+                  '\n        Generate the dictionary of available liquidity\n\n        Returns\n        -------\n        funding_apr: dict\n            dictionary of available liquidity\n\n        '
+                  'GMX v2 Available Liquidity'
                   ('chain',)
                   False
                   ('to_json',)
-                  ('long', 'short')
-                  '\nGMX v2 Available Liquidity\n'
-                  'market_symbol'
-                  'SWAP'
-                  'long_token_address'
                   True
+                  ('market_key', 'long', 'short')
                   10
                   30
-                  'long_token_metadata'
-                  'decimals'
                   'long'
-                  'short_token_address'
-                  'short_token_metadata'
                   'short'
                   'maxPriceFull'
                   'minPriceFull'
                   0.2
+                  'Token: {}'
                   'Available Long Liquidity: ${}'
-                  'Available Short Liquidity: ${}\n'
-               names      ('use_local_datastore', 'json', 'load', 'open', 'os', 'path', 'join', 'base_dir', 'format', 'chain', 'OpenInterest', 'call_open_interest', 'GetMarkets', 'get_available_markets', 'print', 'get_max_reserved_usd', 'GetOraclePrices', 'get_recent_prices', 'np', 'median', 'float', 'execute_threading', 'time', 'sleep', 'zip', 'numerize')
-               varnames   ('self', 'open_interest', 'markets', 'available_liquidity', 'reserved_long_list', 'reserved_short_list', 'token_price_list', 'mapper', 'long_pool_amount_list', 'long_reserve_factor_list', 'long_open_interest_reserve_factor_list', 'short_pool_amount_list', 'short_reserve_factor_list', 'short_open_interest_reserve_factor_list', 'long_precision_list', 'short_precision_list', 'market_key', 'market_symbol', 'long_token_address', 'long_pool_amount', 'long_reserve_factor', 'long_open_interest_reserve_factor', 'long_precision', 'short_token_address', 'short_pool_amount', 'short_reserve_factor', 'short_open_interest_reserve_factor', 'short_precision', 'prices', 'oracle_precision', 'token_price', 'long_pool_amount_output', 'short_pool_amount_output', 'long_reserve_factor_list_output', 'short_reserve_factor_list_output', 'long_open_interest_reserve_factor_list_output', 'short_open_interest_reserve_factor_list_output', 'reserved_long', 'reserved_short', 'token_symbol', 'long_max_reserved_tokens', 'long_max_reserved_usd', 'long_liquidity', 'short_max_reserved_usd', 'short_liquidity')
+                  'Available Short Liquidity: ${}'
+               names      ('log', 'info', 'OpenInterest', 'chain', 'get_data', 'markets', '_filter_swap_markets', '_get_token_addresses', 'get_market_symbol', 'get_decimal_factor', 'append', 'get_max_reserved_usd', '_long_token_address', '_short_token_address', 'OraclePrices', 'get_recent_prices', 'np', 'median', 'float', 'execute_threading', 'time', 'sleep', 'zip', 'format', 'numerize', 'output')
+               varnames   ('self', 'open_interest', 'reserved_long_list', 'reserved_short_list', 'token_price_list', 'mapper', 'long_pool_amount_list', 'long_reserve_factor_list', 'long_open_interest_reserve_factor_list', 'short_pool_amount_list', 'short_reserve_factor_list', 'short_open_interest_reserve_factor_list', 'long_precision_list', 'short_precision_list', 'market_key', 'market_symbol', 'long_decimal_factor', 'short_decimal_factor', 'long_precision', 'short_precision', 'oracle_precision', 'long_pool_amount', 'long_reserve_factor', 'long_open_interest_reserve_factor', 'short_pool_amount', 'short_reserve_factor', 'short_open_interest_reserve_factor', 'prices', 'token_price', 'long_pool_amount_output', 'short_pool_amount_output', 'long_reserve_factor_list_output', 'short_reserve_factor_list_output', 'long_open_interest_reserve_factor_list_output', 'short_open_interest_reserve_factor_list_output', 'reserved_long', 'reserved_short', 'token_symbol', 'long_max_reserved_tokens', 'long_max_reserved_usd', 'long_liquidity', 'short_max_reserved_usd', 'short_liquidity')
                freevars   ()
                cellvars   ()
-               filename   '/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk_2/scripts/v2/get_available_liquidity.py'
-               name       '_available_liquidity'
-               firstlineno 74
+               filename   '/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk/scripts/v2/get/get_available_liquidity.py'
+               name       '_get_data_processing'
+               firstlineno 21
                lnotab
-                  0x020a0e0116010c012c010c01020132fd0eff0eff120a3e0102ff12044e
-                  02020202fd06071e02040104010401040104010401040104010401040104
-                  0104020a031c01080102030c031c0218010201020102fd0eff0801020502
-                  012cff060622ff02030c020aff0204020104ff04ff02040c031c05180102
-                  01020102fd0efc040102010201020602012cff060622ff02040aff02040a
-                  ff0204020104ff04ff02040c034e0102012cff060416020c011aff0e0202
-                  fe04030c011aff0e0202fe04fc02ff100c10041e0128021e0128020c0102
-                  ff100328020c0102ff100328020c0102ff100328020c0102ff10110c0102
-                  01020102010201020102010201020102010201020102f40ef30801020102
-                  01020102010201020102010201020102010201020f1e040c01040308ff02
-                  050eff020424020c01180126ff0eff100516040c0104020a03140102ff12
-                  ff02050c01180126ff0eff10061802
+                  0x020a34023e0102ff120404010401040104010401040104010401040104
+                  01040104021e0128012a01340122010201020102fd120522010201020102
+                  fd12051001100110032a07180102010c0102fd0efc040102010201020642
+                  012a012a01180102ff10032a07180102010c0102fd0efc04010201020102
+                  0642012a012a01180102ff10032a034e0116020c0124ff0e0202fe04030c
+                  0124ff0e0202fe04fc02ff100a2e041e0128021e0128020c0102ff100328
+                  020c0102ff100328020c0102ff100328020c0102ff10110c010201020102
+                  010201020102010201020102010201020102f40ef30a0102010201020102
+                  010201020102010201020102010201020f5a040c01040308ff02050eff02
+                  0424022201180126ff0eff10080c0104020a03140102ff12ff0206220118
+                  0126ff0eff100620012402
             'market'
             'token'
             'is_long'
             code
                argcount  : 4
                nlocals   : 11
                stacksize : 4
@@ -1116,121 +976,119 @@
                   017c03a6020000ab0200000000000000007d077c046a0500000000000000
                   00a00600000000000000000000000000000000000000007c05a6010000ab
                   0100000000000000007d087c046a050000000000000000a0060000000000
                   0000000000000000000000000000007c06a6010000ab0100000000000000
                   007d097c046a050000000000000000a00600000000000000000000000000
                   000000000000007c07a6010000ab0100000000000000007d0a7c087c097c
                   0a66035300
-               309           0 RESUME                   0
+               222           0 RESUME                   0
                
-               336           2 LOAD_GLOBAL              1 (NULL + get_datastore_contract)
+               254           2 LOAD_GLOBAL              1 (NULL + get_datastore_contract)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (chain)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 STORE_FAST               4 (datastore)
                
-               339          42 LOAD_GLOBAL              5 (NULL + pool_amount_key)
+               257          42 LOAD_GLOBAL              5 (NULL + pool_amount_key)
                
-               340          54 LOAD_FAST                1 (market)
+               258          54 LOAD_FAST                1 (market)
                
-               341          56 LOAD_FAST                2 (token)
+               259          56 LOAD_FAST                2 (token)
                
-               339          58 PRECALL                  2
+               257          58 PRECALL                  2
                             62 CALL                     2
                             72 STORE_FAST               5 (pool_amount_hash_data)
                
-               343          74 LOAD_GLOBAL              7 (NULL + reserve_factor_key)
+               261          74 LOAD_GLOBAL              7 (NULL + reserve_factor_key)
                
-               344          86 LOAD_FAST                1 (market)
+               262          86 LOAD_FAST                1 (market)
                
-               345          88 LOAD_FAST                3 (is_long)
+               263          88 LOAD_FAST                3 (is_long)
                
-               343          90 PRECALL                  2
+               261          90 PRECALL                  2
                             94 CALL                     2
                            104 STORE_FAST               6 (reserve_factor_hash_data)
                
-               348         106 LOAD_GLOBAL              9 (NULL + open_interest_reserve_factor_key)
+               266         106 LOAD_GLOBAL              9 (NULL + open_interest_reserve_factor_key)
                
-               349         118 LOAD_FAST                1 (market)
+               267         118 LOAD_FAST                1 (market)
                
-               350         120 LOAD_FAST                3 (is_long)
+               268         120 LOAD_FAST                3 (is_long)
                
-               348         122 PRECALL                  2
+               266         122 PRECALL                  2
                            126 CALL                     2
                
-               347         136 STORE_FAST               7 (open_interest_reserve_factor_hash_data)
+               265         136 STORE_FAST               7 (open_interest_reserve_factor_hash_data)
                
-               354         138 LOAD_FAST                4 (datastore)
+               272         138 LOAD_FAST                4 (datastore)
                            140 LOAD_ATTR                5 (functions)
                            150 LOAD_METHOD              6 (getUint)
                
-               355         172 LOAD_FAST                5 (pool_amount_hash_data)
+               273         172 LOAD_FAST                5 (pool_amount_hash_data)
                
-               354         174 PRECALL                  1
+               272         174 PRECALL                  1
                            178 CALL                     1
                            188 STORE_FAST               8 (pool_amount)
                
-               357         190 LOAD_FAST                4 (datastore)
+               275         190 LOAD_FAST                4 (datastore)
                            192 LOAD_ATTR                5 (functions)
                            202 LOAD_METHOD              6 (getUint)
                
-               358         224 LOAD_FAST                6 (reserve_factor_hash_data)
+               276         224 LOAD_FAST                6 (reserve_factor_hash_data)
                
-               357         226 PRECALL                  1
+               275         226 PRECALL                  1
                            230 CALL                     1
                            240 STORE_FAST               9 (reserve_factor)
                
-               360         242 LOAD_FAST                4 (datastore)
+               278         242 LOAD_FAST                4 (datastore)
                            244 LOAD_ATTR                5 (functions)
                            254 LOAD_METHOD              6 (getUint)
                
-               361         276 LOAD_FAST                7 (open_interest_reserve_factor_hash_data)
+               279         276 LOAD_FAST                7 (open_interest_reserve_factor_hash_data)
                
-               360         278 PRECALL                  1
+               278         278 PRECALL                  1
                            282 CALL                     1
                            292 STORE_FAST              10 (open_interest_reserve_factor)
                
-               364         294 LOAD_FAST                8 (pool_amount)
+               282         294 LOAD_FAST                8 (pool_amount)
                            296 LOAD_FAST                9 (reserve_factor)
                            298 LOAD_FAST               10 (open_interest_reserve_factor)
                            300 BUILD_TUPLE              3
                            302 RETURN_VALUE
                consts
-                  '\n        For a given market, long/short token and pool direction get the\n        uncalled web3 functions to calculate pool size, pool reserve factor\n        and open interest reserve factor\n\n        Parameters\n        ----------\n        market : str\n            contract address of GMX market.\n        token : str\n            contract address of long or short token.\n        is_long : bool\n            pass True for long pool or False for short.\n\n        Returns\n        -------\n        pool_amount : web3.contract_obj\n            uncalled web3 contract object for pool amount.\n        reserve_factor : web3.contract_obj\n            uncalled web3 contract object for pool reserve factor.\n        open_interest_reserve_factor : web3.contract_obj\n            uncalled web3 contract object for open interest reserve factor.\n\n        '
+                  '\n        For a given market, long/short token and pool direction get the\n        uncalled web3 functions to calculate pool size, pool reserve factor\n        and open interest reserve factor\n\n        Parameters\n        ----------\n        market: str\n            contract address of GMX market.\n        token: str\n            contract address of long or short token.\n        is_long: bool\n            pass True for long pool or False for short.\n\n        Returns\n        -------\n        pool_amount: web3.contract_obj\n            uncalled web3 contract object for pool amount.\n        reserve_factor: web3.contract_obj\n            uncalled web3 contract object for pool reserve factor.\n        open_interest_reserve_factor: web3.contract_obj\n            uncalled web3 contract object for open interest reserve factor.\n\n        '
                names      ('get_datastore_contract', 'chain', 'pool_amount_key', 'reserve_factor_key', 'open_interest_reserve_factor_key', 'functions', 'getUint')
                varnames   ('self', 'market', 'token', 'is_long', 'datastore', 'pool_amount_hash_data', 'reserve_factor_hash_data', 'open_interest_reserve_factor_hash_data', 'pool_amount', 'reserve_factor', 'open_interest_reserve_factor')
                freevars   ()
                cellvars   ()
-               filename   '/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk_2/scripts/v2/get_available_liquidity.py'
+               filename   '/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk/scripts/v2/get/get_available_liquidity.py'
                name       'get_max_reserved_usd'
-               firstlineno 309
+               firstlineno 222
                lnotab
-                  0x021b28030c01020102fe10040c01020102fe10050c01020102fe0eff02
+                  0x022028030c01020102fe10040c01020102fe10050c01020102fe0eff02
                   07220102ff1003220102ff1003220102ff1004
-            None
             (False,)
-            (False, False)
-         names      ('__name__', '__module__', '__qualname__', 'str', 'bool', '__init__', 'get_available_liquidity', '_available_liquidity', 'get_max_reserved_usd')
+         names      ('__name__', '__module__', '__qualname__', 'str', 'bool', '__init__', 'dict', '_get_data_processing', 'Tuple', 'Any', 'get_max_reserved_usd', '__classcell__')
          varnames   ()
          freevars   ()
-         cellvars   ()
-         filename   '/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk_2/scripts/v2/get_available_liquidity.py'
+         cellvars   ('__class__',)
+         filename   '/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk/scripts/v2/get/get_available_liquidity.py'
          name       'GetAvailableLiquidity'
-         firstlineno 23
-         lnotab 0x0a02120602ff040102ff020102ff082c067f006c
+         firstlineno 17
+         lnotab 0x0c0116030c7f004a0e0114ff
       'GetAvailableLiquidity'
       '__main__'
       'arbitrum'
       False
       ('chain', 'use_local_datastore')
       ('to_csv',)
-   names      ('os', 'json', 'time', 'numpy', 'np', 'numerize', 'get_markets', 'GetMarkets', 'gmx_utils', 'base_dir', 'execute_threading', 'save_json_file_to_datastore', 'make_timestamped_dataframe', 'save_csv_to_datastore', 'get_oracle_prices', 'GetOraclePrices', 'get_open_interest', 'OpenInterest', 'keys', 'get_datastore_contract', 'pool_amount_key', 'reserve_factor_key', 'open_interest_reserve_factor_key', 'GetAvailableLiquidity', '__name__', 'get_available_liquidity', 'data')
+   names      ('time', 'numpy', 'np', 'numerize', 'typing', 'Tuple', 'Any', 'get', 'GetData', 'get_oracle_prices', 'OraclePrices', 'get_open_interest', 'OpenInterest', 'gmx_utils', 'execute_threading', 'keys', 'get_datastore_contract', 'pool_amount_key', 'reserve_factor_key', 'open_interest_reserve_factor_key', 'GetAvailableLiquidity', '__name__', 'get_data', 'data')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk_2/scripts/v2/get_available_liquidity.py'
+   filename   '/Users/harrykitchener/Personal/crypto/gmx_python_sdk/gmx_python_sdk/scripts/v2/get/get_available_liquidity.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020108010801080208020c020c011c050c010c0118061a7f007f00
-      5a0c010401020102fe1003160102ff10fd06ff
+      0x00ff0201080208010c0110020c010c010c010c0118061c7f007f000e0c
+      010401020102fe1003160102ff10fd06ff
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/approve_token_for_spend.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/approve_token_for_spend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import json
 import os
 
 from web3 import Web3
 
-from .gmx_utils import create_connection, base_dir, get_config, \
-    convert_to_checksum_address
+from .gmx_utils import (
+    create_connection, base_dir, convert_to_checksum_address
+)
 
 
 def check_if_approved(
-        chain: str,
+        config,
         spender: str,
         token_to_approve: str,
         amount_of_tokens_to_spend: int,
+        max_fee_per_gas,
         approve: bool):
     """
     For a given chain, check if a given amount of tokens is approved for spend by a contract, and
     approve is passed as true
 
     Parameters
     ----------
@@ -33,30 +35,36 @@
     Raises
     ------
     Exception
         Insufficient balance or token not approved for spend.
 
     """
 
-    config = get_config()
-    connection = create_connection(chain=chain)
+    connection = create_connection(config)
 
     if token_to_approve == "0x47904963fc8b2340414262125aF798B9655E58Cd":
         token_to_approve = "0x2f2a2543B76A4166549F7aaB2e75Bef0aefC5B0f"
 
-    spender_checksum_address = convert_to_checksum_address(chain, spender)
+    spender_checksum_address = convert_to_checksum_address(
+        config, spender
+    )
 
     # User wallet address will be taken from config file
-    user_checksum_address = convert_to_checksum_address(chain, config['user_wallet_address'])
-
-    token_checksum_address = convert_to_checksum_address(chain, token_to_approve)
-
-    token_contract_abi = json.load(open(os.path.join(base_dir,
-                                                     'contracts',
-                                                     'token_approval.json')))
+    user_checksum_address = convert_to_checksum_address(
+        config,
+        config.user_wallet_address)
+
+    token_checksum_address = convert_to_checksum_address(config, token_to_approve)
+
+    token_contract_abi = json.load(open(os.path.join(
+        base_dir,
+        'gmx_python_sdk',
+        'contracts',
+        'token_approval.json'
+    )))
 
     token_contract_obj = connection.eth.contract(address=token_to_approve,
                                                  abi=token_contract_abi)
 
     # TODO - for AVAX support this will need to incl WAVAX address
     if token_checksum_address == "0x82aF49447D8a07e3bd95BD0d56f35241523fBab1":
         try:
@@ -84,22 +92,22 @@
         nonce = connection.eth.get_transaction_count(user_checksum_address)
 
         arguments = spender_checksum_address, amount_of_tokens_to_spend
         raw_txn = token_contract_obj.functions.approve(
             *arguments
         ).build_transaction({
             'value': 0,
-            'chainId': 42161,
+            'chainId': config.chain_id,
             'gas': 4000000,
-            'maxFeePerGas': Web3.to_wei('0.1', 'gwei'),
-            'maxPriorityFeePerGas': Web3.to_wei('0.1', 'gwei'),
+            'maxFeePerGas': int(max_fee_per_gas),
+            'maxPriorityFeePerGas': 0,
             'nonce': nonce})
 
         signed_txn = connection.eth.account.sign_transaction(raw_txn,
-                                                             config['private_key'])
+                                                             config.private_key)
         tx_hash = connection.eth.send_raw_transaction(signed_txn.rawTransaction)
 
         print("Txn submitted!")
         print("Check status: https://arbiscan.io/tx/{}".format(tx_hash.hex()))
 
     if amount_approved < amount_of_tokens_to_spend and not approve:
         raise Exception("Token not approved for spend, please allow first!")
@@ -107,18 +115,8 @@
     print('Contract "{}" approved to spend {} tokens belonging to token address: {}'.format(
         spender_checksum_address, amount_of_tokens_to_spend, token_checksum_address))
     print("Coins Approved for spend!")
 
 
 if __name__ == "__main__":
 
-    chain = 'arbitrum'
-    spender = "0x7452c558d45f8afC8c83dAe62C3f8A5BE19c71f6"
-    token_to_approve = "0xaf88d065e77c8cC2239327C5EDb3A432268e5831"
-    amount_of_tokens_to_spend = 1
-    approve = True
-
-    test = check_if_approved(chain,
-                             spender,
-                             token_to_approve,
-                             amount_of_tokens_to_spend,
-                             approve)
+    pass
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/create_decrease_order.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/create_decrease_order.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .order import Order
-from .gas_utils import get_gas_limits
-from .gmx_utils import (get_datastore_contract)
+from ..gas_utils import get_gas_limits
+from ..gmx_utils import get_datastore_contract
 
 
 class DecreaseOrder(Order):
     """
     Open a sell order
     Extends base Order class
     """
@@ -14,10 +14,10 @@
             *args, **kwargs
         )
 
         # Close an order
         self.order_builder(is_close=True)
 
     def determine_gas_limits(self):
-        datastore = get_datastore_contract(self.chain)
+        datastore = get_datastore_contract(self.config)
         self._gas_limits = get_gas_limits(datastore)
         self._gas_limits_order_type = self._gas_limits["decrease_order"]
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/create_deposit_order.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/create_deposit_order.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .deposit import Deposit
-from .gas_utils import get_gas_limits
-from .gmx_utils import (get_datastore_contract)
+from ..gas_utils import get_gas_limits
+from ..gmx_utils import get_datastore_contract
 
 
 class DepositOrder(Deposit):
     """
     Open a Deposit order
     Extends base Deposit class
     """
@@ -15,10 +15,10 @@
         )
 
         # Createa a deposit order
         self.create_deposit_order()
 
     def determine_gas_limits(self):
 
-        datastore = get_datastore_contract(self.chain)
+        datastore = get_datastore_contract(self.config)
         self._gas_limits = get_gas_limits(datastore)
         self._gas_limits_order_type = self._gas_limits["increase_order"]
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/create_increase_order.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/create_increase_order.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .order import Order
-from .gas_utils import get_gas_limits
-from .gmx_utils import (get_datastore_contract)
+from ..gas_utils import get_gas_limits
+from ..gmx_utils import get_datastore_contract
 
 
 class IncreaseOrder(Order):
     """
     Open a buy order
     Extends base Order class
     """
@@ -14,10 +14,10 @@
             *args, **kwargs
         )
 
         # Open an order
         self.order_builder(is_open=True)
 
     def determine_gas_limits(self):
-        datastore = get_datastore_contract(self.chain)
+        datastore = get_datastore_contract(self.config)
         self._gas_limits = get_gas_limits(datastore)
         self._gas_limits_order_type = self._gas_limits["increase_order"]
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/create_swap_order.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/create_swap_order.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from web3 import Web3
 
 from .order import Order
-from .gas_utils import get_gas_limits
-from .get_oracle_prices import GetOraclePrices
-from .gmx_utils import (
-    get_estimated_swap_output, contract_map,
-    get_datastore_contract
+from ..gas_utils import get_gas_limits
+from ..get.get_oracle_prices import OraclePrices
+from ..gmx_utils import (
+    get_estimated_swap_output, contract_map, get_datastore_contract
 )
 
 
 class SwapOrder(Order):
     """
     Open a swap order
     Extends base Order class
@@ -23,15 +22,15 @@
         self.out_token = out_token
 
         # Open an order
         self.order_builder(is_swap=True)
 
     def determine_gas_limits(self):
 
-        datastore = get_datastore_contract(self.chain)
+        datastore = get_datastore_contract(self.config)
         self._gas_limits = get_gas_limits(datastore)
         self._gas_limits_order_type = self._gas_limits["swap_order"]
 
     def estimated_swap_output(self, market: dict, in_token: str, in_token_amount: int):
         """
         For a given market, token, and amount, estimate the amount of token returned
         when the in token is swapped through the market.
@@ -48,26 +47,26 @@
         Returns
         -------
         estimated_swap_output : dict
             dict containing amount of tokens and price impact after swap.
 
         """
 
-        prices = GetOraclePrices(chain=self.chain).get_recent_prices()
+        prices = OraclePrices(chain=self.config.chain).get_recent_prices()
 
         try:
             in_token = Web3.to_checksum_address(in_token)
         except AttributeError:
             in_token = Web3.toChecksumAddress(in_token)
 
         # For every path we through we need to call this to get the expected
         # output after x number of swaps
         estimated_swap_output_parameters = {
             'data_store_address': (
-                contract_map[self.chain]["datastore"]['contract_address']
+                contract_map[self.config.chain]["datastore"]['contract_address']
             ),
             'market_addresses': [
                 market['gmx_market_address'],
                 market['index_token_address'],
                 market['long_token_address'],
                 market['short_token_address']
             ],
@@ -87,12 +86,12 @@
             ],
             'token_in': in_token,
             'token_amount_in': in_token_amount,
             'ui_fee_receiver': "0x0000000000000000000000000000000000000000"
         }
 
         estimated_swap_output = get_estimated_swap_output(
-            self.chain,
+            self.config,
             estimated_swap_output_parameters
         )
 
         return estimated_swap_output
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/create_withdrawal_order.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/create_withdrawal_order.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .withdraw import Withdraw
-from .gas_utils import get_gas_limits
-from .gmx_utils import (get_datastore_contract)
+from ..gas_utils import get_gas_limits
+from ..gmx_utils import get_datastore_contract
 
 
 class WithdrawOrder(Withdraw):
     """
     Open a withdrawal order
     Extends base Withdraw class
     """
@@ -15,10 +15,10 @@
         )
 
         # Open a withdrawal order
         self.create_withdraw_order()
 
     def determine_gas_limits(self):
 
-        datastore = get_datastore_contract(self.chain)
+        datastore = get_datastore_contract(self.config)
         self._gas_limits = get_gas_limits(datastore)
         self._gas_limits_order_type = self._gas_limits["increase_order"]
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/deposit.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/deposit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,151 +1,160 @@
 import logging
 
 from web3 import Web3
 
 from hexbytes import HexBytes
 
-from .get_markets import GetMarkets
-from .get_oracle_prices import GetOraclePrices
+from ..get.get_markets import Markets
+from ..get.get_oracle_prices import OraclePrices
 
-from .gmx_utils import get_config, convert_to_checksum_address, \
+from ..gmx_utils import convert_to_checksum_address, \
     get_exchange_router_contract, create_connection, \
     determine_swap_route, contract_map, get_estimated_deposit_amount_out
 
-from .approve_token_for_spend import check_if_approved
+from ..approve_token_for_spend import check_if_approved
 
-from .gas_utils import get_execution_fee
-
-CONFIG = get_config()
+from ..gas_utils import get_execution_fee
 
 
 class Deposit:
 
     def __init__(
         self,
-        chain: str,
+        config,
         market_key: str,
         initial_long_token: str,
         initial_short_token: bool,
         long_token_amount: int,
         short_token_amount: int,
+        max_fee_per_gas: int = None,
         debug_mode: bool = False
     ) -> None:
-        self.chain = chain
+        self.config = config
         self.market_key = market_key
         self.initial_long_token = initial_long_token
         self.initial_short_token = initial_short_token
         self.long_token_amount = long_token_amount
         self.short_token_amount = short_token_amount
         self.long_token_swap_path = []
         self.short_token_swap_path = []
+        self.max_fee_per_gas = max_fee_per_gas
         self.debug_mode = debug_mode
 
+        if self.max_fee_per_gas is None:
+            block = create_connection(
+                config
+            ).eth.get_block('latest')
+            self.max_fee_per_gas = block['baseFeePerGas'] * 1.35
+
         self._exchange_router_contract_obj = get_exchange_router_contract(
-            chain=self.chain
+            config
         )
 
-        self._connection = create_connection(chain=chain)
+        self._connection = create_connection(config)
 
-        self.all_markets_info = GetMarkets(chain=self.chain).get_available_markets()
+        self.all_markets_info = Markets(self.config).get_available_markets()
 
         self.log = logging.getLogger(__name__)
         self.log.info("Creating order...")
 
     def determine_gas_limits(self):
 
         pass
 
     def check_for_approval(self):
         """
         Check for Approval
 
         """
-        spender = contract_map[self.chain]["syntheticsrouter"]['contract_address']
+        spender = contract_map[self.config.chain]["syntheticsrouter"]['contract_address']
 
         if self.long_token_amount > 0:
-            check_if_approved(self.chain,
+            check_if_approved(self.config,
                               spender,
                               self.initial_long_token,
                               self.long_token_amount,
+                              self.max_fee_per_gas,
                               approve=True)
 
         if self.short_token_amount > 0:
-            check_if_approved(self.chain,
+            check_if_approved(self.config,
                               spender,
                               self.initial_short_token,
                               self.short_token_amount,
+                              self.max_fee_per_gas,
                               approve=True)
 
     def _submit_transaction(
         self, user_wallet_address: str, value_amount: float,
         multicall_args: list, gas_limits: dict
     ):
         """
         Submit Transaction
         """
-        self.log.info("Submitting transaction...")
+        self.log.info("Building transaction...")
 
         nonce = self._connection.eth.get_transaction_count(
             user_wallet_address
         )
 
         raw_txn = self._exchange_router_contract_obj.functions.multicall(
             multicall_args
         ).build_transaction(
             {
                 'value': value_amount,
-                'chainId': 42161,
+                'chainId': self.config.chain_id,
 
                 # TODO - this is NOT correct
                 'gas': (
                     self._gas_limits_order_type.call() + self._gas_limits_order_type.call()
                 ),
-                'maxFeePerGas': Web3.to_wei('0.12', 'gwei'),
-                'maxPriorityFeePerGas': Web3.to_wei('0.12', 'gwei'),
+                'maxFeePerGas': int(self.max_fee_per_gas),
+                'maxPriorityFeePerGas': 0,
                 'nonce': nonce
             }
         )
 
         if not self.debug_mode:
             signed_txn = self._connection.eth.account.sign_transaction(
-                raw_txn, get_config()['private_key']
+                raw_txn, self.config.private_key
             )
             tx_hash = self._connection.eth.send_raw_transaction(
                 signed_txn.rawTransaction
             )
             self.log.info("Txn submitted!")
             self.log.info(
                 "Check status: https://arbiscan.io/tx/{}".format(tx_hash.hex())
             )
 
             self.log.info("Transaction submitted!")
 
     def create_deposit_order(self):
 
-        user_wallet_address = CONFIG['user_wallet_address']
+        user_wallet_address = self.config.user_wallet_address
         self.determine_gas_limits()
 
-        self.check_for_approval()
+        if not self.debug_mode:
+            self.check_for_approval()
 
         should_unwrap_native_token = True
 
         eth_zero_address = "0x0000000000000000000000000000000000000000"
         ui_ref_address = "0x0000000000000000000000000000000000000000"
 
         user_wallet_address = convert_to_checksum_address(
-            self.chain,
+            self.config,
             user_wallet_address
         )
         eth_zero_address = convert_to_checksum_address(
-            self.chain,
+            self.config,
             eth_zero_address
         )
         ui_ref_address = convert_to_checksum_address(
-            self.chain,
+            self.config,
             ui_ref_address
         )
 
         # Minimum number of GM tokens we should expect
         min_market_tokens = self._estimate_deposit()
 
         # Giving a 10% buffer here
@@ -235,18 +244,22 @@
     def _check_initial_tokens(self):
         """
         Check if we need to set the long or short token address
         when depositing
         """
 
         if self.long_token_amount == 0:
-            self.initial_long_token = self.all_markets_info[self.market_key]['long_token_address']
+            self.initial_long_token = self.all_markets_info[
+                self.market_key
+            ]['long_token_address']
 
         if self.short_token_amount == 0:
-            self.initial_short_token = self.all_markets_info[self.market_key]['short_token_address']
+            self.initial_short_token = self.all_markets_info[
+                self.market_key
+            ]['short_token_address']
 
     def _determine_swap_paths(self):
         """
         Check the required markets we need to swap our tokens through
         to deposit on the long or short side
         """
 
@@ -310,18 +323,20 @@
         Returns
         -------
         int
             amount of GM tokens.
 
         """
 
-        data_store_contract_address = contract_map[self.chain]['datastore']['contract_address']
+        data_store_contract_address = contract_map[
+            self.config.chain
+        ]['datastore']['contract_address']
 
         market = self.all_markets_info[self.market_key]
-        oracle_prices_dict = GetOraclePrices(chain=self.chain).get_recent_prices()
+        oracle_prices_dict = OraclePrices(chain=self.config.chain).get_recent_prices()
 
         index_token_address = market['index_token_address']
         long_token_address = market['long_token_address']
         short_token_address = market['short_token_address']
 
         market_addresses = [self.market_key,
                             index_token_address,
@@ -346,8 +361,8 @@
             "market_addresses": market_addresses,
             "token_prices_tuple": prices,
             "long_token_amount": self.long_token_amount,
             "short_token_amount": self.short_token_amount,
             "ui_fee_receiver": "0x0000000000000000000000000000000000000000"
         }
 
-        return get_estimated_deposit_amount_out(self.chain, parameters)
+        return get_estimated_deposit_amount_out(self.config, parameters)
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/gas_utils.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/gas_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from .keys import decrease_order_gas_limit_key, increase_order_gas_limit_key, \
-    execution_gas_fee_base_amount_key, execution_gas_fee_multiplier_key, single_swap_gas_limit_key, \
-    swap_order_gas_limit_key, deposit_gas_limit_key, withdraw_gas_limit_key
+from .keys import (
+    decrease_order_gas_limit_key, increase_order_gas_limit_key,
+    execution_gas_fee_base_amount_key, execution_gas_fee_multiplier_key,
+    single_swap_gas_limit_key, swap_order_gas_limit_key, deposit_gas_limit_key,
+    withdraw_gas_limit_key
+)
 
 from .gmx_utils import apply_factor, get_datastore_contract, create_connection
 
 
 def get_execution_fee(gas_limits: dict, estimated_gas_limit, gas_price: int):
     """
     Given a dictionary of gas_limits, the uncalled datastore object of a given operation, and the
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_available_liquidity.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_available_liquidity.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,214 +1,126 @@
-import os
-import json
 import time
 
 import numpy as np
-
 from numerize import numerize
+from typing import Tuple, Any
 
-from .get_markets import GetMarkets
-from .gmx_utils import (
-    base_dir, execute_threading, save_json_file_to_datastore,
-    make_timestamped_dataframe, save_csv_to_datastore
-)
-
-from .get_oracle_prices import GetOraclePrices
+from .get import GetData
+from .get_oracle_prices import OraclePrices
 from .get_open_interest import OpenInterest
-from .keys import (
+from ..gmx_utils import execute_threading
+from ..keys import (
     get_datastore_contract, pool_amount_key, reserve_factor_key,
     open_interest_reserve_factor_key
 )
 
 
-class GetAvailableLiquidity:
-
-    def __init__(self, chain: str, use_local_datastore: bool = False):
-
-        self.chain = chain
-        self.use_local_datastore = use_local_datastore
-
-    def get_available_liquidity(
-        self, to_json: bool = False, to_csv: bool = False
-    ):
-        """
-        Call to get the available liquidity across all pools on a given
-        chain defined in class init. Pass either to_json or to_csv to save
-        locally in datastore
-
-        Parameters
-        ----------
-        to_json : bool, optional
-            save output to json file. The default is False.
-        to_csv : bool, optional
-            save out to csv file. The default is False.
-
-        Returns
-        -------
-        data : dict
-            dictionary of data.
+class GetAvailableLiquidity(GetData):
+    def __init__(self, config: str, use_local_datastore: bool = False):
+        super().__init__(config)
 
-        """
-        data = self._available_liquidity()
-
-        if to_json:
-            save_json_file_to_datastore(
-                "{}_available_liquidity.json".format(self.chain),
-                data
-            )
-
-        if to_csv:
-            long_dataframe = make_timestamped_dataframe(data['long'])
-            short_dataframe = make_timestamped_dataframe(data['short'])
-            save_csv_to_datastore(
-                "{}_long_available_liquidity.csv".format(self.chain),
-                long_dataframe
-            )
-            save_csv_to_datastore(
-                "{}_short_available_liquidity.csv".format(self.chain),
-                short_dataframe
-            )
-
-        else:
-            return data
-
-    def _available_liquidity(self):
+    def _get_data_processing(self) -> dict:
         """
         Generate the dictionary of available liquidity
 
         Returns
         -------
-        funding_apr : dict
+        funding_apr: dict
             dictionary of available liquidity
 
         """
-        if self.use_local_datastore:
-            open_interest = json.load(
-                open(
-                    os.path.join(
-                        base_dir,
-                        "data_store",
-                        "{}_open_interest.json".format(self.chain)
-                    )
-                )
-            )
-        else:
-            open_interest = OpenInterest(chain=self.chain).call_open_interest(
-                to_json=False
-            )
-
-        markets = GetMarkets(chain=self.chain).get_available_markets()
-        available_liquidity = {
-            "long": {
-            },
-            "short": {
-            }
-        }
+        self.log.info("GMX v2 Available Liquidity")
 
-        print("\nGMX v2 Available Liquidity\n")
+        open_interest = OpenInterest(self.config).get_data(
+            to_json=False
+        )
 
         reserved_long_list = []
         reserved_short_list = []
         token_price_list = []
         mapper = []
         long_pool_amount_list = []
         long_reserve_factor_list = []
         long_open_interest_reserve_factor_list = []
         short_pool_amount_list = []
         short_reserve_factor_list = []
         short_open_interest_reserve_factor_list = []
         long_precision_list = []
         short_precision_list = []
 
-        for market_key in markets:
-
-            # this will filter out swap markets
-            market_symbol = markets[market_key]['market_symbol']
-            if "SWAP" in market_symbol:
-                continue
+        for market_key in self.markets.info:
+            self._filter_swap_markets()
+            self._get_token_addresses(market_key)
+            market_symbol = self.markets.get_market_symbol(market_key)
+            long_decimal_factor = self.markets.get_decimal_factor(
+                market_key=market_key,
+                long=True,
+                short=False
+            )
+            short_decimal_factor = self.markets.get_decimal_factor(
+                market_key=market_key,
+                long=False,
+                short=True
+            )
+            long_precision = 10**(30 + long_decimal_factor)
+            short_precision = 10**(30 + short_decimal_factor)
+            oracle_precision = 10**(30 - long_decimal_factor)
 
             # collate market symbol to map dictionary later
-            mapper = mapper + [market_symbol]
-
-            # calculate long pool metrics
-            long_token_address = markets[market_key]['long_token_address']
-            long_pool_amount, long_reserve_factor,\
-                long_open_interest_reserve_factor = self.get_max_reserved_usd(
-                    market_key,
-                    long_token_address,
-                    True
-                )
-            long_precision = 10**(
-                30+markets[market_key]['long_token_metadata']['decimals']
-            )
+            mapper.append(market_symbol)
 
-            # collate long side lists to iterate through
-            reserved_long_list = (
-                reserved_long_list + [open_interest['long'][market_symbol]]
-            )
-            long_pool_amount_list = long_pool_amount_list + [long_pool_amount]
-            long_reserve_factor_list = (
-                long_reserve_factor_list + [long_reserve_factor]
+            # LONG POOL
+            (
+                long_pool_amount,
+                long_reserve_factor,
+                long_open_interest_reserve_factor
+            ) = self.get_max_reserved_usd(
+                market_key,
+                self._long_token_address,
+                True
             )
-            long_open_interest_reserve_factor_list = (
-                long_open_interest_reserve_factor_list +
-                [long_open_interest_reserve_factor]
+            reserved_long_list.append(open_interest['long'][market_symbol])
+            long_pool_amount_list.append(long_pool_amount)
+            long_reserve_factor_list.append(long_reserve_factor)
+            long_open_interest_reserve_factor_list.append(
+                long_open_interest_reserve_factor
             )
-            long_precision_list = long_precision_list + [long_precision]
+            long_precision_list.append(long_precision)
 
-            # calculate short pool metrics
-            short_token_address = markets[market_key]['short_token_address']
+            # SHORT POOL
             (
                 short_pool_amount,
                 short_reserve_factor,
                 short_open_interest_reserve_factor
             ) = self.get_max_reserved_usd(
                 market_key,
-                short_token_address,
+                self._short_token_address,
                 False
             )
-            short_precision = 10**(
-                30 + markets[market_key]['short_token_metadata']['decimals']
-            )
-
-            # collate short side lists to iterate through
-            reserved_short_list = (
-                reserved_short_list + [open_interest['short'][market_symbol]]
-            )
-            short_pool_amount_list = (
-                short_pool_amount_list + [short_pool_amount]
-            )
-            short_reserve_factor_list = (
-                short_reserve_factor_list + [short_reserve_factor]
-            )
-            short_open_interest_reserve_factor_list = (
-                short_open_interest_reserve_factor_list +
-                [short_open_interest_reserve_factor]
-            )
-            short_precision_list = short_precision_list + [short_precision]
-
-            # calculate token price
-            prices = GetOraclePrices(chain=self.chain).get_recent_prices()
-            oracle_precision = 10**(
-                30-markets[market_key]['long_token_metadata']['decimals']
+            reserved_short_list.append(open_interest['short'][market_symbol])
+            short_pool_amount_list.append(short_pool_amount)
+            short_reserve_factor_list.append(short_reserve_factor)
+            short_open_interest_reserve_factor_list.append(
+                short_open_interest_reserve_factor
             )
+            short_precision_list.append(short_precision)
 
+            # Calculate token price
+            prices = OraclePrices(chain=self.config.chain).get_recent_prices()
             token_price = np.median(
                 [
                     float(
-                        prices[long_token_address]['maxPriceFull']
+                        prices[self._long_token_address]['maxPriceFull']
                     ) / oracle_precision,
                     float(
-                        prices[long_token_address]['minPriceFull']
+                        prices[self._long_token_address]['minPriceFull']
                     ) / oracle_precision
                 ]
             )
-
-            # collate token price to iterate through
-            token_price_list = token_price_list + [token_price]
+            token_price_list.append(token_price)
 
         # TODO - Series of sleeps to stop ratelimit on the RPC, should have
         # retry
         long_pool_amount_output = execute_threading(long_pool_amount_list)
         time.sleep(0.2)
 
         short_pool_amount_output = execute_threading(short_pool_amount_list)
@@ -256,88 +168,112 @@
             reserved_long_list,
             reserved_short_list,
             token_price_list,
             mapper,
             long_precision_list,
             short_precision_list
         ):
-            print(token_symbol)
+            self.log.info("Token: {}".format(token_symbol))
 
             # select the lesser of maximum value of pool reserves or open
             # interest limit
             if long_open_interest_reserve_factor < long_reserve_factor:
                 long_reserve_factor = long_open_interest_reserve_factor
 
+            if "2" in token_symbol:
+                long_pool_amount = long_pool_amount / 2
+
             long_max_reserved_tokens = (
                 long_pool_amount * long_reserve_factor
             )
 
             long_max_reserved_usd = (
                 long_max_reserved_tokens / long_precision * token_price
             )
 
             long_liquidity = long_max_reserved_usd - float(reserved_long)
 
-            print(
+            self.log.info(
                 "Available Long Liquidity: ${}".format(
                     numerize.numerize(long_liquidity)
                 )
             )
-            available_liquidity['long'][token_symbol] = long_liquidity
 
             # select the lesser of maximum value of pool reserves or open
             # interest limit
             if short_open_interest_reserve_factor < short_reserve_factor:
                 short_reserve_factor = short_open_interest_reserve_factor
 
-            short_max_reserved_usd = (short_pool_amount*short_reserve_factor)
+            short_max_reserved_usd = (short_pool_amount * short_reserve_factor)
 
             short_liquidity = (
                 short_max_reserved_usd / short_precision - float(
                     reserved_short
                 )
             )
-            print(
-                "Available Short Liquidity: ${}\n".format(
+
+            # If its a single side market need to calculate on token
+            # amount rather than $ value
+            if "2" in token_symbol:
+                short_pool_amount = short_pool_amount / 2
+
+                short_max_reserved_tokens = (
+                    short_pool_amount * short_reserve_factor
+                )
+
+                short_max_reserved_usd = (
+                    short_max_reserved_tokens / short_precision * token_price
+                )
+
+                short_liquidity = short_max_reserved_usd - float(reserved_short)
+
+            self.log.info(
+                "Available Short Liquidity: ${}".format(
                     numerize.numerize(short_liquidity)
                 )
             )
 
-            available_liquidity['short'][token_symbol] = short_liquidity
+            self.output['long'][token_symbol] = long_liquidity
+            self.output['short'][token_symbol] = short_liquidity
 
-        return available_liquidity
+        return self.output
 
-    def get_max_reserved_usd(self, market: str, token: str, is_long: bool):
+    def get_max_reserved_usd(self, market: str, token: str, is_long: bool) -> (
+        Tuple[Any, Any, Any]
+    ):
         """
         For a given market, long/short token and pool direction get the
         uncalled web3 functions to calculate pool size, pool reserve factor
         and open interest reserve factor
 
         Parameters
         ----------
-        market : str
+        market: str
             contract address of GMX market.
-        token : str
+        token: str
             contract address of long or short token.
-        is_long : bool
+        is_long: bool
             pass True for long pool or False for short.
 
         Returns
         -------
-        pool_amount : web3.contract_obj
+        pool_amount: web3.contract_obj
             uncalled web3 contract object for pool amount.
-        reserve_factor : web3.contract_obj
+        reserve_factor: web3.contract_obj
             uncalled web3 contract object for pool reserve factor.
-        open_interest_reserve_factor : web3.contract_obj
+        open_interest_reserve_factor: web3.contract_obj
             uncalled web3 contract object for open interest reserve factor.
 
         """
+        pool_amount: Any  # Type: web3._utils.datatypes.getUint
+        reserve_factor: Any  # Type: web3._utils.datatypes.getUint
+        open_interest_reserve_factor: Any  # Type: web3._utils.datatypes.getUint
 
         # get web3 datastore object
-        datastore = get_datastore_contract(self.chain)
+        datastore = get_datastore_contract(self.config)
 
         # get hashed keys for datastore
         pool_amount_hash_data = pool_amount_key(
             market,
             token
         )
         reserve_factor_hash_data = reserve_factor_key(
@@ -364,10 +300,10 @@
         return pool_amount, reserve_factor, open_interest_reserve_factor
 
 
 if __name__ == "__main__":
     data = GetAvailableLiquidity(
         chain="arbitrum",
         use_local_datastore=False
-    ).get_available_liquidity(
+    ).get_data(
         to_csv=False
     )
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_claimable_fees.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_pool_tvl.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,204 +1,204 @@
 import numpy as np
 
-from numerize import numerize
-
-from .get_markets import GetMarkets
-from .gmx_utils import (
-    execute_threading, make_timestamped_dataframe, save_csv_to_datastore
+from .get_markets import Markets
+from .get_oracle_prices import OraclePrices
+from ..keys import pool_amount_key
+from ..gmx_utils import (
+    get_datastore_contract, save_json_file_to_datastore,
+    make_timestamped_dataframe, save_csv_to_datastore
 )
-from .get_oracle_prices import GetOraclePrices
-from .keys import get_datastore_contract, claimable_fee_amount_key
 
 
-class GetClaimableFees:
-    def __init__(self, chain: str):
-        self.chain = chain
+class GetPoolTVL:
+    def __init__(self, config: str):
+        self.config = config
+        self.oracle_prices_dict = OraclePrices(
+            chain=config.chain
+        ).get_recent_prices
 
-    def get_claimable_fees(self, to_json: bool = False, to_csv: bool = False):
+    def get_pool_balances(self, to_json: bool = False, to_csv: bool = False):
         """
-        Call to get the claimable fees across all pools on a given chain
-        defined in class init. Pass either to_json or to_csv to save locally in
-        datastore
+        Call to get the amounts across all pools on a given chain defined in
+        class init. Pass either to_json or to_csv to save locally in datastore
 
         Parameters
         ----------
         to_json : bool, optional
             save output to json file. The default is False.
         to_csv : bool, optional
             save out to csv file. The default is False.
 
         Returns
         -------
         data : dict
             dictionary of data.
 
         """
+        markets = Markets(self.config).get_available_markets()
+        pool_tvl_dict = {
+            "total_tvl": {},
+            "long_token": {},
+            "short_token": {}
+        }
+
+        for market in markets:
+            print("\n" + markets[market]['market_symbol'])
+
+            index_token_address = markets[market]['index_token_address']
+            long_token_metadata = markets[market]['long_token_metadata']
+            short_token_metadata = markets[market]['short_token_metadata']
+
+            long_token_balance, short_token_balance = self._query_balances(
+                market,
+                long_token_metadata,
+                short_token_metadata
+            )
+
+            long_precision = 10 ** long_token_metadata['decimals']
+            short_precision = 10 ** short_token_metadata['decimals']
+            long_token_balance = long_token_balance / long_precision
+            short_token_balance = short_token_balance / short_precision
+
+            # If market is synthetic we need to use the long token as the
+            # index token for price
+            # try:
+            #     if markets[market]['market_metadata']['synthetic']:
+            index_token_address = markets[market]['long_token_address']
+            # except KeyError:
+            #     pass
 
-        data = self._claimable_fees()
-
-        if to_json:
-            self.save_json_file_to_datastore(
-                "{}_claimable_fees.json".format(self.chain),
-                data
+            oracle_precision = 10 ** (
+                30 - markets[market]['long_token_metadata']['decimals']
             )
-        if to_csv:
-            dataframe = make_timestamped_dataframe(data)
-            save_csv_to_datastore(
-                "{}_total_fees.csv".format(self.chain),
-                dataframe
+            long_usd_balance = self._calculate_usd_value(
+                index_token_address,
+                long_token_balance,
+                oracle_precision
             )
-        else:
-            return data
-
-    def _claimable_fees(self):
-        """
-        Get total fees dictionary
-
-        Returns
-        -------
-        funding_apr : dict
-            dictionary of total fees for week so far.
-
-        """
-        markets = GetMarkets(chain=self.chain).get_available_markets()
+            short_usd_balance = short_token_balance
 
-        total_fees = 0
+            dictionary_key = markets[market]['market_symbol']
 
-        long_output_list = []
-        short_output_list = []
-        long_precision_list = []
-        long_token_price_list = []
-        mapper = []
-
-        for market_key in markets:
-            # TODO - currently filtering out swap markets
-            market_symbol = markets[market_key]['market_symbol']
-            if "SWAP" in market_symbol:
-                continue
-
-            long_token_address = markets[market_key]['long_token_address']
-            short_token_address = markets[market_key]['short_token_address']
-
-            # uncalled web3 object for long fees
-            long_output = self._get_claimable_fee_amount(
-                market_key,
-                long_token_address
+            pool_tvl_dict['total_tvl'][dictionary_key] = (
+                long_usd_balance + short_usd_balance
             )
-
-            prices = GetOraclePrices(chain=self.chain).get_recent_prices()
-            oracle_precision = 10 ** (
-                30-markets[market_key]['long_token_metadata']['decimals']
+            pool_tvl_dict['long_token'][dictionary_key] = (
+                markets[market]['long_token_address']
             )
-            long_token_price = np.median(
-                [
-                    float(
-                        prices[long_token_address]['maxPriceFull']
-                    ) / oracle_precision,
-                    float(
-                        prices[long_token_address]['minPriceFull']
-                    ) / oracle_precision
-                ]
+            pool_tvl_dict['short_token'][dictionary_key] = (
+                markets[market]['short_token_address']
             )
 
-            long_token_price_list = long_token_price_list + [long_token_price]
-
-            long_precision = 10**(
-                markets[market_key]['long_token_metadata']['decimals']-1
-            )
-
-            long_precision_list = long_precision_list + [long_precision]
-
-            # uncalled web3 object for short fees
-            short_output = self._get_claimable_fee_amount(
-                market_key,
-                short_token_address
-            )
-
-            # add the uncalled web3 object to list
-            long_output_list = long_output_list + [long_output]
-
-            # add the uncalled web3 object to list
-            short_output_list = short_output_list + [short_output]
-
-            # add the market symbol to a list to use to map to dictionary later
-            mapper = mapper + [markets[market_key]['market_symbol']]
-
-        # feed the uncalled web3 objects into threading function
-        long_threaded_output = execute_threading(long_output_list)
-        short_threaded_output = execute_threading(short_output_list)
-
-        for (
-            long_claimable_fees,
-            short_claimable_fees,
-            long_precision,
-            long_token_price,
-            token_symbol
-        ) in zip(
-            long_threaded_output,
-            short_threaded_output,
-            long_precision_list,
-            long_token_price_list,
-            mapper
-        ):
-            # convert raw outputs into USD value
-            long_claimable_usd = (
-                long_claimable_fees / long_precision
-            ) * long_token_price
-
-            # TODO - currently all short fees are collected in USDC which is
-            # 6 decimals
-            short_claimable_usd = short_claimable_fees / (10 ** 6)
-
-            print(token_symbol)
             print(
-                "Long Claimable Fees: ${}".format(
-                    numerize.numerize(long_claimable_usd)
+                "Pool USD Value: ${}".format(
+                    long_usd_balance + short_usd_balance
                 )
             )
 
-            print("Short Claimable Fees: ${}\n".format(
-                numerize.numerize(short_claimable_usd))
+        if to_json:
+            save_json_file_to_datastore(
+                "{}_pool_tvl.json".format(self.config.chain),
+                pool_tvl_dict
             )
 
-            total_fees += long_claimable_usd + short_claimable_usd
-
-        return {'latest_total_fees': total_fees}
+        if to_csv:
+            dataframe = make_timestamped_dataframe(pool_tvl_dict['total_tvl'])
+            save_csv_to_datastore(
+                "{}_total_tvl.csv".format(self.config.chain),
+                dataframe
+            )
+        else:
+            return pool_tvl_dict
 
-    def _get_claimable_fee_amount(
-        self, market_address: str, token_address: str
+    def _query_balances(
+        self,
+        market: str,
+        long_token_metadata: dict,
+        short_token_metadata: dict
     ):
         """
-        For a given market and long/short side of the pool get the raw output
-        for pending fees
+        For a given GMX market get the balance of long and short tokens from
+        the datastore contract
 
         Parameters
         ----------
-        market_address : str
-            addess of the GMX market.
-        token_address : str
-            address of either long or short collateral token.
+        market : str
+            contract address of the market.
+        long_token_metadata : dict
+            dictionary containing address.
+        short_token_metadata : dict
+            dictionary containing address.
 
         Returns
         -------
-        claimable_fee : web3 datastore obj
-            uncalled obj of the datastore contract.
-
-        """
-
-        datastore = get_datastore_contract(self.chain)
-
-        # create hashed key to query the datastore
-        claimable_fees_amount_hash_data = claimable_fee_amount_key(
-            market_address,
-            token_address
+        long_token_balance : int
+            amount of tokens.
+        short_token_balance : int
+            amount of tokens.
+        """
+        datastore = get_datastore_contract(self.config)
+        pool_amount_hash_data = pool_amount_key(
+            market,
+            long_token_metadata['address']
         )
-
-        claimable_fee = datastore.functions.getUint(
-            claimable_fees_amount_hash_data
+        long_token_balance = datastore.functions.getUint(
+            pool_amount_hash_data
+        ).call()
+
+        datastore = get_datastore_contract(self.config)
+        pool_amount_hash_data = pool_amount_key(
+            market,
+            short_token_metadata['address']
         )
+        short_token_balance = datastore.functions.getUint(
+            pool_amount_hash_data
+        ).call()
+
+        return long_token_balance, short_token_balance
+
+    def _calculate_usd_value(
+        self,
+        token_address: str,
+        token_balance: int,
+        oracle_precision: int,
+    ):
+        """
+        Calculate the USD value from token amounts for a given token address
+
+        Parameters
+        ----------
+        token_address : str
+            contracta address.
+        token_balance : int
+            amount of tokens.
+        oracle_precision : int
+            factor to power 10 to divide price api output.
 
-        return claimable_fee
+        Returns
+        -------
+        value: float
+            USD value of the token amount.
+        """
+        try:
+            token_price = np.median(
+                [
+                    float(
+                        self.oracle_prices_dict()[
+                            token_address
+                        ]['maxPriceFull']
+                    ) / oracle_precision,
+                    float(
+                        self.oracle_prices_dict()[
+                            token_address
+                        ]['minPriceFull']
+                    ) / oracle_precision
+                ]
+            )
+            return token_price * token_balance
+        except KeyError:
+            return token_balance
 
 
 if __name__ == "__main__":
-    data = GetClaimableFees(chain="arbitrum").get_claimable_fees(to_csv=True)
+    # chain = sys.argv[1]
+    pool_dict = GetPoolTVL(chain="arbitrum").get_pool_balances(to_csv=True)
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_contract_balance.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_contract_balance.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import numpy as np
 
-from .gmx_utils import get_token_balance_contract, save_json_file_to_datastore
-from .get_markets import GetMarkets
-from .get_oracle_prices import GetOraclePrices
+from .get import GetData
+from .get_markets import Markets
+from .get_oracle_prices import OraclePrices
+from ..gmx_utils import get_token_balance_contract, save_json_file_to_datastore
 
 
-class GetPoolTVL:
-    def __init__(self, chain):
-        self.chain = chain
-        self.oracle_prices_dict = GetOraclePrices(
-            chain=chain
+class GetPoolTVL(GetData):
+    def __init__(self, config):
+        super().__init__(config)
+        self.oracle_prices_dict = OraclePrices(
+            chain=config.chain
         ).get_recent_prices
 
     def get_pool_balances(self, to_json: bool = False):
         """
         Get the USD balances of each pool and optionally save to json file
 
         Parameters
@@ -23,19 +24,19 @@
 
         Returns
         -------
         pool_tvl_dict : dict
             dictionary of total USD value per pool.
 
         """
-        markets = GetMarkets(chain=self.chain).get_available_markets()
+        markets = Markets(self.config).get_available_markets()
         pool_tvl_dict = {}
 
         for market in markets:
-            print("\n"+markets[market]['market_symbol'])
+            print("\n" + markets[market]['market_symbol'])
 
             long_token_address = markets[market]['long_token_address']
 
             short_token_address = markets[market]['short_token_address']
             long_token_balance, short_token_balance = self._query_balances(
                 market,
                 long_token_address,
@@ -57,21 +58,21 @@
                 'total_tvl': long_usd_balance + short_token_balance,
                 'long_token': markets[market]['long_token_address'],
                 'short_token': markets[market]['short_token_address']
             }
 
             print(
                 "Pool USD Value: ${}".format(
-                    long_usd_balance+short_token_balance
+                    long_usd_balance + short_token_balance
                 )
             )
 
         if to_json:
             save_json_file_to_datastore(
-                "{}_pool_tvl.json".format(self.chain),
+                "{}_pool_tvl.json".format(self.config.chain),
                 pool_tvl_dict
             )
         else:
             return pool_tvl_dict
 
     def _query_balances(
         self, market: str, long_token_address: str, short_token_address: str
@@ -94,22 +95,22 @@
         long_token_balance : float
             balance of token in adjusted significant figures.
         short_token_balance : float
             balance of token in adjusted significant figures.
 
         """
         long_token_contract = get_token_balance_contract(
-            self.chain,
+            self.config,
             long_token_address
         )
         long_token_balance = long_token_contract.functions.balanceOf(
             market
         ).call() / 10 ** long_token_contract.functions.decimals().call()
         short_token_contract = get_token_balance_contract(
-            self.chain,
+            self.config,
             short_token_address
         )
         short_token_balance = short_token_contract.functions.balanceOf(
             market
         ).call() / 10 ** short_token_contract.functions.decimals().call()
 
         return long_token_balance, short_token_balance
@@ -157,8 +158,8 @@
             print("Contract address not known")
             return token_balance
 
 
 if __name__ == "__main__":
     # chain = sys.argv[1]
     # chain = 'arbitrum'
-    pool_dict = GetPoolTVL(chain='arbitrum').get_pool_balances(to_json=False)
+    pool_dict = GetPoolTVL(chain='arbitrum').get_data(to_json=False)
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_markets.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_markets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,43 @@
-from .gmx_utils import (
+from ..gmx_utils import (
     contract_map, get_tokens_address_dict, get_reader_contract
 )
 
-from .get_oracle_prices import GetOraclePrices
+from .get_oracle_prices import OraclePrices
 
 
-class GetMarkets:
-    def __init__(self, chain):
-        self.chain = chain
+class Markets:
+    def __init__(self, config):
+        self.config = config
+        self.info = self._process_markets()
+
+    def get_index_token_address(self, market_key: str) -> str:
+        return self.info[market_key]['index_token_address']
+
+    def get_long_token_address(self, market_key: str) -> str:
+        return self.info[market_key]['long_token_address']
+
+    def get_short_token_address(self, market_key: str) -> str:
+        return self.info[market_key]['short_token_address']
+
+    def get_market_symbol(self, market_key: str) -> str:
+        return self.info[market_key]['market_symbol']
+
+    def get_decimal_factor(
+        self, market_key: str, long: bool = False, short: bool = False
+    ) -> int:
+        if long:
+            return self.info[market_key]['long_token_metadata']['decimals']
+        elif short:
+            return self.info[market_key]['short_token_metadata']['decimals']
+        else:
+            return self.info[market_key]['market_metadata']['decimals']
+
+    def is_synthetic(self, market_key: str) -> bool:
+        return self.info[market_key]['market_metadata']['synthetic']
 
     def get_available_markets(self):
         """
         Get the available markets on a given chain
 
         Returns
         -------
@@ -27,62 +53,68 @@
 
         Returns
         -------
         Markets: tuple
             tuple of raw output from the reader contract.
 
         """
-        reader_contract = get_reader_contract(self.chain)
+        reader_contract = get_reader_contract(self.config)
         data_store_contract_address = (
-            contract_map[self.chain]['datastore']['contract_address']
+            contract_map[self.config.chain]['datastore']['contract_address']
         )
 
         return reader_contract.functions.getMarkets(
             data_store_contract_address,
             0,
-            20
+            25
         ).call()
 
     def _process_markets(self):
         """
         Call and process the raw market data
 
         Returns
         -------
         decoded_markets : dict
             dictionary decoded market data.
 
         """
-        token_address_dict = get_tokens_address_dict(self.chain)
+        token_address_dict = get_tokens_address_dict(self.config.chain)
         raw_markets = self._get_available_markets_raw()
 
         decoded_markets = {}
         for raw_market in raw_markets:
             try:
 
-                if not self._check_if_index_token_in_signed_prices_api(raw_market[1]):
+                if not self._check_if_index_token_in_signed_prices_api(
+                    raw_market[1]
+                ):
                     continue
+                market_symbol = token_address_dict[raw_market[1]]['symbol']
+                if raw_market[2] == raw_market[3]:
+                    market_symbol = f"{market_symbol}2"
                 decoded_markets[raw_market[0]] = {
                     'gmx_market_address': raw_market[0],
-                    'market_symbol': (
-                        token_address_dict[raw_market[1]]['symbol']
-                    ),
+                    'market_symbol': market_symbol,
                     'index_token_address': raw_market[1],
                     'market_metadata': token_address_dict[raw_market[1]],
                     'long_token_metadata': token_address_dict[raw_market[2]],
                     'long_token_address': raw_market[2],
                     'short_token_metadata': token_address_dict[raw_market[3]],
                     'short_token_address': raw_market[3]
                 }
 
             # If KeyError it is because there is no market symbol and it is a
             # swap market
             except KeyError:
-                if not self._check_if_index_token_in_signed_prices_api(raw_market[1]):
+                if not self._check_if_index_token_in_signed_prices_api(
+                    raw_market[1]
+                ):
                     continue
+
                 decoded_markets[raw_market[0]] = {
                     'gmx_market_address': raw_market[0],
                     'market_symbol': 'SWAP {}-{}'.format(
                         token_address_dict[raw_market[2]]['symbol'],
                         token_address_dict[raw_market[3]]['symbol']
                     ),
                     'index_token_address': raw_market[1],
@@ -97,23 +129,23 @@
                 }
 
         return decoded_markets
 
     def _check_if_index_token_in_signed_prices_api(self, index_token_address):
 
         try:
-            prices = GetOraclePrices(chain=self.chain).get_recent_prices()
+            prices = OraclePrices(chain=self.config.chain).get_recent_prices()
 
             if index_token_address == "0x0000000000000000000000000000000000000000":
                 return True
             prices[index_token_address]
             return True
         except KeyError:
 
             print("{} market not live on GMX yet..".format(index_token_address))
             return False
 
 
 if __name__ == '__main__':
-    raw_markets = GetMarkets(
+    raw_markets = Markets(
         chain="arbitrum"
-    ).get_available_markets(clean=False)
+    ).get_available_markets()
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_open_positions.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import logging
 import numpy as np
 
-from .gmx_utils import (
+from ..gmx_utils import (
     get_reader_contract, contract_map, get_tokens_address_dict,
     convert_to_checksum_address
 )
-from .get_markets import GetMarkets
-from .get_oracle_prices import GetOraclePrices
+from .get_markets import Markets
+from .get_oracle_prices import OraclePrices
 
 chain = 'arbitrum'
 
 
 class GetOpenPositions:
     def __init__(self, chain):
         self.chain = chain
-        self.markets = GetMarkets(chain=chain).get_available_markets()
+        self.markets = Markets(chain=chain).get_available_markets()
         self.reader_contract = get_reader_contract(chain)
 
     def get_positions(self, address: str):
         """
         Get all open positions for a given address on the chain defined in
         class init
 
@@ -91,15 +91,15 @@
         leverage = (
             raw_position[1][0] / 10 ** 30
         ) / (
             raw_position[1][2] / 10 ** chain_tokens[
                 raw_position[0][2]
             ]['decimals']
         )
-        prices = GetOraclePrices(chain=chain).get_recent_prices()
+        prices = OraclePrices(chain=chain).get_recent_prices()
         mark_price = np.median(
             [
                 float(
                     prices[market_info['index_token_address']]['maxPriceFull']
                 ),
                 float(
                     prices[market_info['index_token_address']]['minPriceFull']
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_open_positons.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_open_positions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 import logging
 import numpy as np
 
-from .gmx_utils import (
-    get_reader_contract, contract_map, get_tokens_address_dict,
-    convert_to_checksum_address
-)
-from .get_markets import GetMarkets
-from .get_oracle_prices import GetOraclePrices
+from .get import GetData
+from .get_oracle_prices import OraclePrices
+
+from ..gmx_utils import (get_tokens_address_dict, convert_to_checksum_address)
 
 chain = 'arbitrum'
 
 
-class GetOpenPositions:
-    def __init__(self, chain):
-        self.chain = chain
-        self.markets = GetMarkets(chain=chain).get_available_markets()
-        self.reader_contract = get_reader_contract(chain)
+class GetOpenPositions(GetData):
+    def __init__(self, config: str, address: str):
+        super().__init__(config)
+        self.address = convert_to_checksum_address(config, address)
 
-    def get_positions(self, address: str):
+    def get_data(self):
         """
         Get all open positions for a given address on the chain defined in
         class init
 
         Parameters
         ----------
         address : str
@@ -30,59 +27,63 @@
         Returns
         -------
         processed_positions : dict
             a dictionary containing the open positions, where asset and
             direction are the keys.
 
         """
-        address = convert_to_checksum_address(self.chain, address)
+        raw_positions = self.reader_contract.functions.getAccountPositions(
+            self.data_store_contract_address,
+            self.address,
+            0,
+            10
+        ).call()
 
-        raw_positions = self. _query_for_positions(address)
         if len(raw_positions) == 0:
             logging.info(
                 'No positions open for address: "{}"" on {}.'.format(
                     address,
-                    self.chain.title()
+                    self.config.chain.title()
                 )
             )
         processed_positions = {}
 
         for raw_position in raw_positions:
-            processed_position = self._process_positon(raw_position)
+            processed_position = self._get_data_processing(raw_position)
 
             # TODO - maybe a better way of building the key?
             if processed_position['is_long']:
                 direction = 'long'
             else:
                 direction = 'short'
 
             key = "{}_{}".format(
-                processed_position['market_symbol'],
+                processed_position['market_symbol'][0],
                 direction
             )
             processed_positions[key] = processed_position
 
         return processed_positions
 
-    def _process_positon(self, raw_position: tuple):
+    def _get_data_processing(self, raw_position: tuple):
         """
         A tuple containing the raw information return from the reader contract
         query GetAccountPositions
 
         Parameters
         ----------
         raw_position : tuple
             raw information return from the reader contract .
 
         Returns
         -------
         dict
             a processed dictionary containing info on the positions.
         """
-        market_info = self.markets[raw_position[0][1]]
+        market_info = self.markets.info[raw_position[0][1]]
 
         chain_tokens = get_tokens_address_dict(chain)
 
         entry_price = (
             raw_position[1][0] / raw_position[1][1]
         ) / 10 ** (
             30 - chain_tokens[market_info['index_token_address']]['decimals']
@@ -91,15 +92,15 @@
         leverage = (
             raw_position[1][0] / 10 ** 30
         ) / (
             raw_position[1][2] / 10 ** chain_tokens[
                 raw_position[0][2]
             ]['decimals']
         )
-        prices = GetOraclePrices(chain=chain).get_recent_prices()
+        prices = OraclePrices(chain=chain).get_recent_prices()
         mark_price = np.median(
             [
                 float(
                     prices[market_info['index_token_address']]['maxPriceFull']
                 ),
                 float(
                     prices[market_info['index_token_address']]['minPriceFull']
@@ -108,17 +109,19 @@
         ) / 10 ** (
             30 - chain_tokens[market_info['index_token_address']]['decimals']
         )
 
         return {
             "account": raw_position[0][0],
             "market": raw_position[0][1],
-            "market_symbol": self.markets[raw_position[0][1]]['market_symbol'],
+            "market_symbol": (
+                self.markets.info[raw_position[0][1]]['market_symbol'],
+            ),
             "collateral_token": chain_tokens[raw_position[0][2]]['symbol'],
-            "position_size": raw_position[1][0]/10**30,
+            "position_size": raw_position[1][0] / 10**30,
             "size_in_tokens": raw_position[1][1],
             "entry_price": (
                 (
                     raw_position[1][0] / raw_position[1][1]
                 ) / 10 ** (
                     30 - chain_tokens[
                         market_info['index_token_address']
@@ -141,50 +144,14 @@
                 (
                     1 - (mark_price / entry_price)
                 ) * leverage
             ) * 100,
             "mark_price": mark_price
         }
 
-    def _query_for_positions(
-        self, address: str, start: int = 0, end: int = 10
-    ):
-        """
-        For a given evm address call the getAccountPositions function from
-        the reader contract to return positions for a given start and end
-        position
-
-        Parameters
-        ----------
-        address : str
-            evm address .
-        start: int
-            location of first position to fetch, default is 0
-        end: int
-            location of last position to fetch, default is 10
-
-        Returns
-        -------
-        tuple
-            a tuple of raw positions info currently open for the given address.
-
-        """
-
-        reader_contract = get_reader_contract(self.chain)
-        data_store_contract_address = (
-            contract_map[self.chain]['datastore']['contract_address']
-        )
-
-        return reader_contract.functions.getAccountPositions(
-            data_store_contract_address,
-            address,
-            start,
-            end
-        ).call()
-
 
 if __name__ == "__main__":
     address = "0x99f5585dcc32e2238634f11f32d9be9bd5e98b49"
-    positions = GetOpenPositions(chain='arbitrum').get_positions(address)
+    positions = GetOpenPositions(chain='arbitrum', address=address).get_data()
 
     for position in positions:
         print(positions[position])
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/get_oracle_prices.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/get/get_oracle_prices.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
 
-class GetOraclePrices:
+class OraclePrices:
     def __init__(self, chain: str):
         self.chain = chain
         self.oracle_url = {
             "arbitrum": (
                 "https://arbitrum-api.gmxinfra.io/signed_prices/latest"
             ),
             "avalanche": (
@@ -59,8 +59,9 @@
         for i in output['signedPrices']:
             processed[i['tokenAddress']] = i
 
         return processed
 
 
 if __name__ == '__main__':
-    data = GetOraclePrices(chain="arbitrum").get_recent_prices()
+
+    pass
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/gmx_utils.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/gmx_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,16 +8,20 @@
 
 import pandas as pd
 
 from datetime import datetime
 
 from concurrent.futures import ThreadPoolExecutor
 
-
-base_dir = os.path.join(os.path.dirname(__file__), '..', '..')
+# Get the absolute path of the current script
+current_script_path = os.path.abspath(__file__)
+base_dir = os.path.abspath(
+    os.path.join(current_script_path, '..', '..', '..', '..')
+)
+package_dir = base_dir + '/gmx_python_sdk/'
 print('base_dir', base_dir)
 
 logging.basicConfig(
     format='{asctime} {levelname}: {message}',
     datefmt='%m/%d/%Y %I:%M:%S %p',
     style='{',
     level=logging.INFO
@@ -26,15 +30,14 @@
 
 # Functions required for multithreading
 def execute_call(call):
     return call.call()
 
 
 def execute_threading(function_calls):
-
     with ThreadPoolExecutor() as executor:
         results = list(executor.map(execute_call, function_calls))
     return results
 
 
 contract_map = {
     'arbitrum':
@@ -122,104 +125,59 @@
             "contract_address": "0x820F5FfC5b525cD4d88Cd91aCf2c28F16530Cc68",
             "abi_path": "contracts/avalanche/syntheticsrouter.json"
         }
     }
 }
 
 
-class Config:
+class ConfigManager:
 
-    def __init__(
-            self,
-            filepath: str = os.path.join(base_dir, "config.yaml")
-    ):
-        self.file_path = filepath
-        self.skeleton = {
-            'arbitrum': {
-                'rpc': None,
-                'chain_id': None
-            },
-            'avalanche': {
-                'rpc': None,
-                'chain_id': None
-            },
-            'private_key': None,
-            'user_wallet_address': None
-        }
+    def __init__(self, chain: str):
 
-    def load_config(self):
-        try:
-            config = yaml.safe_load(open(os.path.join(base_dir, "config.yaml")))
-            return self.test_config_format(config)
-        except FileNotFoundError:
-            print(f"Config file '{self.file_path}' not found.\nLoading blank template!")
-            return self.skeleton
-
-    def set_config(self, config):
-        print(f"Setting config file: '{self.file_path}'")
-        with open(self.file_path, 'w') as file:
-            yaml.dump(config, file)
+        self.chain = chain
+        self.rpc = None
+        self.chain_id = None
+        self.user_wallet_address = None
+        self.private_key = None
+        self.tg_bot_token = None
 
-    def test_config_format(self, config):
-
-        if config.keys() == self.skeleton.keys():
-            return config
-        else:
-            structure = """
-                {
-                'arbitrum': {
-                    'rpc': None,
-                    'chain_id': None
-                    },
-                'avalanche': {
-                    'rpc': None,
-                    'chain_id': None
-                    },
-                'private_key': None,
-                'user_wallet_address': None
-                }"""
-            raise Exception(
-            "Please make sure your config file matches the following structure:\n\n{}".format(
-                structure
-                )
-            )
+    def set_config(self, filepath: str = os.path.join(base_dir, "config.yaml")):
 
+        with open(filepath, 'r') as file:
+            config_file = yaml.safe_load(file)
 
-def get_config(filepath: str = os.path.join(base_dir, "config.yaml")):
+        self.set_rpc(config_file['rpcs'][self.chain])
+        self.set_chain_id(config_file['chain_ids'][self.chain])
+        self.set_wallet_address(config_file['user_wallet_address'])
+        self.set_private_key(config_file['private_key'])
 
-    config = Config(filepath).load_config()
+    def set_rpc(self, value):
+        self.rpc = value
 
-    if config['private_key'] is None:
-        logging.warning("Private key not set!")
+    def set_chain_id(self, value):
+        self.chain_id = value
 
-    if config['arbitrum']['rpc'] is None:
-        logging.warning("Arbitrum RPC not set!")
+    def set_wallet_address(self, value):
+        self.user_wallet_address = value
 
-    if config['avalanche']['rpc'] is None:
-        logging.warning("Avalanche RPC not set!")
+    def set_private_key(self, value):
+        self.private_key = value
 
-    if config['user_wallet_address'] is None:
-        logging.warning("Wallet address not set!")
 
-    return config
-
-
-def create_connection(rpc: str = None, chain: str = None):
+def create_connection(config):
     """
     Create a connection to the blockchain
     """
-    if rpc is None:
-        rpc = get_config()[chain]['rpc']
 
-    web3_obj = Web3(Web3.HTTPProvider(rpc))
+    web3_obj = Web3(Web3.HTTPProvider(config.rpc))
 
     return web3_obj
 
 
-def convert_to_checksum_address(chain: str, address: str):
+def convert_to_checksum_address(config, address: str):
     """
     Convert a given address to checksum format
 
     Parameters
     ----------
     chain : str
         arbitrum or avalanche.
@@ -228,16 +186,15 @@
 
     Returns
     -------
     str
         checksum formatted address.
 
     """
-
-    web3_obj = create_connection(chain=chain)
+    web3_obj = create_connection(config)
 
     # Added to support older versions of web3.py for now
     try:
         return web3_obj.toChecksumAddress(address)
     except AttributeError:
         return web3_obj.to_checksum_address(address)
 
@@ -264,43 +221,43 @@
     """
     contract_address = contract_map[chain][contract_name]["contract_address"]
 
     contract_abi = json.load(
         open(
             os.path.join(
                 base_dir,
+                'gmx_python_sdk',
                 contract_map[chain][contract_name]["abi_path"]
             )
         )
     )
     return web3_obj.eth.contract(
         address=contract_address,
         abi=contract_abi
     )
 
 
-def get_token_balance_contract(chain: str, contract_address: str):
+def get_token_balance_contract(config: str, contract_address: str):
     """
     Get the contract object required to query a users token balance
 
     Parameters
     ----------
     chain : str
         arbitrum or avalanche.
     contract_address : str
         the token to determine the balance of.
 
     """
-    rpc = get_config()[chain]['rpc']
 
-    web3_obj = create_connection(rpc)
+    web3_obj = create_connection(config)
     contract_abi = json.load(
         open(
             os.path.join(
-                base_dir,
+                package_dir,
                 'contracts',
                 'balance_abi.json'
             )
         )
     )
     return web3_obj.eth.contract(
         address=contract_address,
@@ -319,15 +276,14 @@
 
     Returns
     -------
     token_address_dict : dict
         dictionary containing available tokens to trade on GMX.
 
     """
-
     url = {
         "arbitrum": "https://arbitrum-api.gmxinfra.io/tokens",
         "avalanche": "https://avalanche-api.gmxinfra.io/tokens"
     }
 
     try:
         response = requests.get(url[chain])
@@ -346,108 +302,103 @@
 
     for token_info in token_infos:
         token_address_dict[token_info['address']] = token_info
 
     return token_address_dict
 
 
-def get_reader_contract(chain: str):
+def get_reader_contract(config):
     """
     Get a reader contract web3_obj for a given chain
 
     Parameters
     ----------
     chain : str
         avalanche or arbitrum.
 
     """
-    rpc = get_config()[chain]['rpc']
 
-    web3_obj = create_connection(rpc)
+    web3_obj = create_connection(config)
     return get_contract_object(
         web3_obj,
         'syntheticsreader',
-        chain
+        config.chain
     )
 
 
-def get_event_emitter_contract(chain: str):
+def get_event_emitter_contract(config):
     """
     Get a event emitter contract web3_obj for a given chain
 
     Parameters
     ----------
     chain : str
         avalanche or arbitrum.
 
     """
-    rpc = get_config()[chain]['rpc']
 
-    web3_obj = create_connection(rpc)
+    web3_obj = create_connection(config)
     return get_contract_object(
         web3_obj,
         'eventemitter',
-        chain
+        config.chain
     )
 
 
-def get_datastore_contract(chain: str):
+def get_datastore_contract(config):
     """
     Get a datastore contract web3_obj for a given chain
 
     Parameters
     ----------
     chain : str
         avalanche or arbitrum.
 
     """
-    rpc = get_config()[chain]['rpc']
 
-    web3_obj = create_connection(rpc)
+    web3_obj = create_connection(config)
     return get_contract_object(
         web3_obj,
         'datastore',
-        chain
+        config.chain
     )
 
 
-def get_exchange_router_contract(chain: str):
+def get_exchange_router_contract(config):
     """
     Get a exchange router contract web3_obj for a given chain
 
     Parameters
     ----------
     chain : str
         avalanche or arbitrum.
 
     """
-    rpc = get_config()[chain]['rpc']
 
-    web3_obj = create_connection(rpc)
+    web3_obj = create_connection(config)
     return get_contract_object(
         web3_obj,
         'exchangerouter',
-        chain
+        config.chain
     )
 
 
-def create_signer(chain: str):
+def create_signer(config: str):
     """
     Creastea a signer for a given chain
 
     Parameters
     ----------
     chain : str
         avalanche or arbitrum.
 
     """
-    config = get_config()
 
-    private_key = config['private_key']
-    rpc = config[chain]['rpc']
+    private_key = config.private_key
+    rpc = config.rpc
     web3_obj = create_connection(rpc)
 
     return web3_obj.eth.account.from_key(private_key)
 
 
 def create_hash(data_type_list: list, data_value_list: list):
     """
@@ -485,30 +436,31 @@
     bytes
         hashed string.
 
     """
     return create_hash(["string"], [string])
 
 
-def get_execution_price_and_price_impact(chain: str, params: dict, decimals: int):
+def get_execution_price_and_price_impact(
+    config, params: dict, decimals: int
+):
     """
     Get the execution price and price impact for a position
 
     Parameters
     ----------
     chain : str
         arbitrum or avalanche.
     params : dict
         dictionary of the position parameters.
     decimals : int
         number of decimals of the token being traded eg ETH == 18.
 
     """
-
-    reader_contract_obj = get_reader_contract(chain)
+    reader_contract_obj = get_reader_contract(config)
 
     output = reader_contract_obj.functions.getExecutionPrice(
         params['data_store_address'],
         params['market_key'],
         params['index_token_price'],
         params['position_size_in_usd'],
         params['position_size_in_tokens'],
@@ -516,29 +468,28 @@
         params['is_long'],
     ).call()
 
     return {'execution_price': output[2] / 10**(PRECISION - decimals),
             'price_impact_usd': output[0] / 10**PRECISION}
 
 
-def get_estimated_swap_output(chain: str, params: dict):
+def get_estimated_swap_output(config, params: dict):
     """
     For a given chain and requested swap get the amount of tokens
     out and the price impact the swap will have.
 
     Parameters
     ----------
     chain : str
         arbitrum or avalanche.
     params : dict
         dictionary of the swap parameters.
 
     """
-
-    reader_contract_obj = get_reader_contract(chain)
+    reader_contract_obj = get_reader_contract(config)
 
     output = reader_contract_obj.functions.getSwapAmountOut(
         params['data_store_address'],
         params['market_addresses'],
         params['token_prices_tuple'],
         params['token_in'],
         params['token_amount_in'],
@@ -546,57 +497,55 @@
     ).call()
 
     return {'out_token_amount': output[0],
             'price_impact_usd': output[1]
             }
 
 
-def get_estimated_deposit_amount_out(chain: str, params: dict):
+def get_estimated_deposit_amount_out(config, params: dict):
     """
     For a given chain and requested deposit amount get the amount of
     gm expected to be output.
 
     Parameters
     ----------
     chain : str
         arbitrum or avalanche.
     params : dict
         dictionary of the gm input parameters.
 
     """
-
-    reader_contract_obj = get_reader_contract(chain)
+    reader_contract_obj = get_reader_contract(config)
 
     output = reader_contract_obj.functions.getDepositAmountOut(
         params['data_store_address'],
         params['market_addresses'],
         params['token_prices_tuple'],
         params['long_token_amount'],
         params['short_token_amount'],
         params['ui_fee_receiver'],
     ).call()
 
     return output
 
 
-def get_estimated_withdrawal_amount_out(chain: str, params: dict):
+def get_estimated_withdrawal_amount_out(config, params: dict):
     """
     For a given chain and requested withdrawal amount get the amount of
     long/shorts tokens expected to be output.
 
     Parameters
     ----------
     chain : str
         arbitrum or avalanche.
     params : dict
         dictionary of the gm parameters.
 
     """
-
-    reader_contract_obj = get_reader_contract(chain)
+    reader_contract_obj = get_reader_contract(config)
 
     output = reader_contract_obj.functions.getWithdrawalAmountOut(
         params['data_store_address'],
         params['market_addresses'],
         params['token_prices_tuple'],
         params['gm_amount'],
         params['ui_fee_receiver'],
@@ -646,20 +595,18 @@
 PRECISION = 30
 
 
 def apply_factor(value, factor):
     return value * factor / 10**30
 
 
-def get_funding_factor_per_period(market_info: dict,
-                                  is_long: bool,
-                                  period_in_seconds: int,
-                                  long_interest_usd: int,
-                                  short_interest_usd: int
-                                  ):
+def get_funding_factor_per_period(
+    market_info: dict, is_long: bool, period_in_seconds: int,
+    long_interest_usd: int, short_interest_usd: int
+):
     """
     For a given market, calculate the funding factor for a given period
 
     Parameters
     ----------
     market_info : dict
         market parameters returned from the reader contract.
@@ -670,15 +617,17 @@
     long_interest_usd : int
         expanded decimal long interest.
     short_interest_usd : int
         expanded decimal short interest.
 
     """
 
-    funding_factor_per_second = market_info['funding_factor_per_second'] * 10**-28
+    funding_factor_per_second = (
+        market_info['funding_factor_per_second'] * 10**-28
+    )
 
     long_pays_shorts = market_info['is_long_pays_short']
 
     if is_long:
         is_larger_side = long_pays_shorts
     else:
         is_larger_side = not long_pays_shorts
@@ -713,17 +662,16 @@
     ----------
     filename : str
         filename of json.
     data : dict
         dictionary of data.
 
     """
-
     filepath = os.path.join(
-        base_dir,
+        package_dir,
         'data_store',
         filename
     )
 
     with open(filepath, 'w') as f:
         json.dump(data, f)
 
@@ -734,15 +682,14 @@
 
     Parameters
     ----------
     data : pd.DataFrame
         dataframe to add timestamp column to.
 
     """
-
     dataframe = pd.DataFrame(data, index=[0])
     dataframe['timestamp'] = datetime.now()
 
     return dataframe
 
 
 def save_csv_to_datastore(filename: str, dataframe):
@@ -755,15 +702,15 @@
         name of file.
     dataframe : pd.DataFrame
         pandas dataframe
 
     """
 
     archive_filepath = os.path.join(
-        base_dir,
+        package_dir,
         "data_store",
         filename
     )
 
     if os.path.exists(archive_filepath):
         archive = pd.read_csv(
             archive_filepath
@@ -771,15 +718,15 @@
 
         dataframe = pd.concat(
             [archive, dataframe]
         )
 
     dataframe.to_csv(
         os.path.join(
-            base_dir,
+            package_dir,
             "data_store",
             filename
         ),
         index=False
     )
 
 
@@ -801,15 +748,14 @@
     -------
     list
         list of GMX markets to swap through.
     is_requires_multi_swap : TYPE
         requires more than one market to pass thru.
 
     """
-
     if in_token == "0xaf88d065e77c8cC2239327C5EDb3A432268e5831":
         gmx_market_address = find_dictionary_by_key_value(
             markets,
             "index_token_address",
             out_token
         )['gmx_market_address']
     else:
@@ -836,9 +782,9 @@
 
         return [gmx_market_address, second_gmx_market_address], is_requires_multi_swap
 
     return [gmx_market_address], is_requires_multi_swap
 
 
 if __name__ == "__main__":
-
-    output = get_tokens_address_dict('avalanche')
+    arbitrum_config_object = ConfigManager(chain='arbitrum')
+    arbitrum_config_object.set_config()
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/keys.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/keys.py`

 * *Files identical despite different names*

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/liquidity_argument_parser.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/liquidity_argument_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import numpy as np
 
-from .get_markets import GetMarkets
-from .get_oracle_prices import GetOraclePrices
+from ..get.get_markets import Markets
+from ..get.get_oracle_prices import OraclePrices
 
-from .gmx_utils import get_tokens_address_dict
+from ..gmx_utils import get_tokens_address_dict
 
 
 class LiquidityArgumentParser:
 
-    def __init__(self, is_deposit: bool = False, is_withdrawal: bool = False):
+    def __init__(self, config, is_deposit: bool = False, is_withdrawal: bool = False):
 
         self.parameters_dict = None
         self.is_deposit = is_deposit
         self.is_withdrawal = is_withdrawal
+        self.config = config
 
         if is_deposit:
 
             self.required_keys = [
                 "chain",
                 "market_key",
                 "long_token_address",
@@ -122,15 +123,15 @@
         """
 
         self._handle_missing_index_token_address()
         index_token_address = self.parameters_dict['market_token_address']
 
         # use the index token address to find the market key from get_available_markets
         self.parameters_dict['market_key'] = self.find_market_key_by_index_address(
-            GetMarkets(chain=self.parameters_dict['chain']).get_available_markets(),
+            Markets(self.config).get_available_markets(),
             index_token_address
         )
 
     def _handle_missing_long_token_address(self):
         """
         Will trigger if start token address is missing. Can be determined if start token symbol is
         found, but will raise an exception if that cant be found either.
@@ -197,35 +198,36 @@
         # search the known tokens for a contract address using the user supplied symbol
         out_token_address = self.find_key_by_symbol(
             get_tokens_address_dict(
                 self.parameters_dict['chain']),
             out_token_symbol
         )
 
-        markets = GetMarkets(chain=self.parameters_dict['chain']).get_available_markets()
+        markets = Markets(self.config).get_available_markets()
         market = markets[self.parameters_dict['market_key']]
 
         if out_token_symbol == "BTC":
             out_token_address = "0x2f2a2543B76A4166549F7aaB2e75Bef0aefC5B0f"
 
         if out_token_address not in [market['long_token_address'], market['short_token_address']]:
-            raise Exception("Out token must be either the long or short token of the market")
+            raise Exception(
+                "Out token must be either the long or short token of the market")
         else:
             self.parameters_dict['out_token_address'] = out_token_address
 
     def _handle_missing_long_token_amount(self):
         """
         Will trigger if long token address is missing. Can be determined if long token symbol
         is found, but will raise an exception if that cant be found either.
         """
 
         if self.parameters_dict["long_token_address"] is None:
             self.parameters_dict["long_token_amount"] = 0
             return
-        prices = GetOraclePrices(chain=self.parameters_dict['chain']).get_recent_prices()
+        prices = OraclePrices(chain=self.config.chain).get_recent_prices()
         price = np.median(
             [float(prices[self.parameters_dict["long_token_address"]]['maxPriceFull']),
              float(prices[self.parameters_dict["long_token_address"]]['minPriceFull'])]
         )
         decimal = get_tokens_address_dict(
             self.parameters_dict['chain']
         )[self.parameters_dict["long_token_address"]]['decimals']
@@ -242,15 +244,15 @@
         is found, but will raise an exception if that cant be found either.
         """
 
         if self.parameters_dict["short_token_address"] is None:
             self.parameters_dict["short_token_amount"] = 0
             return
 
-        prices = GetOraclePrices(chain=self.parameters_dict['chain']).get_recent_prices()
+        prices = OraclePrices(chain=self.parameters_dict['chain']).get_recent_prices()
         price = np.median(
             [float(prices[self.parameters_dict["short_token_address"]]['maxPriceFull']),
              float(prices[self.parameters_dict["short_token_address"]]['minPriceFull'])]
         )
         decimal = get_tokens_address_dict(
             self.parameters_dict['chain']
         )[self.parameters_dict["short_token_address"]]['decimals']
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/order.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/order.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,105 +1,114 @@
 import logging
 import numpy as np
 
 from hexbytes import HexBytes
 from web3 import Web3
 
-from .get_markets import GetMarkets
-from .get_oracle_prices import GetOraclePrices
-from .gmx_utils import (
-    get_exchange_router_contract, create_connection, get_config, contract_map,
+from ..get.get_markets import Markets
+from ..get.get_oracle_prices import OraclePrices
+from ..gmx_utils import (
+    get_exchange_router_contract, create_connection, contract_map,
     PRECISION, get_execution_price_and_price_impact, order_type as order_types,
     decrease_position_swap_type as decrease_position_swap_types,
     convert_to_checksum_address
 )
-from .gas_utils import get_execution_fee
-from .approve_token_for_spend import check_if_approved
+from ..gas_utils import get_execution_fee
+from ..approve_token_for_spend import check_if_approved
 
 
 class Order:
 
     def __init__(
-        self, chain: str, market_key: str, collateral_address: str,
+        self, config: str, market_key: str, collateral_address: str,
         index_token_address: str, is_long: bool, size_delta: float,
         initial_collateral_delta_amount: str, slippage_percent: float,
-        swap_path: list, debug_mode: bool = False
+        swap_path: list, max_fee_per_gas: int = None, debug_mode: bool = False
     ) -> None:
 
-        self.chain = chain
+        self.config = config
         self.market_key = market_key
         self.collateral_address = collateral_address
         self.index_token_address = index_token_address
         self.is_long = is_long
         self.size_delta = size_delta
         self.initial_collateral_delta_amount = initial_collateral_delta_amount
         self.slippage_percent = slippage_percent
         self.swap_path = swap_path
+        self.max_fee_per_gas = max_fee_per_gas
         self.debug_mode = debug_mode
 
+        if self.max_fee_per_gas is None:
+            block = create_connection(
+                config
+            ).eth.get_block('latest')
+            self.max_fee_per_gas = block['baseFeePerGas'] * 1.35
+
         self._exchange_router_contract_obj = get_exchange_router_contract(
-            chain=self.chain
+            config=self.config
         )
-        self._connection = create_connection(chain=self.chain)
+        self._connection = create_connection(config)
         self._is_swap = False
 
         self.log = logging.getLogger(__name__)
         self.log.info("Creating order...")
 
     def determine_gas_limits(self):
         pass
 
     def check_for_approval(self):
         """
         Check for Approval
         """
-        spender = contract_map[self.chain]["syntheticsrouter"]['contract_address']
+        spender = contract_map[self.config.chain]["syntheticsrouter"]['contract_address']
 
-        check_if_approved(self.chain,
+        check_if_approved(self.config,
                           spender,
                           self.collateral_address,
                           self.initial_collateral_delta_amount,
+                          self.max_fee_per_gas,
                           approve=True)
 
     def _submit_transaction(
         self, user_wallet_address: str, value_amount: float,
         multicall_args: list, gas_limits: dict
     ):
         """
         Submit Transaction
         """
-        self.log.info("Submitting transaction...")
+        self.log.info("Building transaction...")
         try:
             wallet_address = Web3.to_checksum_address(user_wallet_address)
         except AttributeError:
             wallet_address = Web3.toChecksumAddress(user_wallet_address)
         nonce = self._connection.eth.get_transaction_count(
             wallet_address
         )
 
         raw_txn = self._exchange_router_contract_obj.functions.multicall(
             multicall_args
         ).build_transaction(
             {
                 'value': value_amount,
-                'chainId': 42161,
+                'chainId': self.config.chain_id,
+
                 # TODO - this is NOT correct
                 'gas': (
                     self._gas_limits_order_type.call(
                     ) + self._gas_limits_order_type.call()
                 ),
-                'maxFeePerGas': Web3.to_wei('0.1', 'gwei'),
-                'maxPriorityFeePerGas': Web3.to_wei('0.1', 'gwei'),
+                'maxFeePerGas': int(self.max_fee_per_gas),
+                'maxPriorityFeePerGas': 0,
                 'nonce': nonce
             }
         )
 
         if not self.debug_mode:
             signed_txn = self._connection.eth.account.sign_transaction(
-                raw_txn, get_config()['private_key']
+                raw_txn, self.config.private_key
             )
             tx_hash = self._connection.eth.send_raw_transaction(
                 signed_txn.rawTransaction
             )
             self.log.info("Txn submitted!")
             self.log.info(
                 "Check status: https://arbiscan.io/tx/{}".format(tx_hash.hex())
@@ -161,42 +170,41 @@
         return price, int(slippage), acceptable_price_in_usd
 
     def order_builder(self, is_open=False, is_close=False, is_swap=False):
         """
         Create Order
         """
 
-        config = get_config()
         self.determine_gas_limits()
         gas_price = self._connection.eth.gas_price
         execution_fee = int(
             get_execution_fee(
                 self._gas_limits,
                 self._gas_limits_order_type,
                 gas_price
             )
         )
 
         # Dont need to check approval when closing
-        if not is_close:
+        if not is_close and not self.debug_mode:
             self.check_for_approval()
 
         # Up execution fee for swap, more complex
         if is_swap:
 
             # 30% buffer
-            execution_fee = int(execution_fee * 1.3)
+            execution_fee = int(execution_fee * 1.5)
         else:
 
             # 20% buffer
             execution_fee = int(execution_fee * 1.2)
 
-        markets = GetMarkets(chain=self.chain).get_available_markets()
+        markets = Markets(self.config).get_available_markets()
         initial_collateral_delta_amount = self.initial_collateral_delta_amount
-        prices = GetOraclePrices(chain=self.chain).get_recent_prices()
+        prices = OraclePrices(chain=self.config.chain).get_recent_prices()
         size_delta_price_price_impact = self.size_delta
 
         # when decreasing size delta must be negative
         if is_close:
             size_delta_price_price_impact = size_delta_price_price_impact * -1
 
         callback_gas_limit = 0
@@ -239,26 +247,26 @@
 
         decrease_position_swap_type = decrease_position_swap_types['no_swap']
 
         should_unwrap_native_token = True
         referral_code = HexBytes(
             "0x0000000000000000000000000000000000000000000000000000000000000000"
         )
-        user_wallet_address = config['user_wallet_address']
+        user_wallet_address = self.config.user_wallet_address
         eth_zero_address = "0x0000000000000000000000000000000000000000"
         ui_ref_address = "0x0000000000000000000000000000000000000000"
         try:
             gmx_market_address = Web3.to_checksum_address(self.market_key)
         except AttributeError:
             gmx_market_address = Web3.toChecksumAddress(self.market_key)
 
         # parameters using to calculate execution price
         execution_price_parameters = {
             'data_store_address': (
-                contract_map[self.chain]["datastore"]['contract_address']
+                contract_map[self.config.chain]["datastore"]['contract_address']
             ),
             'market_key': self.market_key,
             'index_token_price': [
                 int(prices[self.index_token_address]['maxPriceFull']),
                 int(prices[self.index_token_address]['minPriceFull'])
             ],
             'position_size_in_usd': 0,
@@ -284,15 +292,15 @@
 
         # Market address and acceptable price not important for swap
         if is_swap:
             acceptable_price = 0
             gmx_market_address = "0x0000000000000000000000000000000000000000"
 
         execution_price_and_price_impact_dict = get_execution_price_and_price_impact(
-            self.chain,
+            self.config,
             execution_price_parameters,
             decimals
         )
         self.log.info(
             "Execution price: ${:.4f}".format(
                 execution_price_and_price_impact_dict['execution_price']
             )
@@ -315,27 +323,27 @@
                     raise Exception("Execution price falls outside acceptable price!")
             elif not self.is_long:
                 if execution_price_and_price_impact_dict[
                         'execution_price'] > acceptable_price_in_usd:
                     raise Exception("Execution price falls outside acceptable price!")
 
         user_wallet_address = convert_to_checksum_address(
-            self.chain,
+            self.config,
             user_wallet_address
         )
         eth_zero_address = convert_to_checksum_address(
-            self.chain,
+            self.config,
             eth_zero_address
         )
         ui_ref_address = convert_to_checksum_address(
-            self.chain,
+            self.config,
             ui_ref_address
         )
         collateral_address = convert_to_checksum_address(
-            self.chain,
+            self.config,
             self.collateral_address
         )
 
         arguments = (
             (
                 user_wallet_address,
                 eth_zero_address,
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/order_argument_parser.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/order_argument_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 
-from .get_oracle_prices import GetOraclePrices
-from .get_markets import GetMarkets
-from .gmx_utils import get_tokens_address_dict, determine_swap_route
+from ..get.get_oracle_prices import OraclePrices
+from ..get.get_markets import Markets
+from ..gmx_utils import get_tokens_address_dict, determine_swap_route
 
 
 class OrderArgumentParser:
 
-    def __init__(self, is_increase: bool = False, is_decrease: bool = False, is_swap: bool = False):
-
+    def __init__(self, config, is_increase: bool = False, is_decrease: bool = False, is_swap: bool = False):
+        self.config = config
         self.parameters_dict = None
         self.is_increase = is_increase
         self.is_decrease = is_decrease
         self.is_swap = is_swap
 
         if is_increase:
             self.required_keys = [
@@ -137,15 +137,15 @@
         index_token_address = self.parameters_dict['index_token_address']
 
         if index_token_address == "0x2f2a2543B76A4166549F7aaB2e75Bef0aefC5B0f":
             index_token_address = "0x47904963fc8b2340414262125aF798B9655E58Cd"
 
         # use the index token address to find the market key from get_available_markets
         self.parameters_dict['market_key'] = self.find_market_key_by_index_address(
-            GetMarkets(chain=self.parameters_dict['chain']).get_available_markets(),
+            Markets(self.config).get_available_markets(),
             index_token_address
         )
 
     def _handle_missing_start_token_address(self):
         """
         Will trigger if start token address is missing. Can be determined if start token symbol is
         found, but will raise an exception if that cant be found either.
@@ -223,16 +223,16 @@
         Will trigger if swap path is missing. If start token is the same collateral, no swap path is
         required but otherwise will use determine_swap_route to find the path from start token to
         collateral token
         """
 
         if self.is_swap:
             # first get markets to supply to determine_swap_route
-            markets = GetMarkets(
-                chain=self.parameters_dict['chain']
+            markets = Markets(
+                self.config
             ).get_available_markets()
 
             # function returns swap route as a list [0] and a bool if there is a multi swap [1]
             self.parameters_dict['swap_path'] = determine_swap_route(
                 markets,
                 self.parameters_dict['start_token_address'],
                 self.parameters_dict['out_token_address']
@@ -242,16 +242,16 @@
         elif self.parameters_dict['start_token_address'] == \
                 self.parameters_dict['collateral_address']:
             self.parameters_dict['swap_path'] = []
 
         else:
 
             # first get markets to supply to determine_swap_route
-            markets = GetMarkets(
-                chain=self.parameters_dict['chain']
+            markets = Markets(
+                self.config
             ).get_available_markets()
 
             # function returns swap route as a list [0] and a bool if there is a multi swap [1]
             self.parameters_dict['swap_path'] = determine_swap_route(
                 markets,
                 self.parameters_dict['start_token_address'],
                 self.parameters_dict['collateral_address']
@@ -285,16 +285,16 @@
         """
 
         market_key = self.parameters_dict['market_key']
 
         if self.parameters_dict['market_key'] == "0x2f2a2543B76A4166549F7aaB2e75Bef0aefC5B0f":
             market_key = "0x47c031236e19d024b42f8AE6780E44A573170703"
 
-        market = GetMarkets(
-            chain=self.parameters_dict['chain']
+        market = Markets(
+            self.config
         ).get_available_markets()[market_key]
 
         # if collateral address doesnt match long or short token address, no bueno
         if collateral_address == market['long_token_address'] or \
                 collateral_address == market['short_token_address']:
             return True
         else:
@@ -389,15 +389,15 @@
     def _calculate_initial_collateral_usd(self):
         """
         Calculate the USD value of the number of tokens supplied in initial collateral delta
 
         """
 
         initial_collateral_delta_amount = self.parameters_dict['initial_collateral_delta']
-        prices = GetOraclePrices(chain=self.parameters_dict['chain']).get_recent_prices()
+        prices = OraclePrices(chain=self.parameters_dict['chain']).get_recent_prices()
         price = np.median(
             [float(prices[self.parameters_dict["start_token_address"]]['maxPriceFull']),
              float(prices[self.parameters_dict["start_token_address"]]['minPriceFull'])]
         )
         oracle_factor = get_tokens_address_dict(
             self.parameters_dict['chain']
         )[self.parameters_dict["start_token_address"]]['decimals'] - 30
@@ -413,15 +413,15 @@
         Parameters
         ----------
         collateral_usd : float
             Dollar value of collateral.
 
         """
 
-        prices = GetOraclePrices(chain=self.parameters_dict['chain']).get_recent_prices()
+        prices = OraclePrices(chain=self.parameters_dict['chain']).get_recent_prices()
         price = np.median(
             [float(prices[self.parameters_dict["start_token_address"]]['maxPriceFull']),
              float(prices[self.parameters_dict["start_token_address"]]['minPriceFull'])]
         )
         oracle_factor = get_tokens_address_dict(
             self.parameters_dict['chain']
         )[self.parameters_dict["start_token_address"]]['decimals'] - 30
@@ -455,15 +455,16 @@
         """
         Using collateral tokens and size_delta calculate the requested leverage size and raise
         exception if this exceeds x100.
 
         """
 
         collateral_usd_value = self._calculate_initial_collateral_usd
-        leverage_requested = self.parameters_dict["size_delta_usd"] / collateral_usd_value()
+        leverage_requested = self.parameters_dict["size_delta_usd"] / \
+            collateral_usd_value()
 
         # TODO - leverage is now a contract parameter and needs to be queried
         max_leverage = 100
         if leverage_requested > max_leverage:
             raise Exception('Leverage requested "x{:.2f}" can not exceed x100!'.format(
                 leverage_requested
             )
```

### Comparing `gmx_python_sdk-0.0.4/gmx_python_sdk/scripts/v2/withdraw.py` & `gmx_python_sdk-0.0.5/gmx_python_sdk/scripts/v2/order/withdraw.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,139 +1,148 @@
 import logging
 
 from web3 import Web3
 
 from hexbytes import HexBytes
 
-from .get_markets import GetMarkets
-from .get_oracle_prices import GetOraclePrices
+from ..get.get_markets import Markets
+from ..get.get_oracle_prices import OraclePrices
 
-from .gmx_utils import get_config, convert_to_checksum_address, \
+from ..gmx_utils import convert_to_checksum_address, \
     get_exchange_router_contract, create_connection, \
     determine_swap_route, contract_map, \
     get_estimated_withdrawal_amount_out
 
-from .approve_token_for_spend import check_if_approved
+from ..approve_token_for_spend import check_if_approved
 
-from .gas_utils import get_execution_fee
-
-CONFIG = get_config()
+from ..gas_utils import get_execution_fee
 
 
 class Withdraw:
 
     def __init__(
         self,
-        chain: str,
+        config,
         market_key: str,
         out_token: str,
         gm_amount: int,
+        max_fee_per_gas: int = None,
         debug_mode: bool = False
     ) -> None:
-        self.chain = chain
+        self.config = config
         self.market_key = market_key
         self.out_token = out_token
         self.gm_amount = gm_amount
         self.long_token_swap_path = []
         self.short_token_swap_path = []
+        self.max_fee_per_gas = max_fee_per_gas
         self.debug_mode = debug_mode
 
+        if self.max_fee_per_gas is None:
+            block = create_connection(
+                config
+            ).eth.get_block('latest')
+            self.max_fee_per_gas = block['baseFeePerGas'] * 1.35
+
         self._exchange_router_contract_obj = get_exchange_router_contract(
-            chain=self.chain
+            config
         )
 
-        self._connection = create_connection(chain=chain)
+        self._connection = create_connection(config)
 
-        self.all_markets_info = GetMarkets(chain=self.chain).get_available_markets()
+        self.all_markets_info = Markets(config).get_available_markets()
 
         self.log = logging.getLogger(__name__)
         self.log.info("Creating order...")
 
     def determine_gas_limits(self):
 
         pass
 
     def check_for_approval(self):
         """
         Check for Approval
 
         """
-        spender = contract_map[self.chain]["syntheticsrouter"]['contract_address']
+        spender = contract_map[self.config.chain]["syntheticsrouter"]['contract_address']
 
-        check_if_approved(self.chain,
+        check_if_approved(self.config,
                           spender,
                           self.market_key,
                           self.gm_amount,
+                          self.max_fee_per_gas,
                           approve=True)
 
     def _submit_transaction(
         self, user_wallet_address: str, value_amount: float,
         multicall_args: list, gas_limits: dict
     ):
         """
         Submit Transaction
         """
-        self.log.info("Submitting transaction...")
+        self.log.info("Building transaction...")
 
         nonce = self._connection.eth.get_transaction_count(
             user_wallet_address
         )
 
         raw_txn = self._exchange_router_contract_obj.functions.multicall(
             multicall_args
         ).build_transaction(
             {
                 'value': value_amount,
-                'chainId': 42161,
+                'chainId': self.config.chain_id,
 
                 # TODO - this is NOT correct
                 'gas': (
                     self._gas_limits_order_type.call() + self._gas_limits_order_type.call()
                 ),
-                'maxFeePerGas': Web3.to_wei('0.12', 'gwei'),
-                'maxPriorityFeePerGas': Web3.to_wei('0.12', 'gwei'),
+                'maxFeePerGas': int(self.max_fee_per_gas),
+                'maxPriorityFeePerGas': 0,
                 'nonce': nonce
             }
         )
         if not self.debug_mode:
+
             signed_txn = self._connection.eth.account.sign_transaction(
-                raw_txn, get_config()['private_key']
+                raw_txn, self.config.private_key
             )
             tx_hash = self._connection.eth.send_raw_transaction(
                 signed_txn.rawTransaction
             )
             self.log.info("Txn submitted!")
             self.log.info(
                 "Check status: https://arbiscan.io/tx/{}".format(tx_hash.hex())
             )
 
             self.log.info("Transaction submitted!")
 
     def create_withdraw_order(self):
 
-        user_wallet_address = CONFIG['user_wallet_address']
+        user_wallet_address = self.config.user_wallet_address
 
         self.determine_gas_limits()
-        self.check_for_approval()
+        if not self.debug_mode:
+            self.check_for_approval()
 
         should_unwrap_native_token = True
 
         eth_zero_address = "0x0000000000000000000000000000000000000000"
         ui_ref_address = "0x0000000000000000000000000000000000000000"
 
         user_wallet_address = convert_to_checksum_address(
-            self.chain,
+            self.config,
             user_wallet_address
         )
         eth_zero_address = convert_to_checksum_address(
-            self.chain,
+            self.config,
             eth_zero_address
         )
         ui_ref_address = convert_to_checksum_address(
-            self.chain,
+            self.config,
             ui_ref_address
         )
 
         min_long_token_amount, min_short_token_amount = self._estimate_withdrawal()
 
         # Giving a 10% buffer here
         execution_fee = int(
@@ -263,18 +272,20 @@
         Returns
         -------
         list
             list of amount of long and short tokens.
 
         """
 
-        data_store_contract_address = contract_map[self.chain]['datastore']['contract_address']
+        data_store_contract_address = contract_map[
+            self.config.chain
+        ]['datastore']['contract_address']
 
         market = self.all_markets_info[self.market_key]
-        oracle_prices_dict = GetOraclePrices(chain=self.chain).get_recent_prices()
+        oracle_prices_dict = OraclePrices(chain=self.config.chain).get_recent_prices()
 
         index_token_address = market['index_token_address']
         long_token_address = market['long_token_address']
         short_token_address = market['short_token_address']
 
         market_addresses = [self.market_key,
                             index_token_address,
@@ -298,8 +309,8 @@
             "data_store_address": data_store_contract_address,
             "market_addresses": market_addresses,
             "token_prices_tuple": prices,
             "gm_amount": self.gm_amount,
             "ui_fee_receiver": "0x0000000000000000000000000000000000000000"
         }
 
-        return get_estimated_withdrawal_amount_out(self.chain, parameters)
+        return get_estimated_withdrawal_amount_out(self.config, parameters)
```

### Comparing `gmx_python_sdk-0.0.4/pyproject.toml` & `gmx_python_sdk-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmx_python_sdk"
-version = "0.0.4"
+version = "0.0.5"
 description = "A python based SDK developed for interacting with GMX v2"
 
 authors = [
   "snipermonke01 <snipermonke01@proton.me>",
   "alienf33t <alienf33t@yahoo.com>"
 ]
 maintainers = [
```

### Comparing `gmx_python_sdk-0.0.4/PKG-INFO` & `gmx_python_sdk-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmx_python_sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python based SDK developed for interacting with GMX v2
 Home-page: https://github.com/snipermonke01/gmx_python_sdk
 License: MIT
 Author: snipermonke01
 Author-email: snipermonke01@proton.me
 Maintainer: snipermonke01
 Maintainer-email: snipermonke01@proton.me
@@ -23,14 +23,15 @@
 Description-Content-Type: text/markdown
 
 
 # GMX Python SDK
 
 A python based SDK developed for interacting with GMX v2
 
+- [Pip Install](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#pip-install)
 - [Requirements](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#requirements)
 - [Config File Setup](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#config-file-setup)
 - [Example Scripts](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#example-scripts)
 - [General Usage](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#general-usage)
     - [Increase Position](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#increase-position)
     - [Decrease Position](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#decrease-position)
     - [Swap Order](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#swap-order)
@@ -41,14 +42,21 @@
         - [Order Argument Parser](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#order-argument-parser)
         - [Liquidity Argument Parser](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#liquidity-argument-parser)
         - [Closing Positions](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#closing-positions)
     - [GMX Stats](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#gmx-stats)
     - [Debug Mode](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#debug-mode)
 - [Known Limitations](https://github.com/snipermonke01/gmx_python_sdk/tree/main?tab=readme-ov-file#known-limitations)
 
+## Pip Install
+
+The SDK can be installed via pip:
+
+```
+pip install gmx-python-sdk
+```
 
 ## Requirements
 
 Developed using:
 ```python
   python=3.10.4
 ```
@@ -64,58 +72,60 @@
 pip install pandas==1.4.2
 pip install numerize
 ```
 
 The codebase is designed around the usage of web3py [6.10.0](https://web3py.readthedocs.io/en/stable/releases.html#web3-py-v6-10-0-2023-09-21), and will not work with older versions and has not been tested with the latest version.
 ## Config File Setup
 
-[Config file](https://github.com/snipermonke01/gmx_python_sdk/blob/main/config.yaml) must set up before usage. For stats based operations, you will need only an RPC but for execution you need to save both a wallet address and the private key of that wallet. 
+[Config file](https://github.com/snipermonke01/gmx_python_sdk/blob/main/config.yaml) can be set before usage by editing the yaml file. For stats based operations, you will need only an RPC but for execution you need to save both a wallet address and the private key of that wallet. 
 
 ```yaml
-arbitrum:
-  rpc: rpc_url
-  chain_id: chain_id
-avalanche:
-  rpc: rpc_url
-  chain_id: chain_id
+rpcs:
+  arbitrum: arbitrum_rpc
+  avalanche: avax_rpc
+chain_ids:
+  arbitrum: 42161
+  avalanche: 43114
 private_key: private_key
-user_wallet_address: wallet_address
+user_wallet_address: user_wallet_address
+
 ```
 
-The example script [setting_config.py](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/setting_config.py) can be viewed for demonstration on how to import config and update with new details from script.
+The example script [setting_config.py](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/setting_config.py) can be viewed for demonstration on how to import config and update with new details from within a script.
 
-There is an example in [create_increase_.py](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/setting_config.py) of how it is possible to [set config parameters](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/create_increase_order.py#L8-L19) within the py script, and then [reset these](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/create_increase_order.py#L71-L77) once the script has finished running.
+There is an example in all the example scripts of how to import the config and init the object to pass to functions and classes through the SDK.
 
 ## Example Scripts
 
 There are several example scripts which can be run and can be found in [example scripts.](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/) These are mostly for demonstration purposes on how to utilise the SDK, and can should be incoporated into your own scripts and strategies.
 
 
 ## General Usage
 
 ### [Increase Position](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/create_increase_order.py)
 
 The following block demonstrates how to open (or increase) a position:
 
 ```python
-from scripts.v2.create_increase_order import IncreaseOrder
+from gmx_python_sdk_scripts.v2.order.create_increase_order import IncreaseOrder
 
 order = IncreaseOrder(
-    chain,
-    market_key,
-    collateral_address,
-    index_token_address,
-    is_long,
-    size_delta_usd,
-    initial_collateral_delta_amount,
-    slippage_percent,
-    swap_path
+    config=config,
+    market_key=market_key,
+    collateral_address=collateral_address,
+    index_token_address=index_token_address,
+    is_long=is_long,
+    size_delta_usd=size_delta_usd,
+    initial_collateral_delta_amount=initial_collateral_delta_amount,
+    slippage_percent=slippage_percent,
+    swap_path=swap_path,
+    debug_mode=debug_mode
 )
 ```
-**chain** - *type str*: either 'arbitrum' or 'avalanche' (avalanche currently in testing still)
+**config** - *type obj*: an initialised config object (avalanche currently in testing still)
 
 **market_key** - *type str*: the contract address of the GMX market you want to increase a position on
 
 **collateral_address** - *type str*: the contract address of the token you want to use as collateral
 
 **index_token_address** - *type str*: the contract address of the token you want to trade
 
@@ -125,34 +135,37 @@
 
 **initial_collateral_delta_amount** - *type int*: the amount of token you want to use as collateral, 10^decimal of that token
 
 **slippage_percent** - *type float*: the percentage you want to allow slippage
 
 **swap_path** - *type list(str)*: a list of the GMX markets you will need to swap through if the starting token is different to the token you want to use as collateral
 
+**debug_mode** - *type bool*: set to true to create an order without submitting
+
 ### [Decrease Position](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/create_decrease_order.py)
 
 The following block demonstrates how to close (or decrease) a position:
 
 ```python
-from scripts.v2.create_decrease_order import DecreaseOrder
+from gmx_python_sdk_scripts.v2.order.create_decrease_order import DecreaseOrder
 
 order = DecreaseOrder(
-    chain,
-    market_key,
-    collateral_address,
-    index_token_address,
-    is_long,
-    size_delta_usd,
-    initial_collateral_delta_amount,
-    slippage_percent,
-    swap_path
+    config=config,
+    market_key=market_key,
+    collateral_address=collateral_address,
+    index_token_address=index_token_address,
+    is_long=is_long,
+    size_delta_usd=size_delta_usd,
+    initial_collateral_delta_amount=initial_collateral_delta_amount,
+    slippage_percent=slippage_percent,
+    swap_path=swap_path,
+    debug_mode=debug_mode
 )
 ```
-**chain** - *type str*: either 'arbitrum' or 'avalanche' (currently in testing still)
+**config** - *type obj*: an initialised config object (avalanche currently in testing still)
 
 **market_key** - *type str*: the contract address of the GMX market you want to decrease a position for
 
 **collateral_address** - *type str*: the contract address of the token you are using as collateral
 
 **index_token_address** - *type str*: the contract address of the token are trading
 
@@ -162,36 +175,39 @@
 
 **initial_collateral_delta_amount** - *type int*: the amount of collateral token you want to remove, 10^decimal of that token
 
 **slippage_percent** - *type float*: the percentage you want to allow slippage
 
 **swap_path** - *type list(str)*: a list of the GMX markets you will need to swap through to get your desired out token
 
+**debug_mode** - *type bool*: set to true to create an order without submitting
+
 ### [Swap Order](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/create_swap_order.py)
 
 The following block demonstrates how to make a swap:
 
 ```python
-from scripts.v2.create_swap_order import SwapOrder
+from gmx_python_sdk_scripts.v2.order.create_swap_order import SwapOrder
 
 order = SwapOrder(
-    chain,
-    market_key,
-    start_token,
-    out_token,
-    collateral_address,
-    index_token_address,
-    is_long,
-    size_delta,
-    initial_collateral_delta_amount,
-    slippage_percent,
-    swap_path
+    config=config,
+    market_key=market_key,
+    start_token=start_token,
+    out_token=out_token,
+    collateral_address=collateral_address,
+    index_token_address=index_token_address,
+    is_long=is_long,
+    size_delta=size_delta,
+    initial_collateral_delta_amount=initial_collateral_delta_amount,
+    slippage_percent=slippage_percent,
+    swap_path=swap_path,
+    debug_mode=debug_mode
 )
 ```
-**chain** - *type str*: either 'arbitrum' or 'avalanche' (currently in testing still)
+**config** - *type obj*: an initialised config object (avalanche currently in testing still)
 
 **market_key** - *type str*: the contract address of the GMX market you want to (first) market you want to swap through
 
 **start_token** - *type str*: the contract address of the token you start the swap with
 
 **out_token** - *type str*: the contract address of the token you want out
 
@@ -205,146 +221,118 @@
 
 **initial_collateral_delta_amount** - *type int*: the amount of start token you are swapping
 
 **slippage_percent** - *type float*: the percentage you want to allow slippage
 
 **swap_path** - *type list()*: list of gmx market address your swap will go through
 
+**debug_mode** - *type bool*: set to true to create an order without submitting
+
 ### [Deposit Order](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/create_deposit_order.py)
 
 The following block demonstrates how to make a deposit to a gm pool:
 
 ```python
-from scripts.v2.create_deposit_order import DepositOrder
+from gmx_python_sdk_scripts.v2.order.create_deposit_order import DepositOrder
 
 order = DepositOrder(
-    chain,
-    market_key,
-    initial_long_token,
-    initial_short_token,
-    long_token_amount,
-    short_token_amount
+    config=config,
+    market_key=market_key,
+    initial_long_token=initial_long_token,
+    initial_short_token=initial_short_token,
+    long_token_amount=long_token_amount,
+    short_token_amount=short_token_amount,
+    debug_mode=debug_mode
 )
 ```
-**chain** - *type str*: either 'arbitrum' or 'avalanche' (currently in testing still)
+**config** - *type obj*: an initialised config object (avalanche currently in testing still)
 
 **market_key** - *type str*: the contract address of the GMX market you want to deposit into
 
 **initial_long_token** - *type str*: the contract address of the token you want to use to deposit into long side, can be None
 
 **initial_short_token** - *type str*: the contract address of the token you want to use to deposit into short side, can be None
 
 **long_token_amount** - *type str*: the amount of token to add to long side, can be 0
 
 **short_token_amount** - *type str*: the amount of token to add to short side, can be 0
 
+**debug_mode** - *type bool*: set to true to create an order without submitting
+
 ### [Withdraw Order](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/create_withdraw_order.py)
 
 The following block demonstrates how to make a withdrawal from a gm pool:
 
 ```python
-from scripts.v2.create_withdrawal_order import WithdrawOrder
+from gmx_python_sdk_scripts.v2.order.create_withdrawal_order import WithdrawOrder
 
 order = WithdrawOrder(
-    chain,
-    market_key,
-    out_token,
-    gm_amount
+    config=config,
+    market_key=market_key,
+    out_token=out_token,
+    gm_amount=gm_amount,
+    debug_mode=debug_mode
 )
 ```
-**chain** - *type str*: either 'arbitrum' or 'avalanche' (currently in testing still)
+**config** - *type obj*: an initialised config object (avalanche currently in testing still)
 
 **market_key** - *type str*: the contract address of the GMX market you want to withdraw from
 
 **out_token** - *type str*: the contract address of the token you want to use to receive
 
 **gm_amount** - *type str*: amount of gm tokens to burn
 
-### Get Execution Price & Price Impact On Position Change
-
-
-```python
-from scripts.v2.gmx_utils import get_execution_price_and_price_impact
-
-chain = "arbitrum"
-estimated_swap_output_parameters = {
-    'data_store_address': (data_store_address),
-    'market_addresses': [
-        gmx_market_address,
-        index_token_address,
-        long_token_address,
-        short_token_address
-    ],
-    'token_prices_tuple': [
-        [
-            int(max_price_of_index_token),
-            int(min_price_of_index_token)
-        ],
-        [
-            int(max_price_of_long_token),
-            int(min_price_of_long_token)
-        ],
-        [
-            int(max_price_of_short_token),
-            int(min_price_of_short_token])
-        ],
-    ],
-    'token_in': in_token_address,
-    'token_amount_in': in_token_amount,
-    'ui_fee_receiver': "0x0000000000000000000000000000000000000000"
-}
-
-get_execution_price_and_price_impact(
-    chain,
-    estimated_swap_output_parameters,
-    decimals
-)
-
-```
+**debug_mode** - *type bool*: set to true to create an order without submitting
 
 ### Estimate Swap output
 
-Below shows an example of how to estimate swap output using the [EstimateSwapOutput](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/estimate_swap_output.py#L21) class in [estimate_swap_ouput.py](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/estimate_swap_output.py). One can provide either a token symbol or contract address for in and out tokens and the script will return a dictionary containing the estimate output number of tokens and price impact.
+Below shows an example of how to estimate swap output using the [EstimateSwapOutput](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/estimate_swap_output.py#L20) class in [estimate_swap_ouput.py](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/estimate_swap_output.py). One can provide either a token symbol or contract address for in and out tokens and the script will return a dictionary containing the estimate output number of tokens and price impact.
 
 ```python
-from estimate_swap_output import EstimateSwapOutput
+from gmx_python_sdk.example_scripts.estimate_swap_output import EstimateSwapOutput
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
+
+config = ConfigManager("arbitrum")
+config.set_config()
 
-chain = "arbitrum"
-in_token_symbol = "SOL"
+in_token_symbol = "GMX"
 out_token_symbol = "USDC"
-token_amount = 2
+token_amount = 10
 in_token_address = None
 out_token_address = None
 token_amount_expanded = None
 
-output = EstimateSwapOutput(chain=chain).get_swap_output(
-    in_token_symbol=in_token_symbol,
-    out_token_symbol=out_token_symbol,
-    token_amount=token_amount,
-    in_token_address=in_token_address,
-    out_token_address=out_token_address,
-    token_amount_expanded=token_amount_expanded
+output = EstimateSwapOutput(config=config).get_swap_output(
+     in_token_symbol=in_token_symbol,
+     out_token_symbol=out_token_symbol,
+     token_amount=token_amount,
+     in_token_address=in_token_address,
+     out_token_address=out_token_address,
+     token_amount_expanded=token_amount_expanded
 )
 
 ```
 
 ### Helper Scripts
 
 To assist in argument formatting, there are a few helper functions:
 
-#### [Order Argument Parser](https://github.com/snipermonke01/gmx_python_sdk/blob/main/scripts/v2/order_argument_parser.py)
+#### [Order Argument Parser](https://github.com/snipermonke01/gmx_python_sdk/blob/main/gmx_python_sdk/scripts/v2/order/order_argument_parser.py)
 
 Human readable numbers can be parsed in a dictionary with the following keys/values which are processed by a class, OrderArgumentParser. This class should initialised with a bool to indicate is_increase, is_decrease, or is_swap, calling the method: "process_parameters_dictionary". This will output a dictionary containing the user input parameters reformatted to allow for successful order creation.
 
 For increase:
 
 
 ```python
-from scripts.v2.order_argument_parser import OrderArgumentParser
+from gmx_python_sdk.scripts.v2.order.order_argument_parser import OrderArgumentParser
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
 
+config = ConfigManager("arbitrum")
+config.set_config()
 
 parameters = {
     "chain": 'arbitrum',
 
     # the market you want to trade on
     "index_token_symbol": "ARB",
 
@@ -364,21 +352,30 @@
     "leverage": 1,
 
     # as a percentage
     "slippage_percent": 0.03
 }
 
 
-order_parameters = OrderArgumentParser(is_increase=True).process_parameters_dictionary(parameters)
+order_parameters = OrderArgumentParser(
+     config=config,
+     is_increase=True
+).process_parameters_dictionary(
+     parameters
+)
 ```
 
 For decrease:
 
 ```python
-from scripts.v2.order_argument_parser import OrderArgumentParser
+from gmx_python_sdk.scripts.v2.order.order_argument_parser import OrderArgumentParser
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
+
+config = ConfigManager("arbitrum")
+config.set_config()
 
 parameters = {
     "chain": 'arbitrum',
     "index_token_symbol": "ARB",
 
     "collateral_token_symbol": "USDC",
 
@@ -394,20 +391,29 @@
     "initial_collateral_delta": 6,
 
     # as a percentage
     "slippage_percent": 0.03
 }
 
 
-order_parameters = OrderArgumentParser(is_decrease=True).process_parameters_dictionary(parameters)
+order_parameters = OrderArgumentParser(
+     config=config,
+     is_decrease=True
+).process_parameters_dictionary(
+     parameters
+)
 ```
 For Swap:
 
 ```python
-from scripts.v2.order_argument_parser import OrderArgumentParser
+from gmx_python_sdk.scripts.v2.order.order_argument_parser import OrderArgumentParser
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
+
+config = ConfigManager("arbitrum")
+config.set_config()
 
 parameters = {
     "chain": 'arbitrum',
 
     # token to use as collateral. Start token swaps into collateral token if different
     "out_token_symbol": "ETH",
 
@@ -424,134 +430,166 @@
     "initial_collateral_delta": 10,
 
     # as a percentage
     "slippage_percent": 0.03
 }
 
 
-order_parameters = OrderArgumentParser(is_swap=True).process_parameters_dictionary(parameters)
+order_parameters = OrderArgumentParser(
+     config=config,
+     is_swap=True
+).process_parameters_dictionary(
+     parameters
+)
 ```
-#### [Liquidity Argument Parser](https://github.com/snipermonke01/gmx_python_sdk/blob/main/scripts/v2/order_argument_parser.py)
+#### [Liquidity Argument Parser](https://github.com/snipermonke01/gmx_python_sdk/blob/main/gmx_python_sdk/scripts/v2/order/liquidity_argument_parser.py)
 
 Human readable numbers can be parsed in a dictionary with the following keys/values which are processed by a class, LiquidityArgumentParser. This class should initialised with a bool to indicate is_deposit or is_withdraw calling the method: "process_parameters_dictionary". This will output a dictionary containing the user input parameters reformatted to allow for successful deposit/withdrawal order creation.
 
 For Deposit:
 
 ```python
-from scripts.v2.liquidity_argument_parser import LiquidityArgumentParser
+from gmx_python_sdk.scripts.v2.order.liquidity_argument_parser import LiquidityArgumentParser
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
+
+config = ConfigManager("arbitrum")
+config.set_config()
 
 parameters = {
     "chain": "arbitrum",
     "market_token_symbol": "ETH",
     "long_token_symbol": "ETH",
     "short_token_symbol": USDC,
     "long_token_usd": 10,
     "short_token_usd": 10
 }
 
-output = LiquidityArgumentParser(is_deposit=True).process_parameters_dictionary(parameters)
+output = LiquidityArgumentParser(
+     config=config,
+     is_deposit=True
+).process_parameters_dictionary(
+     parameters
+)
 ```
 
 
 For Withdraw:
 
 ```python
-from scripts.v2.liquidity_argument_parser import LiquidityArgumentParser
+from gmx_python_sdk.scripts.v2.order.liquidity_argument_parser import LiquidityArgumentParser
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
 
 parameters = {
     "chain": "arbitrum",
     "market_token_symbol": "ETH",
     "out_token_symbol": "ETH",
     "gm_amount": 1
 }
 
-output = LiquidityArgumentParser(is_withdrawal=True).process_parameters_dictionary(parameters)
+output = LiquidityArgumentParser(
+     config=config,
+     is_withdraw=True
+).process_parameters_dictionary(
+     parameters
+)
 ```
 
 #### Closing positions
 
-Instead of passing the parameters to close a position, if you are aware of the market symbol and the direction of the trade you want to close you can pass these to [transform_open_position_to_order_parameters](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/get_positions.py#L46) after collecting all open positions using [get_positions](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/get_positions.py#L13). You can specify the amount of collateral or position size to remove/close as a decimal, eg 0.5 would close/remove 50% of size/collateral:
+Instead of passing the parameters to close a position, if you are aware of the market symbol and the direction of the trade you want to close you can pass these to [transform_open_position_to_order_parameters](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/get_positions.py#L51) after collecting all open positions using [get_positions](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/get_positions.py#L16). You can specify the amount of collateral or position size to remove/close as a decimal, eg 0.5 would close/remove 50% of size/collateral:
 
 ```python
-from get_positions import get_positions, transform_open_position_to_order_parameters
+from gmx_python_sdk.example_scripts.get_positions import get_positions, transform_open_position_to_order_parameters
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
 
-chain = "arbitrum"
+config = ConfigManager(chain='arbitrum')
+config.set_config()
+
+address = None
 market_symbol = "ETH"
 out_token = "ETH"
 is_long = False
 slippage_percent = 0.003
 amount_of_position_to_close = 1
 amount_of_collateral_to_remove = 1
 
 # gets all open positions as a dictionary, which the keys as each position
-positions = get_positions(chain)
+positions = get_positions(
+     config=config,
+     address=address
+)
 
 order_parameters = transform_open_position_to_order_parameters(
-    chain,
-    positions,
-    market_symbol,
-    is_long,
-    slippage_percent,
-    out_token,
-    amount_of_position_to_close,
-    amount_of_collateral_to_remove
+    config=config,
+    positions=positions,
+    market_symbol=market_symbol,
+    is_long=is_long,
+    slippage_percent=slippage_percent,
+    out_token=out_token,
+    amount_of_position_to_close=amount_of_position_to_close,
+    amount_of_collateral_to_remove=amount_of_collateral_to_remove
 )
 ```
 
 ### GMX Stats
 
-A number of stats can be obtained using a wide range of scripts. The overview on how to call these can be found in [get_gmx_stats](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/get_gmx_stats.py). Each method returns a dictionary containing long/short information for a given chain. When initialising the class, pass to_json or to_csv as True to save the output to the [data store](https://github.com/snipermonke01/gmx_python_sdk/tree/main/data_store): 
+A number of stats can be obtained using a wide range of scripts. The overview on how to call these can be found in [get_gmx_stats](https://github.com/snipermonke01/gmx_python_sdk/blob/main/example_scripts/get_gmx_stats.py). Each method returns a dictionary containing long/short information for a given chain. When initialising the class, pass to_json or to_csv as True to save the output to the [data store](https://github.com/snipermonke01/gmx_python_sdk/tree/main/gmx_python_sdk/data_store): 
 
 ```python
-from get_gmx_stats import GetGMXv2Stats
+from gmx_python_sdk.example_scripts.get_gmx_stats import GetGMXv2Stats
+from gmx_python_sdk.scripts.v2.gmx_utils import ConfigManager
 
 to_json = False
 to_csv = False
-chain = "arbitrum"
+
+config = ConfigManager(chain='arbitrum')
+config.set_config()
 
 stats_object = GetGMXv2Stats(
-    to_json=to_json,
-    to_csv=to_csv
+     config=config,
+     to_json=to_json,
+     to_csv=to_csv
 )
 
-liquidity = stats_object.get_available_liquidity(chain=chain)
-borrow_apr = stats_object.get_borrow_apr(chain=chain)
-claimable_fees = stats_object.get_claimable_fees(chain=chain)
-contract_tvl = stats_object.get_contract_tvl(chain=chain)
-funding_apr = stats_object.get_funding_apr(chain=chain)
-gm_prices = stats_object.get_gm_price(chain=chain)
-markets = stats_object.get_available_markets(chain=chain)
-open_interest = stats_object.get_open_interest(chain=chain)
-oracle_prices = stats_object.get_oracle_prices(chain=chain)
-pool_tvl = stats_object.get_pool_tvl(chain=chain)
+liquidity = stats_object.get_available_liquidity()
+borrow_apr = stats_object.get_borrow_apr()
+claimable_fees = stats_object.get_claimable_fees()
+contract_tvl = stats_object.get_contract_tvl()
+funding_apr = stats_object.get_funding_apr()
+gm_prices = stats_object.get_gm_price()
+markets = stats_object.get_available_markets()
+open_interest = stats_object.get_open_interest()
+oracle_prices = stats_object.get_oracle_prices()
+pool_tvl = stats_object.get_pool_tvl()
 ```
 
 ### Debug Mode
 
 It is possible to call IncreaseOrder, DecreaseOrder, SwapOrder, DepositOrder, and WithdrawOrder in debug mode by passing debug_mode=True when initialising the class:
 
 ```python
-from scripts.v2.create_increase_order import IncreaseOrder
+from gmx_python_sdk.scripts.v2.order.create_increase_order import IncreaseOrder
 
 order = IncreaseOrder(
-    chain,
-    market_key,
-    collateral_address,
-    index_token_address,
-    is_long,
-    size_delta_usd,
-    initial_collateral_delta_amount,
-    slippage_percent,
-    swap_path
+    config=config,
+    market_key=market_key,
+    collateral_address=collateral_address,
+    index_token_address=index_token_address,
+    is_long=is_long,
+    size_delta_usd=size_delta_usd,
+    initial_collateral_delta_amount=initial_collateral_delta_amount,
+    slippage_percent=slippage_percent,
+    swap_path=swap_path,
     debug_mode=True
 )
 ```
 
 This will allow you to submit parameters to the order class and build your txn without executing it.
 
 ### Known Limitations
 
 - Avalanche chain not fully tested.
 - A high rate limit RPC is required to read multiple sets of stats successively.
 - Possible to specify out token not the long/short of the GM market when withdrawing,
   but it will fail and return GM tokens to users wallet.
+- Testnet is currently NOT supported
```

