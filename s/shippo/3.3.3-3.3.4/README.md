# Comparing `tmp/shippo-3.3.3.tar.gz` & `tmp/shippo-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shippo-3.3.3.tar", last modified: Mon Apr 29 15:03:28 2024, max compression
+gzip compressed data, was "shippo-3.3.4.tar", last modified: Fri May  3 17:39:53 2024, max compression
```

## Comparing `shippo-3.3.3.tar` & `shippo-3.3.4.tar`

### file list

```diff
@@ -1,256 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:03:28.420842 shippo-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    17793 2024-04-29 15:03:28.420842 shippo-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-04-29 15:03:19.000000 shippo-3.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:03:28.420842 shippo-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-29 15:03:19.000000 shippo-3.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:03:28.380842 shippo-3.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:03:28.388842 shippo-3.3.3/src/shippo/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:03:28.388842 shippo-3.3.3/src/shippo/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    19356 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/batches.py
--rw-r--r--   0 runner    (1001) docker     (127)    27922 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/carrier_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/carrier_parcel_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/customs_declarations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/customs_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    10900 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/manifests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:03:28.388842 shippo-3.3.3/src/shippo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:03:28.408842 shippo-3.3.3/src/shippo/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/addresscompletecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/addresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/addressimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/addresspaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/addressvalidationresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/addressvalidationresultsmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/batchcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/batchshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/batchshipmentbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/batchshipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountdpddecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountfedexcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountupscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountuspscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrieraccountwithextrainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/carriersenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/cod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/connectexistingownaccountrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/customerreference.py
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/customsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/customsdeclarationcontentstypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/customsdeclarationcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/customsdeclarationeelpfcenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/customsdeclarationincotermenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/customsdeclarationnondeliveryoptionenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/customsdeclarationpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/customsexporteridentification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/customsinvoicedcharges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/customsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/customsitemcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/customsitempaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/customstaxidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/dangerousgoodslithiumbatteries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/dangerousgoodsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/defaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/defaultparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/departmentnumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/distanceunitenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/dryice.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/errormessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/instanttransactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/instanttransactioncreateresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/instanttransactionrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/insurance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/invoicenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/labelfiletypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/lineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/lineitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/liverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/liveratecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/liveratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/manifestcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/manifestpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/objectstateenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/ordercreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/orderpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/orderstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/parcelcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/parcelextra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/parcelinsurance.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/parcelpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/parcelrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/parceltemplateenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/pickupbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/ponumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/ratemessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/ratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/refundpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/refundrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/rmanumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/servicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/servicegroupaccountandservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/servicegroupcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/servicegrouptypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/servicegroupupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/servicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)    42151 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/servicelevelenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/shipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/shipmentcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/shipmentextra.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/shipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/shippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/shippoaccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/shippoaccountupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/trackingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/trackingstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/trackingstatuslocationbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/trackingstatussubstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/tracksrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/transactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/transactionpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/transactionstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/upsconnectexistingownaccountparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/userparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/userparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/components/weightunitenum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:03:28.408842 shippo-3.3.3/src/shippo/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/errors/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:03:28.408842 shippo-3.3.3/src/shippo/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:03:28.420842 shippo-3.3.3/src/shippo/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/addshipmentstobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createliverate.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createpickup.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/createuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/deletedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/deleteservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/deleteuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getcarrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getcarrierregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getdefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/gettrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/gettransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/getuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listaddresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listcarrieraccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listcarrierparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listcustomsdeclarations.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listcustomsitems.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listmanifests.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listorders.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listparcels.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listrefunds.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listservicegroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listshipmentrates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listshipmentratesbycurrencycode.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listshipments.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listshippoaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/listuserparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/purchasebatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/registercarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/removeshipmentsfrombatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/updatecarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/updatedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/updateservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/updateshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/updateuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/models/operations/validateaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15348 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/rates_at_checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/refunds.py
--rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/shipments.py
--rw-r--r--   0 runner    (1001) docker     (127)    14799 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/shippo_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/tracking_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11058 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18766 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/user_parcel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:03:28.420842 shippo-3.3.3/src/shippo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-29 15:03:19.000000 shippo-3.3.3/src/shippo/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:03:28.388842 shippo-3.3.3/src/shippo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17793 2024-04-29 15:03:28.000000 shippo-3.3.3/src/shippo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-04-29 15:03:28.000000 shippo-3.3.3/src/shippo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:03:28.000000 shippo-3.3.3/src/shippo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-29 15:03:28.000000 shippo-3.3.3/src/shippo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 15:03:28.000000 shippo-3.3.3/src/shippo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.217130 shippo-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    17793 2024-05-03 17:39:53.217130 shippo-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-03 17:39:44.000000 shippo-3.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:39:53.217130 shippo-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-03 17:39:44.000000 shippo-3.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.177130 shippo-3.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.181130 shippo-3.3.4/src/shippo/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.181130 shippo-3.3.4/src/shippo/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19356 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27922 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/carrier_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/carrier_parcel_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/customs_declarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/customs_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10900 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/manifests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.181130 shippo-3.3.4/src/shippo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.205130 shippo-3.3.4/src/shippo/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/addresscompletecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/addresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/addressimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/addresspaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/addressvalidationresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/addressvalidationresultsmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/batchcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/batchshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/batchshipmentbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/batchshipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountdpddecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountfedexcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountupscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountuspscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountwithextrainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carriersenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/cod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/connectexistingownaccountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customerreference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclarationcontentstypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclarationcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclarationeelpfcenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclarationincotermenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclarationnondeliveryoptionenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclarationpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsexporteridentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsinvoicedcharges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsitemcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsitempaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customstaxidentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/dangerousgoodslithiumbatteries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/dangerousgoodsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/defaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/defaultparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/departmentnumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/distanceunitenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/dryice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/errormessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/fedexconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/instanttransactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/instanttransactioncreateresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/instanttransactionrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/insurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/invoicenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/labelfiletypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/lineitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/liverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/liveratecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/liveratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/manifestcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/manifestpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/objectstateenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/ordercreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/orderpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/orderstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/parcelcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/parcelextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/parcelinsurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/parcelpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/parcelrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/parceltemplateenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/pickupbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/ponumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/ratemessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/ratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/refundpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/refundrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/rmanumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/servicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/servicegroupaccountandservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/servicegroupcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/servicegrouptypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/servicegroupupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/servicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42151 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/servicelevelenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/shipmentcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/shipmentextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/shipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/shippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/shippoaccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/shippoaccountupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/trackingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/trackingstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/trackingstatuslocationbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/trackingstatussubstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/tracksrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/transactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/transactionpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/transactionstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/upsconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/userparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/userparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/weightunitenum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.205130 shippo-3.3.4/src/shippo/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/errors/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.205130 shippo-3.3.4/src/shippo/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.213130 shippo-3.3.4/src/shippo/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/addshipmentstobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createliverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createpickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/deletedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/deleteservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/deleteuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getcarrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getcarrierregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getdefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/gettrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/gettransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listaddresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listcarrieraccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listcarrierparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listcustomsdeclarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listcustomsitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listmanifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listorders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listparcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listrefunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listservicegroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listshipmentrates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listshipmentratesbycurrencycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listshipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listshippoaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listuserparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/purchasebatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/registercarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/removeshipmentsfrombatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/updatecarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/updatedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/updateservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/updateshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/updateuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/validateaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15348 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/rates_at_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14799 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/shippo_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/tracking_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11058 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18766 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/user_parcel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.213130 shippo-3.3.4/src/shippo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.181130 shippo-3.3.4/src/shippo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17793 2024-05-03 17:39:52.000000 shippo-3.3.4/src/shippo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-03 17:39:53.000000 shippo-3.3.4/src/shippo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:39:52.000000 shippo-3.3.4/src/shippo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-03 17:39:52.000000 shippo-3.3.4/src/shippo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 17:39:52.000000 shippo-3.3.4/src/shippo.egg-info/top_level.txt
```

### Comparing `shippo-3.3.3/PKG-INFO` & `shippo-3.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.3.3
+Version: 3.3.4
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.3.3/README.md` & `shippo-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/setup.py` & `shippo-3.3.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='shippo',
-    version='3.3.3',
+    version='3.3.4',
     author='Shippo',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/goshippo/shippo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `shippo-3.3.3/src/shippo/_hooks/registration.py` & `shippo-3.3.4/src/shippo/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/_hooks/sdkhooks.py` & `shippo-3.3.4/src/shippo/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/_hooks/types.py` & `shippo-3.3.4/src/shippo/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/addresses.py` & `shippo-3.3.4/src/shippo/addresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/batches.py` & `shippo-3.3.4/src/shippo/batches.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/carrier_accounts.py` & `shippo-3.3.4/src/shippo/carrier_accounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/carrier_parcel_templates.py` & `shippo-3.3.4/src/shippo/carrier_parcel_templates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/customs_declarations.py` & `shippo-3.3.4/src/shippo/customs_declarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/customs_items.py` & `shippo-3.3.4/src/shippo/customs_items.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/debug.py` & `shippo-3.3.4/src/shippo/debug.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/manifests.py` & `shippo-3.3.4/src/shippo/manifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/__init__.py` & `shippo-3.3.4/src/shippo/models/components/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 from .dangerousgoodsobject import *
 from .defaultparceltemplate import *
 from .defaultparceltemplateupdaterequest import *
 from .departmentnumber import *
 from .distanceunitenum import *
 from .dryice import *
 from .errormessage import *
+from .fedexconnectexistingownaccountparameters import *
 from .instanttransactioncreaterequest import *
 from .instanttransactioncreateresponse import *
 from .instanttransactionrate import *
 from .insurance import *
 from .invoicenumber import *
 from .labelfiletypeenum import *
 from .lineitem import *
@@ -130,8 +131,8 @@
 from .upsconnectexistingownaccountparameters import *
 from .userparceltemplate import *
 from .userparceltemplateupdaterequest import *
 from .userparceltemplatewithcarriertemplatecreaterequest import *
 from .userparceltemplatewithoutcarriertemplatecreaterequest import *
 from .weightunitenum import *
 
-__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountChronopostCreateRequestParameters","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountFedExCreateRequest","CarrierAccountFedExCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountMondialRelayCreateRequest","CarrierAccountMondialRelayCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","CarriersEnum","Cod","Code","ConnectExistingOwnAccountRequest","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationB13AFilingOptionEnum","CustomsDeclarationContentsTypeEnum","CustomsDeclarationCreateRequest","CustomsDeclarationEelPfcEnum","CustomsDeclarationIncotermEnum","CustomsDeclarationNonDeliveryOptionEnum","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemCreateRequest","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnitEnum","DryIce","ErrorMessage","InstantTransactionCreateRequest","InstantTransactionCreateResponse","InstantTransactionCreateResponseMessages","InstantTransactionCreateResponseResponseType","InstantTransactionRate","Insurance","InvoiceNumber","LabelFileType","LabelFileTypeEnum","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","ObjectInfo","ObjectResults","ObjectState","ObjectStateEnum","Order","OrderCreateRequest","OrderPaginatedList","OrderStatusEnum","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustraliaEnum","ParcelTemplateCouriersPleaseEnum","ParcelTemplateDHLeCommerceEnum","ParcelTemplateDPDUKEnum","ParcelTemplateFedExEnum","ParcelTemplateUPSEnum","ParcelTemplateUSPSEnum","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ResponseType","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupTypeEnum","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostalEnum","ServiceLevelAPGEnum","ServiceLevelAirterraEnum","ServiceLevelAramexAustraliaEnum","ServiceLevelAsendiaEnum","ServiceLevelAustraliaPostEnum","ServiceLevelAxleHireEnum","ServiceLevelBetterTrucksEnum","ServiceLevelCDLEnum","ServiceLevelCanadaPostEnum","ServiceLevelChronopostEnum","ServiceLevelColissimoEnum","ServiceLevelCorreosEspanaEnum","ServiceLevelCouriersPleaseEnum","ServiceLevelDHLExpressEnum","ServiceLevelDHLGermanyEnum","ServiceLevelDHLeCommerceEnum","ServiceLevelDPDDEEnum","ServiceLevelDPDUKEnum","ServiceLevelDeutschePostEnum","ServiceLevelEvriUKEnum","ServiceLevelFedExEnum","ServiceLevelGLSUSEnum","ServiceLevelGlobegisticsEnum","ServiceLevelLSOEnum","ServiceLevelLasershipEnum","ServiceLevelMaergoEnum","ServiceLevelMondialRelayEnum","ServiceLevelOnTracEnum","ServiceLevelParcelforceEnum","ServiceLevelPostItalianeEnum","ServiceLevelPurolatorEnum","ServiceLevelRoyalMailEnum","ServiceLevelSendleEnum","ServiceLevelSwyftEnum","ServiceLevelUDSEnum","ServiceLevelUPSEnum","ServiceLevelUSPSEnum","ServiceLevelVehoEnum","ServiceLevelePostGlobalEnum","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnitEnum"]
+__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountChronopostCreateRequestParameters","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountFedExCreateRequest","CarrierAccountFedExCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountMondialRelayCreateRequest","CarrierAccountMondialRelayCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","CarriersEnum","Cod","Code","ConnectExistingOwnAccountRequest","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationB13AFilingOptionEnum","CustomsDeclarationContentsTypeEnum","CustomsDeclarationCreateRequest","CustomsDeclarationEelPfcEnum","CustomsDeclarationIncotermEnum","CustomsDeclarationNonDeliveryOptionEnum","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemCreateRequest","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnitEnum","DryIce","ErrorMessage","FedExConnectExistingOwnAccountParameters","InstantTransactionCreateRequest","InstantTransactionCreateResponse","InstantTransactionCreateResponseMessages","InstantTransactionCreateResponseResponseType","InstantTransactionRate","Insurance","InvoiceNumber","LabelFileType","LabelFileTypeEnum","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","ObjectInfo","ObjectResults","ObjectState","ObjectStateEnum","Order","OrderCreateRequest","OrderPaginatedList","OrderStatusEnum","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustraliaEnum","ParcelTemplateCouriersPleaseEnum","ParcelTemplateDHLeCommerceEnum","ParcelTemplateDPDUKEnum","ParcelTemplateFedExEnum","ParcelTemplateUPSEnum","ParcelTemplateUSPSEnum","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ResponseType","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupTypeEnum","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostalEnum","ServiceLevelAPGEnum","ServiceLevelAirterraEnum","ServiceLevelAramexAustraliaEnum","ServiceLevelAsendiaEnum","ServiceLevelAustraliaPostEnum","ServiceLevelAxleHireEnum","ServiceLevelBetterTrucksEnum","ServiceLevelCDLEnum","ServiceLevelCanadaPostEnum","ServiceLevelChronopostEnum","ServiceLevelColissimoEnum","ServiceLevelCorreosEspanaEnum","ServiceLevelCouriersPleaseEnum","ServiceLevelDHLExpressEnum","ServiceLevelDHLGermanyEnum","ServiceLevelDHLeCommerceEnum","ServiceLevelDPDDEEnum","ServiceLevelDPDUKEnum","ServiceLevelDeutschePostEnum","ServiceLevelEvriUKEnum","ServiceLevelFedExEnum","ServiceLevelGLSUSEnum","ServiceLevelGlobegisticsEnum","ServiceLevelLSOEnum","ServiceLevelLasershipEnum","ServiceLevelMaergoEnum","ServiceLevelMondialRelayEnum","ServiceLevelOnTracEnum","ServiceLevelParcelforceEnum","ServiceLevelPostItalianeEnum","ServiceLevelPurolatorEnum","ServiceLevelRoyalMailEnum","ServiceLevelSendleEnum","ServiceLevelSwyftEnum","ServiceLevelUDSEnum","ServiceLevelUPSEnum","ServiceLevelUSPSEnum","ServiceLevelVehoEnum","ServiceLevelePostGlobalEnum","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnitEnum"]
```

