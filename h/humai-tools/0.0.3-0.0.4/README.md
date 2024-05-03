# Comparing `tmp/humai_tools-0.0.3.tar.gz` & `tmp/humai_tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humai_tools-0.0.3.tar", last modified: Wed Apr 24 18:15:13 2024, max compression
+gzip compressed data, was "humai_tools-0.0.4.tar", last modified: Fri May  3 02:54:07 2024, max compression
```

## Comparing `humai_tools-0.0.3.tar` & `humai_tools-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 18:15:13.655400 humai_tools-0.0.3/
--rw-rw-rw-   0        0        0      743 2024-04-24 18:15:13.654399 humai_tools-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       68 2023-07-28 14:38:40.000000 humai_tools-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 18:15:13.643400 humai_tools-0.0.3/humai_tools/
--rw-rw-rw-   0        0        0      235 2024-04-24 15:13:36.000000 humai_tools-0.0.3/humai_tools/__init__.py
--rw-rw-rw-   0        0        0    13945 2024-04-24 18:11:08.000000 humai_tools-0.0.3/humai_tools/campus.py
--rw-rw-rw-   0        0        0     8610 2024-04-20 20:45:50.000000 humai_tools-0.0.3/humai_tools/directus.py
--rw-rw-rw-   0        0        0    15257 2023-07-28 14:38:40.000000 humai_tools-0.0.3/humai_tools/mp.py
--rw-rw-rw-   0        0        0     6065 2024-04-24 18:13:09.000000 humai_tools-0.0.3/humai_tools/permissions.py
--rw-rw-rw-   0        0        0      704 2024-04-24 18:03:20.000000 humai_tools-0.0.3/humai_tools/settings.py
--rw-rw-rw-   0        0        0     5912 2024-04-24 15:16:31.000000 humai_tools-0.0.3/humai_tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 18:15:13.653400 humai_tools-0.0.3/humai_tools.egg-info/
--rw-rw-rw-   0        0        0      743 2024-04-24 18:15:13.000000 humai_tools-0.0.3/humai_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-04-24 18:15:13.000000 humai_tools-0.0.3/humai_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 18:15:13.000000 humai_tools-0.0.3/humai_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2024-04-24 18:15:13.000000 humai_tools-0.0.3/humai_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-24 18:15:13.000000 humai_tools-0.0.3/humai_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 18:15:13.655400 humai_tools-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1112 2024-04-24 15:28:54.000000 humai_tools-0.0.3/setup.py
+drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2024-05-03 02:54:07.809797 humai_tools-0.0.4/
+-rw-rw-r--   0 mat       (1000) mat       (1000)      386 2024-05-03 02:54:07.809797 humai_tools-0.0.4/PKG-INFO
+-rw-rw-r--   0 mat       (1000) mat       (1000)       65 2023-06-28 05:04:08.000000 humai_tools-0.0.4/README.md
+drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2024-05-03 02:54:07.809797 humai_tools-0.0.4/humai_tools/
+-rw-rw-r--   0 mat       (1000) mat       (1000)      146 2023-06-28 05:04:08.000000 humai_tools-0.0.4/humai_tools/__init__.py
+-rw-rw-r--   0 mat       (1000) mat       (1000)     6278 2024-05-03 02:40:25.000000 humai_tools-0.0.4/humai_tools/directus.py
+-rw-rw-r--   0 mat       (1000) mat       (1000)      888 2023-08-18 15:59:22.000000 humai_tools-0.0.4/humai_tools/models.py
+-rw-rw-r--   0 mat       (1000) mat       (1000)    14804 2023-06-28 05:04:08.000000 humai_tools-0.0.4/humai_tools/mp.py
+-rw-rw-r--   0 mat       (1000) mat       (1000)      575 2023-06-28 05:04:08.000000 humai_tools-0.0.4/humai_tools/utils.py
+drwxrwxr-x   0 mat       (1000) mat       (1000)        0 2024-05-03 02:54:07.809797 humai_tools-0.0.4/humai_tools.egg-info/
+-rw-rw-r--   0 mat       (1000) mat       (1000)      386 2024-05-03 02:54:07.000000 humai_tools-0.0.4/humai_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mat       (1000) mat       (1000)      301 2024-05-03 02:54:07.000000 humai_tools-0.0.4/humai_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)        1 2024-05-03 02:54:07.000000 humai_tools-0.0.4/humai_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)       54 2024-05-03 02:54:07.000000 humai_tools-0.0.4/humai_tools.egg-info/requires.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)       12 2024-05-03 02:54:07.000000 humai_tools-0.0.4/humai_tools.egg-info/top_level.txt
+-rw-rw-r--   0 mat       (1000) mat       (1000)       38 2024-05-03 02:54:07.809797 humai_tools-0.0.4/setup.cfg
+-rw-rw-r--   0 mat       (1000) mat       (1000)      701 2024-05-03 02:53:49.000000 humai_tools-0.0.4/setup.py
```

### Comparing `humai_tools-0.0.3/humai_tools/mp.py` & `humai_tools-0.0.4/humai_tools/mp.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,454 +1,454 @@
-import os
-from datetime import datetime
-import mercadopago
-import requests
-
-token = os.getenv("MERCADOPAGO_TOKEN", "")
-suscription_keyword = os.getenv("SUSCRIPTION_KEYWORD", "")
-
-headers = {
-    "accept": "application/json",
-    "Authorization": f"Bearer {token}",
-}
-
-base_url = "https://api.mercadopago.com"
-
-
-def get_orders(offset="", limit="10"):
-    """get history of orders"""
-    params = (("offset", offset), ("limit", limit))
-    response = requests.get(
-        f"{base_url}/merchant_orders", headers=headers, params=params
-    )
-    data = response.json()
-    # data = sorted([d for d in data['elements']], key=lambda x: datetime.fromisoformat(x['date_created']))
-    return data
-
-
-def get_suscriptions():
-    """get suscription by email"""
-    response = requests.get(
-        f"https://api.mercadopago.com/preapproval/search?", headers=headers,
-    )
-    data = response.json()
-    # data = sorted([d for d in data['elements']], key=lambda x: datetime.fromisoformat(x['date_created']))
-    return data
-
-
-def get_payer_info(payment_id) -> dict:
-    """All fields but email can be empty"""
-    r = requests.get(f"{base_url}/v1/payments/{payment_id}", headers=headers)
-    data = r.json()
-    print(f"INFO Payload From {base_url}/v1/payments/{payment_id}\n{data}")
-
-    # TODO Improve error handling
-    if "message" in data.keys():
-        return data["message"]
-    else:
-        return data
-
-
-def get_suscription(suscription_id: id) -> dict:
-    """
-    https://www.mercadopago.com.ar/developers/en/reference/subscriptions/_preapproval_id/get
-    """
-    r = requests.get(f"{base_url}/preapproval/{suscription_id}", headers=headers)
-    data = r.json()
-    print(f"INFO Payload From {base_url}/preapproval/{suscription_id}\n{data}")
-
-    # TODO Improve error handling
-    if "message" in data.keys():
-        return data["message"]
-    else:
-        return data
-
-
-def search_suscriptions(params: dict, verbose=False) -> dict:
-    """
-    Use payer_id, payer_email, preapproval_plan_id
-    https://www.mercadopago.com.ar/developers/en/reference/subscriptions/_preapproval_search/get 
-    """
-    r = requests.get(f"{base_url}/preapproval/search", headers=headers, params=params)
-    data = r.json()
-    if verbose:
-        print(f"INFO Payload From {base_url}/preapproval/search\n{data}")
-
-    # TODO Improve error handling
-    if "message" in data.keys():
-        return data["message"]
-    else:
-        return data
-
-
-def get_merchant_info(payment_id) -> dict:
-    """"""
-    r = requests.get(f"{base_url}/merchant_orders/{payment_id}", headers=headers)
-    data = r.json()
-    print(f"INFO Payload From {base_url}/merchant_orders/{payment_id}\n{data}")
-
-    # TODO Improve error handling
-    if "message" in data.keys():
-        return data["message"]
-    else:
-        return data
-
-
-def get_suscript_id_info(
-    id: int, offset="", limit="10",
-):
-    ## TODO: no se como difiere de payer
-    params = (("offset", offset), ("limit", limit))
-    response = requests.get(
-        f"{base_url}/subscriptions/{id}", headers=headers, params=params
-    )
-    data = response.json()
-    return data
-
-
-def is_valid_suscription(external_reference: str) -> bool:
-    """Depende de mantener este protocolo en las suscripciones"""
-    return suscription_keyword in external_reference.lower()
-
-
-def is_active_suscription(status: str) -> bool:
-    return status != "cancelled"
-
-
-def is_mail_active_suscription(mail: str) -> bool:
-    data = search_suscriptions({"payer_email": mail})
-    return any(
-        [
-            is_active_suscription(r)
-            for r in data["results"]
-            if is_valid_suscription(r["external_reference"])
-        ]
-    )
-
-
-def create_course_payment(
-        product_id,
-        name,
-        description,
-        img_url,
-        price,
-        external_reference,
-        notification_url,
-        redirect_url,
-        conversion_id,
-        conversion_label,
-) -> str:
-    # https://www.mercadopago.com.ar/developers/en/reference/preferences/_checkout_preferences/post
-    product_data = {
-        "items": [
-            {
-                "id": product_id,
-                "title": name,
-                "description": description,
-                "picture_url": img_url,
-                "quantity": 1,
-                "currency_id": "ARS",
-                "unit_price": price,
-                "item_category": "learnings",
-            }
-        ],
-        'payment_methods': {'installments':6, 'default_installments':6},
-        "external_reference": external_reference,
-        "back_urls": {
-            "success": redirect_url,
-            "pending": redirect_url,
-            "failure": redirect_url,
-        },
-        "notification_url": notification_url,
-        "tracks": [{'type':'google_ad', 'values': {'conversion_id':conversion_id, 'conversion_label': conversion_label}}]
-
-    }
-    response = requests.post(f"{base_url}/checkout/preferences", headers=headers, json=product_data)
-
-    if response.status_code == 201:
-        data = response.json()
-        print(f'external reference from response = {data["external_reference"]}')
-        payment_url = data["init_point"]
-        return payment_url
-    else:
-        print(f"Failed while trying to create payment {name}"
-              f" with status code {response.status_code} from MP API. Info: {response.text}")
-
-
-def create_suscription(
-    client: mercadopago.SDK,
-    suscription_name,
-    external_reference,
-    payer_email,
-    price,
-    notification_url,
-    redirect_url,
-    conversion_id,
-    conversion_label,
-):
-    product_data = {
-        "reason": suscription_name,
-        "external_reference": external_reference,
-        "payer_email": payer_email,
-        "auto_recurring": {
-            "frequency": 1,
-            "frequency_type": "months",
-            "repetitions": 12,
-            "transaction_amount": price,
-            "currency_id": "ARS",
-            "notification_url": notification_url,
-        },
-        "tracks": [{'type':'google_ad', 'values': {'conversion_id':conversion_id, 'conversion_label': conversion_label}}],
-        "back_url": redirect_url,
-    }
-
-    preference_response = client.subscription().create(product_data)
-    preference = preference_response["response"]
-    try:
-        payment_url = preference["init_point"]
-        return payment_url
-    except Exception as e:
-        print(f"ERROR {e} : {preference_response}")
-
-
-def create_plan_subscription(
-    subscription_name,
-    external_reference,
-    payer_email,
-    price,
-    notification_url,
-    redirect_url,
-    conversion_id,
-    conversion_label,
-) -> str:
-    """
-
-    Creates a new plan subscription that it is visible in UI from MP account.
-
-    Args:
-        subscription_name: str
-        external_reference: str
-        payer_email: str
-        price: float
-        notification_url: str
-        redirect_url: str
-
-    Returns
-        payment_url: str - a link to make the first payment of the mp plan subscription
-    """
-
-    product_data = {
-        "reason": subscription_name,
-        "external_reference": external_reference,
-        "payer_email": payer_email,
-        "auto_recurring": {
-            "frequency": 1,
-            "frequency_type": "months",
-            "repetitions": 12,
-            "start_date": datetime.now().isoformat(),
-            "transaction_amount": price,
-            "currency_id": "ARS",
-            "notification_url": notification_url,
-        },
-        "tracks": [{'type':'google_ad', 'values': {'conversion_id':conversion_id, 'conversion_label': conversion_label}}],
-        "back_url": redirect_url,
-    }
-
-    response = requests.post(f"{base_url}/preapproval_plan", headers=headers, json=product_data)
-
-    if response.status_code == 201:
-        data = response.json()
-        payment_url = data["init_point"]
-        return payment_url
-    else:
-        print(f"Failed while trying to create subscription {subscription_name} for {payer_email}"
-              f" with status code {response.status_code} from MP API. Info: {response.text}")
-
-
-def get_plan_subscription_by_id(subscription_id: str) -> dict:
-    """
-    Args:
-        subscription_id: path parameter of the mp api get /preapproval_plan request to identify subscription
-
-    Returns:
-        subscription_data: dictionary containing full info about plan subscription
-
-        subscription_data example:
-            {
-            "id": "3g198237912873982342371239d",
-            "back_url": "",
-            "collector_id": 12312312,
-            "application_id": 123123123,
-            "reason": "",
-            "status": "cancelled",
-            "date_created": "2022-12-21T18:28:34.936-04:00",
-            "last_modified": "2022-12-21T18:33:23.636-04:00",
-            "init_point": "",
-            "auto_recurring": {
-                                "frequency": 1,
-                                "frequency_type": "months",
-                                "transaction_amount": 123123,
-                                "currency_id": "ARS",
-                                "repetitions": 12,
-                                "free_trial": {
-                                    "frequency": 1,
-                                    "frequency_type": "months",
-                                    "first_invoice_offset": 30
-                                },
-                                "billing_day": 10,
-                                "billing_day_proportional": true,
-                                "transaction_amount_proportional": 2.00
-            },
-            "payment_methods_allowed": {
-                                        "payment_types": [{}],
-                                        "payment_methods": [{}]
-                                       }
-            }
-
-    """
-    response = requests.get(f"{base_url}/preapproval_plan/{subscription_id}", headers=headers)
-    if response.status_code == 200:
-        subscription_data = response.json()
-        return subscription_data
-    elif response.status_code == 404:
-        print(f"Plan Subscription does not exists")
-    else:
-        print(f"Something unexpected has happened while trying to get plan subscription"
-              f" with id {subscription_id}")
-
-
-def search_plan_subscriptions(
-        status: str = None,
-        offset: int = 0,
-        limit: int = 20,
-        keyword: str = None
-):
-    """
-
-    Args:
-        status: str - valid statuses are: active, inactive or cancelled
-        offset: int - start of the list based on total count
-        limit: int - end of the list
-        keyword: str- the so called 'q' parameter (keyword to search by 'reason' , 'back_url', 'external_reference')
-
-    Returns:
-
-    """
-    query_parameters_raw = {
-        "status": status,
-        "offset": offset,
-        "limit": limit,
-        "q": keyword
-    }
-    query_parameters = {parameter: value for parameter, value in query_parameters_raw.items() if value is not None}
-    response = requests.get(f"{base_url}/preapproval_plan/search", headers=headers, params=query_parameters)
-    if response.status_code == 200:
-        search_result = response.json()
-        return search_result
-    else:
-        print(f"Request has unexpected response.\nStatus: {response.status_code}"
-              f"\nInfo: {response.text}")
-
-
-def update_plan_subscription(subscription_id: str, new_status: str = "active", new_external_reference: str = None) -> dict:
-    """
-    Plan Subscription with cancelled status can not be updated.
-
-    Args:
-        subscription_id: identifier for the subscription to be updated
-        new_status: valid statuses are: active, inactive or cancelled.
-        new_external_reference:
-
-    Returns:
-        updated_data: dictionary containing the updated subscription information.
-    """
-    body_raw = {
-        "status": new_status,
-        "external_reference": new_external_reference
-    }
-    body = {parameter: value for parameter, value in body_raw.items() if value is not None}
-
-    response = requests.put(f"{base_url}/preapproval_plan/{subscription_id}", headers=headers, json=body)
-    if response.status_code == 200:
-        updated_data = response.json()
-        return updated_data
-    else:
-        print(f"Request has unexpected response.\nStatus: {response.status_code}"
-              f"\nInfo: {response.text}")
-
-
-def cancel_or_pause_subscription(subscription_id: str, status: str = "cancelled") -> dict:
-    """
-
-    Args:
-        subscription_id: str : example -> 2c938084850b39e2018512e0706a044f
-        status: str: only 2 options here: cancelled | paused
-
-    Returns:
-        data: a dictionary containing the response of PUT requesting change of subscription status
-
-    Example:
-        request url: ""
-        response status code: 200
-        response body:
-        {
-            "id": "drfdfsf",
-            "payer_id": 234242342,
-            "payer_email": "",
-            "back_url": "",
-            "collector_id": 234234,
-            "application_id": 234234324324,
-            "status": "cancelled",
-            "reason": "- 95% Humai Educación 20232342323",
-            "external_reference": "432424242",
-            "date_created": "2022-12-14T19:06:23.320-04:00",
-            "last_modified": "2022-12-16T13:07:03.709-04:00",
-            "auto_recurring": {
-                "frequency": 1,
-                "frequency_type": "months",
-                "transaction_amount": 250.00,
-                "currency_id": "ARS",
-                "end_date": "2023-12-14T19:06:23.320-04:00",
-                "free_trial": {
-                    "frequency": 1,
-                    "first_invoice_offset": 30,
-                    "frequency_type": "months"
-                }
-            },
-            "summarized": {
-                "quotas": null,
-                "charged_quantity": null,
-                "pending_charge_quantity": null,
-                "charged_amount": null,
-                "pending_charge_amount": null,
-                "semaphore": null,
-                "last_charged_date": null,
-                "last_charged_amount": null
-            },
-            "payment_method_id": null,
-            "first_invoice_offset": 30
-        }
-    """
-
-    body = {"status": status}
-    response = requests.put(f"{base_url}/preapproval/{subscription_id}", headers=headers, json=body)
-    data = response.json()
-
-    return data
-
-
-def get_all_active_suscriptions():
-    limit = 100
-    offset = 0
-    suscriptions = []
-    while True:
-        try:
-            params = {"status": 'authorized', 'limit':limit, 'offset':offset}
-            r = requests.get(f"{base_url}/preapproval/search", headers=headers, params=params)
-            data = r.json()['results']
-            if len(data) == 0:
-                break
-            suscriptions.extend(data)
-            offset += limit
-        except:
-            break
+import os
+from datetime import datetime
+import mercadopago
+import requests
+
+token = os.getenv("MERCADOPAGO_TOKEN", "")
+suscription_keyword = os.getenv("SUSCRIPTION_KEYWORD", "")
+
+headers = {
+    "accept": "application/json",
+    "Authorization": f"Bearer {token}",
+}
+
+base_url = "https://api.mercadopago.com"
+
+
+def get_orders(offset="", limit="10"):
+    """get history of orders"""
+    params = (("offset", offset), ("limit", limit))
+    response = requests.get(
+        f"{base_url}/merchant_orders", headers=headers, params=params
+    )
+    data = response.json()
+    # data = sorted([d for d in data['elements']], key=lambda x: datetime.fromisoformat(x['date_created']))
+    return data
+
+
+def get_suscriptions():
+    """get suscription by email"""
+    response = requests.get(
+        f"https://api.mercadopago.com/preapproval/search?", headers=headers,
+    )
+    data = response.json()
+    # data = sorted([d for d in data['elements']], key=lambda x: datetime.fromisoformat(x['date_created']))
+    return data
+
+
+def get_payer_info(payment_id) -> dict:
+    """All fields but email can be empty"""
+    r = requests.get(f"{base_url}/v1/payments/{payment_id}", headers=headers)
+    data = r.json()
+    print(f"INFO Payload From {base_url}/v1/payments/{payment_id}\n{data}")
+
+    # TODO Improve error handling
+    if "message" in data.keys():
+        return data["message"]
+    else:
+        return data
+
+
+def get_suscription(suscription_id: id) -> dict:
+    """
+    https://www.mercadopago.com.ar/developers/en/reference/subscriptions/_preapproval_id/get
+    """
+    r = requests.get(f"{base_url}/preapproval/{suscription_id}", headers=headers)
+    data = r.json()
+    print(f"INFO Payload From {base_url}/preapproval/{suscription_id}\n{data}")
+
+    # TODO Improve error handling
+    if "message" in data.keys():
+        return data["message"]
+    else:
+        return data
+
+
+def search_suscriptions(params: dict, verbose=False) -> dict:
+    """
+    Use payer_id, payer_email, preapproval_plan_id
+    https://www.mercadopago.com.ar/developers/en/reference/subscriptions/_preapproval_search/get 
+    """
+    r = requests.get(f"{base_url}/preapproval/search", headers=headers, params=params)
+    data = r.json()
+    if verbose:
+        print(f"INFO Payload From {base_url}/preapproval/search\n{data}")
+
+    # TODO Improve error handling
+    if "message" in data.keys():
+        return data["message"]
+    else:
+        return data
+
+
+def get_merchant_info(payment_id) -> dict:
+    """"""
+    r = requests.get(f"{base_url}/merchant_orders/{payment_id}", headers=headers)
+    data = r.json()
+    print(f"INFO Payload From {base_url}/merchant_orders/{payment_id}\n{data}")
+
+    # TODO Improve error handling
+    if "message" in data.keys():
+        return data["message"]
+    else:
+        return data
+
+
+def get_suscript_id_info(
+    id: int, offset="", limit="10",
+):
+    ## TODO: no se como difiere de payer
+    params = (("offset", offset), ("limit", limit))
+    response = requests.get(
+        f"{base_url}/subscriptions/{id}", headers=headers, params=params
+    )
+    data = response.json()
+    return data
+
+
+def is_valid_suscription(external_reference: str) -> bool:
+    """Depende de mantener este protocolo en las suscripciones"""
+    return suscription_keyword in external_reference.lower()
+
+
+def is_active_suscription(status: str) -> bool:
+    return status != "cancelled"
+
+
+def is_mail_active_suscription(mail: str) -> bool:
+    data = search_suscriptions({"payer_email": mail})
+    return any(
+        [
+            is_active_suscription(r)
+            for r in data["results"]
+            if is_valid_suscription(r["external_reference"])
+        ]
+    )
+
+
+def create_course_payment(
+        product_id,
+        name,
+        description,
+        img_url,
+        price,
+        external_reference,
+        notification_url,
+        redirect_url,
+        conversion_id,
+        conversion_label,
+) -> str:
+    # https://www.mercadopago.com.ar/developers/en/reference/preferences/_checkout_preferences/post
+    product_data = {
+        "items": [
+            {
+                "id": product_id,
+                "title": name,
+                "description": description,
+                "picture_url": img_url,
+                "quantity": 1,
+                "currency_id": "ARS",
+                "unit_price": price,
+                "item_category": "learnings",
+            }
+        ],
+        'payment_methods': {'installments':6, 'default_installments':6},
+        "external_reference": external_reference,
+        "back_urls": {
+            "success": redirect_url,
+            "pending": redirect_url,
+            "failure": redirect_url,
+        },
+        "notification_url": notification_url,
+        "tracks": [{'type':'google_ad', 'values': {'conversion_id':conversion_id, 'conversion_label': conversion_label}}]
+
+    }
+    response = requests.post(f"{base_url}/checkout/preferences", headers=headers, json=product_data)
+
+    if response.status_code == 201:
+        data = response.json()
+        print(f'external reference from response = {data["external_reference"]}')
+        payment_url = data["init_point"]
+        return payment_url
+    else:
+        print(f"Failed while trying to create payment {name}"
+              f" with status code {response.status_code} from MP API. Info: {response.text}")
+
+
+def create_suscription(
+    client: mercadopago.SDK,
+    suscription_name,
+    external_reference,
+    payer_email,
+    price,
+    notification_url,
+    redirect_url,
+    conversion_id,
+    conversion_label,
+):
+    product_data = {
+        "reason": suscription_name,
+        "external_reference": external_reference,
+        "payer_email": payer_email,
+        "auto_recurring": {
+            "frequency": 1,
+            "frequency_type": "months",
+            "repetitions": 12,
+            "transaction_amount": price,
+            "currency_id": "ARS",
+            "notification_url": notification_url,
+        },
+        "tracks": [{'type':'google_ad', 'values': {'conversion_id':conversion_id, 'conversion_label': conversion_label}}],
+        "back_url": redirect_url,
+    }
+
+    preference_response = client.subscription().create(product_data)
+    preference = preference_response["response"]
+    try:
+        payment_url = preference["init_point"]
+        return payment_url
+    except Exception as e:
+        print(f"ERROR {e} : {preference_response}")
+
+
+def create_plan_subscription(
+    subscription_name,
+    external_reference,
+    payer_email,
+    price,
+    notification_url,
+    redirect_url,
+    conversion_id,
+    conversion_label,
+) -> str:
+    """
+
+    Creates a new plan subscription that it is visible in UI from MP account.
+
+    Args:
+        subscription_name: str
+        external_reference: str
+        payer_email: str
+        price: float
+        notification_url: str
+        redirect_url: str
+
+    Returns
+        payment_url: str - a link to make the first payment of the mp plan subscription
+    """
+
+    product_data = {
+        "reason": subscription_name,
+        "external_reference": external_reference,
+        "payer_email": payer_email,
+        "auto_recurring": {
+            "frequency": 1,
+            "frequency_type": "months",
+            "repetitions": 12,
+            "start_date": datetime.now().isoformat(),
+            "transaction_amount": price,
+            "currency_id": "ARS",
+            "notification_url": notification_url,
+        },
+        "tracks": [{'type':'google_ad', 'values': {'conversion_id':conversion_id, 'conversion_label': conversion_label}}],
+        "back_url": redirect_url,
+    }
+
+    response = requests.post(f"{base_url}/preapproval_plan", headers=headers, json=product_data)
+
+    if response.status_code == 201:
+        data = response.json()
+        payment_url = data["init_point"]
+        return payment_url
+    else:
+        print(f"Failed while trying to create subscription {subscription_name} for {payer_email}"
+              f" with status code {response.status_code} from MP API. Info: {response.text}")
+
+
+def get_plan_subscription_by_id(subscription_id: str) -> dict:
+    """
+    Args:
+        subscription_id: path parameter of the mp api get /preapproval_plan request to identify subscription
+
+    Returns:
+        subscription_data: dictionary containing full info about plan subscription
+
+        subscription_data example:
+            {
+            "id": "3g198237912873982342371239d",
+            "back_url": "",
+            "collector_id": 12312312,
+            "application_id": 123123123,
+            "reason": "",
+            "status": "cancelled",
+            "date_created": "2022-12-21T18:28:34.936-04:00",
+            "last_modified": "2022-12-21T18:33:23.636-04:00",
+            "init_point": "",
+            "auto_recurring": {
+                                "frequency": 1,
+                                "frequency_type": "months",
+                                "transaction_amount": 123123,
+                                "currency_id": "ARS",
+                                "repetitions": 12,
+                                "free_trial": {
+                                    "frequency": 1,
+                                    "frequency_type": "months",
+                                    "first_invoice_offset": 30
+                                },
+                                "billing_day": 10,
+                                "billing_day_proportional": true,
+                                "transaction_amount_proportional": 2.00
+            },
+            "payment_methods_allowed": {
+                                        "payment_types": [{}],
+                                        "payment_methods": [{}]
+                                       }
+            }
+
+    """
+    response = requests.get(f"{base_url}/preapproval_plan/{subscription_id}", headers=headers)
+    if response.status_code == 200:
+        subscription_data = response.json()
+        return subscription_data
+    elif response.status_code == 404:
+        print(f"Plan Subscription does not exists")
+    else:
+        print(f"Something unexpected has happened while trying to get plan subscription"
+              f" with id {subscription_id}")
+
+
+def search_plan_subscriptions(
+        status: str = None,
+        offset: int = 0,
+        limit: int = 20,
+        keyword: str = None
+):
+    """
+
+    Args:
+        status: str - valid statuses are: active, inactive or cancelled
+        offset: int - start of the list based on total count
+        limit: int - end of the list
+        keyword: str- the so called 'q' parameter (keyword to search by 'reason' , 'back_url', 'external_reference')
+
+    Returns:
+
+    """
+    query_parameters_raw = {
+        "status": status,
+        "offset": offset,
+        "limit": limit,
+        "q": keyword
+    }
+    query_parameters = {parameter: value for parameter, value in query_parameters_raw.items() if value is not None}
+    response = requests.get(f"{base_url}/preapproval_plan/search", headers=headers, params=query_parameters)
+    if response.status_code == 200:
+        search_result = response.json()
+        return search_result
+    else:
+        print(f"Request has unexpected response.\nStatus: {response.status_code}"
+              f"\nInfo: {response.text}")
+
+
+def update_plan_subscription(subscription_id: str, new_status: str = "active", new_external_reference: str = None) -> dict:
+    """
+    Plan Subscription with cancelled status can not be updated.
+
+    Args:
+        subscription_id: identifier for the subscription to be updated
+        new_status: valid statuses are: active, inactive or cancelled.
+        new_external_reference:
+
+    Returns:
+        updated_data: dictionary containing the updated subscription information.
+    """
+    body_raw = {
+        "status": new_status,
+        "external_reference": new_external_reference
+    }
+    body = {parameter: value for parameter, value in body_raw.items() if value is not None}
+
+    response = requests.put(f"{base_url}/preapproval_plan/{subscription_id}", headers=headers, json=body)
+    if response.status_code == 200:
+        updated_data = response.json()
+        return updated_data
+    else:
+        print(f"Request has unexpected response.\nStatus: {response.status_code}"
+              f"\nInfo: {response.text}")
+
+
+def cancel_or_pause_subscription(subscription_id: str, status: str = "cancelled") -> dict:
+    """
+
+    Args:
+        subscription_id: str : example -> 2c938084850b39e2018512e0706a044f
+        status: str: only 2 options here: cancelled | paused
+
+    Returns:
+        data: a dictionary containing the response of PUT requesting change of subscription status
+
+    Example:
+        request url: ""
+        response status code: 200
+        response body:
+        {
+            "id": "drfdfsf",
+            "payer_id": 234242342,
+            "payer_email": "",
+            "back_url": "",
+            "collector_id": 234234,
+            "application_id": 234234324324,
+            "status": "cancelled",
+            "reason": "- 95% Humai Educación 20232342323",
+            "external_reference": "432424242",
+            "date_created": "2022-12-14T19:06:23.320-04:00",
+            "last_modified": "2022-12-16T13:07:03.709-04:00",
+            "auto_recurring": {
+                "frequency": 1,
+                "frequency_type": "months",
+                "transaction_amount": 250.00,
+                "currency_id": "ARS",
+                "end_date": "2023-12-14T19:06:23.320-04:00",
+                "free_trial": {
+                    "frequency": 1,
+                    "first_invoice_offset": 30,
+                    "frequency_type": "months"
+                }
+            },
+            "summarized": {
+                "quotas": null,
+                "charged_quantity": null,
+                "pending_charge_quantity": null,
+                "charged_amount": null,
+                "pending_charge_amount": null,
+                "semaphore": null,
+                "last_charged_date": null,
+                "last_charged_amount": null
+            },
+            "payment_method_id": null,
+            "first_invoice_offset": 30
+        }
+    """
+
+    body = {"status": status}
+    response = requests.put(f"{base_url}/preapproval/{subscription_id}", headers=headers, json=body)
+    data = response.json()
+
+    return data
+
+
+def get_all_active_suscriptions():
+    limit = 100
+    offset = 0
+    suscriptions = []
+    while True:
+        try:
+            params = {"status": 'authorized', 'limit':limit, 'offset':offset}
+            r = requests.get(f"{base_url}/preapproval/search", headers=headers, params=params)
+            data = r.json()['results']
+            if len(data) == 0:
+                break
+            suscriptions.extend(data)
+            offset += limit
+        except:
+            break
     return suscriptions
```

