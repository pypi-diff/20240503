# Comparing `tmp/lecert-1.1.tar.gz` & `tmp/lecert-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lecert-1.1.tar", last modified: Wed May  1 09:19:43 2024, max compression
+gzip compressed data, was "lecert-1.2.tar", last modified: Fri May  3 10:41:23 2024, max compression
```

## Comparing `lecert-1.1.tar` & `lecert-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 09:19:43.958261 lecert-1.1/
--rw-rw-rw-   0        0        0     2912 2024-05-01 09:19:43.957290 lecert-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2463 2024-04-26 09:46:02.000000 lecert-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 09:19:43.930777 lecert-1.1/lecert/
--rw-rw-rw-   0        0        0     6363 2024-05-01 09:18:02.000000 lecert-1.1/lecert/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 09:19:43.956289 lecert-1.1/lecert.egg-info/
--rw-rw-rw-   0        0        0     2912 2024-05-01 09:19:43.000000 lecert-1.1/lecert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-05-01 09:19:43.000000 lecert-1.1/lecert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 09:19:43.000000 lecert-1.1/lecert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-01 09:19:43.000000 lecert-1.1/lecert.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-01 09:19:43.000000 lecert-1.1/lecert.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 09:19:43.958261 lecert-1.1/setup.cfg
--rw-rw-rw-   0        0        0      714 2024-05-01 09:18:11.000000 lecert-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:41:23.712098 lecert-1.2/
+-rw-rw-rw-   0        0        0     2971 2024-05-03 10:41:23.711099 lecert-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2522 2024-05-01 09:21:54.000000 lecert-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 10:41:23.702924 lecert-1.2/lecert/
+-rw-rw-rw-   0        0        0     6479 2024-05-03 10:39:04.000000 lecert-1.2/lecert/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 10:41:23.710098 lecert-1.2/lecert.egg-info/
+-rw-rw-rw-   0        0        0     2971 2024-05-03 10:41:23.000000 lecert-1.2/lecert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-05-03 10:41:23.000000 lecert-1.2/lecert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 10:41:23.000000 lecert-1.2/lecert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-03 10:41:23.000000 lecert-1.2/lecert.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-03 10:41:23.000000 lecert-1.2/lecert.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 10:41:23.712098 lecert-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      714 2024-05-03 10:40:32.000000 lecert-1.2/setup.py
```

### Comparing `lecert-1.1/PKG-INFO` & `lecert-1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecert
-Version: 1.1
+Version: 1.2
 Summary: Python module for obtaining SSL certificates from Let's Encrypt for self-service projects
 Home-page: https://github.com/EightShift/lecert
 Author: EightShift
 Author-email: the8shift@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,14 +53,15 @@
 The get_cert function takes the following optional arguments:
 - www: Whether to include the www subdomain in the certificate.
 - cert_lifetime: The lifetime of the certificate in days.
 - timeout: The timeout in seconds for the certificate issuance process.
 - force: Whether to force the certificate issuance even if the current certificate is still valid.
 - privkey_file_name: The name of the private key file.
 - cert_file_name: The name of the certificate file.
+- backup_time_format: Time format for backup directories.
 
 
 ## Example
 The following example shows how to use LeCert to obtain and maintain SSL certificates for a small web application:
 ```
 import lecert
 import schedule
```

### Comparing `lecert-1.1/README.md` & `lecert-1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 The get_cert function takes the following optional arguments:
 - www: Whether to include the www subdomain in the certificate.
 - cert_lifetime: The lifetime of the certificate in days.
 - timeout: The timeout in seconds for the certificate issuance process.
 - force: Whether to force the certificate issuance even if the current certificate is still valid.
 - privkey_file_name: The name of the private key file.
 - cert_file_name: The name of the certificate file.
+- backup_time_format: Time format for backup directories.
 
 
 ## Example
 The following example shows how to use LeCert to obtain and maintain SSL certificates for a small web application:
 ```
 import lecert
 import schedule
```

