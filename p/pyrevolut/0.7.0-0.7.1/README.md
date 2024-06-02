# Comparing `tmp/pyrevolut-0.7.0.tar.gz` & `tmp/pyrevolut-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrevolut-0.7.0.tar", max compression
+gzip compressed data, was "pyrevolut-0.7.1.tar", max compression
```

## Comparing `pyrevolut-0.7.0.tar` & `pyrevolut-0.7.1.tar`

### file list

```diff
@@ -1,192 +1,202 @@
--rw-r--r--   0        0        0     1070 2024-06-01 13:49:29.114070 pyrevolut-0.7.0/LICENSE
--rw-r--r--   0        0        0     6350 2024-06-01 13:49:29.114070 pyrevolut-0.7.0/README.md
--rw-r--r--   0        0        0     2962 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/__init__.py
--rw-r--r--   0        0        0      391 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/__init__.py
--rw-r--r--   0        0        0      249 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/__init__.py
--rw-r--r--   0        0        0      173 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/endpoint/__init__.py
--rw-r--r--   0        0        0     2550 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/endpoint/asynchronous.py
--rw-r--r--   0        0        0     2505 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/endpoint/synchronous.py
--rw-r--r--   0        0        0      244 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/get/__init__.py
--rw-r--r--   0        0        0      432 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/get/retrieve_all_accounts.py
--rw-r--r--   0        0        0      489 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/get/retrieve_an_account.py
--rw-r--r--   0        0        0     4310 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/get/retrieve_full_bank_details.py
--rw-r--r--   0        0        0      114 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/resources/__init__.py
--rw-r--r--   0        0        0     1353 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/accounts/resources/account.py
--rw-r--r--   0        0        0      378 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/__init__.py
--rw-r--r--   0        0        0      115 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/delete/__init__.py
--rw-r--r--   0        0        0      468 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/delete/terminate_card.py
--rw-r--r--   0        0        0      164 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/endpoint/__init__.py
--rw-r--r--   0        0        0    21903 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/endpoint/asynchronous.py
--rw-r--r--   0        0        0    21798 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/endpoint/synchronous.py
--rw-r--r--   0        0        0      255 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/get/__init__.py
--rw-r--r--   0        0        0      450 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/get/retrieve_card_details.py
--rw-r--r--   0        0        0     1534 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/get/retrieve_list_of_cards.py
--rw-r--r--   0        0        0      854 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/get/retrieve_sensitive_card_details.py
--rw-r--r--   0        0        0      123 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/patch/__init__.py
--rw-r--r--   0        0        0     5567 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/patch/update_card_details.py
--rw-r--r--   0        0        0      183 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/post/__init__.py
--rw-r--r--   0        0        0     6523 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/post/create_card.py
--rw-r--r--   0        0        0      562 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/post/freeze_card.py
--rw-r--r--   0        0        0      565 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/post/unfreeze_card.py
--rw-r--r--   0        0        0      104 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/resources/__init__.py
--rw-r--r--   0        0        0     3954 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/cards/resources/card.py
--rw-r--r--   0        0        0      191 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/common/__init__.py
--rw-r--r--   0        0        0      741 2024-06-01 13:49:29.118070 pyrevolut-0.7.0/pyrevolut/api/common/endpoint.py
--rw-r--r--   0        0        0     1351 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/__init__.py
--rw-r--r--   0        0        0     1046 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/account_name_match_code.py
--rw-r--r--   0        0        0     1908 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/account_name_match_reason_code.py
--rw-r--r--   0        0        0      232 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/account_name_match_reason_type.py
--rw-r--r--   0        0        0      138 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/account_state.py
--rw-r--r--   0        0        0      156 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/account_type.py
--rw-r--r--   0        0        0      134 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/card_scheme.py
--rw-r--r--   0        0        0      205 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/card_state.py
--rw-r--r--   0        0        0      176 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/charge_bearer.py
--rw-r--r--   0        0        0      651 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/merchant_category.py
--rw-r--r--   0        0        0      313 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/payment_draft_state.py
--rw-r--r--   0        0        0      336 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/payment_scheme.py
--rw-r--r--   0        0        0      345 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/payout_link_cancellation_reason.py
--rw-r--r--   0        0        0      443 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/payout_link_payment_method.py
--rw-r--r--   0        0        0     1061 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/payout_link_state.py
--rw-r--r--   0        0        0      162 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/profile_state.py
--rw-r--r--   0        0        0      140 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/profile_type.py
--rw-r--r--   0        0        0      138 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/recipient_charges.py
--rw-r--r--   0        0        0      226 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/simulate_transfer_state_action.py
--rw-r--r--   0        0        0      247 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/team_member_state.py
--rw-r--r--   0        0        0      120 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/time_unit.py
--rw-r--r--   0        0        0     1251 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/transaction_state.py
--rw-r--r--   0        0        0      489 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/transaction_type.py
--rw-r--r--   0        0        0     1093 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/transfer_reason_code.py
--rw-r--r--   0        0        0      318 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/enums/webhook_event.py
--rw-r--r--   0        0        0      126 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/models/__init__.py
--rw-r--r--   0        0        0      386 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/common/models/amount.py
--rw-r--r--   0        0        0      772 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/__init__.py
--rw-r--r--   0        0        0      135 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/delete/__init__.py
--rw-r--r--   0        0        0      474 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/delete/delete_counterparty.py
--rw-r--r--   0        0        0      191 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/endpoint/__init__.py
--rw-r--r--   0        0        0    14383 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/endpoint/asynchronous.py
--rw-r--r--   0        0        0    14313 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/endpoint/synchronous.py
--rw-r--r--   0        0        0      210 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/get/__init__.py
--rw-r--r--   0        0        0      485 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/get/retrieve_counterparty.py
--rw-r--r--   0        0        0     3888 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/get/retrieve_list_of_counterparties.py
--rw-r--r--   0        0        0      188 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/post/__init__.py
--rw-r--r--   0        0        0     8872 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/post/create_counterparty.py
--rw-r--r--   0        0        0     8378 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/post/validate_account_name.py
--rw-r--r--   0        0        0      130 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/resources/__init__.py
--rw-r--r--   0        0        0     5381 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/counterparties/resources/counterparty.py
--rw-r--r--   0        0        0      271 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/__init__.py
--rw-r--r--   0        0        0      195 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/endpoint/__init__.py
--rw-r--r--   0        0        0     4364 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/endpoint/asynchronous.py
--rw-r--r--   0        0        0     4331 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/endpoint/synchronous.py
--rw-r--r--   0        0        0      129 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/get/__init__.py
--rw-r--r--   0        0        0     1231 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/get/get_exchange_rate.py
--rw-r--r--   0        0        0      125 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/post/__init__.py
--rw-r--r--   0        0        0     6574 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/post/exchange_money.py
--rw-r--r--   0        0        0      139 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/resources/__init__.py
--rw-r--r--   0        0        0     1158 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/resources/foreign_exchange.py
--rw-r--r--   0        0        0      475 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/__init__.py
--rw-r--r--   0        0        0      136 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/delete/__init__.py
--rw-r--r--   0        0        0      462 2024-06-01 13:49:29.122070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/delete/delete_payment_draft.py
--rw-r--r--   0        0        0      189 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/endpoint/__init__.py
--rw-r--r--   0        0        0     6986 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/endpoint/asynchronous.py
--rw-r--r--   0        0        0     6929 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/endpoint/synchronous.py
--rw-r--r--   0        0        0      203 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/get/__init__.py
--rw-r--r--   0        0        0     1328 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/get/retrieve_all_payment_drafts.py
--rw-r--r--   0        0        0     6034 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/get/retrieve_payment_draft.py
--rw-r--r--   0        0        0      134 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/post/__init__.py
--rw-r--r--   0        0        0     3944 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payment_drafts/post/create_payment_draft.py
--rw-r--r--   0        0        0      331 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/__init__.py
--rw-r--r--   0        0        0      183 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/endpoint/__init__.py
--rw-r--r--   0        0        0     9350 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/endpoint/asynchronous.py
--rw-r--r--   0        0        0     9436 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/endpoint/synchronous.py
--rw-r--r--   0        0        0      200 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/get/__init__.py
--rw-r--r--   0        0        0     3198 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/get/retrieve_list_of_payout_links.py
--rw-r--r--   0        0        0      560 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/get/retrieve_payout_link.py
--rw-r--r--   0        0        0      177 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/post/__init__.py
--rw-r--r--   0        0        0      580 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/post/cancel_payout_link.py
--rw-r--r--   0        0        0     4911 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/post/create_payout_link.py
--rw-r--r--   0        0        0      125 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/resources/__init__.py
--rw-r--r--   0        0        0     5949 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/payout_links/resources/payout_link.py
--rw-r--r--   0        0        0      398 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/simulations/__init__.py
--rw-r--r--   0        0        0      182 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/simulations/endpoint/__init__.py
--rw-r--r--   0        0        0     4995 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/simulations/endpoint/asynchronous.py
--rw-r--r--   0        0        0     4962 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/simulations/endpoint/synchronous.py
--rw-r--r--   0        0        0      206 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/simulations/post/__init__.py
--rw-r--r--   0        0        0     4930 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/simulations/post/simulate_account_topup.py
--rw-r--r--   0        0        0     2195 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/simulations/post/simulate_transfer_state_update.py
--rw-r--r--   0        0        0      363 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/__init__.py
--rw-r--r--   0        0        0      183 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/endpoint/__init__.py
--rw-r--r--   0        0        0     5782 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/endpoint/asynchronous.py
--rw-r--r--   0        0        0     5737 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/endpoint/synchronous.py
--rw-r--r--   0        0        0      198 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/get/__init__.py
--rw-r--r--   0        0        0     2852 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/get/retrieve_list_of_team_members.py
--rw-r--r--   0        0        0     2218 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/get/retrieve_team_roles.py
--rw-r--r--   0        0        0      128 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/post/__init__.py
--rw-r--r--   0        0        0     1670 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/team_members/post/invite_team_member.py
--rw-r--r--   0        0        0      291 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/__init__.py
--rw-r--r--   0        0        0      185 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/endpoint/__init__.py
--rw-r--r--   0        0        0     5902 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/endpoint/asynchronous.py
--rw-r--r--   0        0        0     5869 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/endpoint/synchronous.py
--rw-r--r--   0        0        0      202 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/get/__init__.py
--rw-r--r--   0        0        0     3868 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/get/retrieve_list_of_transactions.py
--rw-r--r--   0        0        0     1393 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/get/retrieve_transaction.py
--rw-r--r--   0        0        0      126 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/resources/__init__.py
--rw-r--r--   0        0        0     6725 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transactions/resources/transaction.py
--rw-r--r--   0        0        0      276 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transfers/__init__.py
--rw-r--r--   0        0        0      176 2024-06-01 13:49:29.126070 pyrevolut-0.7.0/pyrevolut/api/transfers/endpoint/__init__.py
--rw-r--r--   0        0        0     8101 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/endpoint/asynchronous.py
--rw-r--r--   0        0        0     8056 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/endpoint/synchronous.py
--rw-r--r--   0        0        0      128 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/get/__init__.py
--rw-r--r--   0        0        0     1804 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/get/get_transfer_reasons.py
--rw-r--r--   0        0        0      221 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/post/__init__.py
--rw-r--r--   0        0        0     5738 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/post/create_transfer_to_another_account.py
--rw-r--r--   0        0        0     2090 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/post/move_money_between_accounts.py
--rw-r--r--   0        0        0      117 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/resources/__init__.py
--rw-r--r--   0        0        0     1897 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/transfers/resources/transfer.py
--rw-r--r--   0        0        0      666 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/__init__.py
--rw-r--r--   0        0        0      119 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/delete/__init__.py
--rw-r--r--   0        0        0      429 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/delete/delete_webhook.py
--rw-r--r--   0        0        0      173 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/endpoint/__init__.py
--rw-r--r--   0        0        0     9281 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/endpoint/asynchronous.py
--rw-r--r--   0        0        0     1494 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/endpoint/base.py
--rw-r--r--   0        0        0     9190 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/endpoint/synchronous.py
--rw-r--r--   0        0        0      257 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/get/__init__.py
--rw-r--r--   0        0        0     3139 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/get/retrieve_list_of_failed_webhooks.py
--rw-r--r--   0        0        0      470 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/get/retrieve_list_of_webhooks.py
--rw-r--r--   0        0        0      691 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/get/retrieve_webhook.py
--rw-r--r--   0        0        0      118 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/patch/__init__.py
--rw-r--r--   0        0        0     1228 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/patch/update_webhook.py
--rw-r--r--   0        0        0      172 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/post/__init__.py
--rw-r--r--   0        0        0     1531 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/post/create_webhook.py
--rw-r--r--   0        0        0     1252 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/post/rotate_webhook_secret.py
--rw-r--r--   0        0        0      426 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/__init__.py
--rw-r--r--   0        0        0      589 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/payout_link_created.py
--rw-r--r--   0        0        0      738 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/payout_link_state_changed.py
--rw-r--r--   0        0        0     4801 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/transaction_created.py
--rw-r--r--   0        0        0      737 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/transaction_state_changed.py
--rw-r--r--   0        0        0      633 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/webhook.py
--rw-r--r--   0        0        0      937 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/webhook_payload.py
--rw-r--r--   0        0        0       71 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/cli/__init__.py
--rw-r--r--   0        0        0       50 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/cli/__main__.py
--rw-r--r--   0        0        0     2498 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/cli/main.py
--rw-r--r--   0        0        0      195 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/client/__init__.py
--rw-r--r--   0        0        0     7406 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/client/asynchronous.py
--rw-r--r--   0        0        0    19986 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/client/base.py
--rw-r--r--   0        0        0     7207 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/client/synchronous.py
--rw-r--r--   0        0        0      312 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/exceptions/__init__.py
--rw-r--r--   0        0        0      177 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/exceptions/bad_request.py
--rw-r--r--   0        0        0      105 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/exceptions/common.py
--rw-r--r--   0        0        0      241 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/exceptions/internal_revolut_error.py
--rw-r--r--   0        0        0      161 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/exceptions/invalid_environment.py
--rw-r--r--   0        0        0       75 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/utils/__init__.py
--rw-r--r--   0        0        0      452 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/utils/auth/__init__.py
--rw-r--r--   0        0        0    10702 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/utils/auth/auth_manual.py
--rw-r--r--   0        0        0     2630 2024-06-01 13:49:29.130070 pyrevolut-0.7.0/pyrevolut/utils/auth/create_client_assert_jwt.py
--rw-r--r--   0        0        0     5204 2024-06-01 13:49:29.134070 pyrevolut-0.7.0/pyrevolut/utils/auth/creds.py
--rw-r--r--   0        0        0      858 2024-06-01 13:49:29.134070 pyrevolut-0.7.0/pyrevolut/utils/auth/enum_auth_scope.py
--rw-r--r--   0        0        0     4409 2024-06-01 13:49:29.134070 pyrevolut-0.7.0/pyrevolut/utils/auth/gen_public_private_cert.py
--rw-r--r--   0        0        0     3346 2024-06-01 13:49:29.134070 pyrevolut-0.7.0/pyrevolut/utils/auth/get_auth_tokens.py
--rw-r--r--   0        0        0     3273 2024-06-01 13:49:29.134070 pyrevolut-0.7.0/pyrevolut/utils/auth/refresh_access_token.py
--rw-r--r--   0        0        0     3269 2024-06-01 13:49:29.134070 pyrevolut-0.7.0/pyrevolut/utils/date.py
--rw-r--r--   0        0        0     4391 2024-06-01 13:49:29.134070 pyrevolut-0.7.0/pyrevolut/utils/datetime.py
--rw-r--r--   0        0        0     7218 1970-01-01 00:00:00.000000 pyrevolut-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-06-02 14:59:25.080155 pyrevolut-0.7.1/LICENSE
+-rw-r--r--   0        0        0     6385 2024-06-02 14:59:25.080155 pyrevolut-0.7.1/README.md
+-rw-r--r--   0        0        0     3033 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/__init__.py
+-rw-r--r--   0        0        0      391 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/__init__.py
+-rw-r--r--   0        0        0      249 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/accounts/__init__.py
+-rw-r--r--   0        0        0      173 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/accounts/endpoint/__init__.py
+-rw-r--r--   0        0        0     2550 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/accounts/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     2505 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/accounts/endpoint/synchronous.py
+-rw-r--r--   0        0        0      244 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/accounts/get/__init__.py
+-rw-r--r--   0        0        0      432 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/accounts/get/retrieve_all_accounts.py
+-rw-r--r--   0        0        0      489 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/accounts/get/retrieve_an_account.py
+-rw-r--r--   0        0        0     4310 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/accounts/get/retrieve_full_bank_details.py
+-rw-r--r--   0        0        0      114 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/accounts/resources/__init__.py
+-rw-r--r--   0        0        0     1353 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/accounts/resources/account.py
+-rw-r--r--   0        0        0      378 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/__init__.py
+-rw-r--r--   0        0        0      115 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/delete/__init__.py
+-rw-r--r--   0        0        0      468 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/delete/terminate_card.py
+-rw-r--r--   0        0        0      164 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/endpoint/__init__.py
+-rw-r--r--   0        0        0    21903 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/endpoint/asynchronous.py
+-rw-r--r--   0        0        0    21798 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/endpoint/synchronous.py
+-rw-r--r--   0        0        0      255 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/get/__init__.py
+-rw-r--r--   0        0        0      450 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/get/retrieve_card_details.py
+-rw-r--r--   0        0        0     1534 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/get/retrieve_list_of_cards.py
+-rw-r--r--   0        0        0      854 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/get/retrieve_sensitive_card_details.py
+-rw-r--r--   0        0        0      123 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/patch/__init__.py
+-rw-r--r--   0        0        0     5567 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/patch/update_card_details.py
+-rw-r--r--   0        0        0      183 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/post/__init__.py
+-rw-r--r--   0        0        0     6523 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/post/create_card.py
+-rw-r--r--   0        0        0      562 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/post/freeze_card.py
+-rw-r--r--   0        0        0      565 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/post/unfreeze_card.py
+-rw-r--r--   0        0        0      104 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/resources/__init__.py
+-rw-r--r--   0        0        0     3954 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/cards/resources/card.py
+-rw-r--r--   0        0        0      191 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/__init__.py
+-rw-r--r--   0        0        0      741 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/endpoint.py
+-rw-r--r--   0        0        0     1275 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/__init__.py
+-rw-r--r--   0        0        0     1046 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/account_name_match_code.py
+-rw-r--r--   0        0        0     1908 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/account_name_match_reason_code.py
+-rw-r--r--   0        0        0      232 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/account_name_match_reason_type.py
+-rw-r--r--   0        0        0      138 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/account_state.py
+-rw-r--r--   0        0        0      156 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/account_type.py
+-rw-r--r--   0        0        0      134 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/card_scheme.py
+-rw-r--r--   0        0        0      205 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/card_state.py
+-rw-r--r--   0        0        0      176 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/charge_bearer.py
+-rw-r--r--   0        0        0      651 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/merchant_category.py
+-rw-r--r--   0        0        0      313 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/payment_draft_state.py
+-rw-r--r--   0        0        0      336 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/payment_scheme.py
+-rw-r--r--   0        0        0      345 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/payout_link_cancellation_reason.py
+-rw-r--r--   0        0        0      443 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/payout_link_payment_method.py
+-rw-r--r--   0        0        0     1061 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/payout_link_state.py
+-rw-r--r--   0        0        0      162 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/profile_state.py
+-rw-r--r--   0        0        0      140 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/profile_type.py
+-rw-r--r--   0        0        0      138 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/recipient_charges.py
+-rw-r--r--   0        0        0      247 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/team_member_state.py
+-rw-r--r--   0        0        0      120 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/time_unit.py
+-rw-r--r--   0        0        0     1251 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/transaction_state.py
+-rw-r--r--   0        0        0      489 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/transaction_type.py
+-rw-r--r--   0        0        0     1093 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/transfer_reason_code.py
+-rw-r--r--   0        0        0      318 2024-06-02 14:59:25.084156 pyrevolut-0.7.1/pyrevolut/api/common/enums/webhook_event.py
+-rw-r--r--   0        0        0      126 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/common/models/__init__.py
+-rw-r--r--   0        0        0      386 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/common/models/amount.py
+-rw-r--r--   0        0        0      772 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/counterparties/__init__.py
+-rw-r--r--   0        0        0      135 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/counterparties/delete/__init__.py
+-rw-r--r--   0        0        0      474 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/counterparties/delete/delete_counterparty.py
+-rw-r--r--   0        0        0      191 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/counterparties/endpoint/__init__.py
+-rw-r--r--   0        0        0    14383 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/counterparties/endpoint/asynchronous.py
+-rw-r--r--   0        0        0    14313 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/counterparties/endpoint/synchronous.py
+-rw-r--r--   0        0        0      210 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/counterparties/get/__init__.py
+-rw-r--r--   0        0        0      485 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/counterparties/get/retrieve_counterparty.py
+-rw-r--r--   0        0        0     3888 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/counterparties/get/retrieve_list_of_counterparties.py
+-rw-r--r--   0        0        0      188 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/counterparties/post/__init__.py
+-rw-r--r--   0        0        0     8872 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/counterparties/post/create_counterparty.py
+-rw-r--r--   0        0        0     8378 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/counterparties/post/validate_account_name.py
+-rw-r--r--   0        0        0      130 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/counterparties/resources/__init__.py
+-rw-r--r--   0        0        0     5381 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/counterparties/resources/counterparty.py
+-rw-r--r--   0        0        0      271 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/foreign_exchange/__init__.py
+-rw-r--r--   0        0        0      195 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/foreign_exchange/endpoint/__init__.py
+-rw-r--r--   0        0        0     4364 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/foreign_exchange/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     4331 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/foreign_exchange/endpoint/synchronous.py
+-rw-r--r--   0        0        0      129 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/foreign_exchange/get/__init__.py
+-rw-r--r--   0        0        0     1231 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/foreign_exchange/get/get_exchange_rate.py
+-rw-r--r--   0        0        0      125 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/foreign_exchange/post/__init__.py
+-rw-r--r--   0        0        0     6574 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/foreign_exchange/post/exchange_money.py
+-rw-r--r--   0        0        0      139 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/foreign_exchange/resources/__init__.py
+-rw-r--r--   0        0        0     1158 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/foreign_exchange/resources/foreign_exchange.py
+-rw-r--r--   0        0        0      475 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payment_drafts/__init__.py
+-rw-r--r--   0        0        0      136 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payment_drafts/delete/__init__.py
+-rw-r--r--   0        0        0      462 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payment_drafts/delete/delete_payment_draft.py
+-rw-r--r--   0        0        0      189 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payment_drafts/endpoint/__init__.py
+-rw-r--r--   0        0        0     6986 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payment_drafts/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     6929 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payment_drafts/endpoint/synchronous.py
+-rw-r--r--   0        0        0      203 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payment_drafts/get/__init__.py
+-rw-r--r--   0        0        0     1328 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payment_drafts/get/retrieve_all_payment_drafts.py
+-rw-r--r--   0        0        0     6034 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payment_drafts/get/retrieve_payment_draft.py
+-rw-r--r--   0        0        0      134 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payment_drafts/post/__init__.py
+-rw-r--r--   0        0        0     3944 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payment_drafts/post/create_payment_draft.py
+-rw-r--r--   0        0        0      331 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payout_links/__init__.py
+-rw-r--r--   0        0        0      183 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payout_links/endpoint/__init__.py
+-rw-r--r--   0        0        0     9350 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payout_links/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     9436 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payout_links/endpoint/synchronous.py
+-rw-r--r--   0        0        0      200 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payout_links/get/__init__.py
+-rw-r--r--   0        0        0     3198 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payout_links/get/retrieve_list_of_payout_links.py
+-rw-r--r--   0        0        0      560 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payout_links/get/retrieve_payout_link.py
+-rw-r--r--   0        0        0      177 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payout_links/post/__init__.py
+-rw-r--r--   0        0        0      580 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payout_links/post/cancel_payout_link.py
+-rw-r--r--   0        0        0     4911 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payout_links/post/create_payout_link.py
+-rw-r--r--   0        0        0      125 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payout_links/resources/__init__.py
+-rw-r--r--   0        0        0     5949 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/payout_links/resources/payout_link.py
+-rw-r--r--   0        0        0      398 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/simulations/__init__.py
+-rw-r--r--   0        0        0      182 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/simulations/endpoint/__init__.py
+-rw-r--r--   0        0        0     5104 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/simulations/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     5071 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/simulations/endpoint/synchronous.py
+-rw-r--r--   0        0        0      206 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/simulations/post/__init__.py
+-rw-r--r--   0        0        0     4930 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/simulations/post/simulate_account_topup.py
+-rw-r--r--   0        0        0     2195 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/simulations/post/simulate_transfer_state_update.py
+-rw-r--r--   0        0        0      363 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/team_members/__init__.py
+-rw-r--r--   0        0        0      183 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/team_members/endpoint/__init__.py
+-rw-r--r--   0        0        0     5782 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/team_members/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     5737 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/team_members/endpoint/synchronous.py
+-rw-r--r--   0        0        0      198 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/team_members/get/__init__.py
+-rw-r--r--   0        0        0     2852 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/team_members/get/retrieve_list_of_team_members.py
+-rw-r--r--   0        0        0     2218 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/team_members/get/retrieve_team_roles.py
+-rw-r--r--   0        0        0      128 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/team_members/post/__init__.py
+-rw-r--r--   0        0        0     1670 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/team_members/post/invite_team_member.py
+-rw-r--r--   0        0        0      291 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/transactions/__init__.py
+-rw-r--r--   0        0        0      185 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/transactions/endpoint/__init__.py
+-rw-r--r--   0        0        0     5902 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/transactions/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     5869 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/transactions/endpoint/synchronous.py
+-rw-r--r--   0        0        0      202 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/transactions/get/__init__.py
+-rw-r--r--   0        0        0     3868 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/transactions/get/retrieve_list_of_transactions.py
+-rw-r--r--   0        0        0     1393 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/transactions/get/retrieve_transaction.py
+-rw-r--r--   0        0        0      126 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/transactions/resources/__init__.py
+-rw-r--r--   0        0        0     6725 2024-06-02 14:59:25.088156 pyrevolut-0.7.1/pyrevolut/api/transactions/resources/transaction.py
+-rw-r--r--   0        0        0      276 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/transfers/__init__.py
+-rw-r--r--   0        0        0      176 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/transfers/endpoint/__init__.py
+-rw-r--r--   0        0        0     8101 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/transfers/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     8056 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/transfers/endpoint/synchronous.py
+-rw-r--r--   0        0        0      128 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/transfers/get/__init__.py
+-rw-r--r--   0        0        0     1804 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/transfers/get/get_transfer_reasons.py
+-rw-r--r--   0        0        0      221 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/transfers/post/__init__.py
+-rw-r--r--   0        0        0     5738 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/transfers/post/create_transfer_to_another_account.py
+-rw-r--r--   0        0        0     2090 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/transfers/post/move_money_between_accounts.py
+-rw-r--r--   0        0        0      117 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/transfers/resources/__init__.py
+-rw-r--r--   0        0        0     1897 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/transfers/resources/transfer.py
+-rw-r--r--   0        0        0      666 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/__init__.py
+-rw-r--r--   0        0        0      119 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/delete/__init__.py
+-rw-r--r--   0        0        0      429 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/delete/delete_webhook.py
+-rw-r--r--   0        0        0      173 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/endpoint/__init__.py
+-rw-r--r--   0        0        0     9281 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/endpoint/asynchronous.py
+-rw-r--r--   0        0        0     7435 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/endpoint/base.py
+-rw-r--r--   0        0        0     9190 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/endpoint/synchronous.py
+-rw-r--r--   0        0        0      257 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/get/__init__.py
+-rw-r--r--   0        0        0     3139 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/get/retrieve_list_of_failed_webhooks.py
+-rw-r--r--   0        0        0      470 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/get/retrieve_list_of_webhooks.py
+-rw-r--r--   0        0        0      691 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/get/retrieve_webhook.py
+-rw-r--r--   0        0        0      118 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/patch/__init__.py
+-rw-r--r--   0        0        0     1228 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/patch/update_webhook.py
+-rw-r--r--   0        0        0      172 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/post/__init__.py
+-rw-r--r--   0        0        0     1531 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/post/create_webhook.py
+-rw-r--r--   0        0        0     1252 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/post/rotate_webhook_secret.py
+-rw-r--r--   0        0        0      426 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/resources/__init__.py
+-rw-r--r--   0        0        0      589 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/resources/payout_link_created.py
+-rw-r--r--   0        0        0      738 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/resources/payout_link_state_changed.py
+-rw-r--r--   0        0        0     4801 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/resources/transaction_created.py
+-rw-r--r--   0        0        0      737 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/resources/transaction_state_changed.py
+-rw-r--r--   0        0        0      633 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/resources/webhook.py
+-rw-r--r--   0        0        0      937 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/api/webhooks/resources/webhook_payload.py
+-rw-r--r--   0        0        0       71 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/cli/__init__.py
+-rw-r--r--   0        0        0       50 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/cli/__main__.py
+-rw-r--r--   0        0        0     2498 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/cli/main.py
+-rw-r--r--   0        0        0      195 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/client/__init__.py
+-rw-r--r--   0        0        0     7406 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/client/asynchronous.py
+-rw-r--r--   0        0        0    21579 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/client/base.py
+-rw-r--r--   0        0        0     7207 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/client/synchronous.py
+-rw-r--r--   0        0        0      866 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/__init__.py
+-rw-r--r--   0        0        0      346 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/bad_request.py
+-rw-r--r--   0        0        0      291 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/common.py
+-rw-r--r--   0        0        0      409 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/conflict.py
+-rw-r--r--   0        0        0      367 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/forbidden.py
+-rw-r--r--   0        0        0      384 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/internal_server_error.py
+-rw-r--r--   0        0        0      387 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/invalid_environment.py
+-rw-r--r--   0        0        0      413 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/invalid_payload.py
+-rw-r--r--   0        0        0      420 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/method_not_allowed.py
+-rw-r--r--   0        0        0      398 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/network_error.py
+-rw-r--r--   0        0        0      382 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/not_acceptable.py
+-rw-r--r--   0        0        0      360 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/not_found.py
+-rw-r--r--   0        0        0      421 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/server_unavailable.py
+-rw-r--r--   0        0        0      324 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/timeout_error.py
+-rw-r--r--   0        0        0      370 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/too_many_requests.py
+-rw-r--r--   0        0        0      360 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/exceptions/unauthorized.py
+-rw-r--r--   0        0        0       75 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/utils/__init__.py
+-rw-r--r--   0        0        0      452 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/utils/auth/__init__.py
+-rw-r--r--   0        0        0    10702 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/utils/auth/auth_manual.py
+-rw-r--r--   0        0        0     2630 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/utils/auth/create_client_assert_jwt.py
+-rw-r--r--   0        0        0     5204 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/utils/auth/creds.py
+-rw-r--r--   0        0        0      858 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/utils/auth/enum_auth_scope.py
+-rw-r--r--   0        0        0     4409 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/utils/auth/gen_public_private_cert.py
+-rw-r--r--   0        0        0     3346 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/utils/auth/get_auth_tokens.py
+-rw-r--r--   0        0        0     3273 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/utils/auth/refresh_access_token.py
+-rw-r--r--   0        0        0     3269 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/utils/date.py
+-rw-r--r--   0        0        0     4391 2024-06-02 14:59:25.092156 pyrevolut-0.7.1/pyrevolut/utils/datetime.py
+-rw-r--r--   0        0        0     7253 1970-01-01 00:00:00.000000 pyrevolut-0.7.1/PKG-INFO
```

### Comparing `pyrevolut-0.7.0/LICENSE` & `pyrevolut-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/README.md` & `pyrevolut-0.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,15 @@
   - [x] Create a new webhook
   - [x] Retrieve a list of webhooks
   - [x] Retrieve a webhook
   - [x] Update a webhook
   - [x] Delete a webhook
   - [x] Rotate a webhook signing secret
   - [x] Retrieve a list of failed webhook events
