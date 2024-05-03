# Comparing `tmp/openfisca_country_template-7.0.0.tar.gz` & `tmp/openfisca_country_template-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfisca_country_template-7.0.0.tar", last modified: Thu May  2 07:44:18 2024, max compression
+gzip compressed data, was "openfisca_country_template-7.1.0.tar", last modified: Fri May  3 15:40:35 2024, max compression
```

## Comparing `openfisca_country_template-7.0.0.tar` & `openfisca_country_template-7.1.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.304840 openfisca_country_template-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-05-02 07:44:18.304840 openfisca_country_template-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.296840 openfisca_country_template-7.0.0/openfisca_country_template/
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.296840 openfisca_country_template-7.0.0/openfisca_country_template/parameters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/parameters/benefits/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/benefits/basic_income.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/benefits/housing_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/benefits/index.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/parameters/benefits/parenting_allowance/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/benefits/parenting_allowance/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/benefits/parenting_allowance/income_threshold.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/parameters/general/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/general/age_of_majority.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/general/age_of_retirement.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/parameters/taxes/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/taxes/housing_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/taxes/income_tax_rate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/taxes/social_security_contribution.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/reforms/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/reforms/add_dynamic_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/reforms/add_new_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/reforms/flat_social_security_contribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/reforms/modify_social_security_taxation.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/reforms/removal_basic_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/situation_examples/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/situation_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/situation_examples/couple.json
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/situation_examples/housing.json
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/situation_examples/single.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/age.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/basic_income.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/disposable_income.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/housing_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/housing_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/tests/reforms/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/reforms/add_dynamic_variable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/reforms/add_new_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.304840 openfisca_country_template-7.0.0/openfisca_country_template/tests/situations/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/situations/income_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/situations/parenting_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/social_security_contribution.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.304840 openfisca_country_template-7.0.0/openfisca_country_template/variables/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/variables/benefits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/variables/demographics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/variables/housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/variables/income.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/variables/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/variables/taxes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.304840 openfisca_country_template-7.0.0/openfisca_country_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-05-02 07:44:18.000000 openfisca_country_template-7.0.0/openfisca_country_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-02 07:44:18.000000 openfisca_country_template-7.0.0/openfisca_country_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 07:44:18.000000 openfisca_country_template-7.0.0/openfisca_country_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 07:44:18.000000 openfisca_country_template-7.0.0/openfisca_country_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 07:44:18.000000 openfisca_country_template-7.0.0/openfisca_country_template.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 07:44:18.304840 openfisca_country_template-7.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:40:35.791432 openfisca_country_template-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-03 15:40:35.791432 openfisca_country_template-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:40:35.783432 openfisca_country_template-7.1.0/openfisca_country_template/
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:40:35.779432 openfisca_country_template-7.1.0/openfisca_country_template/parameters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:40:35.783432 openfisca_country_template-7.1.0/openfisca_country_template/parameters/benefits/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/parameters/benefits/basic_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/parameters/benefits/housing_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/parameters/benefits/index.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:40:35.783432 openfisca_country_template-7.1.0/openfisca_country_template/parameters/benefits/parenting_allowance/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/parameters/benefits/parenting_allowance/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/parameters/benefits/parenting_allowance/income_threshold.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:40:35.783432 openfisca_country_template-7.1.0/openfisca_country_template/parameters/general/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/parameters/general/age_of_majority.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/parameters/general/age_of_retirement.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:40:35.787432 openfisca_country_template-7.1.0/openfisca_country_template/parameters/taxes/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/parameters/taxes/housing_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/parameters/taxes/income_tax_rate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/parameters/taxes/social_security_contribution.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:40:35.787432 openfisca_country_template-7.1.0/openfisca_country_template/reforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/reforms/add_dynamic_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/reforms/add_new_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/reforms/flat_social_security_contribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/reforms/modify_social_security_taxation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/reforms/removal_basic_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:40:35.787432 openfisca_country_template-7.1.0/openfisca_country_template/situation_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/situation_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/situation_examples/couple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/situation_examples/housing.json
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/situation_examples/single.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:40:35.787432 openfisca_country_template-7.1.0/openfisca_country_template/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/tests/age.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/tests/basic_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/tests/disposable_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/tests/housing_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/tests/housing_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/tests/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:40:35.787432 openfisca_country_template-7.1.0/openfisca_country_template/tests/reforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/tests/reforms/add_dynamic_variable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/tests/reforms/add_new_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:40:35.787432 openfisca_country_template-7.1.0/openfisca_country_template/tests/situations/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/tests/situations/income_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/tests/situations/parenting_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/tests/social_security_contribution.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:40:35.791432 openfisca_country_template-7.1.0/openfisca_country_template/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/variables/benefits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/variables/demographics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/variables/housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/variables/income.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/variables/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/openfisca_country_template/variables/taxes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:40:35.791432 openfisca_country_template-7.1.0/openfisca_country_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-03 15:40:35.000000 openfisca_country_template-7.1.0/openfisca_country_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-03 15:40:35.000000 openfisca_country_template-7.1.0/openfisca_country_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:40:35.000000 openfisca_country_template-7.1.0/openfisca_country_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-03 15:40:35.000000 openfisca_country_template-7.1.0/openfisca_country_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-03 15:40:35.000000 openfisca_country_template-7.1.0/openfisca_country_template.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-03 15:40:17.000000 openfisca_country_template-7.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:40:35.791432 openfisca_country_template-7.1.0/setup.cfg
```

### Comparing `openfisca_country_template-7.0.0/LICENSE` & `openfisca_country_template-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/PKG-INFO` & `openfisca_country_template-7.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfisca-country_template
-Version: 7.0.0
+Version: 7.1.0
 Summary: OpenFisca Rules as Code model for Country-Template.
 Project-URL: Homepage, https://github.com/openfisca/country-template
 Project-URL: Repository, https://github.com/openfisca/country-template
 Project-URL: Documentation, https://openfisca.org/doc
 Project-URL: Issues, https://github.com/openfisca/country-template/issues
 Project-URL: Changelog, https://github.com/openfisca/country-template/blob/main/CHANGELOG.md
 Keywords: microsimulation,tax,benefit,rac,rules-as-code
