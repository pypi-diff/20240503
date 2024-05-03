# Comparing `tmp/monnifyease-0.1.0.tar.gz` & `tmp/monnifyease-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monnifyease-0.1.0.tar", max compression
+gzip compressed data, was "monnifyease-0.2.0.tar", max compression
```

## Comparing `monnifyease-0.1.0.tar` & `monnifyease-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
--rwxr-xr-x   0        0        0     1090 2024-02-21 14:06:29.101210 monnifyease-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     4289 2024-04-29 22:37:54.703590 monnifyease-0.1.0/README.md
--rwxr-xr-x   0        0        0      313 2024-04-30 01:20:29.795944 monnifyease-0.1.0/monnifyease/__init__.py
--rwxr-xr-x   0        0        0      131 2024-04-24 10:25:13.568857 monnifyease-0.1.0/monnifyease/apis/__init__.py
--rwxr-xr-x   0        0        0      140 2024-04-24 10:25:13.568857 monnifyease-0.1.0/monnifyease/apis/sync_apis/__init__.py
--rwxr-xr-x   0        0        0     9494 2024-04-30 01:20:29.796944 monnifyease-0.1.0/monnifyease/apis/sync_apis/customer_reserved_account.py
--rwxr-xr-x   0        0        0     8409 2024-04-30 01:20:29.797944 monnifyease-0.1.0/monnifyease/apis/sync_apis/transactions.py
--rwxr-xr-x   0        0        0      556 2024-04-29 22:38:52.786514 monnifyease-0.1.0/monnifyease/core/__init__.py
--rwxr-xr-x   0        0        0     1673 2024-04-29 22:38:52.787514 monnifyease-0.1.0/monnifyease/core/_api_access_header.py
--rwxr-xr-x   0        0        0     3841 2024-04-30 00:11:43.114088 monnifyease-0.1.0/monnifyease/core/_api_base.py
--rwxr-xr-x   0        0        0     2738 2024-04-29 22:38:52.789514 monnifyease-0.1.0/monnifyease/core/_api_base_envar.py
--rwxr-xr-x   0        0        0     3181 2024-04-29 22:38:52.791513 monnifyease-0.1.0/monnifyease/core/_api_base_request.py
--rwxr-xr-x   0        0        0     1692 2024-04-29 22:38:52.792513 monnifyease-0.1.0/monnifyease/core/_api_client_requests.py
--rwxr-xr-x   0        0        0     1137 2024-04-24 10:25:13.575858 monnifyease-0.1.0/monnifyease/core/_api_client_response.py
--rwxr-xr-x   0        0        0     1062 2024-04-27 17:20:05.476595 monnifyease-0.1.0/monnifyease/core/_api_errors.py
--rwxr-xr-x   0        0        0      149 2024-04-30 01:20:29.799943 monnifyease-0.1.0/monnifyease/helpers/__init__.py
--rwxr-xr-x   0        0        0      370 2024-04-30 01:20:29.800943 monnifyease-0.1.0/monnifyease/helpers/tool_kit.py
--rwxr-xr-x   0        0        0      519 2024-04-30 00:22:18.853114 monnifyease-0.1.0/monnifyease/monnify.py
--rwxr-xr-x   0        0        0      117 2024-04-29 22:38:52.796515 monnifyease-0.1.0/monnifyease/utils/__init__.py
--rwxr-xr-x   0        0        0     1171 2024-04-29 22:38:52.797515 monnifyease-0.1.0/monnifyease/utils/convert_to_strings.py
--rwxr-xr-x   0        0        0      387 2024-04-29 22:38:52.798515 monnifyease-0.1.0/monnifyease/utils/join_url.py
--rwxr-xr-x   0        0        0     1885 2024-04-30 01:27:54.599411 monnifyease-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 monnifyease-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-03 02:22:35.392252 monnifyease-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4126 2024-05-03 02:22:35.392252 monnifyease-0.2.0/README.md
+-rw-r--r--   0        0        0      298 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/apis/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/apis/sync_apis/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/apis/sync_apis/banks.py
+-rw-r--r--   0        0        0     9222 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/apis/sync_apis/customer_reserved_account.py
+-rw-r--r--   0        0        0     1346 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/apis/sync_apis/settlements.py
+-rw-r--r--   0        0        0     2475 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/apis/sync_apis/subaccounts.py
+-rw-r--r--   0        0        0     8184 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/apis/sync_apis/transactions.py
+-rw-r--r--   0        0        0     2983 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/apis/sync_apis/wallet.py
+-rw-r--r--   0        0        0      547 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/core/__init__.py
+-rw-r--r--   0        0        0     1624 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/core/_api_access_header.py
+-rw-r--r--   0        0        0     3735 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/core/_api_base.py
+-rw-r--r--   0        0        0     2646 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/core/_api_base_envar.py
+-rw-r--r--   0        0        0     3093 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/core/_api_base_request.py
+-rw-r--r--   0        0        0     1633 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/core/_api_client_requests.py
+-rw-r--r--   0        0        0     1094 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/core/_api_client_response.py
+-rw-r--r--   0        0        0     1021 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/core/_api_errors.py
+-rw-r--r--   0        0        0      143 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/helpers/__init__.py
+-rw-r--r--   0        0        0      351 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/helpers/tool_kit.py
+-rw-r--r--   0        0        0      738 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/monnify.py
+-rw-r--r--   0        0        0      115 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/utils/__init__.py
+-rw-r--r--   0        0        0     1135 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/utils/convert_to_strings.py
+-rw-r--r--   0        0        0      443 2024-05-03 02:22:35.392252 monnifyease-0.2.0/monnifyease/utils/join_url.py
+-rw-r--r--   0        0        0     2125 2024-05-03 02:22:36.132246 monnifyease-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5450 1970-01-01 00:00:00.000000 monnifyease-0.2.0/PKG-INFO
```

### Comparing `monnifyease-0.1.0/LICENSE` & `monnifyease-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 PETER MBACHU
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 PETER MBACHU
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `monnifyease-0.1.0/README.md` & `monnifyease-0.2.0/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-# MonnifyEase Library
-
-------------
-
-![Python Versions](https://img.shields.io/badge/python-3.9|3.10|3.11|3.12-blue)
-
-MonnifyEase simplifies interacting with the Monnify payment gateway in Python. 
-It offers wrappers for various functionalities, streamlining payment processing 
-for your projects.
-
-Monnify (owned by **Moniepoint**) is a Nigerian payment gateway that allows 
-businesses to accept payments easily and securely.
-
-
-> 📝: Read more on Monnify api documentation: [Monnify API DOCUMENTATION](https://developers.monnify.com/api/)
-
-> 📝: Read more on monnifyease api documentation: [MonnifyEase DOCUMENTATION](https://monnifyease.readthedocs.io/en/latest/)
-
-
-## Getting Started
-
-You should create a Monnify account to generate: 
-
-1. **Monnify Secret Key**
-2. **Monnify Api Key**
-3. **Monnify Merchant Code**
-4. **Monnify Base URL**
-
-You can see this in the *developer page >> API keys and Contracts section*.
-
-> ⚠️: **Warning:** Do not expose your secret key, api key, merchant code, base url or 
->commit your any to git, or use them in client-side code.
-
-> 💡: **Take Note:**  The Monnify SDK is to be used from your front-end when integrating using Monnify.
-
-> ✅: **Good**: Set your secret key, api key, base url and merchant code in environment variables as seen: 
-> 1. *MONNIFY_SECRET_KEY=your-secret-key*
-> 2. *MONNIFY_API_KEY=your-api-key*
-> 3. *MONNIFY_SECRET_KEY=your-secret-key*
-> 4. *MONNIFY_MERCHANT_CODE=your-merchant-code*
-
-
-## Create a Virtual Environment
-
-1. For Windows:
-
-    * Create virtual environment
-
-        ```
-            py -m venv <environment_name>
-       ```
-    * Activate the virtual environment
-
-        ```
-            <environment_name>\Scripts\activate
-       ```
-
-2. For Unix/macOS
-
-    * Create virtual environment
-
-        ```
-            python3 -m venv <environment_name>
-       ```
-    * Activate the virtual environment
-
-        ```
-            <environment_name>/bin/activate
-       ```
-
-----------------------------------------------------------------------
-
-## Install monnifyease library:
-
-
-* #### Install monnifyease using pip.
-
-> pip install monnifyease
-
-* #### Install monnifyease using pipx.
-
-> pipx install monnifyease
-
-* #### Install monnifyease using poetry.
-
-> poetry add monnifyease
-
-
-## If you want to download the sdist packages directly:
-
-Download the wheel distribution file and install using pip
-
->  pip install monnifyease-0.i.0-py3-none-any.whl 
-
-Download the source distribution file, and install using pip
-
-> pip install monnifyease-0.i.0.tar.gz 
-
-
-## To get a development version of monnifyease
-
-Clone from the ``dev`` branch GitHub repository, unzip and install:
-
-> git clone -b dev https://github.com/cla-bit/MonnifyEase.git
-
-> cd monnifyease
-
-> pip install monnifyease
-
-----------------------------------------------------------------------
-
-## API usage
-
--------------------------------------------------------
-
-### Making a Transaction [Synchronous]
-
-If after setting your secret key in environment variables, for a synchronous transaction process 
-all you need to do is use the transaction API to make a transaction. 
-
-To create a transaction or initialize a transaction:
-
-* import the Monnify API wrapper.
-
-```python
-
-from monnifyease import Monnify, Currency, MERCHANT_CODE
-
-client = Monnify()
-
-create_transaction = client.transactions.initialize_transaction(
-    amount=1000.00,
-    customer_name="Test Customer",
-    customer_email="test@gmal.com",
-    payment_reference="test123prod",
-    payment_description="Testing payment",
-    currency=Currency.NGN.value,
-    merchant_contract_code=MERCHANT_CODE,
-   # add other parameters here
-)
-
-print(f"Transaction Created: {create_transaction}")
-
-```
-
-> ✅: **Good**: You can check your Monnify account, go to the Transaction page, and you will see the transaction just created.
-
-
-# Other Tools
-Similar to calling the Monnify, you can also call other tools to make your work easy. For example:
-
-* ### Currency Type
-```python
-
-from monnifyease import Currency
-
-val1 = Currency.NGN.value
-print(val1)
-
-```
-> "NGN"
-
-See documentation for more: https://monnifyease.readthedocs.io/en/latest/
+# MonnifyEase Library
+
+------------
+
+![Python Versions](https://img.shields.io/badge/python-3.9|3.10|3.11|3.12-blue)
+
+MonnifyEase simplifies interacting with the Monnify payment gateway in Python. 
+It offers wrappers for various functionalities, streamlining payment processing 
+for your projects.
+
+Monnify (owned by **Moniepoint**) is a Nigerian payment gateway that allows 
+businesses to accept payments easily and securely.
+
+
+> 📝: Read more on Monnify api documentation: [Monnify API DOCUMENTATION](https://developers.monnify.com/api/)
+
+> 📝: Read more on monnifyease api documentation: [MonnifyEase DOCUMENTATION](https://monnifyease.readthedocs.io/en/latest/)
+
+
+## Getting Started
+
+You should create a Monnify account to generate: 
+
+1. **Monnify Secret Key**
+2. **Monnify Api Key**
+3. **Monnify Merchant Code**
+4. **Monnify Base URL**
+
+You can see this in the *developer page >> API keys and Contracts section*.
+
+> ⚠️: **Warning:** Do not expose your secret key, api key, merchant code, base url or 
+>commit your any to git, or use them in client-side code.
+
+> 💡: **Take Note:**  The Monnify SDK is to be used from your front-end when integrating using Monnify.
+
+> ✅: **Good**: Set your secret key, api key, base url and merchant code in environment variables as seen: 
+> 1. *MONNIFY_SECRET_KEY=your-secret-key*
+> 2. *MONNIFY_API_KEY=your-api-key*
+> 3. *MONNIFY_SECRET_KEY=your-secret-key*
+> 4. *MONNIFY_MERCHANT_CODE=your-merchant-code*
+
+
+## Create a Virtual Environment
+
+1. For Windows:
+
+    * Create virtual environment
+
+        ```
+            py -m venv <environment_name>
+       ```
+    * Activate the virtual environment
+
+        ```
+            <environment_name>\Scripts\activate
+       ```
+
+2. For Unix/macOS
+
+    * Create virtual environment
+
+        ```
+            python3 -m venv <environment_name>
+       ```
+    * Activate the virtual environment
+
+        ```
+            <environment_name>/bin/activate
+       ```
+
+----------------------------------------------------------------------
+
+## Install monnifyease library:
+
+
+* #### Install monnifyease using pip.
+
+> pip install monnifyease
+
+* #### Install monnifyease using pipx.
+
+> pipx install monnifyease
+
+* #### Install monnifyease using poetry.
+
+> poetry add monnifyease
+
+
+## If you want to download the sdist packages directly:
+
+Download the wheel distribution file and install using pip
+
+>  pip install monnifyease-0.i.0-py3-none-any.whl 
+
+Download the source distribution file, and install using pip
+
+> pip install monnifyease-0.i.0.tar.gz 
+
+
+## To get a development version of monnifyease
+
+Clone from the ``dev`` branch GitHub repository, unzip and install:
+
+> git clone -b dev https://github.com/cla-bit/MonnifyEase.git
+
+> cd monnifyease
+
+> pip install monnifyease
+
+----------------------------------------------------------------------
+
+## API usage
+
+-------------------------------------------------------
+
+### Making a Transaction [Synchronous]
+
+If after setting your secret key in environment variables, for a synchronous transaction process 
+all you need to do is use the transaction API to make a transaction. 
+
+To create a transaction or initialize a transaction:
+
+* import the Monnify API wrapper.
+
+```python
+
+from monnifyease import Monnify, Currency, MERCHANT_CODE
+
+client = Monnify()
+
+create_transaction = client.transactions.initialize_transaction(
+    amount=1000.00,
+    customer_name="Test Customer",
+    customer_email="test@gmal.com",
+    payment_reference="test123prod",
+    payment_description="Testing payment",
+    currency=Currency.NGN.value,
+    merchant_contract_code=MERCHANT_CODE,
+   # add other parameters here
+)
+
+print(f"Transaction Created: {create_transaction}")
+
+```
+
+> ✅: **Good**: You can check your Monnify account, go to the Transaction page, and you will see the transaction just created.
+
+
+# Other Tools
+Similar to calling the Monnify, you can also call other tools to make your work easy. For example:
+
+* ### Currency Type
+```python
+
+from monnifyease import Currency
+
+val1 = Currency.NGN.value
+print(val1)
+
+```
+> "NGN"
+
+See documentation for more: https://monnifyease.readthedocs.io/en/latest/
```

