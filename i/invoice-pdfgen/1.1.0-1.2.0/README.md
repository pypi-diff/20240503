# Comparing `tmp/invoice_pdfgen-1.1.0.tar.gz` & `tmp/invoice_pdfgen-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invoice_pdfgen-1.1.0.tar", last modified: Fri May  3 15:04:42 2024, max compression
+gzip compressed data, was "invoice_pdfgen-1.2.0.tar", last modified: Fri May  3 15:22:03 2024, max compression
```

## Comparing `invoice_pdfgen-1.1.0.tar` & `invoice_pdfgen-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 15:04:42.824312 invoice_pdfgen-1.1.0/
--rw-rw-rw-   0        0        0     1104 2024-04-13 08:12:31.000000 invoice_pdfgen-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     3956 2024-05-03 15:04:42.821656 invoice_pdfgen-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3118 2024-05-03 14:35:13.000000 invoice_pdfgen-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 15:04:42.763817 invoice_pdfgen-1.1.0/invoice_pdfgen/
--rw-rw-rw-   0        0        0      253 2024-05-03 13:05:01.000000 invoice_pdfgen-1.1.0/invoice_pdfgen/__init__.py
--rw-rw-rw-   0        0        0     5975 2024-05-03 12:21:43.000000 invoice_pdfgen-1.1.0/invoice_pdfgen/pdf_invoice_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-03 15:04:42.819060 invoice_pdfgen-1.1.0/invoice_pdfgen.egg-info/
--rw-rw-rw-   0        0        0     3956 2024-05-03 15:04:42.000000 invoice_pdfgen-1.1.0/invoice_pdfgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2024-05-03 15:04:42.000000 invoice_pdfgen-1.1.0/invoice_pdfgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 15:04:42.000000 invoice_pdfgen-1.1.0/invoice_pdfgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-05-03 15:04:42.000000 invoice_pdfgen-1.1.0/invoice_pdfgen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-03 15:04:42.000000 invoice_pdfgen-1.1.0/invoice_pdfgen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 15:04:42.825306 invoice_pdfgen-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1689 2024-05-03 15:04:35.000000 invoice_pdfgen-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 15:04:42.813763 invoice_pdfgen-1.1.0/tests/
--rw-rw-rw-   0        0        0      801 2024-05-03 14:21:22.000000 invoice_pdfgen-1.1.0/tests/test_invoice_pdfgen.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:22:03.716526 invoice_pdfgen-1.2.0/
+-rw-rw-rw-   0        0        0     1104 2024-04-13 08:12:31.000000 invoice_pdfgen-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3469 2024-05-03 15:22:03.713256 invoice_pdfgen-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2631 2024-05-03 15:20:33.000000 invoice_pdfgen-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 15:22:03.663387 invoice_pdfgen-1.2.0/invoice_pdfgen/
+-rw-rw-rw-   0        0        0      253 2024-05-03 13:05:01.000000 invoice_pdfgen-1.2.0/invoice_pdfgen/__init__.py
+-rw-rw-rw-   0        0        0     5975 2024-05-03 12:21:43.000000 invoice_pdfgen-1.2.0/invoice_pdfgen/pdf_invoice_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:22:03.709321 invoice_pdfgen-1.2.0/invoice_pdfgen.egg-info/
+-rw-rw-rw-   0        0        0     3469 2024-05-03 15:22:03.000000 invoice_pdfgen-1.2.0/invoice_pdfgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2024-05-03 15:22:03.000000 invoice_pdfgen-1.2.0/invoice_pdfgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 15:22:03.000000 invoice_pdfgen-1.2.0/invoice_pdfgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-05-03 15:22:03.000000 invoice_pdfgen-1.2.0/invoice_pdfgen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-03 15:22:03.000000 invoice_pdfgen-1.2.0/invoice_pdfgen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 15:22:03.716526 invoice_pdfgen-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1689 2024-05-03 15:21:59.000000 invoice_pdfgen-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 15:22:03.704701 invoice_pdfgen-1.2.0/tests/
+-rw-rw-rw-   0        0        0      801 2024-05-03 14:21:22.000000 invoice_pdfgen-1.2.0/tests/test_invoice_pdfgen.py
```

### Comparing `invoice_pdfgen-1.1.0/LICENSE` & `invoice_pdfgen-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invoice_pdfgen-1.1.0/PKG-INFO` & `invoice_pdfgen-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoice_pdfgen
-Version: 1.1.0
+Version: 1.2.0
 Summary: This package can be used for generating PDF invoices from Excel invoices.
 Home-page: https://github.com/emads22/invoice-pdfgen-python
 Author: emads22
 Author-email: emads@email.com
 License: MIT
 Keywords: invoice,excel,pdf
 Classifier: Development Status :: 3 - Alpha