### Comparing `lecert-1.1/lecert/__init__.py` & `lecert-1.2/lecert/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,24 +63,24 @@
 		if os.path.exists(path):
 			if not created_datetime:
 				created_datetime = datetime.fromtimestamp(os.path.getctime(path)).strftime(backup_time_format)
 			
 			backup_dir = os.path.join(backups_dir, f'{created_datetime}~{current_datetime}')
 			os.makedirs(backup_dir, exist_ok=True)
 
-			backup_path = os.path.join(backup_dir, path)
+			backup_path = os.path.join(backup_dir, name)
 			try:
 				shutil.move(path, backup_path)
 			except:
 				pass
 
 		with open(path, 'w') as _file:
 			_file.write(data)
 
-
+_backup_saving('./', ('cert_file_name', 'finalized_order.fullchain_pem'), ('privkey_file_name', 'privkey_pem.decode()'))
 def _select_http01_challb(auths):
 	for chall_body in auths.body.challenges:
 		if isinstance(chall_body.chall, challenges.HTTP01):
 			return chall_body
 
 
 def _generate_privkey_pem():
@@ -100,15 +100,14 @@
 		with open(challenge_token_path, 'w') as challenge_token_file:
 			challenge_token_file.write(validation)
 
 		# Let the CA server know that we are ready for the challenge.
 		client_acme.answer_challenge(challb, response)
 
 
-
 @contextmanager
 def _get_acme_challenge_dir(certs_dir):
 	acme_challenge_dir = os.path.join(certs_dir, ACME_CHALLENGE_DIR_NAME)
 	try:
 		os.makedirs(acme_challenge_dir, exist_ok=True)
 
 		yield acme_challenge_dir
@@ -127,15 +126,14 @@
 	regr = client_acme.new_account(messages.NewRegistration.from_data(email=email, terms_of_service_agreed=True))
 	try:
 		yield client_acme
 	finally:
 		client_acme.deactivate_registration(regr)
 
 
-
 def get_cert(certs_dir, email, domains, www=True, cert_lifetime=30, timeout=150, force=False, privkey_file_name='privkey.pem', cert_file_name='cert.pem', backup_time_format='%Y-%m-%d_%H-%M-%S'):
 	"""Obtains a new certificate from Let's Encrypt.
 
 	Args:
 		certs_dir (str): The directory where the certificates are stored.
 		email (str): The email address of the account.
 		domains (list): The list of domains to include in the certificate.
```

### Comparing `lecert-1.1/lecert.egg-info/PKG-INFO` & `lecert-1.2/lecert.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lecert
-Version: 1.1
+Version: 1.2
 Summary: Python module for obtaining SSL certificates from Let's Encrypt for self-service projects
 Home-page: https://github.com/EightShift/lecert
 Author: EightShift
 Author-email: the8shift@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,14 +53,15 @@
 The get_cert function takes the following optional arguments:
 - www: Whether to include the www subdomain in the certificate.
 - cert_lifetime: The lifetime of the certificate in days.
 - timeout: The timeout in seconds for the certificate issuance process.
 - force: Whether to force the certificate issuance even if the current certificate is still valid.
 - privkey_file_name: The name of the private key file.
 - cert_file_name: The name of the certificate file.
+- backup_time_format: Time format for backup directories.
 
 
 ## Example
 The following example shows how to use LeCert to obtain and maintain SSL certificates for a small web application:
 ```
 import lecert
 import schedule
```

### Comparing `lecert-1.1/setup.py` & `lecert-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lecert',
-    version='1.1',
+    version='1.2',
     description='Python module for obtaining SSL certificates from Let\'s Encrypt for self-service projects',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='EightShift',
     author_email='the8shift@gmail.com',
     url='https://github.com/EightShift/lecert',
     packages=find_packages(),
```