### Comparing `shippo-3.3.3/src/shippo/models/components/address.py` & `shippo-3.3.4/src/shippo/models/components/address.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/addresscompletecreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/addresscompletecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/addresscreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/addresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/addressimporter.py` & `shippo-3.3.4/src/shippo/models/components/addressimporter.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/addresspaginatedlist.py` & `shippo-3.3.4/src/shippo/models/components/addresspaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/addressvalidationresults.py` & `shippo-3.3.4/src/shippo/models/components/addressvalidationresults.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/addressvalidationresultsmessage.py` & `shippo-3.3.4/src/shippo/models/components/addressvalidationresultsmessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/alcohol.py` & `shippo-3.3.4/src/shippo/models/components/alcohol.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/batch.py` & `shippo-3.3.4/src/shippo/models/components/batch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/batchcreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/batchcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/batchshipment.py` & `shippo-3.3.4/src/shippo/models/components/batchshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/batchshipmentbase.py` & `shippo-3.3.4/src/shippo/models/components/batchshipmentbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/batchshipmentpaginatedlist.py` & `shippo-3.3.4/src/shippo/models/components/batchshipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/billing.py` & `shippo-3.3.4/src/shippo/models/components/billing.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccount.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccount.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .carrieraccountservicelevel import CarrierAccountServiceLevel
+from .fedexconnectexistingownaccountparameters import FedExConnectExistingOwnAccountParameters
 from .upsconnectexistingownaccountparameters import UPSConnectExistingOwnAccountParameters
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Any, Dict, List, Optional, Union
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
@@ -21,15 +22,15 @@
     r"""Carrier token, see <a href=\\"#tag/Carriers\\">Carriers</a><br>
     Please check the <a href=\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\">carrier accounts tutorial</a> page for all supported carriers.
     """
     active: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('active'), 'exclude': lambda f: f is None }})
     r"""Determines whether the account is active. When creating a shipment, if no `carrier_accounts` are explicitly
     passed Shippo will query all carrier accounts that have this field set. By default, this is set to True.
     """