### Comparing `monnifyease-0.1.0/monnifyease/apis/sync_apis/customer_reserved_account.py` & `monnifyease-0.2.0/monnifyease/apis/sync_apis/customer_reserved_account.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,272 +1,272 @@
-""" Wrapper for Monnify Customer Reserved Account API
-The Customer API allows you to create and manage payments on your integration.
-"""
-
-from typing import List, Dict, Any, Optional, Union
-from monnifyease.core import MonnifyResponse, SyncRequestClient
-from monnifyease.helpers.tool_kit import Currency
-
-
-class CustomerReservedAccount(SyncRequestClient):
-    """Monnify Customer Reserved Account API"""
-
-    def create_general_reserve(
-            self,
-            account_reference: str,
-            account_name: str,
-            currency: Currency,
-            merchant_code: str,
-            customer_email: str,
-            customer_name: str,
-            bvn: str,
-            nin: str,
-            income_split_config: Optional[List[Dict[str, Any]]] = None,
-            allow_pay_source: Optional[Dict[str, List[Any]]] = None,
-            restrict_pay_source: Optional[bool] = False,
-            preferred_bank: Optional[Union[List[Any], None]] = None,
-            get_all_banks: Optional[bool] = True,
-    ) -> MonnifyResponse:
-        """
-        Creation of dedicated virtual accounts for your customers (General).
-        Reference: https://developers.monnify.com/api/#create-reserved-accountgeneral
-
-        :param: account_reference
-        :param: account_name
-        :param: currency
-        :param: merchant_code
-        :param: customer_email
-        :param: customer_name
-        :param: bvn
-        :param: nin
-        :param: preferred_bank
-        :param: income_split_config
-        :param: allow_pay_source
-        :param: restrict_pay_source
-        :param: get_all_banks
-
-        :return: The response from the API
-        :rtype: MonnifyResponse object
-        """
-        data = {
-            "accountReference": account_reference,
-            "accountName": account_name,
-            "currencyCode": currency,
-            "contractCode": merchant_code,
-            "customerEmail": customer_email,
-            "customerName": customer_name,
-            "bvn": bvn,
-            "nin": nin,
-            "preferredBanks": preferred_bank,
-            "incomeSplitConfig": income_split_config,
-            "allowedPaymentSource": allow_pay_source,
-            "restrictPaymentSource": restrict_pay_source,
-            "getAllAvailableBanks": get_all_banks,
-        }
-        return self._post("/v2/bank-transfer/reserved-accounts", data=data)
-
-    def create_invoice_reserve(
-            self,
-            account_reference: str,
-            account_name: str,
-            currency: str,
-            merchant_code: str,
-            customer_email: str,
-            customer_name: str,
-            bvn: str,
-            nin: str,
-            reserved_account: Optional[str] = "INVOICE",
-    ) -> MonnifyResponse:
-        """
-         Creation of an invoiced reserved account.
-        Reference: https://developers.monnify.com/api/#create-reserved-accountinvoice
-
-        :param: account_reference
-        :param: account_name
-        :param: currency
-        :param: merchant_code
-        :param: customer_email
-        :param: customer_name
-        :param: reserved_account
-        :param: bvn
-        :param: nin
-
-        :return: The response from the API
-        :rtype: MonnifyResponse object
-        """
-        data = {
-            "accountReference": account_reference,
-            "accountName": account_name,
-            "currencyCode": currency,
-            "contractCode": merchant_code,
-            "customerEmail": customer_email,
-            "customerName": customer_name,
-            "reservedAccountType": reserved_account,
-            "bvn": bvn,
-            "nin": nin,
-        }
-        return self._post("/v1/bank-transfer/reserved-accounts", data=data)
-
-    def get_reserve_detail(self, account_reference: str) -> MonnifyResponse:
-        """
-        Get details of a reserved account.
-        Reference: https://developers.monnify.com/api/#get-reserved-account-details
-
-        :param: account_reference
-
-        :return: The response from the API
-        :rtype: MonnifyResponse object
-        """
-        return self._get(f"/v2/bank-transfer/reserved-accounts/{account_reference}")
-
-    def add_linked_account(
-            self,
-            account_reference: str,
-            preferred_bank: Optional[Union[List[str], None]] = None,
-            get_all_banks: Optional[bool] = True
-    ) -> MonnifyResponse:
-        """
-        Add a linked account to a reserved account.
-        Reference: https://developers.monnify.com/api/#add-linked-accounts
-
-        :param: preferred_bank
-        :param: account_reference
-        :param: get_all_banks
-
-        :return: The response from the API
-        :rtype: MonnifyResponse object
-        """
-        data = {
-            "preferredBank": preferred_bank,
-            "getAllAvailableBanks": get_all_banks,
-        }
-        return self._put(
-            f"v1/bank-transfer/reserved-accounts/add-linked-accounts/{account_reference}",
-            data=data,
-        )
-
-    def update_bvn_reserve(self, account_reference: str, bvn: str) -> MonnifyResponse:
-        """
-        Update the BVN of a reserved account.
-        Reference: https://developers.monnify.com/api/#update-bvn-for-a-reserve-account
-
-        :param: bvn
-        :param: account_reference
-
-        :return: The response from the API
-        :rtype: MonnifyResponse object
-        """
-        data = {
-            "bvn": bvn,
-        }
-        return self._put(
-            f"/v1/bank-transfer/reserved-accounts/update-customer-bvn/{account_reference}",
-            data=data,
-        )
-
-    def allow_payment_source(
-            self,
-            account_reference: str,
-            allow_payment_source: Dict[str, List[Any]],
-            restrict_pay_source: Optional[bool] = True,
-    ) -> MonnifyResponse:
-        """
-        Manages accounts of a reserved account using [BVNs, Account Name or Account Number].
-        Reference: https://developers.monnify.com/api/#allowed-payment-sources
-
-        :param: allow_payment_source
-        :param: account_reference
-        :param: payment_source
-
-        :return: The response from the API
-        :rtype: MonnifyResponse object
-        """
-        data = {
-            "allowedPaymentSource": allow_payment_source,
-            "restrictPaymentSource": restrict_pay_source,
-        }
-        return self._put(
-            f"/v1/bank-transfer/reserved-accounts/update-payment-source-filter/{account_reference}",
-            data=data,
-        )
-
-    def update_split_config_account(
-            self,
-            account_reference: str,
-            objects: List[Dict[str, Any]]
-    ) -> MonnifyResponse:
-        """
-        Updates the split config of a customer reserved account.
-        Reference: https://developers.monnify.com/api/#updating-split-config-for-reserved-account
-
-        :param: account_reference
-        :param: objects contains list of dictionaries.
-        [
-            {
-                "subAccountCode": {{SubaccountCode}},
-                "feePercentage": {{fee in percent}},
-                "splitPercentage": {{split in percent}},
-                "feeBearer": {{true or false}}
-            }
-        ]
-
-        :return: Response from the API
-        :rtype: MonnifyResponse object
-        """
-        return self._put(
-            f"/v1/bank-transfer/reserved-accounts/update-income-split-config/{account_reference}",
-            data=objects,
-        )
-
-    def deallocate_customer(self, account_reference: str) -> MonnifyResponse:
-        """
-        Deallocate/delete already created a reserved account.
-        Reference: https://developers.monnify.com/api/#deallocating-a-reserved-account
-
-        :param: account_reference
-
-        :return: The response from the API
-        :rtype: MonnifyResponse object
-        """
-        return self._delete(f"/v1/bank-transfer/reserved-accounts/{account_reference}")
-
-    def get_reserve_transactions(
-        self, account_reference: str, per_page: Optional[Union[int, None]] = 50, page: Optional[Union[int, None]] = 0
-    ) -> MonnifyResponse:
-        """
-        Get transactions for a reserved account.
-        Reference: https://developers.monnify.com/api/#get-transactions-for-a-reserved-account
-
-        :param: account_reference
-        :param: per_page
-        :param: page
-
-        :return: The response from the API
-        :rtype: MonnifyResponse object
-        """
-        params = {"accountReference": account_reference, "page": page, "size": per_page}
-        return self._get(
-            "/v1/bank-transfer/reserved-accounts/transactions", params=params
-        )
-
-    def update_kyc_info(
-            self, account_reference: str, bvn: str, nin: str
-    ) -> MonnifyResponse:
-        """
-        This links customers' BVN/NIN to their respective reserved accounts.
-        Reference: https://developers.monnify.com/api/#update-kyc-info
-
-        :param: account_reference
-        :param: bvn
-        :param: nin
-
-        :return: The response from the API
-        :rtype: MonnifyResponse object
-        """
-        data = {
-            "bvn": bvn,
-            "nin": nin,
-        }
-        return self._put(
-            f"/v1/bank-transfer/reserved-accounts/{account_reference}/kyc-info",
-            data=data,
-        )
+""" Wrapper for Monnify Customer Reserved Account API
+The Customer API allows you to create and manage payments on your integration.
+"""
+
+from typing import List, Dict, Any, Optional, Union
+from monnifyease.core import MonnifyResponse, SyncRequestClient
+from monnifyease.helpers.tool_kit import Currency
+
+
+class CustomerReservedAccount(SyncRequestClient):
+    """Monnify Customer Reserved Account API"""
+
+    def create_general_reserve(
+            self,
+            account_reference: str,
+            account_name: str,
+            currency: Currency,
+            merchant_code: str,
+            customer_email: str,
+            customer_name: str,
+            bvn: str,
+            nin: str,
+            income_split_config: Optional[List[Dict[str, Any]]] = None,
+            allow_pay_source: Optional[Dict[str, List[Any]]] = None,
+            restrict_pay_source: Optional[bool] = False,
+            preferred_bank: Optional[Union[List[Any], None]] = None,
+            get_all_banks: Optional[bool] = True,
+    ) -> MonnifyResponse:
+        """
+        Creation of dedicated virtual accounts for your customers (General).
+        Reference: https://developers.monnify.com/api/#create-reserved-accountgeneral
+
+        :param: account_reference
+        :param: account_name
+        :param: currency
+        :param: merchant_code
+        :param: customer_email
+        :param: customer_name
+        :param: bvn
+        :param: nin
+        :param: preferred_bank
+        :param: income_split_config
+        :param: allow_pay_source
+        :param: restrict_pay_source
+        :param: get_all_banks
+
+        :return: The response from the API
+        :rtype: MonnifyResponse object
+        """
+        data = {
+            "accountReference": account_reference,
+            "accountName": account_name,
+            "currencyCode": currency,
+            "contractCode": merchant_code,
+            "customerEmail": customer_email,
+            "customerName": customer_name,
+            "bvn": bvn,
+            "nin": nin,
+            "preferredBanks": preferred_bank,
+            "incomeSplitConfig": income_split_config,
+            "allowedPaymentSource": allow_pay_source,
+            "restrictPaymentSource": restrict_pay_source,
+            "getAllAvailableBanks": get_all_banks,
+        }
+        return self._post("/v2/bank-transfer/reserved-accounts", data=data)
+
+    def create_invoice_reserve(
+            self,
+            account_reference: str,
+            account_name: str,
+            currency: str,
+            merchant_code: str,
+            customer_email: str,
+            customer_name: str,
+            bvn: str,
+            nin: str,
+            reserved_account: Optional[str] = "INVOICE",
+    ) -> MonnifyResponse:
+        """
+         Creation of an invoiced reserved account.
+        Reference: https://developers.monnify.com/api/#create-reserved-accountinvoice
+
+        :param: account_reference
+        :param: account_name
+        :param: currency
+        :param: merchant_code
+        :param: customer_email
+        :param: customer_name
+        :param: reserved_account
+        :param: bvn
+        :param: nin
+
+        :return: The response from the API
+        :rtype: MonnifyResponse object
+        """
+        data = {
+            "accountReference": account_reference,
+            "accountName": account_name,
+            "currencyCode": currency,
+            "contractCode": merchant_code,
+            "customerEmail": customer_email,
+            "customerName": customer_name,
+            "reservedAccountType": reserved_account,
+            "bvn": bvn,
+            "nin": nin,
+        }
+        return self._post("/v1/bank-transfer/reserved-accounts", data=data)
+
+    def get_reserve_detail(self, account_reference: str) -> MonnifyResponse:
+        """
+        Get details of a reserved account.
+        Reference: https://developers.monnify.com/api/#get-reserved-account-details
+
+        :param: account_reference
+
+        :return: The response from the API
+        :rtype: MonnifyResponse object
+        """
+        return self._get(f"/v2/bank-transfer/reserved-accounts/{account_reference}")
+
+    def add_linked_account(
+            self,
+            account_reference: str,
+            preferred_bank: Optional[Union[List[str], None]] = None,
+            get_all_banks: Optional[bool] = True
+    ) -> MonnifyResponse:
+        """
+        Add a linked account to a reserved account.
+        Reference: https://developers.monnify.com/api/#add-linked-accounts
+
+        :param: preferred_bank
+        :param: account_reference
+        :param: get_all_banks
+
+        :return: The response from the API
+        :rtype: MonnifyResponse object
+        """
+        data = {
+            "preferredBank": preferred_bank,
+            "getAllAvailableBanks": get_all_banks,
+        }
+        return self._put(
+            f"v1/bank-transfer/reserved-accounts/add-linked-accounts/{account_reference}",
+            data=data,
+        )
+
+    def update_bvn_reserve(self, account_reference: str, bvn: str) -> MonnifyResponse:
+        """
+        Update the BVN of a reserved account.
+        Reference: https://developers.monnify.com/api/#update-bvn-for-a-reserve-account
+
+        :param: bvn
+        :param: account_reference
+
+        :return: The response from the API
+        :rtype: MonnifyResponse object
+        """
+        data = {
+            "bvn": bvn,
+        }
+        return self._put(
+            f"/v1/bank-transfer/reserved-accounts/update-customer-bvn/{account_reference}",
+            data=data,
+        )
+
+    def allow_payment_source(
+            self,
+            account_reference: str,
+            allow_payment_source: Dict[str, List[Any]],
+            restrict_pay_source: Optional[bool] = True,
+    ) -> MonnifyResponse:
+        """
+        Manages accounts of a reserved account using [BVNs, Account Name or Account Number].
+        Reference: https://developers.monnify.com/api/#allowed-payment-sources
+
+        :param: allow_payment_source
+        :param: account_reference
+        :param: payment_source
+
+        :return: The response from the API
+        :rtype: MonnifyResponse object
+        """
+        data = {
+            "allowedPaymentSource": allow_payment_source,
+            "restrictPaymentSource": restrict_pay_source,
+        }
+        return self._put(
+            f"/v1/bank-transfer/reserved-accounts/update-payment-source-filter/{account_reference}",
+            data=data,
+        )
+
+    def update_split_config_account(
+            self,
+            account_reference: str,
+            objects: List[Dict[str, Any]]
+    ) -> MonnifyResponse:
+        """
+        Updates the split config of a customer reserved account.
+        Reference: https://developers.monnify.com/api/#updating-split-config-for-reserved-account
+
+        :param: account_reference
+        :param: objects contains list of dictionaries.
+        [
+            {
+                "subAccountCode": {{SubaccountCode}},
+                "feePercentage": {{fee in percent}},
+                "splitPercentage": {{split in percent}},
+                "feeBearer": {{true or false}}
+            }
+        ]
+
+        :return: Response from the API
+        :rtype: MonnifyResponse object
+        """
+        return self._put(
+            f"/v1/bank-transfer/reserved-accounts/update-income-split-config/{account_reference}",
+            data=objects,
+        )
+
+    def deallocate_customer(self, account_reference: str) -> MonnifyResponse:
+        """
+        Deallocate/delete already created a reserved account.
+        Reference: https://developers.monnify.com/api/#deallocating-a-reserved-account
+
+        :param: account_reference
+
+        :return: The response from the API
+        :rtype: MonnifyResponse object
+        """
+        return self._delete(f"/v1/bank-transfer/reserved-accounts/{account_reference}")
+
+    def get_reserve_transactions(
+        self, account_reference: str, per_page: Optional[Union[int, None]] = 50, page: Optional[Union[int, None]] = 0
+    ) -> MonnifyResponse:
+        """
+        Get transactions for a reserved account.
+        Reference: https://developers.monnify.com/api/#get-transactions-for-a-reserved-account
+
+        :param: account_reference
+        :param: per_page
+        :param: page
+
+        :return: The response from the API
+        :rtype: MonnifyResponse object
+        """
+        params = {"accountReference": account_reference, "page": page, "size": per_page}
+        return self._get(
+            "/v1/bank-transfer/reserved-accounts/transactions", params=params
+        )
+
+    def update_kyc_info(
+            self, account_reference: str, bvn: str, nin: str
+    ) -> MonnifyResponse:
+        """
+        This links customers' BVN/NIN to their respective reserved accounts.
+        Reference: https://developers.monnify.com/api/#update-kyc-info
+
+        :param: account_reference
+        :param: bvn
+        :param: nin
+
+        :return: The response from the API
+        :rtype: MonnifyResponse object
+        """
+        data = {
+            "bvn": bvn,
+            "nin": nin,
+        }
+        return self._put(
+            f"/v1/bank-transfer/reserved-accounts/{account_reference}/kyc-info",
+            data=data,
+        )
```

### Comparing `monnifyease-0.1.0/monnifyease/apis/sync_apis/transactions.py` & `monnifyease-0.2.0/monnifyease/apis/sync_apis/transactions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,225 +1,225 @@
-""" Wrapper for Monnify Transactions API
-The Transactions API allows you to create and manage payments on your integration.
-"""
-
-from datetime import date
-from typing import Optional, List, Dict, Any, Union
-
-from monnifyease.core import MonnifyResponse, SyncRequestClient
-from monnifyease.helpers.tool_kit import PaymentMethods, Currency
-from monnifyease.utils.convert_to_strings import convert_to_string
-
-
-class Transactions(SyncRequestClient):
-    """Monnify Transaction API"""
-
-    def initialize_transaction(
-            self,
-            amount: float,
-            customer_name: str,
-            customer_email: str,
-            payment_reference: str,
-            payment_description: str,
-            currency: Currency,
-            merchant_code: str,
-            payment_methods: Optional[Union[List[PaymentMethods], None]] = None,
-            redirect_url: Optional[Union[str, None]] = None,
-            income_split_config: Optional[Union[List[Dict[str, Any]], None]] = None,
-            metadata: Optional[Union[Dict[str, Any], None]] = None,
-    ) -> MonnifyResponse:
-        """
-        Create a transaction
-        Reference: https://developers.monnify.com/api/#initialize-transaction
-
-        :param: amount
-        :param: customer_name
-        :param: customer_email
-        :param: payment_reference: A unique string of characters that identifies each transaction
-        :param: payment_description: Reason of payment
-        :param: currency
-        :param: merchant_code: The merchant contract code
-        :param: redirect_url: A url to redirect to after payment completion
-        :param: payment_methods: The method of payment collection
-        :param: income_split_config: A way to split payments among subAccounts.
-        :param: metadata: pass extra information from customers.
-
-        :return: The response form the API
-        :rtype: MonnifyResponse object
-        """
-        data = {
-            "amount": amount,
-            "customerName": customer_name,
-            "customerEmail": customer_email,
-            "paymentReference": payment_reference,
-            "paymentDescription": payment_description,
-            "currencyCode": currency,
-            "contractCode": merchant_code,
-            "redirectUrl": redirect_url,
-            "paymentMethods": payment_methods,
-            "incomeSplitConfig": income_split_config,
-            "metadata": metadata,
-        }
-        return self._post("/v1/merchant/transactions/init-transaction", data=data)
-
-    def pay_with_bank_transfer(
-            self, transaction_reference: str, bank_code: str
-    ) -> MonnifyResponse:
-        """
-        Create a transaction
-        Reference: https://developers.monnify.com/api/#initialize-transaction
-
-        :param: transaction_reference: This is the transaction reference gotten from the initialize_transaction method
-        :param: bank_code
-
-        :return: The response form the API
-        :rtype: MonnifyResponse object
-        """
-        data = {"transactionReference": transaction_reference, "bankCode": bank_code}
-        return self._post("/v1/merchant/bank-transfer/init-payment", data=data)
-
-    def charge_card(
-            self,
-            transaction_reference: str,
-            card: Dict[str, str],
-            collection_channel: Optional[str] = "API_NOTIFICATION",
-    ) -> MonnifyResponse:
-        """
-        Initiate a charge on a card
-        Reference: https://developers.monnify.com/api/#charge-card
-
-        :param: transaction_reference
-        :param: collection_channel
-        :param: card: The card to charge
-
-        :return: The response from the API
-        :rtype: MonnifyResponse object
-        """
-        data = {
-            "transactionReference": transaction_reference,
-            "collectionChannel": collection_channel,
-            "card": card,
-        }
-        return self._post("/v1/merchant/cards/charge", data=data)
-
-    def authorize_otp(
-            self,
-            transaction_reference: str,
-            token_id: str,
-            token: str,
-            collection_channel: Optional[str] = "API_NOTIFICATION",
-    ) -> MonnifyResponse:
-        """
-        Authorize an OTP to complete a charge on a card
-        Reference: https://developers.monnify.com/api/#authorize-otp
-
-        :param: transaction_reference
-        :param: collection_channel
-        :param: token_id
-        :param: token
-
-        :return: The response from the API
-        :rtype: MonnifyResponse object
-        """
-        data = {
-            "transactionReference": transaction_reference,
-            "collectionChannel": collection_channel,
-            "tokenId": token_id,
-            "token": token,
-        }
-        return self._post("/v1/merchant/cards/charge", data=data)
-
-    def authorize_3ds(
-            self,
-            transaction_reference: str,
-            card: Dict[str, str],
-            collection_channel: Optional[str] = "API_NOTIFICATION",
-            api_key: Optional[Union[str, None]] = None,
-    ) -> MonnifyResponse:
-        """
-        Authorizes charge on a card that uses 3DS Secure Authentication.
-        Reference: https://developers.monnify.com/api/#authorize-3ds-card
-
-        :param: transaction_reference
-        :param: collection_channel
-        :param: card
-        :param: api_key
-
-        :return: The response from the API
-        :rtype: MonnifyResponse object
-        """
-        data = {
-            "transactionReference": transaction_reference,
-            "collectionChannel": collection_channel,
-            "card": card,
-            "apiKey": api_key,
-        }
-        return self._post("v1/sdk/cards/secure-3d/authorize", data=data)
-
-    def list_transaction(
-            self,
-            per_page: Optional[Union[int, None]] = 50,
-            page_size: Optional[Union[int, None]] = 1,
-            payment_reference: Optional[Union[str, None]] = None,
-            transaction_reference: Optional[Union[str, None]] = None,
-            from_amount: Optional[Union[float, None]] = None,
-            to_amount: Optional[Union[float, None]] = None,
-            amount: Optional[Union[float, None]] = None,
-            customer_name: Optional[Union[str, None]] = None,
-            customer_email: Optional[Union[str, None]] = None,
-            payment_status: Optional[Union[str, None]] = None,
-            from_date: Optional[Union[date, None]] = None,
-            to_date: Optional[Union[date, None]] = None,
-    ) -> MonnifyResponse:
-        """
-        Get all Transactions List
-        Reference: https://developers.monnify.com/api/#get-all-transactions
-
-        :param: per_page
-        :param: page_size
-        :param: payment_reference
-        :param: transaction_reference
-        :param: from_amount
-        :param: to_amount
-        :param: amount
-        :param: customer_name
-        :param: customer_email
-        :param: payment_status
-        :param: from_date
-        :param: to_date
-
-        :return: The response form the API
-        :rtype: MonnifyResponse object
-        """
-
-        # convert to string
-        from_date = convert_to_string(from_date)
-        to_date = convert_to_string(to_date)
-
-        params = {
-            "page": per_page,
-            "size": page_size,
-            "paymentReference": payment_reference,
-            "transactionReference": transaction_reference,
-            "fromAmount": from_amount,
-            "toAmount": to_amount,
-            "amount": amount,
-            "customerName": customer_name,
-            "customerEmail": customer_email,
-            "paymentStatus": payment_status,
-            "from": from_date,
-            "to": to_date,
-        }
-        return self._get("/v1/transactions/search", params=params)
-
-    def get_transaction_status(self, transaction_reference: str) -> MonnifyResponse:
-        """
-        Status of a transaction
-        Reference: https://developers.monnify.com/api/#get-transaction-status
-
-        :param: transaction_reference
-
-        :return: The response from the API
-        :rtype: MonnifyResponse object
-        """
-        # params = {"transactionReference": transaction_reference}
-        return self._get(f"/v2/transactions/{transaction_reference}")
+""" Wrapper for Monnify Transactions API
+The Transactions API allows you to create and manage payments on your integration.
+"""
+
+from datetime import date
+from typing import Optional, List, Dict, Any, Union
+
+from monnifyease.core import MonnifyResponse, SyncRequestClient
+from monnifyease.helpers.tool_kit import PaymentMethods, Currency
+from monnifyease.utils.convert_to_strings import convert_to_string
+
+
+class Transactions(SyncRequestClient):
+    """Monnify Transaction API"""
+
+    def initialize_transaction(
+            self,
+            amount: float,
+            customer_name: str,
+            customer_email: str,
+            payment_reference: str,
+            payment_description: str,
+            currency: Currency,
+            merchant_code: str,
+            payment_methods: Optional[Union[List[PaymentMethods], None]] = None,
+            redirect_url: Optional[Union[str, None]] = None,
+            income_split_config: Optional[Union[List[Dict[str, Any]], None]] = None,
+            metadata: Optional[Union[Dict[str, Any], None]] = None,
+    ) -> MonnifyResponse:
+        """
+        Create a transaction
+        Reference: https://developers.monnify.com/api/#initialize-transaction
+
+        :param: amount
+        :param: customer_name
+        :param: customer_email
+        :param: payment_reference: A unique string of characters that identifies each transaction
+        :param: payment_description: Reason of payment
+        :param: currency
+        :param: merchant_code: The merchant contract code
+        :param: redirect_url: A url to redirect to after payment completion
+        :param: payment_methods: The method of payment collection
+        :param: income_split_config: A way to split payments among subAccounts.
+        :param: metadata: pass extra information from customers.
+
+        :return: The response form the API
+        :rtype: MonnifyResponse object
+        """
+        data = {
+            "amount": amount,
+            "customerName": customer_name,
+            "customerEmail": customer_email,
+            "paymentReference": payment_reference,
+            "paymentDescription": payment_description,
+            "currencyCode": currency,
+            "contractCode": merchant_code,
+            "redirectUrl": redirect_url,
+            "paymentMethods": payment_methods,
+            "incomeSplitConfig": income_split_config,
+            "metadata": metadata,
+        }
+        return self._post("/v1/merchant/transactions/init-transaction", data=data)
+
+    def pay_with_bank_transfer(
+            self, transaction_reference: str, bank_code: str
+    ) -> MonnifyResponse:
+        """
+        Create a transaction
+        Reference: https://developers.monnify.com/api/#initialize-transaction
+
+        :param: transaction_reference: This is the transaction reference gotten from the initialize_transaction method
+        :param: bank_code
+
+        :return: The response form the API
+        :rtype: MonnifyResponse object
+        """
+        data = {"transactionReference": transaction_reference, "bankCode": bank_code}
+        return self._post("/v1/merchant/bank-transfer/init-payment", data=data)
+
+    def charge_card(
+            self,
+            transaction_reference: str,
+            card: Dict[str, str],
+            collection_channel: Optional[str] = "API_NOTIFICATION",
+    ) -> MonnifyResponse:
+        """
+        Initiate a charge on a card
+        Reference: https://developers.monnify.com/api/#charge-card
+
+        :param: transaction_reference
+        :param: collection_channel
+        :param: card: The card to charge
+
+        :return: The response from the API
+        :rtype: MonnifyResponse object
+        """
+        data = {
+            "transactionReference": transaction_reference,
+            "collectionChannel": collection_channel,
+            "card": card,
+        }
+        return self._post("/v1/merchant/cards/charge", data=data)
+
+    def authorize_otp(
+            self,
+            transaction_reference: str,
+            token_id: str,
+            token: str,
+            collection_channel: Optional[str] = "API_NOTIFICATION",
+    ) -> MonnifyResponse:
+        """
+        Authorize an OTP to complete a charge on a card
+        Reference: https://developers.monnify.com/api/#authorize-otp
+
+        :param: transaction_reference
+        :param: collection_channel
+        :param: token_id
+        :param: token
+
+        :return: The response from the API
+        :rtype: MonnifyResponse object
+        """
+        data = {
+            "transactionReference": transaction_reference,
+            "collectionChannel": collection_channel,
+            "tokenId": token_id,
+            "token": token,
+        }
+        return self._post("/v1/merchant/cards/charge", data=data)
+
+    def authorize_3ds(
+            self,
+            transaction_reference: str,
+            card: Dict[str, str],
+            collection_channel: Optional[str] = "API_NOTIFICATION",
+            api_key: Optional[Union[str, None]] = None,
+    ) -> MonnifyResponse:
+        """
+        Authorizes charge on a card that uses 3DS Secure Authentication.
+        Reference: https://developers.monnify.com/api/#authorize-3ds-card
+
+        :param: transaction_reference
+        :param: collection_channel
+        :param: card
+        :param: api_key
+
+        :return: The response from the API
+        :rtype: MonnifyResponse object
+        """
+        data = {
+            "transactionReference": transaction_reference,
+            "collectionChannel": collection_channel,
+            "card": card,
+            "apiKey": api_key,
+        }
+        return self._post("v1/sdk/cards/secure-3d/authorize", data=data)
+
+    def list_transaction(
+            self,
+            per_page: Optional[Union[int, None]] = 0,
+            page_size: Optional[Union[int, None]] = 50,
+            payment_reference: Optional[Union[str, None]] = None,
+            transaction_reference: Optional[Union[str, None]] = None,
+            from_amount: Optional[Union[float, None]] = None,
+            to_amount: Optional[Union[float, None]] = None,
+            amount: Optional[Union[float, None]] = None,
+            customer_name: Optional[Union[str, None]] = None,
+            customer_email: Optional[Union[str, None]] = None,
+            payment_status: Optional[Union[str, None]] = None,
+            from_date: Optional[Union[date, None]] = None,
+            to_date: Optional[Union[date, None]] = None,
+    ) -> MonnifyResponse:
+        """
+        Get all Transactions List
+        Reference: https://developers.monnify.com/api/#get-all-transactions
+
+        :param: per_page
+        :param: page_size
+        :param: payment_reference
+        :param: transaction_reference
+        :param: from_amount
+        :param: to_amount
+        :param: amount
+        :param: customer_name
+        :param: customer_email
+        :param: payment_status
+        :param: from_date
+        :param: to_date
+
+        :return: The response form the API
+        :rtype: MonnifyResponse object
+        """
+
+        # convert to string
+        from_date = convert_to_string(from_date)
+        to_date = convert_to_string(to_date)
+
+        params = {
+            "page": per_page,
+            "size": page_size,
+            "paymentReference": payment_reference,
+            "transactionReference": transaction_reference,
+            "fromAmount": from_amount,
+            "toAmount": to_amount,
+            "amount": amount,
+            "customerName": customer_name,
+            "customerEmail": customer_email,
+            "paymentStatus": payment_status,
+            "from": from_date,
+            "to": to_date,
+        }
+        return self._get("/v1/transactions/search", params=params)
+
+    def get_transaction_status(self, transaction_reference: str) -> MonnifyResponse:
+        """
+        Status of a transaction
+        Reference: https://developers.monnify.com/api/#get-transaction-status
+
+        :param: transaction_reference
+
+        :return: The response from the API
+        :rtype: MonnifyResponse object
+        """
+        # params = {"transactionReference": transaction_reference}
+        return self._get(f"/v2/transactions/{transaction_reference}")
```

### Comparing `monnifyease-0.1.0/monnifyease/core/__init__.py` & `monnifyease-0.2.0/monnifyease/core/__init__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-""" Internal wrapper for monnifyease"""
-
-from monnifyease.core._api_access_header import AccessHeaderToken, AccessHeader
-from monnifyease.core._api_base import MonnifyBaseClient
-from monnifyease.core._api_base_envar import EnvConfig, EnvBase, MERCHANT_CODE
-from monnifyease.core._api_base_request import SyncBaseRequestClient
-from monnifyease.core._api_client_requests import SyncRequestClient
-from monnifyease.core._api_client_response import MonnifyResponse
-from monnifyease.core._api_errors import MonnifyEaseError, EnvKeyError, TypeValueError
+""" Internal wrapper for monnifyease"""
+
+from monnifyease.core._api_access_header import AccessHeaderToken, AccessHeader
+from monnifyease.core._api_base import MonnifyBaseClient
+from monnifyease.core._api_base_envar import EnvConfig, EnvBase, MERCHANT_CODE
+from monnifyease.core._api_base_request import SyncBaseRequestClient
+from monnifyease.core._api_client_requests import SyncRequestClient
+from monnifyease.core._api_client_response import MonnifyResponse
+from monnifyease.core._api_errors import MonnifyEaseError, EnvKeyError, TypeValueError
```

### Comparing `monnifyease-0.1.0/monnifyease/core/_api_access_header.py` & `monnifyease-0.2.0/monnifyease/core/_api_access_header.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-"""
-This is aninterface betwee the MonnifyBaseClient and SyncBaseRequestClient classes to implement the
-access token header generated by the MonnifyBaseClient class
-"""
-
-from typing import Protocol
-
-from monnifyease.core._api_base import MonnifyBaseClient
-from monnifyease.core._api_base_envar import EnvConfig
-
-
-class AccessHeaderToken(Protocol):
-    """
-    This protocol defines the interface for generating an authorization header
-    used for authentication with the Monnify API.
-
-    A class conforming to this protocol should implement the
-    `generate_auth_header` method.
-    """
-    def get_auth_header(self) -> dict:
-        """
-        Generates an authorization header dictionary for Monnify API requests.
-
-        The specific format and content of the header might depend on the
-        implementation details.
-
-        Returns:
-            dict: A dictionary containing the authorization header information.
-        """
-
-
-class AccessHeader(AccessHeaderToken):
-    """
-    An implementation of the AccessHeaderToken protocol that retrieves
-    an authorization header from a MonnifyBaseClient instance using the
-    default environment configuration (EnvConfig).
-    """
-    @classmethod
-    def get_auth_header(cls) -> dict:
-        """
-        Gets an authorization header dictionary for Monnify API requests
-        using the default environment configuration (EnvConfig) to retrieve
-        access tokens.
-
-        Returns:
-            dict: A dictionary containing the authorization header information.
-        """
-        client = MonnifyBaseClient(EnvConfig)
-        return client.get_access_token()
+"""
+This is aninterface betwee the MonnifyBaseClient and SyncBaseRequestClient classes to implement the
+access token header generated by the MonnifyBaseClient class
+"""
+
+from typing import Protocol
+
+from monnifyease.core._api_base import MonnifyBaseClient
+from monnifyease.core._api_base_envar import EnvConfig
+
+
+class AccessHeaderToken(Protocol):
+    """
+    This protocol defines the interface for generating an authorization header
+    used for authentication with the Monnify API.
+
+    A class conforming to this protocol should implement the
+    `generate_auth_header` method.
+    """
+    def get_auth_header(self) -> dict:
+        """
+        Generates an authorization header dictionary for Monnify API requests.
+
+        The specific format and content of the header might depend on the
+        implementation details.
+
+        Returns:
+            dict: A dictionary containing the authorization header information.
+        """
+
+
+class AccessHeader(AccessHeaderToken):
+    """
+    An implementation of the AccessHeaderToken protocol that retrieves
+    an authorization header from a MonnifyBaseClient instance using the
+    default environment configuration (EnvConfig).
+    """
+    @classmethod
+    def get_auth_header(cls) -> dict:
+        """
+        Gets an authorization header dictionary for Monnify API requests
+        using the default environment configuration (EnvConfig) to retrieve
+        access tokens.
+
+        Returns:
+            dict: A dictionary containing the authorization header information.
+        """
+        client = MonnifyBaseClient(EnvConfig)
+        return client.get_access_token()
```

### Comparing `monnifyease-0.1.0/monnifyease/core/_api_base.py` & `monnifyease-0.2.0/monnifyease/core/_api_base.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-"""
-Base client API for Monnify API with methods for handling HTTP requests, authentication using a secret key,
-constructing HTTP headers, joining URLs with the API base URL, and logging response information.
-"""
-
-import base64
-import logging
-from datetime import datetime, timedelta
-from urllib.parse import urljoin
-
-from requests import Session, RequestException
-
-from monnifyease.core._api_base_envar import EnvBase
-from monnifyease.core._api_errors import MonnifyEaseError
-
-
-logger = logging.getLogger(__name__)
-
-
-class MonnifyBaseClient:
-    """Base Client API for Monnify API"""
-
-    def __init__(self, env: EnvBase, session: Session = Session()) -> None:
-        """
-        Initialize the Monnify Base Client with the chosen environment
-
-        :param: environment: the environment platform you want to connect
-
-        :return: the connection to the server
-        """
-        self._env = env
-        self._session = session
-        self._access_token = None
-        self._token_expiry = None
-
-    def _generate_auth_basic(self) -> str:
-        """
-        Generates a Basic authentication header value by encoding the API key and secret key.
-
-        Returns:
-            str: The Basic authentication header value.
-        """
-        code = base64.b64encode(
-            f"{self._env.get_api_key()}:{self._env.get_secret_key()}".encode()
-        ).decode("utf-8")
-        auth_code = f"Basic {code}"
-        return auth_code
-
-    def get_access_token(self) -> dict:
-        """
-        Retrieves a Monnify API access token.
-
-        This method manages caching the access token and refreshes it before it expires.
-
-        Returns:
-            dict: A dictionary containing the authorization header, content type header,
-                and user-agent header. The authorization header uses a Bearer token retrieved
-                from the Monnify API.
-        """
-        if not self._access_token or datetime.now() > self._token_expiry:
-            self._access_token = self._generate_access_token()
-            self._token_expiry = datetime.now() + timedelta(
-                seconds=self._access_token["responseBody"]["expiresIn"]
-            )
-        return {
-            "Authorization": f"Bearer {self._access_token['responseBody']['accessToken']}",
-            "Content-Type": "application/json",
-            "User-Agent": "monnifyease/0.1.0",
-        }
-
-    def _generate_access_token(self) -> dict:
-        """
-        Generates a new Monnify API access token using Basic authentication.
-
-        Returns:
-            dict: A dictionary containing the access token, expiry time
-
-        Raises:
-            MonnifyEaseError: If there is an error during the access token request.
-        """
-        auth_code = self._generate_auth_basic()
-        headers = {
-            "Authorization": auth_code,
-            "Content-Type": "application/json",
-            "User-Agent": "monnifyease/0.1.0",
-        }
-        token_request_body = {"grant_type": "authorization_code"}
-
-        try:
-            access_response = self._session.post(
-                url=urljoin(self._env.get_base_url(), "v1/auth/login"),
-                headers=headers,
-                json=token_request_body,
-            )
-            access_response.raise_for_status()
-            access_token = access_response.json()
-            return access_token
-        except RequestException as error:
-            error_message = str(error)
-            status_code = getattr(error, "response", None) and getattr(
-                error.response, "status_code", None
-            )
-            logger.error("Error %s:", error)
-            raise MonnifyEaseError(
-                message=error_message, status_code=status_code
-            ) from error
+"""
+Base client API for Monnify API with methods for handling HTTP requests, authentication using a secret key,
+constructing HTTP headers, joining URLs with the API base URL, and logging response information.
+"""
+
+import base64
+import logging
+from datetime import datetime, timedelta
+from urllib.parse import urljoin
+
+from requests import Session, RequestException
+
+from monnifyease.core._api_base_envar import EnvBase
+from monnifyease.core._api_errors import MonnifyEaseError
+
+
+logger = logging.getLogger(__name__)
+
+
+class MonnifyBaseClient:
+    """Base Client API for Monnify API"""
+
+    def __init__(self, env: EnvBase, session: Session = Session()) -> None:
+        """
+        Initialize the Monnify Base Client with the chosen environment
+
+        :param: environment: the environment platform you want to connect
+
+        :return: the connection to the server
+        """
+        self._env = env
+        self._session = session
+        self._access_token = None
+        self._token_expiry = None
+
+    def _generate_auth_basic(self) -> str:
+        """
+        Generates a Basic authentication header value by encoding the API key and secret key.
+
+        Returns:
+            str: The Basic authentication header value.
+        """
+        code = base64.b64encode(
+            f"{self._env.get_api_key()}:{self._env.get_secret_key()}".encode()
+        ).decode("utf-8")
+        auth_code = f"Basic {code}"
+        return auth_code
+
+    def get_access_token(self) -> dict:
+        """
+        Retrieves a Monnify API access token.
+
+        This method manages caching the access token and refreshes it before it expires.
+
+        Returns:
+            dict: A dictionary containing the authorization header, content type header,
+                and user-agent header. The authorization header uses a Bearer token retrieved
+                from the Monnify API.
+        """
+        if not self._access_token or datetime.now() > self._token_expiry:
+            self._access_token = self._generate_access_token()
+            self._token_expiry = datetime.now() + timedelta(
+                seconds=self._access_token["responseBody"]["expiresIn"]
+            )
+        return {
+            "Authorization": f"Bearer {self._access_token['responseBody']['accessToken']}",
+            "Content-Type": "application/json",
+            "User-Agent": "monnifyease/0.1.0",
+        }
+
+    def _generate_access_token(self) -> dict:
+        """
+        Generates a new Monnify API access token using Basic authentication.
+
+        Returns:
+            dict: A dictionary containing the access token, expiry time
+
+        Raises:
+            MonnifyEaseError: If there is an error during the access token request.
+        """
+        auth_code = self._generate_auth_basic()
+        headers = {
+            "Authorization": auth_code,
+            "Content-Type": "application/json",
+            "User-Agent": "monnifyease/0.1.0",
+        }
+        token_request_body = {"grant_type": "authorization_code"}
+
+        try:
+            access_response = self._session.post(
+                url=urljoin(self._env.get_base_url(), "v1/auth/login"),
+                headers=headers,
+                json=token_request_body,
+            )
+            access_response.raise_for_status()
+            access_token = access_response.json()
+            return access_token
+        except RequestException as error:
+            error_message = str(error)
+            status_code = getattr(error, "response", None) and getattr(
+                error.response, "status_code", None
+            )
+            logger.error("Error %s:", error)
+            raise MonnifyEaseError(
+                message=error_message, status_code=status_code
+            ) from error
```

### Comparing `monnifyease-0.1.0/monnifyease/core/_api_base_envar.py` & `monnifyease-0.2.0/monnifyease/core/_api_base_envar.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-""" Environment variables for the application to be executed when the application is started"""
-
-from typing import Protocol
-from decouple import config
-from monnifyease.core._api_errors import EnvKeyError
-
-
-MERCHANT_CODE = config("MONNIFY_CONTRACT_CODE")
-
-
-class EnvBase(Protocol):
-    """
-    This is a base protocol that defines the methods required to access environment variables
-    used by the MonnifyEase library.
-
-    Implementations of this protocol should provide concrete methods for retrieving the environment variables:
-        - MONNIFY_API_KEY: The Monnify API key used for authentication.
-        - MONNIFY_SECRET_KEY: The Monnify secret key used for authentication.
-        - MONNIFY_BASE_URL: The base URL of the Monnify API.
-    """
-
-    def get_api_key(self) -> str:
-        """
-        Retrieves the Monnify API key from environment variables.
-
-        Raises:
-            EnvKeyError: If the MONNIFY_API_KEY environment variable is not set.
-
-        Returns:
-            str: The Monnify API key.
-        """
-
-    def get_secret_key(self) -> str:
-        """
-        Retrieves the Monnify SECRET key from environment variables.
-
-        Raises:
-            EnvKeyError: If the MONNIFY_SECRET_KEY environment variable is not set.
-
-        Returns:
-            str: The Monnify SECRET key.
-        """
-
-    def get_base_url(self) -> str:
-        """
-        Retrieves the Monnify BASE URL from environment variables.
-
-        Raises:
-            EnvKeyError: If the MONNIFY_BASE_URL environment variable is not set.
-
-        Returns:
-            str: The Monnify BASE URL.
-        """
-
-
-class EnvConfig(EnvBase):
-    """The configuration"""
-    @classmethod
-    def get_api_key(cls):
-        """
-        See EnvBase.get_api_key()
-        """
-        api_key = config("MONNIFY_API_KEY")
-        if not api_key:
-            raise EnvKeyError(
-                message="Kindly ensure you have MONNIFY_API_KEY variable intact"
-            )
-        return api_key
-
-    @classmethod
-    def get_secret_key(cls):
-        """
-        See EnvBase.get_secret_key()
-        """
-        secret_key = config("MONNIFY_SECRET_KEY")
-        if not secret_key:
-            raise EnvKeyError(
-                message="Kindly ensure you have MONNIFY_SECRET_KEY variable intact"
-            )
-        return secret_key
-
-    @classmethod
-    def get_base_url(cls):
-        """
-        See EnvBase.get_base_url()
-        """
-        base_url = config("MONNIFY_BASE_URL")
-        if not base_url:
-            raise EnvKeyError(
-                message="Kindly ensure you have MONNIFY_BASE_URL variable intact"
-            )
-        return base_url
+""" Environment variables for the application to be executed when the application is started"""
+
+from typing import Protocol
+from decouple import config
+from monnifyease.core._api_errors import EnvKeyError
+
+
+MERCHANT_CODE = config("MONNIFY_CONTRACT_CODE")
+
+
+class EnvBase(Protocol):
+    """
+    This is a base protocol that defines the methods required to access environment variables
+    used by the MonnifyEase library.
+
+    Implementations of this protocol should provide concrete methods for retrieving the environment variables:
+        - MONNIFY_API_KEY: The Monnify API key used for authentication.
+        - MONNIFY_SECRET_KEY: The Monnify secret key used for authentication.
+        - MONNIFY_BASE_URL: The base URL of the Monnify API.
+    """
+
+    def get_api_key(self) -> str:
+        """
+        Retrieves the Monnify API key from environment variables.
+
+        Raises:
+            EnvKeyError: If the MONNIFY_API_KEY environment variable is not set.
+
+        Returns:
+            str: The Monnify API key.
+        """
+
+    def get_secret_key(self) -> str:
+        """
+        Retrieves the Monnify SECRET key from environment variables.
+
+        Raises:
+            EnvKeyError: If the MONNIFY_SECRET_KEY environment variable is not set.
+
+        Returns:
+            str: The Monnify SECRET key.
+        """
+
+    def get_base_url(self) -> str:
+        """
+        Retrieves the Monnify BASE URL from environment variables.
+
+        Raises:
+            EnvKeyError: If the MONNIFY_BASE_URL environment variable is not set.
+
+        Returns:
+            str: The Monnify BASE URL.
+        """
+
+
+class EnvConfig(EnvBase):
+    """The configuration"""
+    @classmethod
+    def get_api_key(cls):
+        """
+        See EnvBase.get_api_key()
+        """
+        api_key = config("MONNIFY_API_KEY")
+        if not api_key:
+            raise EnvKeyError(
+                message="Kindly ensure you have MONNIFY_API_KEY variable intact"
+            )
+        return api_key
+
+    @classmethod
+    def get_secret_key(cls):
+        """
+        See EnvBase.get_secret_key()
+        """
+        secret_key = config("MONNIFY_SECRET_KEY")
+        if not secret_key:
+            raise EnvKeyError(
+                message="Kindly ensure you have MONNIFY_SECRET_KEY variable intact"
+            )
+        return secret_key
+
+    @classmethod
+    def get_base_url(cls):
+        """
+        See EnvBase.get_base_url()
+        """
+        base_url = config("MONNIFY_BASE_URL")
+        if not base_url:
+            raise EnvKeyError(
+                message="Kindly ensure you have MONNIFY_BASE_URL variable intact"
+            )
+        return base_url
```

### Comparing `monnifyease-0.1.0/monnifyease/core/_api_base_request.py` & `monnifyease-0.2.0/monnifyease/core/_api_base_request.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-""" Base class for implementing requests"""
-
-import json
-import logging
-from typing import Optional, Union, Any, List, Dict
-
-from requests import RequestException, Session
-
-from monnifyease.core._api_access_header import AccessHeader
-from monnifyease.core._api_client_response import MonnifyResponse
-from monnifyease.core._api_errors import MonnifyEaseError, InvalidRequestMethodError
-from monnifyease.utils.join_url import join_url
-
-
-logger = logging.getLogger(__name__)
-
-
-class SyncBaseRequestClient:
-    """Monnify Request"""
-
-    _VALID_HTTP_METHODS: set[str] = {"GET", "POST", "PUT", "DELETE"}
-
-    def __init__(
-        self, session: Session = Session(), auth_header: AccessHeader = AccessHeader()
-    ) -> None:
-        """Monnify Request"""
-        self._session = session
-        self._access_header = auth_header
-
-    def _request_url(
-        self,
-        method: str,
-        url: str,
-        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        params: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        **kwargs,
-    ) -> MonnifyResponse:
-        """
-        :param method:
-        :param url:
-        :param data:
-        :param params:
-        :param kwargs:
-        :return:
-        """
-        if method.upper() not in self._VALID_HTTP_METHODS:
-            error_message = f"Invalid HTTP method. Supported methods are GET, POST, PUT, DELETE. {method}"
-            logger.error(error_message)
-            raise InvalidRequestMethodError(error_message)
-
-        url = join_url(url)
-
-        # Filtering params and data, then converting data to JSON
-        params = (
-            {key: value for key, value in params.items() if value is not None}
-            if params
-            else None
-        )
-        data = json.dumps(data) if data else None
-        try:
-            with self._session.request(
-                method=method,
-                headers=self._access_header.get_auth_header(),
-                url=url,
-                data=data,
-                params=params,
-                **kwargs,
-                timeout=10,
-            ) as response:
-                logger.info("Response Status Code: %s", response.status_code)
-                logger.info("Response JSON: %s", response.json())
-                response_data = response.json()
-                return MonnifyResponse(
-                    status_code=response.status_code,
-                    requestSuccessful=response_data.get("requestSuccessful"),
-                    responseMessage=response_data.get("responseMessage"),
-                    responseCode=response_data.get("responseCode"),
-                    responseBody=response_data.get("responseBody"),
-                )
-        except RequestException as error:
-            error_message = str(error)
-            status_code = getattr(error, "response", None) and getattr(
-                error.response, "status_code", None
-            )
-            logger.error("Error %s:", error)
-            raise MonnifyEaseError(
-                message=error_message, status_code=status_code
-            ) from error
+""" Base class for implementing requests"""
+
+import json
+import logging
+from typing import Optional, Union, Any, List, Dict
+
+from requests import RequestException, Session
+
+from monnifyease.core._api_access_header import AccessHeader
+from monnifyease.core._api_client_response import MonnifyResponse
+from monnifyease.core._api_errors import MonnifyEaseError, InvalidRequestMethodError
+from monnifyease.utils.join_url import join_url
+
+
+logger = logging.getLogger(__name__)
+
+
+class SyncBaseRequestClient:
+    """Monnify Request"""
+
+    _VALID_HTTP_METHODS: set[str] = {"GET", "POST", "PUT", "DELETE"}
+
+    def __init__(
+        self, session: Session = Session(), auth_header: AccessHeader = AccessHeader()
+    ) -> None:
+        """Monnify Request"""
+        self._session = session
+        self._access_header = auth_header
+
+    def _request_url(
+        self,
+        method: str,
+        url: str,
+        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        params: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        **kwargs,
+    ) -> MonnifyResponse:
+        """
+        :param method:
+        :param url:
+        :param data:
+        :param params:
+        :param kwargs:
+        :return:
+        """
+        if method.upper() not in self._VALID_HTTP_METHODS:
+            error_message = f"Invalid HTTP method. Supported methods are GET, POST, PUT, DELETE. {method}"
+            logger.error(error_message)
+            raise InvalidRequestMethodError(error_message)
+
+        url = join_url(url)
+
+        # Filtering params and data, then converting data to JSON
+        params = (
+            {key: value for key, value in params.items() if value is not None}
+            if params
+            else None
+        )
+        data = json.dumps(data) if data else None
+        try:
+            with self._session.request(
+                method=method,
+                headers=self._access_header.get_auth_header(),
+                url=url,
+                data=data,
+                params=params,
+                **kwargs,
+                timeout=10,
+            ) as response:
+                logger.info("Response Status Code: %s", response.status_code)
+                logger.info("Response JSON: %s", response.json())
+                response_data = response.json()
+                return MonnifyResponse(
+                    status_code=response.status_code,
+                    requestSuccessful=response_data.get("requestSuccessful"),
+                    responseMessage=response_data.get("responseMessage"),
+                    responseCode=response_data.get("responseCode"),
+                    responseBody=response_data.get("responseBody"),
+                )
+        except RequestException as error:
+            error_message = str(error)
+            status_code = getattr(error, "response", None) and getattr(
+                error.response, "status_code", None
+            )
+            logger.error("Error %s:", error)
+            raise MonnifyEaseError(
+                message=error_message, status_code=status_code
+            ) from error
```

### Comparing `monnifyease-0.1.0/monnifyease/core/_api_client_requests.py` & `monnifyease-0.2.0/monnifyease/core/_api_client_requests.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-""" Implementation of the request methods """
-
-from typing import Optional, Union, Dict, List, Any
-from monnifyease.core._api_base_request import SyncBaseRequestClient
-from monnifyease.core._api_client_response import MonnifyResponse
-
-
-class SyncRequestClient(SyncBaseRequestClient):
-    """Class representing a sync request client methods"""
-
-    def _get(
-        self,
-        endpoint: str,
-        params: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        **kwargs,
-    ) -> MonnifyResponse:
-        """
-        :param: endpoint
-        :param: params
-        :param: kwargs
-        :return:
-        """
-        return self._request_url("GET", url=endpoint, params=params, **kwargs)
-
-    def _post(
-        self,
-        endpoint: str,
-        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        **kwargs,
-    ) -> MonnifyResponse:
-        """
-        :param: endpoint
-        :param: data
-        :param: kwargs
-        :return:
-        """
-        return self._request_url("POST", url=endpoint, data=data, **kwargs)
-
-    def _put(
-        self,
-        endpoint: str,
-        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
-        **kwargs,
-    ) -> MonnifyResponse:
-        """
-        :param: endpoint
-        :param: data
-        :param: kwargs
-        :return:
-        """
-        return self._request_url("PUT", url=endpoint, data=data, **kwargs)
-
-    def _delete(self, endpoint: str, **kwargs) -> MonnifyResponse:
-        """
-        :param: endpoint
-        :param: kwargs
-        :return:
-        """
-        return self._request_url("DELETE", url=endpoint, **kwargs)
+""" Implementation of the request methods """
+
+from typing import Optional, Union, Dict, List, Any
+from monnifyease.core._api_base_request import SyncBaseRequestClient
+from monnifyease.core._api_client_response import MonnifyResponse
+
+
+class SyncRequestClient(SyncBaseRequestClient):
+    """Class representing a sync request client methods"""
+
+    def _get(
+        self,
+        endpoint: str,
+        params: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        **kwargs,
+    ) -> MonnifyResponse:
+        """
+        :param: endpoint
+        :param: params
+        :param: kwargs
+        :return:
+        """
+        return self._request_url("GET", url=endpoint, params=params, **kwargs)
+
+    def _post(
+        self,
+        endpoint: str,
+        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        **kwargs,
+    ) -> MonnifyResponse:
+        """
+        :param: endpoint
+        :param: data
+        :param: kwargs
+        :return:
+        """
+        return self._request_url("POST", url=endpoint, data=data, **kwargs)
+
+    def _put(
+        self,
+        endpoint: str,
+        data: Optional[Union[Dict[str, Any], List[Any], None]] = None,
+        **kwargs,
+    ) -> MonnifyResponse:
+        """
+        :param: endpoint
+        :param: data
+        :param: kwargs
+        :return:
+        """
+        return self._request_url("PUT", url=endpoint, data=data, **kwargs)
+
+    def _delete(self, endpoint: str, **kwargs) -> MonnifyResponse:
+        """
+        :param: endpoint
+        :param: kwargs
+        :return:
+        """
+        return self._request_url("DELETE", url=endpoint, **kwargs)
```

### Comparing `monnifyease-0.1.0/monnifyease/core/_api_client_response.py` & `monnifyease-0.2.0/monnifyease/core/_api_client_response.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-""" Response object from Monnify API server """
-
-from typing import Optional, Union, Dict, List, Any
-from dataclasses import dataclass
-
-
-@dataclass
-class MonnifyResponse:
-    """
-    Monnify API Response from the server after HTTP requests have been made
-    """
-
-    status_code: int
-    requestSuccessful: bool
-    responseMessage: str
-    responseCode: int
-    responseBody: Optional[Union[Dict[str, Any], List[Any]]]
-
-    @property
-    def url(self) -> Optional[Union[str, None]]:
-        """
-        :return:
-        """
-        if (
-            self.status_code == 200
-            and self.responseBody
-            and isinstance(self.responseBody, dict)
-        ):
-            return self.responseBody["checkoutUrl"]
-        return None
-
-    @property
-    def transaction_reference(self) -> Optional[Union[str, None]]:
-        """
-        :return:
-        """
-        if (
-            self.status_code == 200
-            and self.responseBody
-            and isinstance(self.responseBody, dict)
-        ):
-            return self.responseBody["transactionReference"]
-        return None
+""" Response object from Monnify API server """
+
+from typing import Optional, Union, Dict, List, Any
+from dataclasses import dataclass
+
+
+@dataclass
+class MonnifyResponse:
+    """
+    Monnify API Response from the server after HTTP requests have been made
+    """
+
+    status_code: int
+    requestSuccessful: bool
+    responseMessage: str
+    responseCode: int
+    responseBody: Optional[Union[Dict[str, Any], List[Any]]]
+
+    @property
+    def url(self) -> Optional[Union[str, None]]:
+        """
+        :return:
+        """
+        if (
+            self.status_code == 200
+            and self.responseBody
+            and isinstance(self.responseBody, dict)
+        ):
+            return self.responseBody["checkoutUrl"]
+        return None
+
+    @property
+    def transaction_reference(self) -> Optional[Union[str, None]]:
+        """
+        :return:
+        """
+        if (
+            self.status_code == 200
+            and self.responseBody
+            and isinstance(self.responseBody, dict)
+        ):
+            return self.responseBody["transactionReference"]
+        return None
```

### Comparing `monnifyease-0.1.0/monnifyease/monnify.py` & `monnifyease-0.2.0/monnifyease/monnify.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,25 @@
-""" Wrapper classes for various Synchronous Monnify API endpoints,
-providing simplified access to functionality in Monnify
-"""
-
-from monnifyease.apis import (
-    customer_reserved_account,
-    transactions
-)
-
-
-class Monnify:
-    """Monnify acts as a wrapper around various client APIs to
-    interact with the Monnify API
-    """
-    def __init__(self) -> None:
-        self.reserve_account = customer_reserved_account.CustomerReservedAccount()
-        self.transactions = transactions.Transactions()
+""" Wrapper classes for various Synchronous Monnify API endpoints,
+providing simplified access to functionality in Monnify
+"""
+
+from monnifyease.apis import (
+    banks,
+    customer_reserved_account,
+    settlements,
+    subaccounts,
+    transactions,
+    wallet
+)
+
+
+class Monnify:
+    """Monnify acts as a wrapper around various client APIs to
+    interact with the Monnify API
+    """
+    def __init__(self) -> None:
+        self.banks = banks.Banks()
+        self.reserve_account = customer_reserved_account.CustomerReservedAccount()
+        self.settlements = settlements.Settlements()
+        self.subaccounts = subaccounts.SubAccounts()
+        self.transactions = transactions.Transactions()
+        self.wallet = wallet.Wallet()
```

### Comparing `monnifyease-0.1.0/monnifyease/utils/convert_to_strings.py` & `monnifyease-0.2.0/monnifyease/utils/convert_to_strings.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-""" Implements the conversion of data types to strings """
-
-import logging
-from typing import Union
-from datetime import date, datetime
-
-from monnifyease.core._api_errors import TypeValueError
-
-
-logger = logging.getLogger(__name__)
-
-
-def convert_to_string(value: Union[bool, date, datetime, None]) -> Union[str, int, None]:
-    """
-    Convert the type of value to a string
-    :param value: The value to be converted
-
-    :raise TypeError: if the value is not a supported type
-
-    :return: The value as a string
-    :rtype: str
-    """
-    # each supported type is mapped to its corresponding conversion function
-    conversion_functions = {
-        bool: str,
-        date: lambda val: val.strftime("%Y-%m-%d"),
-        datetime: lambda val: val.strftime("%Y-%m-%d %H:%M:%S"),
-    }
-
-    if value is None:
-        return None
-    if type(value) in conversion_functions:
-        return conversion_functions[type(value)](value)
-    error_message = f"Unsupported type: {type(value)}. Expected type -bool, -date"
-    logger.error("Unsupported type: %s Expected type -bool, -date", {type(value)})
-    raise TypeValueError(error_message)
+""" Implements the conversion of data types to strings """
+
+import logging
+from typing import Union
+from datetime import date, datetime
+
+from monnifyease.core._api_errors import TypeValueError
+
+
+logger = logging.getLogger(__name__)
+
+
+def convert_to_string(value: Union[bool, date, datetime, None]) -> Union[str, int, None]:
+    """
+    Convert the type of value to a string
+    :param value: The value to be converted
+
+    :raise TypeError: if the value is not a supported type
+
+    :return: The value as a string
+    :rtype: str
+    """
+    # each supported type is mapped to its corresponding conversion function
+    conversion_functions = {
+        bool: str,
+        date: lambda val: val.strftime("%Y-%m-%d"),
+        datetime: lambda val: val.strftime("%Y-%m-%d %H:%M:%S"),
+    }
+
+    if value is None:
+        return None
+    if type(value) in conversion_functions:
+        return conversion_functions[type(value)](value)
+    error_message = f"Unsupported type: {type(value)}. Expected type -bool, -date"
+    logger.error("Unsupported type: %s Expected type -bool, -date", {type(value)})
+    raise TypeValueError(error_message)
```

### Comparing `monnifyease-0.1.0/pyproject.toml` & `monnifyease-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,84 @@
-[tool.poetry]
-name = "monnifyease"
-version = "0.1.0"
-description = "This is a Monnify API wrapper"
-authors = ["Peter Mbachu <doublep098@gmail.com>"]
-maintainers = [
-    "petermbachu.bincom <petermbachu.bincom@gmail.com>",
-]
-license = "MIT"
-readme = "README.md"
-keywords = ["moniepoint", "monnifyease", "monnify", "python", "api", "wrapper"]
-classifiers = [
-    "Programming Language :: Python :: 3.11",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Intended Audience :: Developers",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Development Status :: 5 - Production/Stable",
-    "Natural Language :: English",
-    "Topic :: Software Development :: Libraries :: Python Modules"
-]
-packages = [{include = "monnifyease"}]
-
-
-[license]
-text = "Copyright ©2024 Peter Mbachu"
-
-
-[tool.poetry.urls]
-"Homepage" = "https://github.com/cla-bit/MonnifyEase"
-"Source Code" = "https://github.com/cla-bit/MonnifyEase"
-"Documentation" = "https://monnifyease.readthedocs.io/en/latest/"
-"Bug Tracker" = "https://github.com/cla-bit/MonnifyEase/issues"
-
-
-[tool.poetry.dependencies]
-python = "^3.9"
-aiohttp = "^3.8"
-requests = "^2.31"
-python-decouple = "^3.8"
-
-
-[tool.poetry.group.docs.dependencies]
-pdflatex = "^0.1.3"
-sphinx = "^7.2.6"
-sphinx-rtd-theme = "^2.0.0"
-sphinxawesome-theme = "^5.1.1"
-sphinx-autobuild = "^2024.2.4"
-
-
-[tool.poetry.group.dev.dependencies]
-black = "^24.2"
-pylint = "^3.1"
-
-
-[tool.poetry.group.test.dependencies]
-pytest = "^8.0"
-responses = "^0.25"
-pytest-asyncio = "^0.23"
-aioresponses = "^0.7"
-
-
-[tool.pytest.ini_options]
-testpaths = ["tests"]
-addopts = "--doctest-modules"
-
-
-[tool.black]
-target-version = ['py310', 'py311']
-include = '\.pyi?$'
-
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "monnifyease"
+version = "0.2.0"
+description = "This is a Monnify API wrapper"
+authors = ["Peter Mbachu <doublep098@gmail.com>"]
+maintainers = [
+    "petermbachu.bincom <petermbachu.bincom@gmail.com>",
+]
+license = "MIT"
+readme = "README.md"
+keywords = ["moniepoint", "monnifyease", "monnify", "python", "api", "wrapper"]
+classifiers = [
+    "Programming Language :: Python :: 3.11",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Intended Audience :: Developers",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Development Status :: 5 - Production/Stable",
+    "Natural Language :: English",
+    "Topic :: Software Development :: Libraries :: Python Modules"
+]
+packages = [{include = "monnifyease"}]
+
+
+[license]
+text = "Copyright ©2024 Peter Mbachu"
+
+
+[tool.poetry.urls]
+"Homepage" = "https://github.com/cla-bit/MonnifyEase"
+"Source Code" = "https://github.com/cla-bit/MonnifyEase"
+"Documentation" = "https://monnifyease.readthedocs.io/en/latest/"
+"Bug Tracker" = "https://github.com/cla-bit/MonnifyEase/issues"
+
+
+[tool.poetry.dependencies]
+python = "^3.9"
+aiohttp = "^3.8"
+requests = "^2.31"
+python-decouple = "^3.8"
+
+
+[tool.poetry.group.docs.dependencies]
+pdflatex = "^0.1.3"
+sphinx = "^7.2.6"
+sphinx-rtd-theme = "^2.0.0"
+sphinxawesome-theme = "^5.1.1"
+sphinx-autobuild = "^2024.2.4"
+
+
+[tool.poetry.group.dev.dependencies]
+black = "^24.2"
+pylint = "^3.1"
+python-semantic-release = "^9.0"
+
+
+[tool.poetry.group.test.dependencies]
+pytest = "^8.0"
+pytest-cov = "^5.0"
+responses = "^0.25"
+pytest-asyncio = "^0.23"
+aioresponses = "^0.7"
+
+
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+addopts = "--doctest-modules"
+
+
+[tool.black]
+target-version = ['py310', 'py311']
+include = '\.pyi?$'
+
+
+[tool.semantic_release]
+version_toml = ["pyproject.toml:tool.poetry.version"]  # version location
+branch = "main"  # branch to make release of
+changelog_file = "CHANGELOG.md"  # changelog file
+build_command = "pip install poetry && poetry build"  # build dist
+
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `monnifyease-0.1.0/PKG-INFO` & `monnifyease-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monnifyease
-Version: 0.1.0
+Version: 0.2.0
 Summary: This is a Monnify API wrapper
 License: MIT
 Keywords: moniepoint,monnifyease,monnify,python,api,wrapper
 Author: Peter Mbachu
 Author-email: doublep098@gmail.com
 Maintainer: petermbachu.bincom
 Maintainer-email: petermbachu.bincom@gmail.com
```