@@ -58,36 +58,20 @@
 # Create an instance of PDFInvoiceGenerator
 generator = PDFInvoiceGenerator(excel_filepath='invoice_data.xlsx', logo_filepath='company_logo.png')
 
 # Generate the PDF invoice
 generator.generate()
 ```
 
-For more detailed usage instructions and examples, please refer to the [examples](./examples) directory.
-
 ## Documentation
 
-For more detailed documentation, including API references and usage examples, please visit the [documentation](./docs/index.md).
-
-## Examples
-
-Check out the [examples](./examples) directory for usage examples of the Invoice PDF Generator package.
-
-## Tests
-
-The tests for the package can be found in the [tests](./tests) directory. You can run the tests using your preferred testing framework.
-
-## Contributing
-Contributions are welcome! Here are some ways you can contribute to the project:
-- Report bugs and issues
-- Suggest new features or improvements
-- Submit pull requests with bug fixes or enhancements
+For more detailed documentation, including API references and usage examples, please visit the [documentation](https://github.com/emads22/invoice-pdfgen-python/blob/main/docs/index.md).
 
 ## Author
 - Emad &nbsp; E>
   
   [<img src="https://img.shields.io/badge/GitHub-Profile-blue?logo=github" width="150">](https://github.com/emads22)
 
 ## License
 This project is licensed under the **MIT License**, which grants permission for free use, modification, distribution, and sublicense of the code, provided that the copyright notice (attributed to [emads22](https://github.com/emads22)) and permission notice are included in all copies or substantial portions of the software. This license is permissive and allows users to utilize the code for both commercial and non-commercial purposes.
 
-Please see the [LICENSE](LICENSE) file for more details.
+Please see the [LICENSE](https://github.com/emads22/invoice-pdfgen-python/blob/main/LICENSE) file for more details.
```

### Comparing `invoice_pdfgen-1.1.0/README.md` & `invoice_pdfgen-1.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -35,36 +35,20 @@
 # Create an instance of PDFInvoiceGenerator
 generator = PDFInvoiceGenerator(excel_filepath='invoice_data.xlsx', logo_filepath='company_logo.png')
 
 # Generate the PDF invoice
 generator.generate()
 ```
 
-For more detailed usage instructions and examples, please refer to the [examples](./examples) directory.
-
 ## Documentation
 
-For more detailed documentation, including API references and usage examples, please visit the [documentation](./docs/index.md).
-
-## Examples
-
-Check out the [examples](./examples) directory for usage examples of the Invoice PDF Generator package.
-
-## Tests
-
-The tests for the package can be found in the [tests](./tests) directory. You can run the tests using your preferred testing framework.
-
-## Contributing
-Contributions are welcome! Here are some ways you can contribute to the project:
-- Report bugs and issues
-- Suggest new features or improvements
-- Submit pull requests with bug fixes or enhancements
+For more detailed documentation, including API references and usage examples, please visit the [documentation](https://github.com/emads22/invoice-pdfgen-python/blob/main/docs/index.md).
 
 ## Author
 - Emad &nbsp; E>
   
   [<img src="https://img.shields.io/badge/GitHub-Profile-blue?logo=github" width="150">](https://github.com/emads22)
 
 ## License
 This project is licensed under the **MIT License**, which grants permission for free use, modification, distribution, and sublicense of the code, provided that the copyright notice (attributed to [emads22](https://github.com/emads22)) and permission notice are included in all copies or substantial portions of the software. This license is permissive and allows users to utilize the code for both commercial and non-commercial purposes.
 
-Please see the [LICENSE](LICENSE) file for more details.
+Please see the [LICENSE](https://github.com/emads22/invoice-pdfgen-python/blob/main/LICENSE) file for more details.
```