-    parameters: Optional[Union[Dict[str, Any], UPSConnectExistingOwnAccountParameters]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
+    parameters: Optional[Union[Dict[str, Any], FedExConnectExistingOwnAccountParameters, UPSConnectExistingOwnAccountParameters]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
     carrier_name: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_name'), 'exclude': lambda f: f is None }})
     r"""Carrier name, see <a href=\\"#tag/Carriers\\">Carriers</a><br>"""
     is_shippo_account: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_shippo_account'), 'exclude': lambda f: f is None }})
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the carrier account object."""
     object_owner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_owner'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountbase.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountbase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from .fedexconnectexistingownaccountparameters import FedExConnectExistingOwnAccountParameters
 from .upsconnectexistingownaccountparameters import UPSConnectExistingOwnAccountParameters
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Any, Dict, Optional, Union
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
@@ -20,10 +21,10 @@
     r"""Carrier token, see <a href=\\"#tag/Carriers\\">Carriers</a><br>
     Please check the <a href=\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\">carrier accounts tutorial</a> page for all supported carriers.
     """
     active: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('active'), 'exclude': lambda f: f is None }})
     r"""Determines whether the account is active. When creating a shipment, if no `carrier_accounts` are explicitly
     passed Shippo will query all carrier accounts that have this field set. By default, this is set to True.
     """
-    parameters: Optional[Union[Dict[str, Any], UPSConnectExistingOwnAccountParameters]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
+    parameters: Optional[Union[Dict[str, Any], FedExConnectExistingOwnAccountParameters, UPSConnectExistingOwnAccountParameters]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountchronopostcreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountchronopostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountcolissimocreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountcolissimocreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountcorreoscreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountcorreoscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountdpddecreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountdpddecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountdpdukcreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountdpdukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountfedexcreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountfedexcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccounthermesukcreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccounthermesukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountpaginatedlist.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountregistrationstatus.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountservicelevel.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountupscreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountupscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountupscreaterequestparameters.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountupscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountuspscreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountuspscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carrieraccountwithextrainfo.py` & `shippo-3.3.4/src/shippo/models/components/carrieraccountwithextrainfo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .carrieraccountservicelevel import CarrierAccountServiceLevel
+from .fedexconnectexistingownaccountparameters import FedExConnectExistingOwnAccountParameters
 from .upsconnectexistingownaccountparameters import UPSConnectExistingOwnAccountParameters
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import Any, Dict, List, Optional, Union
 
 class CarrierAccountWithExtraInfoType(str, Enum):
@@ -53,15 +54,15 @@
     r"""Carrier token, see <a href=\\"#tag/Carriers\\">Carriers</a><br>
     Please check the <a href=\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\">carrier accounts tutorial</a> page for all supported carriers.
     """
     active: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('active'), 'exclude': lambda f: f is None }})
     r"""Determines whether the account is active. When creating a shipment, if no `carrier_accounts` are explicitly
     passed Shippo will query all carrier accounts that have this field set. By default, this is set to True.
     """
-    parameters: Optional[Union[Dict[str, Any], UPSConnectExistingOwnAccountParameters]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
+    parameters: Optional[Union[Dict[str, Any], FedExConnectExistingOwnAccountParameters, UPSConnectExistingOwnAccountParameters]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
     carrier_name: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_name'), 'exclude': lambda f: f is None }})
     r"""Carrier name, see <a href=\\"#tag/Carriers\\">Carriers</a><br>"""
     is_shippo_account: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_shippo_account'), 'exclude': lambda f: f is None }})
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the carrier account object."""
     object_owner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_owner'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.3.3/src/shippo/models/components/carrierparceltemplate.py` & `shippo-3.3.4/src/shippo/models/components/carrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/carriersenum.py` & `shippo-3.3.4/src/shippo/models/components/carriersenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/cod.py` & `shippo-3.3.4/src/shippo/models/components/cod.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/connectexistingownaccountrequest.py` & `shippo-3.3.4/src/shippo/models/components/shipmentpaginatedlist.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .upsconnectexistingownaccountparameters import UPSConnectExistingOwnAccountParameters
+from .shipment import Shipment
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
-from typing import Any, Dict, Optional, Union
+from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ConnectExistingOwnAccountRequest:
-    account_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_id') }})
-    carrier: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier') }})
-    parameters: Union[Dict[str, Any], UPSConnectExistingOwnAccountParameters] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters') }})
-    active: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('active'), 'exclude': lambda f: f is None }})
-    metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
-    test: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('test'), 'exclude': lambda f: f is None }})
+class ShipmentPaginatedList:
+    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
+    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
+    results: Optional[List[Shipment]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.3.3/src/shippo/models/components/customerreference.py` & `shippo-3.3.4/src/shippo/models/components/customerreference.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/customsdeclaration.py` & `shippo-3.3.4/src/shippo/models/components/customsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py` & `shippo-3.3.4/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/customsdeclarationcreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/customsdeclarationcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/customsdeclarationeelpfcenum.py` & `shippo-3.3.4/src/shippo/models/components/customsdeclarationeelpfcenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/customsdeclarationincotermenum.py` & `shippo-3.3.4/src/shippo/models/components/customsdeclarationincotermenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/customsdeclarationpaginatedlist.py` & `shippo-3.3.4/src/shippo/models/components/customsdeclarationpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/customsexporteridentification.py` & `shippo-3.3.4/src/shippo/models/components/customsexporteridentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/customsinvoicedcharges.py` & `shippo-3.3.4/src/shippo/models/components/customsinvoicedcharges.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/customsitem.py` & `shippo-3.3.4/src/shippo/models/components/customsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/customsitemcreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/customsitemcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/customsitempaginatedlist.py` & `shippo-3.3.4/src/shippo/models/components/customsitempaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/customstaxidentification.py` & `shippo-3.3.4/src/shippo/models/components/customstaxidentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py` & `shippo-3.3.4/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/dangerousgoodslithiumbatteries.py` & `shippo-3.3.4/src/shippo/models/components/dangerousgoodslithiumbatteries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/dangerousgoodsobject.py` & `shippo-3.3.4/src/shippo/models/components/dangerousgoodsobject.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/defaultparceltemplate.py` & `shippo-3.3.4/src/shippo/models/components/defaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/defaultparceltemplateupdaterequest.py` & `shippo-3.3.4/src/shippo/models/components/defaultparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/departmentnumber.py` & `shippo-3.3.4/src/shippo/models/components/departmentnumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/dryice.py` & `shippo-3.3.4/src/shippo/models/components/dryice.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/errormessage.py` & `shippo-3.3.4/src/shippo/models/components/errormessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/instanttransactioncreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/instanttransactioncreaterequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,11 +22,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class InstantTransactionCreateRequest:
     carrier_account: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_account') }})
     servicelevel_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('servicelevel_token') }})
     shipment: ShipmentCreateRequest = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipment') }})