@@ -24,34 +24,51 @@
 Requires-Dist: isort>=5.13.2; extra == "dev"
 Requires-Dist: pylint>=3.1.0; extra == "dev"
 Requires-Dist: pyupgrade>=3.15.1; extra == "dev"
 Requires-Dist: yamllint>=1.35.1; extra == "dev"
 
 # OpenFisca Country-Template
 
-This repository helps you quickly bootstrap and use your own OpenFisca country package.
+This repository helps you quickly set up and use your own OpenFisca country package.
 
-**You should NOT fork it but [download a copy](https://github.com/openfisca/country-template/archive/master.zip) of it** and follow the bootstrapping instructions below.
+**You should NOT fork it** but follow the set up instructions below.
 
 > Otherwise, you will have to clean up all tags when you deploy your own country package.
 
-## Bootstrapping your Country Package
+## Setting up your Country Package
 
 This set of instructions **only needs to be followed once** and will create your own copy of this boilerplate directory, customising it to the country you want to work on. You will need to have [Git](https://git-scm.com) installed.
 
-1. [Download a copy](https://github.com/openfisca/country-template/archive/master.zip) of this repository, unzip it and `cd` into it in a Terminal window.
+### Using GitHub (recommended for GitHub users)
+
+1. Click on the [“Use this template” dropdown and select “Create a new repository”](https://github.com/new?template_name=country-template&template_owner=openfisca).
+
+2. Set the repository name to `openfisca-<your_country_name>`; use underscore `_` as separator if there are spaces in the country name. For example, `openfisca-new_zealand` or `openfisca-france`.
 
-2. Create a new repository on your favourite git host (Github, Bitbucket, GitLab, etc) with the name openfisca-your_country_name. For example, `openfisca-new_zealand` or `openfisca-france`.
+3. After being redirected to your newly created repository, please allow a few minutes for the automatic setup to be executed. Once done, the title of the README file should be updated to `OpenFisca <your_country_name>`. 
 
-3. Execute the `bootstrap.sh` script to initialise the git repository. This performs numerous tasks including replacing all references to `openfisca-country_template` with references to the new country package. 
-   - To execute the script run `bash bootstrap.sh` from the command line. _Note: this script can only run on Unix systems, but OpenFisca and the resulting package will work on Windows too._
-   - After the `bootstrap.sh` has run both it and these instructions are removed.
+> If the automatic setup does not start within a few minutes, you can initiate it manually:
+> - Navigate to the “Actions” tab.
+> - Select the “First time setup” workflow.
+> - Click on “Run workflow” to start the setup process manually.
 
 4. Follow the instructions in the new repository's README.md.
 
+### Manual setup (recommended for users of other Git hosts)
+
+1. [Download a copy](https://github.com/openfisca/country-template/archive/master.zip) of this repository, unzip it and `cd` into it in a Terminal window.
+
+2. Create a new repository on your favourite git host (Bitbucket, GitLab, …) with the name `openfisca-<your_country_name>`. For example, `openfisca-new_zealand` or `openfisca-france`.
+
+3. Execute the `first-time-setup.sh` script to initialise the git repository. This performs numerous tasks including replacing all references to `openfisca-country_template` with references to the new country package.
+   - To execute the script run `bash first-time-setup.sh` from the command line
+   - After the `first-time-setup.sh` has run both it and these instructions are removed.
+
+4. Follow the instructions in the new repository's `README.md.`
+
 ## Writing the Legislation
 
 The country whose law is modelled here has a very simple tax and benefit system.
 
 - It has a flat rate tax whose rates increase every year.
 - On the first of December, 2015, it introduced a basic income for all its citizens of age who have no income.
 - On the first of December, 2016, it removed the income condition, providing all its adult citizens with a basic income.
```

### Comparing `openfisca_country_template-7.0.0/README.md` & `openfisca_country_template-7.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,46 @@
 # OpenFisca Country-Template
 
-This repository helps you quickly bootstrap and use your own OpenFisca country package.
+This repository helps you quickly set up and use your own OpenFisca country package.
 
-**You should NOT fork it but [download a copy](https://github.com/openfisca/country-template/archive/master.zip) of it** and follow the bootstrapping instructions below.
+**You should NOT fork it** but follow the set up instructions below.
 
 > Otherwise, you will have to clean up all tags when you deploy your own country package.
 
-## Bootstrapping your Country Package
+## Setting up your Country Package
 
 This set of instructions **only needs to be followed once** and will create your own copy of this boilerplate directory, customising it to the country you want to work on. You will need to have [Git](https://git-scm.com) installed.
 
-1. [Download a copy](https://github.com/openfisca/country-template/archive/master.zip) of this repository, unzip it and `cd` into it in a Terminal window.
+### Using GitHub (recommended for GitHub users)
+
+1. Click on the [“Use this template” dropdown and select “Create a new repository”](https://github.com/new?template_name=country-template&template_owner=openfisca).
+
+2. Set the repository name to `openfisca-<your_country_name>`; use underscore `_` as separator if there are spaces in the country name. For example, `openfisca-new_zealand` or `openfisca-france`.
 
-2. Create a new repository on your favourite git host (Github, Bitbucket, GitLab, etc) with the name openfisca-your_country_name. For example, `openfisca-new_zealand` or `openfisca-france`.
+3. After being redirected to your newly created repository, please allow a few minutes for the automatic setup to be executed. Once done, the title of the README file should be updated to `OpenFisca <your_country_name>`. 
 
-3. Execute the `bootstrap.sh` script to initialise the git repository. This performs numerous tasks including replacing all references to `openfisca-country_template` with references to the new country package. 
-   - To execute the script run `bash bootstrap.sh` from the command line. _Note: this script can only run on Unix systems, but OpenFisca and the resulting package will work on Windows too._
-   - After the `bootstrap.sh` has run both it and these instructions are removed.
+> If the automatic setup does not start within a few minutes, you can initiate it manually:
+> - Navigate to the “Actions” tab.
+> - Select the “First time setup” workflow.
+> - Click on “Run workflow” to start the setup process manually.
 
 4. Follow the instructions in the new repository's README.md.
 
+### Manual setup (recommended for users of other Git hosts)
+
+1. [Download a copy](https://github.com/openfisca/country-template/archive/master.zip) of this repository, unzip it and `cd` into it in a Terminal window.
+
+2. Create a new repository on your favourite git host (Bitbucket, GitLab, …) with the name `openfisca-<your_country_name>`. For example, `openfisca-new_zealand` or `openfisca-france`.
+
+3. Execute the `first-time-setup.sh` script to initialise the git repository. This performs numerous tasks including replacing all references to `openfisca-country_template` with references to the new country package.
+   - To execute the script run `bash first-time-setup.sh` from the command line
+   - After the `first-time-setup.sh` has run both it and these instructions are removed.
+
+4. Follow the instructions in the new repository's `README.md.`
+
 ## Writing the Legislation
 
 The country whose law is modelled here has a very simple tax and benefit system.
 
 - It has a flat rate tax whose rates increase every year.
 - On the first of December, 2015, it introduced a basic income for all its citizens of age who have no income.
 - On the first of December, 2016, it removed the income condition, providing all its adult citizens with a basic income.
```

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/__init__.py` & `openfisca_country_template-7.1.0/openfisca_country_template/__init__.py`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/entities.py` & `openfisca_country_template-7.1.0/openfisca_country_template/entities.py`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/parameters/taxes/social_security_contribution.yaml` & `openfisca_country_template-7.1.0/openfisca_country_template/parameters/taxes/social_security_contribution.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/reforms/add_dynamic_variable.py` & `openfisca_country_template-7.1.0/openfisca_country_template/reforms/add_dynamic_variable.py`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/reforms/add_new_tax.py` & `openfisca_country_template-7.1.0/openfisca_country_template/reforms/add_new_tax.py`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/reforms/flat_social_security_contribution.py` & `openfisca_country_template-7.1.0/openfisca_country_template/reforms/flat_social_security_contribution.py`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/reforms/modify_social_security_taxation.py` & `openfisca_country_template-7.1.0/openfisca_country_template/reforms/modify_social_security_taxation.py`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/reforms/removal_basic_income.py` & `openfisca_country_template-7.1.0/openfisca_country_template/reforms/removal_basic_income.py`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/situation_examples/couple.json` & `openfisca_country_template-7.1.0/openfisca_country_template/situation_examples/couple.json`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/tests/age.yaml` & `openfisca_country_template-7.1.0/openfisca_country_template/tests/age.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/tests/basic_income.yaml` & `openfisca_country_template-7.1.0/openfisca_country_template/tests/basic_income.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/tests/disposable_income.yaml` & `openfisca_country_template-7.1.0/openfisca_country_template/tests/disposable_income.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/tests/housing_tax.yaml` & `openfisca_country_template-7.1.0/openfisca_country_template/tests/housing_tax.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/tests/reforms/add_new_tax.yaml` & `openfisca_country_template-7.1.0/openfisca_country_template/tests/reforms/add_new_tax.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml` & `openfisca_country_template-7.1.0/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/tests/situations/income_tax.yaml` & `openfisca_country_template-7.1.0/openfisca_country_template/tests/situations/income_tax.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/tests/situations/parenting_allowance.yaml` & `openfisca_country_template-7.1.0/openfisca_country_template/tests/situations/parenting_allowance.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/tests/social_security_contribution.yaml` & `openfisca_country_template-7.1.0/openfisca_country_template/tests/social_security_contribution.yaml`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/variables/benefits.py` & `openfisca_country_template-7.1.0/openfisca_country_template/variables/benefits.py`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/variables/demographics.py` & `openfisca_country_template-7.1.0/openfisca_country_template/variables/demographics.py`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/variables/housing.py` & `openfisca_country_template-7.1.0/openfisca_country_template/variables/housing.py`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/variables/income.py` & `openfisca_country_template-7.1.0/openfisca_country_template/variables/income.py`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/variables/stats.py` & `openfisca_country_template-7.1.0/openfisca_country_template/variables/stats.py`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template/variables/taxes.py` & `openfisca_country_template-7.1.0/openfisca_country_template/variables/taxes.py`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template.egg-info/PKG-INFO` & `openfisca_country_template-7.1.0/openfisca_country_template.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfisca-country_template
-Version: 7.0.0
+Version: 7.1.0
 Summary: OpenFisca Rules as Code model for Country-Template.
 Project-URL: Homepage, https://github.com/openfisca/country-template
 Project-URL: Repository, https://github.com/openfisca/country-template
 Project-URL: Documentation, https://openfisca.org/doc
 Project-URL: Issues, https://github.com/openfisca/country-template/issues
 Project-URL: Changelog, https://github.com/openfisca/country-template/blob/main/CHANGELOG.md
 Keywords: microsimulation,tax,benefit,rac,rules-as-code
@@ -24,34 +24,51 @@
 Requires-Dist: isort>=5.13.2; extra == "dev"
 Requires-Dist: pylint>=3.1.0; extra == "dev"
 Requires-Dist: pyupgrade>=3.15.1; extra == "dev"
 Requires-Dist: yamllint>=1.35.1; extra == "dev"
 
 # OpenFisca Country-Template
 
-This repository helps you quickly bootstrap and use your own OpenFisca country package.
+This repository helps you quickly set up and use your own OpenFisca country package.
 
-**You should NOT fork it but [download a copy](https://github.com/openfisca/country-template/archive/master.zip) of it** and follow the bootstrapping instructions below.
+**You should NOT fork it** but follow the set up instructions below.
 
 > Otherwise, you will have to clean up all tags when you deploy your own country package.
 
-## Bootstrapping your Country Package
+## Setting up your Country Package
 
 This set of instructions **only needs to be followed once** and will create your own copy of this boilerplate directory, customising it to the country you want to work on. You will need to have [Git](https://git-scm.com) installed.
 
-1. [Download a copy](https://github.com/openfisca/country-template/archive/master.zip) of this repository, unzip it and `cd` into it in a Terminal window.
+### Using GitHub (recommended for GitHub users)
+
+1. Click on the [“Use this template” dropdown and select “Create a new repository”](https://github.com/new?template_name=country-template&template_owner=openfisca).
+
+2. Set the repository name to `openfisca-<your_country_name>`; use underscore `_` as separator if there are spaces in the country name. For example, `openfisca-new_zealand` or `openfisca-france`.
 
-2. Create a new repository on your favourite git host (Github, Bitbucket, GitLab, etc) with the name openfisca-your_country_name. For example, `openfisca-new_zealand` or `openfisca-france`.
+3. After being redirected to your newly created repository, please allow a few minutes for the automatic setup to be executed. Once done, the title of the README file should be updated to `OpenFisca <your_country_name>`. 
 
-3. Execute the `bootstrap.sh` script to initialise the git repository. This performs numerous tasks including replacing all references to `openfisca-country_template` with references to the new country package. 
-   - To execute the script run `bash bootstrap.sh` from the command line. _Note: this script can only run on Unix systems, but OpenFisca and the resulting package will work on Windows too._
-   - After the `bootstrap.sh` has run both it and these instructions are removed.
+> If the automatic setup does not start within a few minutes, you can initiate it manually:
+> - Navigate to the “Actions” tab.
+> - Select the “First time setup” workflow.
+> - Click on “Run workflow” to start the setup process manually.
 
 4. Follow the instructions in the new repository's README.md.
 
+### Manual setup (recommended for users of other Git hosts)
+
+1. [Download a copy](https://github.com/openfisca/country-template/archive/master.zip) of this repository, unzip it and `cd` into it in a Terminal window.
+
+2. Create a new repository on your favourite git host (Bitbucket, GitLab, …) with the name `openfisca-<your_country_name>`. For example, `openfisca-new_zealand` or `openfisca-france`.
+
+3. Execute the `first-time-setup.sh` script to initialise the git repository. This performs numerous tasks including replacing all references to `openfisca-country_template` with references to the new country package.
+   - To execute the script run `bash first-time-setup.sh` from the command line
+   - After the `first-time-setup.sh` has run both it and these instructions are removed.
+
+4. Follow the instructions in the new repository's `README.md.`
+
 ## Writing the Legislation
 
 The country whose law is modelled here has a very simple tax and benefit system.
 
 - It has a flat rate tax whose rates increase every year.
 - On the first of December, 2015, it introduced a basic income for all its citizens of age who have no income.
 - On the first of December, 2016, it removed the income condition, providing all its adult citizens with a basic income.
```

### Comparing `openfisca_country_template-7.0.0/openfisca_country_template.egg-info/SOURCES.txt` & `openfisca_country_template-7.1.0/openfisca_country_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openfisca_country_template-7.0.0/pyproject.toml` & `openfisca_country_template-7.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openfisca-country_template"
-version = "7.0.0"
+version = "7.1.0"
 description = "OpenFisca Rules as Code model for Country-Template."
 readme = "README.md"
 keywords = ["microsimulation", "tax", "benefit", "rac", "rules-as-code"]
 authors = []
 maintainers = []
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