### Comparing `invoice_pdfgen-1.1.0/invoice_pdfgen/pdf_invoice_generator.py` & `invoice_pdfgen-1.2.0/invoice_pdfgen/pdf_invoice_generator.py`

 * *Files identical despite different names*

### Comparing `invoice_pdfgen-1.1.0/invoice_pdfgen.egg-info/PKG-INFO` & `invoice_pdfgen-1.2.0/invoice_pdfgen.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoice_pdfgen
-Version: 1.1.0
+Version: 1.2.0
 Summary: This package can be used for generating PDF invoices from Excel invoices.
 Home-page: https://github.com/emads22/invoice-pdfgen-python
 Author: emads22
 Author-email: emads@email.com
 License: MIT
 Keywords: invoice,excel,pdf
 Classifier: Development Status :: 3 - Alpha
@@ -58,36 +58,20 @@
 # Create an instance of PDFInvoiceGenerator
 generator = PDFInvoiceGenerator(excel_filepath='invoice_data.xlsx', logo_filepath='company_logo.png')
 
 # Generate the PDF invoice
 generator.generate()
 ```
 
-For more detailed usage instructions and examples, please refer to the [examples](./examples) directory.
-
 ## Documentation
 
-For more detailed documentation, including API references and usage examples, please visit the [documentation](./docs/index.md).
-
-## Examples
-
-Check out the [examples](./examples) directory for usage examples of the Invoice PDF Generator package.
-
-## Tests
-
-The tests for the package can be found in the [tests](./tests) directory. You can run the tests using your preferred testing framework.
-
-## Contributing
-Contributions are welcome! Here are some ways you can contribute to the project:
-- Report bugs and issues
-- Suggest new features or improvements
-- Submit pull requests with bug fixes or enhancements
+For more detailed documentation, including API references and usage examples, please visit the [documentation](https://github.com/emads22/invoice-pdfgen-python/blob/main/docs/index.md).
 
 ## Author
 - Emad &nbsp; E>
   
   [<img src="https://img.shields.io/badge/GitHub-Profile-blue?logo=github" width="150">](https://github.com/emads22)
 
 ## License
 This project is licensed under the **MIT License**, which grants permission for free use, modification, distribution, and sublicense of the code, provided that the copyright notice (attributed to [emads22](https://github.com/emads22)) and permission notice are included in all copies or substantial portions of the software. This license is permissive and allows users to utilize the code for both commercial and non-commercial purposes.
 
-Please see the [LICENSE](LICENSE) file for more details.
+Please see the [LICENSE](https://github.com/emads22/invoice-pdfgen-python/blob/main/LICENSE) file for more details.
```

### Comparing `invoice_pdfgen-1.1.0/setup.py` & `invoice_pdfgen-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 # Setup function call with package information
 setup(
     name='invoice_pdfgen',  # Package name
     # Automatically find all packages and sub-packages within the directory
     packages=find_packages(),
-    version='1.1.0',  # Package version
+    version='1.2.0',  # Package version
     license='MIT',  # License type
     # Brief description
     description='This package can be used for generating PDF invoices from Excel invoices.',
     long_description=long_description,  # Use README.md content as long description
     # Specify that long description is in Markdown format
     long_description_content_type='text/markdown',
     author='emads22',  # GitHub username
```

### Comparing `invoice_pdfgen-1.1.0/tests/test_invoice_pdfgen.py` & `invoice_pdfgen-1.2.0/tests/test_invoice_pdfgen.py`

 * *Files identical despite different names*