+    async_: Optional[bool] = dataclasses.field(default=False, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('async'), 'exclude': lambda f: f is None }})
     label_file_type: Optional[LabelFileType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_file_type'), 'exclude': lambda f: f is None }})
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.3.3/src/shippo/models/components/instanttransactioncreateresponse.py` & `shippo-3.3.4/src/shippo/models/components/instanttransactioncreateresponse.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/instanttransactionrate.py` & `shippo-3.3.4/src/shippo/models/components/instanttransactionrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/insurance.py` & `shippo-3.3.4/src/shippo/models/components/insurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/invoicenumber.py` & `shippo-3.3.4/src/shippo/models/components/invoicenumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/labelfiletypeenum.py` & `shippo-3.3.4/src/shippo/models/components/labelfiletypeenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/lineitem.py` & `shippo-3.3.4/src/shippo/models/components/lineitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/lineitembase.py` & `shippo-3.3.4/src/shippo/models/components/lineitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/liverate.py` & `shippo-3.3.4/src/shippo/models/components/liverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/liveratecreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/liveratecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/liveratepaginatedlist.py` & `shippo-3.3.4/src/shippo/models/components/liveratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/location.py` & `shippo-3.3.4/src/shippo/models/components/location.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/manifest.py` & `shippo-3.3.4/src/shippo/models/components/manifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/manifestcreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/manifestcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/manifestpaginatedlist.py` & `shippo-3.3.4/src/shippo/models/components/manifestpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/order.py` & `shippo-3.3.4/src/shippo/models/components/order.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/ordercreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/ordercreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/orderpaginatedlist.py` & `shippo-3.3.4/src/shippo/models/components/orderpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/orderstatusenum.py` & `shippo-3.3.4/src/shippo/models/components/orderstatusenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/parcel.py` & `shippo-3.3.4/src/shippo/models/components/parcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/parcelcreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/parcelcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/parcelextra.py` & `shippo-3.3.4/src/shippo/models/components/parcelextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/parcelinsurance.py` & `shippo-3.3.4/src/shippo/models/components/parcelinsurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/parcelpaginatedlist.py` & `shippo-3.3.4/src/shippo/models/components/parcelpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/parcelrequest.py` & `shippo-3.3.4/src/shippo/models/components/parcelrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/parceltemplateenumset.py` & `shippo-3.3.4/src/shippo/models/components/parceltemplateenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/pickup.py` & `shippo-3.3.4/src/shippo/models/components/pickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/pickupbase.py` & `shippo-3.3.4/src/shippo/models/components/pickupbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/ponumber.py` & `shippo-3.3.4/src/shippo/models/components/ponumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/rate.py` & `shippo-3.3.4/src/shippo/models/components/rate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/ratemessage.py` & `shippo-3.3.4/src/shippo/models/components/ratemessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/ratepaginatedlist.py` & `shippo-3.3.4/src/shippo/models/components/ratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/refund.py` & `shippo-3.3.4/src/shippo/models/components/refund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/refundpaginatedlist.py` & `shippo-3.3.4/src/shippo/models/components/refundpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/refundrequestbody.py` & `shippo-3.3.4/src/shippo/models/components/refundrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/rmanumber.py` & `shippo-3.3.4/src/shippo/models/components/rmanumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/servicegroup.py` & `shippo-3.3.4/src/shippo/models/components/servicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/servicegroupaccountandservicelevel.py` & `shippo-3.3.4/src/shippo/models/components/servicegroupaccountandservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/servicegroupcreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/servicegroupcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/servicegrouptypeenum.py` & `shippo-3.3.4/src/shippo/models/components/servicegrouptypeenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/servicegroupupdaterequest.py` & `shippo-3.3.4/src/shippo/models/components/servicegroupupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/servicelevel.py` & `shippo-3.3.4/src/shippo/models/components/servicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/servicelevelenumset.py` & `shippo-3.3.4/src/shippo/models/components/servicelevelenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/shipment.py` & `shippo-3.3.4/src/shippo/models/components/shipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/shipmentcreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/shipmentcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/shipmentextra.py` & `shippo-3.3.4/src/shippo/models/components/shipmentextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/shipmentpaginatedlist.py` & `shippo-3.3.4/src/shippo/models/components/trackingstatuslocationbase.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .shipment import Shipment
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
-from typing import List, Optional
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ShipmentPaginatedList:
-    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
-    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
-    results: Optional[List[Shipment]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
+class TrackingStatusLocationBase:
+    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
+    country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
+    state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})
+    zip: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('zip'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.3.3/src/shippo/models/components/shippoaccount.py` & `shippo-3.3.4/src/shippo/models/components/shippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/shippoaccountpaginatedlist.py` & `shippo-3.3.4/src/shippo/models/components/shippoaccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/shippoaccountupdaterequest.py` & `shippo-3.3.4/src/shippo/models/components/shippoaccountupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/track.py` & `shippo-3.3.4/src/shippo/models/components/track.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/trackingstatus.py` & `shippo-3.3.4/src/shippo/models/components/trackingstatus.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TrackingStatus:
     r"""The latest tracking information of this shipment."""
-    location: TrackingStatusLocationBase = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location') }})
-    r"""An object containing zip, city, state and country information of the tracking event."""
     object_created: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
     object_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id') }})
     object_updated: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_updated'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
     status: TrackingStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
     r"""Indicates the high level status of the shipment."""
     status_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
     r"""Date and time when the carrier scanned this tracking event. This is displayed in UTC."""
     status_details: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status_details') }})
     r"""The human-readable description of the status."""
+    location: Optional[TrackingStatusLocationBase] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
+    r"""An object containing zip, city, state and country information of the tracking event."""
     substatus: Optional[TrackingStatusSubstatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('substatus'), 'exclude': lambda f: f is None }})
     r"""A finer-grained classification of the tracking event."""