+  - [x] Verify a webhook signature
 
 ## **Contributing**
 
 In order to facilitate a streamlined development process, we have a few guidelines that we would like to follow. Please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file for more information.
 
 ## **License**
```

### Comparing `pyrevolut-0.7.0/pyproject.toml` & `pyrevolut-0.7.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyrevolut"
-version = "0.7.0"
+version = "0.7.1"
 description = "An unofficial Python API Wrapper for the Revolut Business API"
 authors = ["Trevor Visser <trevor.visser@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/Trevypants/pyrevolut"
 readme = "README.md"
 
 [tool.poetry.scripts]
@@ -38,14 +38,18 @@
 pytest-sugar = "0.*"
 pytest-instafail = "0.*"
 pytest-profiling = "1.*"
 pytest-randomly = "3.*"
 pytest-clarity = "1.*"
 pytest-split = "0.*"
 pytest-env = "1.*"
+pyngrok = "7.*"
+litestar = "2.*"
+uvicorn = "0.*"
+python-dotenv = "1.*"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "9.*"
 mkdocstrings = { extras = ["python"], version = "0.*" }
 
 [tool.pytest.ini_options]
 pythonpath = ["."]
@@ -109,15 +113,15 @@
 docstring-code-format = true
 
 [tool.ruff.lint.isort]
 known-first-party = ["pyrevolut", "tests"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.7.0"
+version = "0.7.1"
 tag_format = "v$major.$minor.$patch$prerelease"
 version_scheme = "pep440"
 version_provider = "poetry"
 update_changelog_on_bump = true
 major_version_zero = true
 version_files = ["pyrevolut/__init__.py:__version__", "pyproject.toml:^version"]
```

### Comparing `pyrevolut-0.7.0/pyrevolut/api/accounts/endpoint/asynchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/accounts/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/accounts/endpoint/synchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/accounts/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/accounts/get/retrieve_full_bank_details.py` & `pyrevolut-0.7.1/pyrevolut/api/accounts/get/retrieve_full_bank_details.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/accounts/resources/account.py` & `pyrevolut-0.7.1/pyrevolut/api/accounts/resources/account.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/cards/endpoint/asynchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/cards/endpoint/synchronous.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from typing import Literal, Type
 from uuid import UUID
 from datetime import datetime
 
 from pydantic import BaseModel
 
 from pyrevolut.utils import DateTime
-from pyrevolut.exceptions import InvalidEnvironmentException
-from pyrevolut.api.common import BaseEndpointAsync, EnumMerchantCategory
+from pyrevolut.exceptions import PyRevolutInvalidEnvironment
+from pyrevolut.api.common import BaseEndpointSync, EnumMerchantCategory
 from pyrevolut.api.cards.get import (
     RetrieveListOfCards,
     RetrieveCardDetails,
     RetrieveSensitiveCardDetails,
 )
 from pyrevolut.api.cards.post import CreateCard, FreezeCard, UnfreezeCard
 from pyrevolut.api.cards.patch import UpdateCardDetails
 from pyrevolut.api.cards.delete import TerminateCard
 
 
-class EndpointCardsAsync(BaseEndpointAsync):
-    """The async Cards API
+class EndpointCardsSync(BaseEndpointSync):
+    """The Cards API
     Manage cards for the business team members, freeze, unfreeze,
     terminate and update card settings, such as transaction limits.
 
     This feature is available in the UK, US and the EEA.
     This feature is not available in Sandbox.
     """
 
-    async def get_all_cards(
+    def get_all_cards(
         self,
         created_before: datetime | DateTime | str | int | float | None = None,
         limit: int | None = None,
         **kwargs,
     ) -> list[dict] | list[RetrieveListOfCards.Response]:
         """
         Get the list of all cards in your organisation.
@@ -59,22 +59,22 @@
         endpoint = RetrieveListOfCards
         path = endpoint.ROUTE
         params = endpoint.Params(
             created_before=created_before,
             limit=limit,
         )
 
-        return await self.client.get(
+        return self.client.get(
             path=path,
             response_model=endpoint.Response,
             params=params,
             **kwargs,
         )
 
-    async def get_card(
+    def get_card(
         self,
         card_id: UUID,
         **kwargs,
     ) -> dict | RetrieveCardDetails.Response:
         """
         Get the details of a specific card, based on its ID.
 
@@ -89,22 +89,22 @@
             The details of the card.
         """
         self.__check_sandbox()
         endpoint = RetrieveCardDetails
         path = endpoint.ROUTE.format(card_id=card_id)
         params = endpoint.Params()
 
-        return await self.client.get(
+        return self.client.get(
             path=path,
             response_model=endpoint.Response,
             params=params,
             **kwargs,
         )
 
-    async def get_card_sensitive_details(
+    def get_card_sensitive_details(
         self,
         card_id: UUID,
         **kwargs,
     ) -> dict | RetrieveSensitiveCardDetails.Response:
         """
         Get sensitive details of a specific card, based on its ID.
         Requires the READ_SENSITIVE_CARD_DATA token scope.
@@ -120,22 +120,22 @@
             The sensitive details of the card.
         """
         self.__check_sandbox()
         endpoint = RetrieveSensitiveCardDetails
         path = endpoint.ROUTE.format(card_id=card_id)
         params = endpoint.Params()
 
-        return await self.client.get(
+        return self.client.get(
             path=path,
             response_model=endpoint.Response,
             params=params,
             **kwargs,
         )
 
-    async def create_card(
+    def create_card(
         self,
         request_id: str,
         holder_id: UUID,
         label: str | None = None,
         accounts: list[UUID] | None = None,
         categories: list[EnumMerchantCategory] | None = None,
         single_limit_amount: float | None = None,
@@ -296,22 +296,22 @@
             holder_id=holder_id,
             label=label,
             accounts=accounts,
             categories=categories,
             spending_limits=spending_limits,
         )
 
-        return await self.client.post(
+        return self.client.post(
             path=path,
             response_model=endpoint.Response,
             body=body,
             **kwargs,
         )
 
-    async def freeze_card(
+    def freeze_card(
         self,
         card_id: UUID,
         **kwargs,
     ) -> dict | FreezeCard.Response:
         """
         Freeze a card to make it temporarily unavailable for spending.
         You can only freeze a card that is in the state active.
@@ -330,22 +330,22 @@
             An empty dictionary.
         """
         self.__check_sandbox()
         endpoint = FreezeCard
         path = endpoint.ROUTE.format(card_id=card_id)
         body = endpoint.Body()
 
-        await self.client.post(
+        return self.client.post(
             path=path,
             response_model=endpoint.Response,
             body=body,
             **kwargs,
         )
 
-    async def unfreeze_card(
+    def unfreeze_card(
         self,
         card_id: UUID,
         **kwargs,
     ) -> dict | UnfreezeCard.Response:
         """
         Unfreeze a card to make it available for spending again.
         You can only unfreeze a card that is in the state frozen.
@@ -364,22 +364,22 @@
             An empty dictionary.
         """
         self.__check_sandbox()
         endpoint = UnfreezeCard
         path = endpoint.ROUTE.format(card_id=card_id)
         body = endpoint.Body()
 
-        return await self.client.post(
+        self.client.post(
             path=path,
             response_model=endpoint.Response,
             body=body,
             **kwargs,
         )
 
-    async def update_card(
+    def update_card(
         self,
         card_id: UUID,
         label: str | None = None,
         categories: list[EnumMerchantCategory] | Literal["null"] | None = None,
         single_limit_amount: float | Literal["null"] | None = None,
         single_limit_currency: str | Literal["null"] | None = None,
         day_limit_amount: float | Literal["null"] | None = None,
@@ -526,22 +526,22 @@
 
         body = endpoint.Body(
             label=label,
             categories=categories,
             spending_limits=spending_limits,
         )
 
-        return await self.client.patch(
+        return self.client.patch(
             path=path,
             response_model=endpoint.Response,
             body=body,
             **kwargs,
         )
 
-    async def delete_card(
+    def delete_card(
         self,
         card_id: UUID,
         **kwargs,
     ) -> dict | TerminateCard.Response:
         """
         Terminate a specific card, based on its ID.
 
@@ -560,15 +560,15 @@
             An empty dictionary.
         """
         self.__check_sandbox()
         endpoint = TerminateCard
         path = endpoint.ROUTE.format(card_id=card_id)
         params = endpoint.Params()
 
-        return await self.client.delete(
+        return self.client.delete(
             path=path,
             response_model=endpoint.Response,
             params=params,
             **kwargs,
         )
 
     def __process_limit_model(
@@ -591,14 +591,14 @@
 
     def __check_sandbox(self):
         """
         Check if the sandbox is enabled.
 
         Raises
         ------
-        InvalidEnvironmentException
+        PyRevolutInvalidEnvironment
             If the sandbox is enabled.
         """
         if self.client.sandbox:
-            raise InvalidEnvironmentException(
+            raise PyRevolutInvalidEnvironment(
                 "This feature is not available in Sandbox."
             )
```

### Comparing `pyrevolut-0.7.0/pyrevolut/api/cards/endpoint/synchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/cards/endpoint/asynchronous.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from typing import Literal, Type
 from uuid import UUID
 from datetime import datetime
 
 from pydantic import BaseModel
 
 from pyrevolut.utils import DateTime
-from pyrevolut.exceptions import InvalidEnvironmentException
-from pyrevolut.api.common import BaseEndpointSync, EnumMerchantCategory
+from pyrevolut.exceptions import PyRevolutInvalidEnvironment
+from pyrevolut.api.common import BaseEndpointAsync, EnumMerchantCategory
 from pyrevolut.api.cards.get import (
     RetrieveListOfCards,
     RetrieveCardDetails,
     RetrieveSensitiveCardDetails,
 )
 from pyrevolut.api.cards.post import CreateCard, FreezeCard, UnfreezeCard
 from pyrevolut.api.cards.patch import UpdateCardDetails
 from pyrevolut.api.cards.delete import TerminateCard
 
 
-class EndpointCardsSync(BaseEndpointSync):
-    """The Cards API
+class EndpointCardsAsync(BaseEndpointAsync):
+    """The async Cards API
     Manage cards for the business team members, freeze, unfreeze,
     terminate and update card settings, such as transaction limits.
 
     This feature is available in the UK, US and the EEA.
     This feature is not available in Sandbox.
     """
 
-    def get_all_cards(
+    async def get_all_cards(
         self,
         created_before: datetime | DateTime | str | int | float | None = None,
         limit: int | None = None,
         **kwargs,
     ) -> list[dict] | list[RetrieveListOfCards.Response]:
         """
         Get the list of all cards in your organisation.
@@ -59,22 +59,22 @@
         endpoint = RetrieveListOfCards
         path = endpoint.ROUTE
         params = endpoint.Params(
             created_before=created_before,
             limit=limit,
         )
 
-        return self.client.get(
+        return await self.client.get(
             path=path,
             response_model=endpoint.Response,
             params=params,
             **kwargs,
         )
 
-    def get_card(
+    async def get_card(
         self,
         card_id: UUID,
         **kwargs,
     ) -> dict | RetrieveCardDetails.Response:
         """
         Get the details of a specific card, based on its ID.
 
@@ -89,22 +89,22 @@
             The details of the card.
         """
         self.__check_sandbox()
         endpoint = RetrieveCardDetails
         path = endpoint.ROUTE.format(card_id=card_id)
         params = endpoint.Params()
 
-        return self.client.get(
+        return await self.client.get(
             path=path,
             response_model=endpoint.Response,
             params=params,
             **kwargs,
         )
 
-    def get_card_sensitive_details(
+    async def get_card_sensitive_details(
         self,
         card_id: UUID,
         **kwargs,
     ) -> dict | RetrieveSensitiveCardDetails.Response:
         """
         Get sensitive details of a specific card, based on its ID.
         Requires the READ_SENSITIVE_CARD_DATA token scope.
@@ -120,22 +120,22 @@
             The sensitive details of the card.
         """
         self.__check_sandbox()
         endpoint = RetrieveSensitiveCardDetails
         path = endpoint.ROUTE.format(card_id=card_id)
         params = endpoint.Params()
 
-        return self.client.get(
+        return await self.client.get(
             path=path,
             response_model=endpoint.Response,
             params=params,
             **kwargs,
         )
 
-    def create_card(
+    async def create_card(
         self,
         request_id: str,
         holder_id: UUID,
         label: str | None = None,
         accounts: list[UUID] | None = None,
         categories: list[EnumMerchantCategory] | None = None,
         single_limit_amount: float | None = None,
@@ -296,22 +296,22 @@
             holder_id=holder_id,
             label=label,
             accounts=accounts,
             categories=categories,
             spending_limits=spending_limits,
         )
 
-        return self.client.post(
+        return await self.client.post(
             path=path,
             response_model=endpoint.Response,
             body=body,
             **kwargs,
         )
 
-    def freeze_card(
+    async def freeze_card(
         self,
         card_id: UUID,
         **kwargs,
     ) -> dict | FreezeCard.Response:
         """
         Freeze a card to make it temporarily unavailable for spending.
         You can only freeze a card that is in the state active.
@@ -330,22 +330,22 @@
             An empty dictionary.
         """
         self.__check_sandbox()
         endpoint = FreezeCard
         path = endpoint.ROUTE.format(card_id=card_id)
         body = endpoint.Body()
 
-        return self.client.post(
+        await self.client.post(
             path=path,
             response_model=endpoint.Response,
             body=body,
             **kwargs,
         )
 
-    def unfreeze_card(
+    async def unfreeze_card(
         self,
         card_id: UUID,
         **kwargs,
     ) -> dict | UnfreezeCard.Response:
         """
         Unfreeze a card to make it available for spending again.
         You can only unfreeze a card that is in the state frozen.
@@ -364,22 +364,22 @@
             An empty dictionary.
         """
         self.__check_sandbox()
         endpoint = UnfreezeCard
         path = endpoint.ROUTE.format(card_id=card_id)
         body = endpoint.Body()
 
-        self.client.post(
+        return await self.client.post(
             path=path,
             response_model=endpoint.Response,
             body=body,
             **kwargs,
         )
 
-    def update_card(
+    async def update_card(
         self,
         card_id: UUID,
         label: str | None = None,
         categories: list[EnumMerchantCategory] | Literal["null"] | None = None,
         single_limit_amount: float | Literal["null"] | None = None,
         single_limit_currency: str | Literal["null"] | None = None,
         day_limit_amount: float | Literal["null"] | None = None,
@@ -526,22 +526,22 @@
 
         body = endpoint.Body(
             label=label,
             categories=categories,
             spending_limits=spending_limits,
         )
 
-        return self.client.patch(
+        return await self.client.patch(
             path=path,
             response_model=endpoint.Response,
             body=body,
             **kwargs,
         )
 
-    def delete_card(
+    async def delete_card(
         self,
         card_id: UUID,
         **kwargs,
     ) -> dict | TerminateCard.Response:
         """
         Terminate a specific card, based on its ID.
 
@@ -560,15 +560,15 @@
             An empty dictionary.
         """
         self.__check_sandbox()
         endpoint = TerminateCard
         path = endpoint.ROUTE.format(card_id=card_id)
         params = endpoint.Params()
 
-        return self.client.delete(
+        return await self.client.delete(
             path=path,
             response_model=endpoint.Response,
             params=params,
             **kwargs,
         )
 
     def __process_limit_model(
@@ -591,14 +591,14 @@
 
     def __check_sandbox(self):
         """
         Check if the sandbox is enabled.
 
         Raises
         ------
-        InvalidEnvironmentException
+        PyRevolutInvalidEnvironment
             If the sandbox is enabled.
         """
         if self.client.sandbox:
-            raise InvalidEnvironmentException(
+            raise PyRevolutInvalidEnvironment(
                 "This feature is not available in Sandbox."
             )
```

### Comparing `pyrevolut-0.7.0/pyrevolut/api/cards/get/retrieve_list_of_cards.py` & `pyrevolut-0.7.1/pyrevolut/api/cards/get/retrieve_list_of_cards.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/cards/get/retrieve_sensitive_card_details.py` & `pyrevolut-0.7.1/pyrevolut/api/cards/get/retrieve_sensitive_card_details.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/cards/patch/update_card_details.py` & `pyrevolut-0.7.1/pyrevolut/api/cards/patch/update_card_details.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/cards/post/create_card.py` & `pyrevolut-0.7.1/pyrevolut/api/cards/post/create_card.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/cards/post/freeze_card.py` & `pyrevolut-0.7.1/pyrevolut/api/cards/post/freeze_card.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/cards/post/unfreeze_card.py` & `pyrevolut-0.7.1/pyrevolut/api/cards/post/unfreeze_card.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/cards/resources/card.py` & `pyrevolut-0.7.1/pyrevolut/api/cards/resources/card.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/common/endpoint.py` & `pyrevolut-0.7.1/pyrevolut/api/common/endpoint.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/common/enums/__init__.py` & `pyrevolut-0.7.1/pyrevolut/api/common/enums/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,13 @@
 from .payment_scheme import EnumPaymentScheme
 from .payout_link_cancellation_reason import EnumPayoutLinkCancellationReason
 from .payout_link_payment_method import EnumPayoutLinkPaymentMethod
 from .payout_link_state import EnumPayoutLinkState
 from .profile_state import EnumProfileState
 from .profile_type import EnumProfileType
 from .recipient_charges import EnumRecipientCharges
-from .simulate_transfer_state_action import EnumSimulateTransferStateAction
 from .team_member_state import EnumTeamMemberState
 from .time_unit import EnumTimeUnit
 from .transaction_type import EnumTransactionType
 from .transaction_state import EnumTransactionState
 from .transfer_reason_code import EnumTransferReasonCode
 from .webhook_event import EnumWebhookEvent
```

### Comparing `pyrevolut-0.7.0/pyrevolut/api/common/enums/account_name_match_code.py` & `pyrevolut-0.7.1/pyrevolut/api/common/enums/account_name_match_code.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/common/enums/account_name_match_reason_code.py` & `pyrevolut-0.7.1/pyrevolut/api/common/enums/account_name_match_reason_code.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/common/enums/merchant_category.py` & `pyrevolut-0.7.1/pyrevolut/api/common/enums/merchant_category.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/common/enums/payout_link_state.py` & `pyrevolut-0.7.1/pyrevolut/api/common/enums/payout_link_state.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/common/enums/transaction_state.py` & `pyrevolut-0.7.1/pyrevolut/api/common/enums/transaction_state.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/common/enums/transfer_reason_code.py` & `pyrevolut-0.7.1/pyrevolut/api/common/enums/transfer_reason_code.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/counterparties/__init__.py` & `pyrevolut-0.7.1/pyrevolut/api/counterparties/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/counterparties/endpoint/asynchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/counterparties/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/counterparties/endpoint/synchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/counterparties/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/counterparties/get/retrieve_list_of_counterparties.py` & `pyrevolut-0.7.1/pyrevolut/api/counterparties/get/retrieve_list_of_counterparties.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/counterparties/post/create_counterparty.py` & `pyrevolut-0.7.1/pyrevolut/api/counterparties/post/create_counterparty.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/counterparties/post/validate_account_name.py` & `pyrevolut-0.7.1/pyrevolut/api/counterparties/post/validate_account_name.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/counterparties/resources/counterparty.py` & `pyrevolut-0.7.1/pyrevolut/api/counterparties/resources/counterparty.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/endpoint/asynchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/foreign_exchange/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/endpoint/synchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/foreign_exchange/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/get/get_exchange_rate.py` & `pyrevolut-0.7.1/pyrevolut/api/foreign_exchange/get/get_exchange_rate.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/post/exchange_money.py` & `pyrevolut-0.7.1/pyrevolut/api/foreign_exchange/post/exchange_money.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/foreign_exchange/resources/foreign_exchange.py` & `pyrevolut-0.7.1/pyrevolut/api/foreign_exchange/resources/foreign_exchange.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/payment_drafts/endpoint/asynchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/payment_drafts/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/payment_drafts/endpoint/synchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/payment_drafts/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/payment_drafts/get/retrieve_all_payment_drafts.py` & `pyrevolut-0.7.1/pyrevolut/api/payment_drafts/get/retrieve_all_payment_drafts.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/payment_drafts/get/retrieve_payment_draft.py` & `pyrevolut-0.7.1/pyrevolut/api/payment_drafts/get/retrieve_payment_draft.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/payment_drafts/post/create_payment_draft.py` & `pyrevolut-0.7.1/pyrevolut/api/payment_drafts/post/create_payment_draft.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/payout_links/endpoint/asynchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/payout_links/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/payout_links/endpoint/synchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/payout_links/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/payout_links/get/retrieve_list_of_payout_links.py` & `pyrevolut-0.7.1/pyrevolut/api/payout_links/get/retrieve_list_of_payout_links.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/payout_links/get/retrieve_payout_link.py` & `pyrevolut-0.7.1/pyrevolut/api/payout_links/get/retrieve_payout_link.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/payout_links/post/cancel_payout_link.py` & `pyrevolut-0.7.1/pyrevolut/api/payout_links/post/cancel_payout_link.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/payout_links/post/create_payout_link.py` & `pyrevolut-0.7.1/pyrevolut/api/payout_links/post/create_payout_link.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/payout_links/resources/payout_link.py` & `pyrevolut-0.7.1/pyrevolut/api/payout_links/resources/payout_link.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/simulations/endpoint/asynchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/simulations/endpoint/asynchronous.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from uuid import UUID
+from typing import Literal
 
-from pyrevolut.exceptions import InvalidEnvironmentException
+from pyrevolut.exceptions import PyRevolutInvalidEnvironment
 from pyrevolut.api.common import (
     BaseEndpointAsync,
     EnumTransactionState,
-    EnumSimulateTransferStateAction,
 )
 from pyrevolut.api.simulations.post import (
     SimulateAccountTopup,
     SimulateTransferStateUpdate,
 )
 
 
@@ -88,30 +88,30 @@
             body=body,
             **kwargs,
         )
 
     async def simulate_transfer_state_update(
         self,
         transfer_id: UUID,
-        action: EnumSimulateTransferStateAction,
+        action: Literal["complete", "revert", "decline", "fail"],
         **kwargs,
     ) -> dict | SimulateTransferStateUpdate.Response:
         """
         Simulate a transfer state change in the Sandbox environment.
 
         For example, after you make a transfer in Sandbox, you can change its
         state to completed.
 
         The resulting state is final and cannot be changed.
 
         Parameters
         ----------
         transfer_id : UUID
             The ID of the transfer whose state you want to update.
-        action : EnumSimulateTransferStateAction
+        action : Literal["complete", "revert", "decline", "fail"]
             The action you want to perform on the transfer. Possible values:
 
                 complete:
                     Simulate a completed transfer.
                 revert:
                     Simulate a reverted transfer.
                 decline:
@@ -121,14 +121,15 @@
 
         Returns
         -------
         dict | SimulateTransferStateUpdate.Response
             The updated transfer information.
         """
         self.__check_sandbox()
+        assert action in ["complete", "revert", "decline", "fail"], "Invalid action"
         endpoint = SimulateTransferStateUpdate
         path = endpoint.ROUTE.format(transfer_id=transfer_id, action=action)
         body = endpoint.Body()
 
         return await self.client.post(
             path=path,
             response_model=endpoint.Response,
@@ -138,14 +139,14 @@
 
     def __check_sandbox(self):
         """
         Check if the sandbox is enabled.
 
         Raises
         ------
-        InvalidEnvironmentException
+        PyRevolutInvalidEnvironment
             If the sandbox is enabled.
         """
         if not self.client.sandbox:
-            raise InvalidEnvironmentException(
+            raise PyRevolutInvalidEnvironment(
                 "This feature is only available in the Sandbox."
             )
```

### Comparing `pyrevolut-0.7.0/pyrevolut/api/simulations/endpoint/synchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/simulations/endpoint/synchronous.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from uuid import UUID
+from typing import Literal
 
-from pyrevolut.exceptions import InvalidEnvironmentException
+from pyrevolut.exceptions import PyRevolutInvalidEnvironment
 from pyrevolut.api.common import (
     BaseEndpointSync,
     EnumTransactionState,
-    EnumSimulateTransferStateAction,
 )
 from pyrevolut.api.simulations.post import (
     SimulateAccountTopup,
     SimulateTransferStateUpdate,
 )
 
 
@@ -88,30 +88,30 @@
             body=body,
             **kwargs,
         )
 
     def simulate_transfer_state_update(
         self,
         transfer_id: UUID,
-        action: EnumSimulateTransferStateAction,
+        action: Literal["complete", "revert", "decline", "fail"],
         **kwargs,
     ) -> dict | SimulateTransferStateUpdate.Response:
         """
         Simulate a transfer state change in the Sandbox environment.
 
         For example, after you make a transfer in Sandbox, you can change its
         state to completed.
 
         The resulting state is final and cannot be changed.
 
         Parameters
         ----------
         transfer_id : UUID
             The ID of the transfer whose state you want to update.
-        action : EnumSimulateTransferStateAction
+        action : Literal["complete", "revert", "decline", "fail"]
             The action you want to perform on the transfer. Possible values:
 
                 complete:
                     Simulate a completed transfer.
                 revert:
                     Simulate a reverted transfer.
                 decline:
@@ -121,14 +121,15 @@
 
         Returns
         -------
         dict | SimulateTransferStateUpdate.Response
             The updated transfer information.
         """
         self.__check_sandbox()
+        assert action in ["complete", "revert", "decline", "fail"], "Invalid action"
         endpoint = SimulateTransferStateUpdate
         path = endpoint.ROUTE.format(transfer_id=transfer_id, action=action)
         body = endpoint.Body()
 
         return self.client.post(
             path=path,
             response_model=endpoint.Response,
@@ -138,14 +139,14 @@
 
     def __check_sandbox(self):
         """
         Check if the sandbox is enabled.
 
         Raises
         ------
-        InvalidEnvironmentException
+        PyRevolutInvalidEnvironment
             If the sandbox is enabled.
         """
         if not self.client.sandbox:
-            raise InvalidEnvironmentException(
+            raise PyRevolutInvalidEnvironment(
                 "This feature is only available in the Sandbox."
             )
```

### Comparing `pyrevolut-0.7.0/pyrevolut/api/simulations/post/simulate_account_topup.py` & `pyrevolut-0.7.1/pyrevolut/api/simulations/post/simulate_account_topup.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/simulations/post/simulate_transfer_state_update.py` & `pyrevolut-0.7.1/pyrevolut/api/simulations/post/simulate_transfer_state_update.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/team_members/endpoint/asynchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/team_members/endpoint/asynchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from uuid import UUID
 from datetime import datetime
 
-from pyrevolut.exceptions import InvalidEnvironmentException
+from pyrevolut.exceptions import PyRevolutInvalidEnvironment
 from pyrevolut.utils.datetime import DateTime
 from pyrevolut.api.common import BaseEndpointAsync
 from pyrevolut.api.team_members.get import RetrieveListOfTeamMembers, RetrieveTeamRoles
 from pyrevolut.api.team_members.post import InviteTeamMember
 
 
 class EndpointTeamMembersAsync(BaseEndpointAsync):
@@ -166,14 +166,14 @@
 
     def __check_sandbox(self):
         """
         Check if the sandbox is enabled.
 
         Raises
         ------
-        InvalidEnvironmentException
+        PyRevolutInvalidEnvironment
             If the sandbox is enabled.
         """
         if self.client.sandbox:
-            raise InvalidEnvironmentException(
+            raise PyRevolutInvalidEnvironment(
                 "This feature is not available in Sandbox."
             )
```

### Comparing `pyrevolut-0.7.0/pyrevolut/api/team_members/endpoint/synchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/team_members/endpoint/synchronous.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from uuid import UUID
 from datetime import datetime
 
-from pyrevolut.exceptions import InvalidEnvironmentException
+from pyrevolut.exceptions import PyRevolutInvalidEnvironment
 from pyrevolut.utils.datetime import DateTime
 from pyrevolut.api.common import BaseEndpointSync
 from pyrevolut.api.team_members.get import RetrieveListOfTeamMembers, RetrieveTeamRoles
 from pyrevolut.api.team_members.post import InviteTeamMember
 
 
 class EndpointTeamMembersSync(BaseEndpointSync):
@@ -166,14 +166,14 @@
 
     def __check_sandbox(self):
         """
         Check if the sandbox is enabled.
 
         Raises
         ------
-        InvalidEnvironmentException
+        PyRevolutInvalidEnvironment
             If the sandbox is enabled.
         """
         if self.client.sandbox:
-            raise InvalidEnvironmentException(
+            raise PyRevolutInvalidEnvironment(
                 "This feature is not available in Sandbox."
             )
```

### Comparing `pyrevolut-0.7.0/pyrevolut/api/team_members/get/retrieve_list_of_team_members.py` & `pyrevolut-0.7.1/pyrevolut/api/team_members/get/retrieve_list_of_team_members.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/team_members/get/retrieve_team_roles.py` & `pyrevolut-0.7.1/pyrevolut/api/team_members/get/retrieve_team_roles.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/team_members/post/invite_team_member.py` & `pyrevolut-0.7.1/pyrevolut/api/team_members/post/invite_team_member.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/transactions/endpoint/asynchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/transactions/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/transactions/endpoint/synchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/transactions/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/transactions/get/retrieve_list_of_transactions.py` & `pyrevolut-0.7.1/pyrevolut/api/transactions/get/retrieve_list_of_transactions.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/transactions/get/retrieve_transaction.py` & `pyrevolut-0.7.1/pyrevolut/api/transactions/get/retrieve_transaction.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/transactions/resources/transaction.py` & `pyrevolut-0.7.1/pyrevolut/api/transactions/resources/transaction.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/transfers/endpoint/asynchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/transfers/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/transfers/endpoint/synchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/transfers/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/transfers/get/get_transfer_reasons.py` & `pyrevolut-0.7.1/pyrevolut/api/transfers/get/get_transfer_reasons.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/transfers/post/create_transfer_to_another_account.py` & `pyrevolut-0.7.1/pyrevolut/api/transfers/post/create_transfer_to_another_account.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/transfers/post/move_money_between_accounts.py` & `pyrevolut-0.7.1/pyrevolut/api/transfers/post/move_money_between_accounts.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/transfers/resources/transfer.py` & `pyrevolut-0.7.1/pyrevolut/api/transfers/resources/transfer.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/webhooks/__init__.py` & `pyrevolut-0.7.1/pyrevolut/api/webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/webhooks/endpoint/asynchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/webhooks/endpoint/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/webhooks/endpoint/synchronous.py` & `pyrevolut-0.7.1/pyrevolut/api/webhooks/endpoint/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/webhooks/get/retrieve_list_of_failed_webhooks.py` & `pyrevolut-0.7.1/pyrevolut/api/webhooks/get/retrieve_list_of_failed_webhooks.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/webhooks/get/retrieve_webhook.py` & `pyrevolut-0.7.1/pyrevolut/api/webhooks/get/retrieve_webhook.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/webhooks/patch/update_webhook.py` & `pyrevolut-0.7.1/pyrevolut/api/webhooks/patch/update_webhook.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/webhooks/post/create_webhook.py` & `pyrevolut-0.7.1/pyrevolut/api/webhooks/post/create_webhook.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/webhooks/post/rotate_webhook_secret.py` & `pyrevolut-0.7.1/pyrevolut/api/webhooks/post/rotate_webhook_secret.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/payout_link_created.py` & `pyrevolut-0.7.1/pyrevolut/api/webhooks/resources/payout_link_created.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/payout_link_state_changed.py` & `pyrevolut-0.7.1/pyrevolut/api/webhooks/resources/payout_link_state_changed.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/transaction_created.py` & `pyrevolut-0.7.1/pyrevolut/api/webhooks/resources/transaction_created.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/transaction_state_changed.py` & `pyrevolut-0.7.1/pyrevolut/api/webhooks/resources/transaction_state_changed.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/webhook.py` & `pyrevolut-0.7.1/pyrevolut/api/webhooks/resources/webhook.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/api/webhooks/resources/webhook_payload.py` & `pyrevolut-0.7.1/pyrevolut/api/webhooks/resources/webhook_payload.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/cli/main.py` & `pyrevolut-0.7.1/pyrevolut/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/client/asynchronous.py` & `pyrevolut-0.7.1/pyrevolut/client/asynchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/client/base.py` & `pyrevolut-0.7.1/pyrevolut/client/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 from typing import Type, TypeVar, Literal, Annotated
 import logging
 import json
 
 from pydantic import BaseModel, Field
 import pendulum
 
-from httpx import AsyncClient
-from httpx import Client as SyncClient
-from httpx import Request, Response
+from httpx import (
+    AsyncClient,
+    Client as SyncClient,
+    Request,
+    Response,
+    HTTPError,
+    TimeoutException,
+    NetworkError,
+)
 
 from pyrevolut.utils.auth import (
     ModelCreds,
     refresh_access_token,
     save_creds,
     load_creds,
 )
 from pyrevolut.exceptions import (
-    PyRevolutAPIException,
-    BadRequestException,
-    InternalRevolutError,
+    PyRevolutBaseException,
+    PyRevolutTimeoutError,
+    PyRevolutNetworkError,
+    PyRevolutBadRequest,
+    PyRevolutUnauthorized,
+    PyRevolutForbidden,
+    PyRevolutNotFound,
+    PyRevolutMethodNotAllowed,
+    PyRevolutNotAcceptable,
+    PyRevolutConflict,
+    PyRevolutTooManyRequests,
+    PyRevolutInternalServerError,
+    PyRevolutServerUnavailable,
 )
 
 
 BM = TypeVar("BM", bound=Type[BaseModel])
 D = TypeVar("D", dict, list)  # TypeVar for dictionary or list
 
 
@@ -158,19 +174,42 @@
 
         # Log the response
         self.log_response(response=response)
 
         # Check for error response
         if response.is_error:
             if error_response == "raise":
-                if response.status_code == 400:
-                    raise BadRequestException(response.text)
-                elif response.status_code // 100 == 5:
-                    raise InternalRevolutError(response.text)
-                raise PyRevolutAPIException(response.text)
+                try:
+                    response.raise_for_status()
+                except TimeoutException as exc:
+                    raise PyRevolutTimeoutError() from exc
+                except NetworkError as exc:
+                    raise PyRevolutNetworkError() from exc
+                except HTTPError as exc:
+                    if response.status_code == 400:
+                        raise PyRevolutBadRequest() from exc
+                    elif response.status_code == 401:
+                        raise PyRevolutUnauthorized() from exc
+                    elif response.status_code == 403:
+                        raise PyRevolutForbidden() from exc
+                    elif response.status_code == 404:
+                        raise PyRevolutNotFound() from exc
+                    elif response.status_code == 405:
+                        raise PyRevolutMethodNotAllowed() from exc
+                    elif response.status_code == 406:
+                        raise PyRevolutNotAcceptable() from exc
+                    elif response.status_code == 409:
+                        raise PyRevolutConflict() from exc
+                    elif response.status_code == 429:
+                        raise PyRevolutTooManyRequests() from exc
+                    elif response.status_code == 500:
+                        raise PyRevolutInternalServerError() from exc
+                    elif response.status_code == 503:
+                        raise PyRevolutServerUnavailable() from exc
+                    raise PyRevolutBaseException() from exc
             elif error_response == "raw":
                 return response.json()
             elif error_response == "dict":
                 return ModelError(**response.json()).model_dump()
             elif error_response == "model":
                 return ModelError(**response.json())
             else:
```

### Comparing `pyrevolut-0.7.0/pyrevolut/client/synchronous.py` & `pyrevolut-0.7.1/pyrevolut/client/synchronous.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/utils/auth/auth_manual.py` & `pyrevolut-0.7.1/pyrevolut/utils/auth/auth_manual.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/utils/auth/create_client_assert_jwt.py` & `pyrevolut-0.7.1/pyrevolut/utils/auth/create_client_assert_jwt.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/utils/auth/creds.py` & `pyrevolut-0.7.1/pyrevolut/utils/auth/creds.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/utils/auth/enum_auth_scope.py` & `pyrevolut-0.7.1/pyrevolut/utils/auth/enum_auth_scope.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/utils/auth/gen_public_private_cert.py` & `pyrevolut-0.7.1/pyrevolut/utils/auth/gen_public_private_cert.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/utils/auth/get_auth_tokens.py` & `pyrevolut-0.7.1/pyrevolut/utils/auth/get_auth_tokens.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/utils/auth/refresh_access_token.py` & `pyrevolut-0.7.1/pyrevolut/utils/auth/refresh_access_token.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/utils/date.py` & `pyrevolut-0.7.1/pyrevolut/utils/date.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/pyrevolut/utils/datetime.py` & `pyrevolut-0.7.1/pyrevolut/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `pyrevolut-0.7.0/PKG-INFO` & `pyrevolut-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrevolut
-Version: 0.7.0
+Version: 0.7.1
 Summary: An unofficial Python API Wrapper for the Revolut Business API
 Home-page: https://github.com/Trevypants/pyrevolut
 License: MIT
 Author: Trevor Visser
 Author-email: trevor.visser@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -205,14 +205,15 @@
   - [x] Create a new webhook
   - [x] Retrieve a list of webhooks
   - [x] Retrieve a webhook
   - [x] Update a webhook
   - [x] Delete a webhook
   - [x] Rotate a webhook signing secret
   - [x] Retrieve a list of failed webhook events
+  - [x] Verify a webhook signature
 
 ## **Contributing**
 
 In order to facilitate a streamlined development process, we have a few guidelines that we would like to follow. Please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file for more information.
 
 ## **License**
```