```

### Comparing `shippo-3.3.3/src/shippo/models/components/trackingstatuslocationbase.py` & `shippo-3.3.4/src/shippo/models/components/transactionpaginatedlist.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from .transaction import Transaction
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
-from typing import Optional
+from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class TrackingStatusLocationBase:
-    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
-    country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
-    state: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})
-    zip: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('zip'), 'exclude': lambda f: f is None }})
+class TransactionPaginatedList:
+    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
+    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
+    results: Optional[List[Transaction]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.3.3/src/shippo/models/components/trackingstatussubstatus.py` & `shippo-3.3.4/src/shippo/models/components/trackingstatussubstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/tracksrequest.py` & `shippo-3.3.4/src/shippo/models/components/tracksrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/transaction.py` & `shippo-3.3.4/src/shippo/models/components/transaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/transactioncreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/transactioncreaterequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TransactionCreateRequest:
     rate: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rate') }})
-    async_: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('async'), 'exclude': lambda f: f is None }})
+    async_: Optional[bool] = dataclasses.field(default=True, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('async'), 'exclude': lambda f: f is None }})
     label_file_type: Optional[LabelFileTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('label_file_type'), 'exclude': lambda f: f is None }})
     r"""Print format of the <a href=\\"https://docs.goshippo.com/docs/shipments/shippinglabelsizes/\\">label</a>. If empty, will use the default format set from
     <a href=\"https://apps.goshippo.com/settings/labels\">the Shippo dashboard.</a>
     """
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.3.3/src/shippo/models/components/transactionpaginatedlist.py` & `shippo-3.3.4/src/shippo/models/operations/listaddresses.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .transaction import Transaction
-from dataclasses_json import Undefined, dataclass_json
-from shippo import utils
-from typing import List, Optional
+from typing import Optional
 
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class TransactionPaginatedList:
-    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
-    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
-    results: Optional[List[Transaction]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
+class ListAddressesGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class ListAddressesRequest:
+    page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
+    r"""The page number you want to select"""
+    results: Optional[int] = dataclasses.field(default=5, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
+    r"""The number of results to return per page (max 100, default 5)"""
```

### Comparing `shippo-3.3.3/src/shippo/models/components/upsconnectexistingownaccountparameters.py` & `shippo-3.3.4/src/shippo/models/components/upsconnectexistingownaccountparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/userparceltemplate.py` & `shippo-3.3.4/src/shippo/models/components/userparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/userparceltemplateupdaterequest.py` & `shippo-3.3.4/src/shippo/models/components/userparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py` & `shippo-3.3.4/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/errors/initiateoauth2signin.py` & `shippo-3.3.4/src/shippo/models/errors/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/errors/sdkerror.py` & `shippo-3.3.4/src/shippo/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/__init__.py` & `shippo-3.3.4/src/shippo/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/addshipmentstobatch.py` & `shippo-3.3.4/src/shippo/models/operations/addshipmentstobatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/deletedefaultparceltemplate.py` & `shippo-3.3.4/src/shippo/models/operations/deletedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/deleteservicegroup.py` & `shippo-3.3.4/src/shippo/models/operations/deleteservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/deleteuserparceltemplate.py` & `shippo-3.3.4/src/shippo/models/operations/deleteuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getaddress.py` & `shippo-3.3.4/src/shippo/models/operations/getaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getbatch.py` & `shippo-3.3.4/src/shippo/models/operations/getbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getcarrieraccount.py` & `shippo-3.3.4/src/shippo/models/operations/getcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getcarrierparceltemplate.py` & `shippo-3.3.4/src/shippo/models/operations/getcarrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getcarrierregistrationstatus.py` & `shippo-3.3.4/src/shippo/models/operations/getcarrierregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getcustomsdeclaration.py` & `shippo-3.3.4/src/shippo/models/operations/getcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getcustomsitem.py` & `shippo-3.3.4/src/shippo/models/operations/getcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getdefaultparceltemplate.py` & `shippo-3.3.4/src/shippo/models/operations/getdefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getmanifest.py` & `shippo-3.3.4/src/shippo/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getorder.py` & `shippo-3.3.4/src/shippo/models/operations/getorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getparcel.py` & `shippo-3.3.4/src/shippo/models/operations/getparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getrate.py` & `shippo-3.3.4/src/shippo/models/operations/getrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getrefund.py` & `shippo-3.3.4/src/shippo/models/operations/getrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getshipment.py` & `shippo-3.3.4/src/shippo/models/operations/getshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getshippoaccount.py` & `shippo-3.3.4/src/shippo/models/operations/getshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/gettrack.py` & `shippo-3.3.4/src/shippo/models/operations/gettrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/gettransaction.py` & `shippo-3.3.4/src/shippo/models/operations/gettransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/getuserparceltemplate.py` & `shippo-3.3.4/src/shippo/models/operations/getuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/initiateoauth2signin.py` & `shippo-3.3.4/src/shippo/models/operations/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/listaddresses.py` & `shippo-3.3.4/src/shippo/models/operations/listmanifests.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListAddressesGlobals:
+class ListManifestsGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class ListAddressesRequest:
+class ListManifestsRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     results: Optional[int] = dataclasses.field(default=5, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
     r"""The number of results to return per page (max 100, default 5)"""
```

### Comparing `shippo-3.3.3/src/shippo/models/operations/listcarrieraccounts.py` & `shippo-3.3.4/src/shippo/models/operations/listcarrieraccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/listcarrierparceltemplates.py` & `shippo-3.3.4/src/shippo/models/operations/listcarrierparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/listcustomsdeclarations.py` & `shippo-3.3.4/src/shippo/models/operations/listcustomsdeclarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/listcustomsitems.py` & `shippo-3.3.4/src/shippo/models/operations/listcustomsitems.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/listmanifests.py` & `shippo-3.3.4/src/shippo/models/operations/listorders.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListManifestsGlobals:
+class ListOrdersGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class ListManifestsRequest:
+class ListOrdersRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
-    results: Optional[int] = dataclasses.field(default=5, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
-    r"""The number of results to return per page (max 100, default 5)"""
+    results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
+    r"""The number of results to return per page (max 100)"""
```

### Comparing `shippo-3.3.3/src/shippo/models/operations/listorders.py` & `shippo-3.3.4/src/shippo/models/operations/listshipments.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListOrdersGlobals:
+class ListShipmentsGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class ListOrdersRequest:
+class ListShipmentsRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
     r"""The number of results to return per page (max 100)"""
```

### Comparing `shippo-3.3.3/src/shippo/models/operations/listparcels.py` & `shippo-3.3.4/src/shippo/models/operations/listparcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/listservicegroups.py` & `shippo-3.3.4/src/shippo/models/operations/listservicegroups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/listshipmentrates.py` & `shippo-3.3.4/src/shippo/models/operations/listshipmentrates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/listshipmentratesbycurrencycode.py` & `shippo-3.3.4/src/shippo/models/operations/listshipmentratesbycurrencycode.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/listshipments.py` & `shippo-3.3.4/src/shippo/models/operations/listshippoaccounts.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListShipmentsGlobals:
+class ListShippoAccountsGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class ListShipmentsRequest:
+class ListShippoAccountsRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
     r"""The number of results to return per page (max 100)"""
```

### Comparing `shippo-3.3.3/src/shippo/models/operations/listshippoaccounts.py` & `shippo-3.3.4/src/shippo/models/operations/removeshipmentsfrombatch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from typing import Optional
+from typing import List, Optional
 
 
 @dataclasses.dataclass
-class ListShippoAccountsGlobals:
+class RemoveShipmentsFromBatchGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class ListShippoAccountsRequest:
-    page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-    r"""The page number you want to select"""
-    results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
-    r"""The number of results to return per page (max 100)"""
+class RemoveShipmentsFromBatchRequest:
+    batch_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'BatchId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the batch"""
+    request_body: Optional[List[str]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    r"""Array of shipments object ids to remove from the batch"""
```

### Comparing `shippo-3.3.3/src/shippo/models/operations/listtransactions.py` & `shippo-3.3.4/src/shippo/models/operations/listtransactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/listuserparceltemplates.py` & `shippo-3.3.4/src/shippo/models/operations/listuserparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/purchasebatch.py` & `shippo-3.3.4/src/shippo/models/operations/purchasebatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/removeshipmentsfrombatch.py` & `shippo-3.3.4/src/shippo/models/operations/updateuserparceltemplate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from typing import List, Optional
+from ...models.components import userparceltemplateupdaterequest as components_userparceltemplateupdaterequest
+from typing import Optional
 
 
 @dataclasses.dataclass
-class RemoveShipmentsFromBatchGlobals:
+class UpdateUserParcelTemplateGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class RemoveShipmentsFromBatchRequest:
-    batch_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'BatchId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the batch"""
-    request_body: Optional[List[str]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    r"""Array of shipments object ids to remove from the batch"""
+class UpdateUserParcelTemplateRequest:
+    user_parcel_template_object_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'UserParcelTemplateObjectId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the user parcel template"""
+    user_parcel_template_update_request: Optional[components_userparceltemplateupdaterequest.UserParcelTemplateUpdateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
```

### Comparing `shippo-3.3.3/src/shippo/models/operations/updatecarrieraccount.py` & `shippo-3.3.4/src/shippo/models/operations/updatecarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/updateshippoaccount.py` & `shippo-3.3.4/src/shippo/models/operations/updateshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/models/operations/validateaddress.py` & `shippo-3.3.4/src/shippo/models/operations/validateaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/orders.py` & `shippo-3.3.4/src/shippo/orders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/parcels.py` & `shippo-3.3.4/src/shippo/parcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/pickups.py` & `shippo-3.3.4/src/shippo/pickups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/rates.py` & `shippo-3.3.4/src/shippo/rates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/rates_at_checkout.py` & `shippo-3.3.4/src/shippo/rates_at_checkout.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/refunds.py` & `shippo-3.3.4/src/shippo/refunds.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/sdk.py` & `shippo-3.3.4/src/shippo/sdk.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/sdkconfiguration.py` & `shippo-3.3.4/src/shippo/sdkconfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '2018-02-08'
-    sdk_version: str = '3.3.3'
-    gen_version: str = '2.314.0'
-    user_agent: str = 'speakeasy-sdk/python 3.3.3 2.314.0 2018-02-08 shippo'
+    sdk_version: str = '3.3.4'
+    gen_version: str = '2.322.5'
+    user_agent: str = 'speakeasy-sdk/python 3.3.4 2.322.5 2018-02-08 shippo'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `shippo-3.3.3/src/shippo/service_groups.py` & `shippo-3.3.4/src/shippo/service_groups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/shipments.py` & `shippo-3.3.4/src/shippo/shipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/shippo_accounts.py` & `shippo-3.3.4/src/shippo/shippo_accounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/tracking_status.py` & `shippo-3.3.4/src/shippo/tracking_status.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/transactions.py` & `shippo-3.3.4/src/shippo/transactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/user_parcel_templates.py` & `shippo-3.3.4/src/shippo/user_parcel_templates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/utils/retries.py` & `shippo-3.3.4/src/shippo/utils/retries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.3/src/shippo/utils/utils.py` & `shippo-3.3.4/src/shippo/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -904,14 +904,41 @@
 
 
 def bigintdecoder(val):
     if isinstance(val, float):
         raise ValueError(f"{val} is a float")
     return int(val)
 
+def integerstrencoder(optional: bool):
+    def integerstrencode(val: int):
+        if optional and val is None:
+            return None
+        return str(val)
+
+    return integerstrencode
+
+
+def integerstrdecoder(val):
+    if isinstance(val, float):
+        raise ValueError(f"{val} is a float")
+    return int(val)
+
+
+def numberstrencoder(optional: bool):
+    def numberstrencode(val: float):
+        if optional and val is None:
+            return None
+        return str(val)
+
+    return numberstrencode
+
+
+def numberstrdecoder(val):
+    return float(val)
+
 
 def decimalencoder(optional: bool, as_str: bool):
     def decimalencode(val: Decimal):
         if optional and val is None:
             return None
 
         if as_str:
```

### Comparing `shippo-3.3.3/src/shippo.egg-info/PKG-INFO` & `shippo-3.3.4/src/shippo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.3.3
+Version: 3.3.4
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.3.3/src/shippo.egg-info/SOURCES.txt` & `shippo-3.3.4/src/shippo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 src/shippo/models/components/dangerousgoodsobject.py
 src/shippo/models/components/defaultparceltemplate.py
 src/shippo/models/components/defaultparceltemplateupdaterequest.py
 src/shippo/models/components/departmentnumber.py
 src/shippo/models/components/distanceunitenum.py
 src/shippo/models/components/dryice.py
 src/shippo/models/components/errormessage.py
+src/shippo/models/components/fedexconnectexistingownaccountparameters.py
 src/shippo/models/components/instanttransactioncreaterequest.py
 src/shippo/models/components/instanttransactioncreateresponse.py
 src/shippo/models/components/instanttransactionrate.py
 src/shippo/models/components/insurance.py
 src/shippo/models/components/invoicenumber.py
 src/shippo/models/components/labelfiletypeenum.py
 src/shippo/models/components/lineitem.py
```

