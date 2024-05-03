# Comparing `tmp/pywikibot-9.1.1.tar.gz` & `tmp/pywikibot-9.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywikibot-9.1.1.tar", last modified: Sat Apr 27 11:16:01 2024, max compression
+gzip compressed data, was "pywikibot-9.1.2.tar", last modified: Fri May  3 06:01:55 2024, max compression
```

## Comparing `pywikibot-9.1.1.tar` & `pywikibot-9.1.2.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 11:16:01.797104 pywikibot-9.1.1/
--rw-rw-rw-   0        0        0     4184 2024-04-22 08:27:47.000000 pywikibot-9.1.1/AUTHORS.rst
--rw-rw-rw-   0        0        0      177 2024-04-20 14:45:29.000000 pywikibot-9.1.1/CODE_OF_CONDUCT.rst
--rw-rw-rw-   0        0        0     1086 2024-04-20 14:45:29.000000 pywikibot-9.1.1/LICENSE
--rw-rw-rw-   0        0        0       90 2024-04-20 14:45:29.000000 pywikibot-9.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    17437 2024-04-27 11:16:01.794203 pywikibot-9.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5484 2024-04-20 14:45:29.000000 pywikibot-9.1.1/README.rst
--rw-rw-rw-   0        0        0     5934 2024-04-27 11:12:58.000000 pywikibot-9.1.1/ROADMAP.rst
--rw-rw-rw-   0        0        0     4617 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-27 11:15:59.495188 pywikibot-9.1.1/pywikibot/
--rw-rw-rw-   0        0        0    14027 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/__init__.py
--rw-rw-rw-   0        0        0      367 2024-04-27 11:12:58.000000 pywikibot-9.1.1/pywikibot/__metadata__.py
--rw-rw-rw-   0        0        0    43977 2024-04-22 08:27:47.000000 pywikibot-9.1.1/pywikibot/_wbtypes.py
--rw-rw-rw-   0        0        0     6897 2024-04-22 08:27:47.000000 pywikibot-9.1.1/pywikibot/backports.py
--rw-rw-rw-   0        0        0    87385 2024-04-22 10:42:12.000000 pywikibot-9.1.1/pywikibot/bot.py
--rw-rw-rw-   0        0        0    27855 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/bot_choice.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:15:59.612498 pywikibot-9.1.1/pywikibot/comms/
--rw-rw-rw-   0        0        0      121 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/comms/__init__.py
--rw-rw-rw-   0        0        0    15778 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/comms/eventstreams.py
--rw-rw-rw-   0        0        0    20032 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/comms/http.py
--rw-rw-rw-   0        0        0    45908 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/config.py
--rw-rw-rw-   0        0        0    46627 2024-04-22 08:27:47.000000 pywikibot-9.1.1/pywikibot/cosmetic_changes.py
--rw-rw-rw-   0        0        0     2096 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/daemonize.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:15:59.670389 pywikibot-9.1.1/pywikibot/data/
--rw-rw-rw-   0        0        0     1990 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:15:59.682312 pywikibot-9.1.1/pywikibot/data/api/
--rw-rw-rw-   0        0        0     3212 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/data/api/__init__.py
--rw-rw-rw-   0        0        0    41998 2024-04-22 08:27:47.000000 pywikibot-9.1.1/pywikibot/data/api/_generators.py
--rw-rw-rw-   0        0        0     7556 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/data/api/_optionset.py
--rw-rw-rw-   0        0        0    16895 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/data/api/_paraminfo.py
--rw-rw-rw-   0        0        0    53137 2024-04-22 08:27:47.000000 pywikibot-9.1.1/pywikibot/data/api/_requests.py
--rw-rw-rw-   0        0        0    14075 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/data/memento.py
--rw-rw-rw-   0        0        0     2599 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/data/mysql.py
--rw-rw-rw-   0        0        0     9737 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/data/sparql.py
--rw-rw-rw-   0        0        0     4104 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/data/wikistats.py
--rw-rw-rw-   0        0        0    97086 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/date.py
--rw-rw-rw-   0        0        0    24621 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/diff.py
--rw-rw-rw-   0        0        0     1937 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/echo.py
--rw-rw-rw-   0        0        0     8033 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/editor.py
--rw-rw-rw-   0        0        0    20754 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:16:00.149067 pywikibot-9.1.1/pywikibot/families/
--rw-rw-rw-   0        0        0      118 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/__init__.py
--rw-rw-rw-   0        0        0     1792 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/commons_family.py
--rw-rw-rw-   0        0        0      481 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/foundation_family.py
--rw-rw-rw-   0        0        0      376 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/i18n_family.py
--rw-rw-rw-   0        0        0      393 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/incubator_family.py
--rw-rw-rw-   0        0        0      621 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/lingualibre_family.py
--rw-rw-rw-   0        0        0      439 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/mediawiki_family.py
--rw-rw-rw-   0        0        0      629 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/meta_family.py
--rw-rw-rw-   0        0        0     1243 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/osm_family.py
--rw-rw-rw-   0        0        0      407 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/outreach_family.py
--rw-rw-rw-   0        0        0      399 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/species_family.py
--rw-rw-rw-   0        0        0     1169 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/vikidia_family.py
--rw-rw-rw-   0        0        0     2444 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/wikibooks_family.py
--rw-rw-rw-   0        0        0      996 2024-04-23 14:22:19.000000 pywikibot-9.1.1/pywikibot/families/wikidata_family.py
--rw-rw-rw-   0        0        0      403 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/wikifunctions_family.py
--rw-rw-rw-   0        0        0     1669 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/wikihow_family.py
--rw-rw-rw-   0        0        0     1047 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/wikimania_family.py
--rw-rw-rw-   0        0        0      813 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/wikimediachapter_family.py
--rw-rw-rw-   0        0        0     1856 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/wikinews_family.py
--rw-rw-rw-   0        0        0    11124 2024-04-27 10:05:30.000000 pywikibot-9.1.1/pywikibot/families/wikipedia_family.py
--rw-rw-rw-   0        0        0     2919 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/wikiquote_family.py
--rw-rw-rw-   0        0        0     5373 2024-04-27 10:05:30.000000 pywikibot-9.1.1/pywikibot/families/wikisource_family.py
--rw-rw-rw-   0        0        0      469 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/wikispore_family.py
--rw-rw-rw-   0        0        0      463 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/wikitech_family.py
--rw-rw-rw-   0        0        0     1176 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/wikiversity_family.py
--rw-rw-rw-   0        0        0     1053 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/wikivoyage_family.py
--rw-rw-rw-   0        0        0     4166 2024-04-27 10:05:30.000000 pywikibot-9.1.1/pywikibot/families/wiktionary_family.py
--rw-rw-rw-   0        0        0     2452 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/families/wowwiki_family.py
--rw-rw-rw-   0        0        0    43417 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/family.py
--rw-rw-rw-   0        0        0    33229 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/fixes.py
--rw-rw-rw-   0        0        0    20614 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/flow.py
--rw-rw-rw-   0        0        0    29937 2024-04-22 08:27:47.000000 pywikibot-9.1.1/pywikibot/i18n.py
--rw-rw-rw-   0        0        0     7896 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/interwiki_graph.py
--rw-rw-rw-   0        0        0    13048 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/logentries.py
--rw-rw-rw-   0        0        0    12576 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/logging.py
--rw-rw-rw-   0        0        0    22774 2024-04-22 08:27:47.000000 pywikibot-9.1.1/pywikibot/login.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:16:00.184968 pywikibot-9.1.1/pywikibot/page/
--rw-rw-rw-   0        0        0     1289 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/page/__init__.py
--rw-rw-rw-   0        0        0    88531 2024-04-22 08:27:47.000000 pywikibot-9.1.1/pywikibot/page/_basepage.py
--rw-rw-rw-   0        0        0    14617 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/page/_category.py
--rw-rw-rw-   0        0        0    19031 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/page/_collections.py
--rw-rw-rw-   0        0        0     2175 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/page/_decorators.py
--rw-rw-rw-   0        0        0    19962 2024-04-22 08:27:47.000000 pywikibot-9.1.1/pywikibot/page/_filepage.py
--rw-rw-rw-   0        0        0    29468 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/page/_links.py
--rw-rw-rw-   0        0        0     8551 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/page/_page.py
--rw-rw-rw-   0        0        0     3035 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/page/_revision.py
--rw-rw-rw-   0        0        0     4055 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/page/_toolforge.py
--rw-rw-rw-   0        0        0    16532 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/page/_user.py
--rw-rw-rw-   0        0        0    90813 2024-04-22 08:27:47.000000 pywikibot-9.1.1/pywikibot/page/_wikibase.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:16:00.301666 pywikibot-9.1.1/pywikibot/pagegenerators/
--rw-rw-rw-   0        0        0    29759 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/pagegenerators/__init__.py
--rw-rw-rw-   0        0        0    41066 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/pagegenerators/_factory.py
--rw-rw-rw-   0        0        0    18463 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/pagegenerators/_filters.py
--rw-rw-rw-   0        0        0    46417 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/pagegenerators/_generators.py
--rw-rw-rw-   0        0        0     3955 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/plural.py
--rw-rw-rw-   0        0        0    49322 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/proofreadpage.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:16:00.404382 pywikibot-9.1.1/pywikibot/scripts/
--rw-rw-rw-   0        0        0      921 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/scripts/__init__.py
--rw-rw-rw-   0        0        0    12328 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/scripts/generate_family_file.py
--rw-rw-rw-   0        0        0    20040 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/scripts/generate_user_files.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:16:00.419344 pywikibot-9.1.1/pywikibot/scripts/i18n/
--rw-rw-rw-   0        0        0      349 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:16:01.523834 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/
--rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ab.json
--rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/af.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/an.json
--rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ar.json
--rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/arc.json
--rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ast.json
--rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/av.json
--rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/awa.json
--rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/az.json
--rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/azb.json
--rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ba.json
--rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/bar.json
--rw-rw-rw-   0        0        0      991 2023-10-07 15:32:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/bcc.json
--rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/be-tarask.json
--rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/be.json
--rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/bg.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/bjn.json
--rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/bn.json
--rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/bo.json
--rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/br.json
--rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/bs.json
--rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ca.json
--rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ce.json
--rw-rw-rw-   0        0        0      865 2023-10-07 15:32:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ckb.json
--rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/cs.json
--rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/csb.json
--rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/cy.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/da.json
--rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/de.json
--rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/diq.json
--rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/el.json
--rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/en.json
--rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/eo.json
--rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/es.json
--rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/et.json
--rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/eu.json
--rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/fa.json
--rw-rw-rw-   0        0        0      713 2023-07-21 09:20:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/fi.json
--rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/fo.json
--rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/fr.json
--rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/frp.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/frr.json
--rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/fy.json
--rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ga.json
--rw-rw-rw-   0        0        0     1083 2023-07-21 09:20:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/gl.json
--rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/gsw.json
--rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/hak.json
--rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/haw.json
--rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/he.json
--rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/hi.json
--rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/hr.json
--rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/hsb.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/hu.json
--rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/hy.json
--rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ia.json
--rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/id.json
--rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ie.json
--rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ig.json
--rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ilo.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/io.json
--rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/is.json
--rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/it.json
--rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ja.json
--rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/jv.json
--rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/kab.json
--rw-rw-rw-   0        0        0     1079 2023-07-21 09:20:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/kk.json
--rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/km.json
--rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/kn.json
--rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ko.json
--rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/krc.json
--rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ksh.json
--rw-rw-rw-   0        0        0      652 2024-01-30 13:30:45.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ku.json
--rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ky.json
--rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/la.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/lb.json
--rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/li.json
--rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/lki.json
--rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/lt.json
--rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/lv.json
--rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/map-bms.json
--rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/mg.json
--rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/min.json
--rw-rw-rw-   0        0        0     1360 2023-07-21 09:20:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/mk.json
--rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ml.json
--rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/mni.json
--rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/mr.json
--rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ms.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/mt.json
--rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/my.json
--rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/nan.json
--rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/nb.json
--rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/nds-nl.json
--rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/nds.json
--rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ne.json
--rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/new.json
--rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/nl.json
--rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/nn.json
--rw-rw-rw-   0        0        0     1443 2023-07-21 09:20:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/nqo.json
--rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/nyn.json
--rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/oc.json
--rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/olo.json
--rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/or.json
--rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/pa.json
--rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/pdc.json
--rw-rw-rw-   0        0        0      150 2023-07-21 09:20:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/pfl.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/pl.json
--rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/pms.json
--rw-rw-rw-   0        0        0     1092 2023-10-07 15:32:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/pt-br.json
--rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/pt.json
--rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/qqq.json
--rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ro.json
--rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ru.json
--rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/scn.json
--rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sco.json
--rw-rw-rw-   0        0        0      369 2023-07-21 09:20:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sd.json
--rw-rw-rw-   0        0        0      101 2023-10-07 15:32:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sdh.json
--rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sh.json
--rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/si.json
--rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sk.json
--rw-rw-rw-   0        0        0      193 2023-10-07 15:32:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/skr.json
--rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sl.json
--rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sms.json
--rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/so.json
--rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sq.json
--rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sr.json
--rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/su.json
--rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sv.json
--rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sw.json
--rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/szl.json
--rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ta.json
--rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/te.json
--rw-rw-rw-   0        0        0      116 2023-07-21 09:20:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/tg.json
--rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/th.json
--rw-rw-rw-   0        0        0      170 2023-07-21 09:20:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/tk.json
--rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/tl.json
--rw-rw-rw-   0        0        0     1126 2023-07-21 09:20:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/tly.json
--rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/tr.json
--rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/tt.json
--rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/uk.json
--rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ur.json
--rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/uz.json
--rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/vec.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/vep.json
--rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/vi.json
--rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/vo.json
--rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/war.json
--rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/yi.json
--rw-rw-rw-   0        0        0      832 2023-10-07 15:32:07.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/yue.json
--rw-rw-rw-   0        0        0     1094 2023-12-04 18:41:20.000000 pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/zh.json
--rw-rw-rw-   0        0        0     6095 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/scripts/login.py
--rw-rw-rw-   0        0        0     3449 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/scripts/preload_sites.py
--rw-rw-rw-   0        0        0     2045 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/scripts/shell.py
--rw-rw-rw-   0        0        0     3139 2024-04-27 10:08:50.000000 pywikibot-9.1.1/pywikibot/scripts/version.py
--rw-rw-rw-   0        0        0    18718 2024-04-22 08:27:47.000000 pywikibot-9.1.1/pywikibot/scripts/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:16:01.560735 pywikibot-9.1.1/pywikibot/site/
--rw-rw-rw-   0        0        0     1051 2024-04-22 08:27:47.000000 pywikibot-9.1.1/pywikibot/site/__init__.py
--rw-rw-rw-   0        0        0   116994 2024-04-23 17:36:35.000000 pywikibot-9.1.1/pywikibot/site/_apisite.py
--rw-rw-rw-   0        0        0    16617 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/site/_basesite.py
--rw-rw-rw-   0        0        0    38399 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/site/_datasite.py
--rw-rw-rw-   0        0        0     4090 2024-04-27 10:05:30.000000 pywikibot-9.1.1/pywikibot/site/_decorators.py
--rw-rw-rw-   0        0        0    29727 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/site/_extensions.py
--rw-rw-rw-   0        0        0    98105 2024-04-23 16:31:41.000000 pywikibot-9.1.1/pywikibot/site/_generators.py
--rw-rw-rw-   0        0        0     3004 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/site/_interwikimap.py
--rw-rw-rw-   0        0        0    15079 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/site/_namespace.py
--rw-rw-rw-   0        0        0     1586 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/site/_obsoletesites.py
--rw-rw-rw-   0        0        0    12928 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/site/_siteinfo.py
--rw-rw-rw-   0        0        0     4844 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/site/_tokenwallet.py
--rw-rw-rw-   0        0        0    25238 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/site/_upload.py
--rw-rw-rw-   0        0        0    11158 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/site_detect.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:16:01.613617 pywikibot-9.1.1/pywikibot/specialbots/
--rw-rw-rw-   0        0        0      409 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/specialbots/__init__.py
--rw-rw-rw-   0        0        0     3142 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/specialbots/_unlink.py
--rw-rw-rw-   0        0        0    20865 2024-04-22 08:27:47.000000 pywikibot-9.1.1/pywikibot/specialbots/_upload.py
--rw-rw-rw-   0        0        0    87673 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/textlib.py
--rw-rw-rw-   0        0        0    12246 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/throttle.py
--rw-rw-rw-   0        0        0    20620 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/time.py
--rw-rw-rw-   0        0        0     3259 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/titletranslate.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:16:01.676432 pywikibot-9.1.1/pywikibot/tools/
--rw-rw-rw-   0        0        0    27110 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/tools/__init__.py
--rw-rw-rw-   0        0        0    25676 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/tools/_deprecate.py
--rw-rw-rw-   0        0        0     1243 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/tools/_logging.py
--rw-rw-rw-   0        0        0    22245 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/tools/_unidata.py
--rw-rw-rw-   0        0        0     4456 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/tools/chars.py
--rw-rw-rw-   0        0        0    10286 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/tools/collections.py
--rw-rw-rw-   0        0        0    10984 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/tools/djvu.py
--rw-rw-rw-   0        0        0     4060 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/tools/formatter.py
--rw-rw-rw-   0        0        0     8988 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/tools/itertools.py
--rw-rw-rw-   0        0        0     7248 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/tools/threading.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:16:01.756299 pywikibot-9.1.1/pywikibot/userinterfaces/
--rw-rw-rw-   0        0        0      910 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/userinterfaces/__init__.py
--rw-rw-rw-   0        0        0     1885 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/userinterfaces/_interface_base.py
--rw-rw-rw-   0        0        0     2713 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/userinterfaces/buffer_interface.py
--rw-rw-rw-   0        0        0    22357 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/userinterfaces/gui.py
--rw-rw-rw-   0        0        0      495 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/userinterfaces/terminal_interface.py
--rw-rw-rw-   0        0        0    25232 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/userinterfaces/terminal_interface_base.py
--rw-rw-rw-   0        0        0     2152 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/userinterfaces/terminal_interface_unix.py
--rw-rw-rw-   0        0        0     2048 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/userinterfaces/terminal_interface_win32.py
--rw-rw-rw-   0        0        0    90667 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/userinterfaces/transliteration.py
--rw-rw-rw-   0        0        0    14992 2024-04-22 08:27:47.000000 pywikibot-9.1.1/pywikibot/version.py
--rw-rw-rw-   0        0        0    11113 2024-04-20 14:45:29.000000 pywikibot-9.1.1/pywikibot/xmlreader.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:16:01.777157 pywikibot-9.1.1/pywikibot.egg-info/
--rw-rw-rw-   0        0        0    17437 2024-04-27 11:15:59.000000 pywikibot-9.1.1/pywikibot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10561 2024-04-27 11:15:59.000000 pywikibot-9.1.1/pywikibot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 11:15:59.000000 pywikibot-9.1.1/pywikibot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-27 11:15:59.000000 pywikibot-9.1.1/pywikibot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      982 2024-04-27 11:15:59.000000 pywikibot-9.1.1/pywikibot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-27 11:15:59.000000 pywikibot-9.1.1/pywikibot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 11:16:01.797320 pywikibot-9.1.1/setup.cfg
--rw-rw-rw-   0        0        0     8130 2024-04-20 14:45:29.000000 pywikibot-9.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 11:16:01.774305 pywikibot-9.1.1/tests/
--rw-rw-rw-   0        0        0     2832 2024-04-20 14:45:29.000000 pywikibot-9.1.1/tests/tests_tests.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.801658 pywikibot-9.1.2/
+-rw-rw-rw-   0        0        0     4207 2024-05-02 14:46:17.000000 pywikibot-9.1.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0      177 2024-04-20 14:45:29.000000 pywikibot-9.1.2/CODE_OF_CONDUCT.rst
+-rw-rw-rw-   0        0        0     1086 2024-04-20 14:45:29.000000 pywikibot-9.1.2/LICENSE
+-rw-rw-rw-   0        0        0       90 2024-04-20 14:45:29.000000 pywikibot-9.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    17474 2024-05-03 06:01:55.800200 pywikibot-9.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5484 2024-04-20 14:45:29.000000 pywikibot-9.1.2/README.rst
+-rw-rw-rw-   0        0        0     5939 2024-05-03 06:00:19.000000 pywikibot-9.1.2/ROADMAP.rst
+-rw-rw-rw-   0        0        0     4617 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.363586 pywikibot-9.1.2/pywikibot/
+-rw-rw-rw-   0        0        0    14027 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/__init__.py
+-rw-rw-rw-   0        0        0      363 2024-05-03 06:00:19.000000 pywikibot-9.1.2/pywikibot/__metadata__.py
+-rw-rw-rw-   0        0        0    43977 2024-05-02 08:38:56.000000 pywikibot-9.1.2/pywikibot/_wbtypes.py
+-rw-rw-rw-   0        0        0     6897 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/backports.py
+-rw-rw-rw-   0        0        0    87385 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/bot.py
+-rw-rw-rw-   0        0        0    27855 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/bot_choice.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.438739 pywikibot-9.1.2/pywikibot/comms/
+-rw-rw-rw-   0        0        0      121 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/comms/__init__.py
+-rw-rw-rw-   0        0        0    15778 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/comms/eventstreams.py
+-rw-rw-rw-   0        0        0    20032 2024-05-02 11:42:30.000000 pywikibot-9.1.2/pywikibot/comms/http.py
+-rw-rw-rw-   0        0        0    45908 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/config.py
+-rw-rw-rw-   0        0        0    46627 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/cosmetic_changes.py
+-rw-rw-rw-   0        0        0     2096 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/daemonize.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.450699 pywikibot-9.1.2/pywikibot/data/
+-rw-rw-rw-   0        0        0     1990 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.467657 pywikibot-9.1.2/pywikibot/data/api/
+-rw-rw-rw-   0        0        0     3212 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/data/api/__init__.py
+-rw-rw-rw-   0        0        0    41998 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/data/api/_generators.py
+-rw-rw-rw-   0        0        0     7556 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/data/api/_optionset.py
+-rw-rw-rw-   0        0        0    16895 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/data/api/_paraminfo.py
+-rw-rw-rw-   0        0        0    53137 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/data/api/_requests.py
+-rw-rw-rw-   0        0        0    14075 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/data/memento.py
+-rw-rw-rw-   0        0        0     2599 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/data/mysql.py
+-rw-rw-rw-   0        0        0     9737 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/data/sparql.py
+-rw-rw-rw-   0        0        0     4104 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/data/wikistats.py
+-rw-rw-rw-   0        0        0    97086 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/date.py
+-rw-rw-rw-   0        0        0    24621 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/diff.py
+-rw-rw-rw-   0        0        0     1937 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/echo.py
+-rw-rw-rw-   0        0        0     8033 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/editor.py
+-rw-rw-rw-   0        0        0    20732 2024-05-02 15:55:46.000000 pywikibot-9.1.2/pywikibot/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.528648 pywikibot-9.1.2/pywikibot/families/
+-rw-rw-rw-   0        0        0      118 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/__init__.py
+-rw-rw-rw-   0        0        0     1792 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/commons_family.py
+-rw-rw-rw-   0        0        0      481 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/foundation_family.py
+-rw-rw-rw-   0        0        0      376 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/i18n_family.py
+-rw-rw-rw-   0        0        0      393 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/incubator_family.py
+-rw-rw-rw-   0        0        0      621 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/lingualibre_family.py
+-rw-rw-rw-   0        0        0      439 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/mediawiki_family.py
+-rw-rw-rw-   0        0        0      629 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/meta_family.py
+-rw-rw-rw-   0        0        0     1243 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/osm_family.py
+-rw-rw-rw-   0        0        0      407 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/outreach_family.py
+-rw-rw-rw-   0        0        0      399 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/species_family.py
+-rw-rw-rw-   0        0        0     1169 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/vikidia_family.py
+-rw-rw-rw-   0        0        0     2444 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikibooks_family.py
+-rw-rw-rw-   0        0        0      996 2024-04-23 14:22:19.000000 pywikibot-9.1.2/pywikibot/families/wikidata_family.py
+-rw-rw-rw-   0        0        0      403 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/wikifunctions_family.py
+-rw-rw-rw-   0        0        0     1669 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikihow_family.py
+-rw-rw-rw-   0        0        0     1047 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikimania_family.py
+-rw-rw-rw-   0        0        0      813 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikimediachapter_family.py
+-rw-rw-rw-   0        0        0     1856 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikinews_family.py
+-rw-rw-rw-   0        0        0    11124 2024-05-02 08:38:56.000000 pywikibot-9.1.2/pywikibot/families/wikipedia_family.py
+-rw-rw-rw-   0        0        0     2919 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikiquote_family.py
+-rw-rw-rw-   0        0        0     5373 2024-05-02 08:38:56.000000 pywikibot-9.1.2/pywikibot/families/wikisource_family.py
+-rw-rw-rw-   0        0        0      469 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/wikispore_family.py
+-rw-rw-rw-   0        0        0      463 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/families/wikitech_family.py
+-rw-rw-rw-   0        0        0     1176 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikiversity_family.py
+-rw-rw-rw-   0        0        0     1053 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wikivoyage_family.py
+-rw-rw-rw-   0        0        0     4166 2024-05-02 08:38:56.000000 pywikibot-9.1.2/pywikibot/families/wiktionary_family.py
+-rw-rw-rw-   0        0        0     2452 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/families/wowwiki_family.py
+-rw-rw-rw-   0        0        0    43417 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/family.py
+-rw-rw-rw-   0        0        0    33229 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/fixes.py
+-rw-rw-rw-   0        0        0    20614 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/flow.py
+-rw-rw-rw-   0        0        0    29937 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/i18n.py
+-rw-rw-rw-   0        0        0     7896 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/interwiki_graph.py
+-rw-rw-rw-   0        0        0    13048 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/logentries.py
+-rw-rw-rw-   0        0        0    12576 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/logging.py
+-rw-rw-rw-   0        0        0    22774 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/login.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.552548 pywikibot-9.1.2/pywikibot/page/
+-rw-rw-rw-   0        0        0     1289 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/__init__.py
+-rw-rw-rw-   0        0        0    88531 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/page/_basepage.py
+-rw-rw-rw-   0        0        0    14617 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_category.py
+-rw-rw-rw-   0        0        0    19031 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_collections.py
+-rw-rw-rw-   0        0        0     2175 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_decorators.py
+-rw-rw-rw-   0        0        0    19962 2024-05-02 08:38:56.000000 pywikibot-9.1.2/pywikibot/page/_filepage.py
+-rw-rw-rw-   0        0        0    29468 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_links.py
+-rw-rw-rw-   0        0        0     8551 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_page.py
+-rw-rw-rw-   0        0        0     3035 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_revision.py
+-rw-rw-rw-   0        0        0     4055 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_toolforge.py
+-rw-rw-rw-   0        0        0    16532 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/page/_user.py
+-rw-rw-rw-   0        0        0    90813 2024-05-02 08:38:56.000000 pywikibot-9.1.2/pywikibot/page/_wikibase.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.562727 pywikibot-9.1.2/pywikibot/pagegenerators/
+-rw-rw-rw-   0        0        0    29759 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/pagegenerators/__init__.py
+-rw-rw-rw-   0        0        0    41066 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/pagegenerators/_factory.py
+-rw-rw-rw-   0        0        0    18463 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/pagegenerators/_filters.py
+-rw-rw-rw-   0        0        0    46417 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/pagegenerators/_generators.py
+-rw-rw-rw-   0        0        0     3955 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/plural.py
+-rw-rw-rw-   0        0        0    49322 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/proofreadpage.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.578806 pywikibot-9.1.2/pywikibot/scripts/
+-rw-rw-rw-   0        0        0      921 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/scripts/__init__.py
+-rw-rw-rw-   0        0        0    12328 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/scripts/generate_family_file.py
+-rw-rw-rw-   0        0        0    20040 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/scripts/generate_user_files.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:54.592440 pywikibot-9.1.2/pywikibot/scripts/i18n/
+-rw-rw-rw-   0        0        0      349 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.679358 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/
+-rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ab.json
+-rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/af.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/an.json
+-rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ar.json
+-rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/arc.json
+-rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ast.json
+-rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/av.json
+-rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/awa.json
+-rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/az.json
+-rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/azb.json
+-rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ba.json
+-rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bar.json
+-rw-rw-rw-   0        0        0      991 2023-10-07 15:32:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bcc.json
+-rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/be-tarask.json
+-rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/be.json
+-rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bg.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bjn.json
+-rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bn.json
+-rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bo.json
+-rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/br.json
+-rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bs.json
+-rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ca.json
+-rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ce.json
+-rw-rw-rw-   0        0        0      865 2023-10-07 15:32:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ckb.json
+-rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/cs.json
+-rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/csb.json
+-rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/cy.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/da.json
+-rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/de.json
+-rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/diq.json
+-rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/el.json
+-rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/en.json
+-rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/eo.json
+-rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/es.json
+-rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/et.json
+-rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/eu.json
+-rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fa.json
+-rw-rw-rw-   0        0        0      713 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fi.json
+-rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fo.json
+-rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fr.json
+-rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/frp.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/frr.json
+-rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fy.json
+-rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ga.json
+-rw-rw-rw-   0        0        0     1083 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/gl.json
+-rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/gsw.json
+-rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hak.json
+-rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/haw.json
+-rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/he.json
+-rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hi.json
+-rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hr.json
+-rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hsb.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hu.json
+-rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hy.json
+-rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ia.json
+-rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/id.json
+-rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ie.json
+-rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ig.json
+-rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ilo.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/io.json
+-rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/is.json
+-rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/it.json
+-rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ja.json
+-rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/jv.json
+-rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/kab.json
+-rw-rw-rw-   0        0        0     1079 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/kk.json
+-rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/km.json
+-rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/kn.json
+-rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ko.json
+-rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/krc.json
+-rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ksh.json
+-rw-rw-rw-   0        0        0      652 2024-01-30 13:30:45.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ku.json
+-rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ky.json
+-rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/la.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/lb.json
+-rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/li.json
+-rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/lki.json
+-rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/lt.json
+-rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/lv.json
+-rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/map-bms.json
+-rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/mg.json
+-rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/min.json
+-rw-rw-rw-   0        0        0     1360 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/mk.json
+-rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ml.json
+-rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/mni.json
+-rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/mr.json
+-rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ms.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/mt.json
+-rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/my.json
+-rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nan.json
+-rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nb.json
+-rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nds-nl.json
+-rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nds.json
+-rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ne.json
+-rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/new.json
+-rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nl.json
+-rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nn.json
+-rw-rw-rw-   0        0        0     1443 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nqo.json
+-rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nyn.json
+-rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/oc.json
+-rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/olo.json
+-rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/or.json
+-rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pa.json
+-rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pdc.json
+-rw-rw-rw-   0        0        0      150 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pfl.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pl.json
+-rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pms.json
+-rw-rw-rw-   0        0        0     1092 2023-10-07 15:32:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pt-br.json
+-rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pt.json
+-rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/qqq.json
+-rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ro.json
+-rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ru.json
+-rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/scn.json
+-rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sco.json
+-rw-rw-rw-   0        0        0      369 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sd.json
+-rw-rw-rw-   0        0        0      101 2023-10-07 15:32:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sdh.json
+-rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sh.json
+-rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/si.json
+-rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sk.json
+-rw-rw-rw-   0        0        0      193 2023-10-07 15:32:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/skr.json
+-rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sl.json
+-rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sms.json
+-rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/so.json
+-rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sq.json
+-rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sr.json
+-rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/su.json
+-rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sv.json
+-rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sw.json
+-rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/szl.json
+-rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ta.json
+-rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/te.json
+-rw-rw-rw-   0        0        0      116 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tg.json
+-rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/th.json
+-rw-rw-rw-   0        0        0      170 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tk.json
+-rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tl.json
+-rw-rw-rw-   0        0        0     1126 2023-07-21 09:20:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tly.json
+-rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tr.json
+-rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tt.json
+-rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/uk.json
+-rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ur.json
+-rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/uz.json
+-rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/vec.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/vep.json
+-rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/vi.json
+-rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/vo.json
+-rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/war.json
+-rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/yi.json
+-rw-rw-rw-   0        0        0      832 2023-10-07 15:32:07.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/yue.json
+-rw-rw-rw-   0        0        0     1094 2023-12-04 18:41:20.000000 pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/zh.json
+-rw-rw-rw-   0        0        0     6095 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/scripts/login.py
+-rw-rw-rw-   0        0        0     3449 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/scripts/preload_sites.py
+-rw-rw-rw-   0        0        0     2045 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/scripts/shell.py
+-rw-rw-rw-   0        0        0     3501 2024-05-03 06:00:19.000000 pywikibot-9.1.2/pywikibot/scripts/version.py
+-rw-rw-rw-   0        0        0    18718 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/scripts/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.719192 pywikibot-9.1.2/pywikibot/site/
+-rw-rw-rw-   0        0        0     1051 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/site/__init__.py
+-rw-rw-rw-   0        0        0   116994 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/site/_apisite.py
+-rw-rw-rw-   0        0        0    16617 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/site/_basesite.py
+-rw-rw-rw-   0        0        0    38399 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site/_datasite.py
+-rw-rw-rw-   0        0        0     4105 2024-05-02 14:46:17.000000 pywikibot-9.1.2/pywikibot/site/_decorators.py
+-rw-rw-rw-   0        0        0    29727 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site/_extensions.py
+-rw-rw-rw-   0        0        0    98105 2024-05-02 08:38:56.000000 pywikibot-9.1.2/pywikibot/site/_generators.py
+-rw-rw-rw-   0        0        0     3004 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site/_interwikimap.py
+-rw-rw-rw-   0        0        0    15079 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site/_namespace.py
+-rw-rw-rw-   0        0        0     1586 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site/_obsoletesites.py
+-rw-rw-rw-   0        0        0    12928 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/site/_siteinfo.py
+-rw-rw-rw-   0        0        0     4844 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site/_tokenwallet.py
+-rw-rw-rw-   0        0        0    25238 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site/_upload.py
+-rw-rw-rw-   0        0        0    11158 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/site_detect.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.730212 pywikibot-9.1.2/pywikibot/specialbots/
+-rw-rw-rw-   0        0        0      409 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/specialbots/__init__.py
+-rw-rw-rw-   0        0        0     3142 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/specialbots/_unlink.py
+-rw-rw-rw-   0        0        0    20865 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/specialbots/_upload.py
+-rw-rw-rw-   0        0        0    87673 2024-04-30 12:33:22.000000 pywikibot-9.1.2/pywikibot/textlib.py
+-rw-rw-rw-   0        0        0    12246 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/throttle.py
+-rw-rw-rw-   0        0        0    20620 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/time.py
+-rw-rw-rw-   0        0        0     3259 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/titletranslate.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.759332 pywikibot-9.1.2/pywikibot/tools/
+-rw-rw-rw-   0        0        0    27110 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/tools/__init__.py
+-rw-rw-rw-   0        0        0    25676 2024-05-02 14:46:17.000000 pywikibot-9.1.2/pywikibot/tools/_deprecate.py
+-rw-rw-rw-   0        0        0     1243 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/tools/_logging.py
+-rw-rw-rw-   0        0        0    22245 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/tools/_unidata.py
+-rw-rw-rw-   0        0        0     4456 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/tools/chars.py
+-rw-rw-rw-   0        0        0    10286 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/tools/collections.py
+-rw-rw-rw-   0        0        0    10984 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/tools/djvu.py
+-rw-rw-rw-   0        0        0     4060 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/tools/formatter.py
+-rw-rw-rw-   0        0        0     8988 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/tools/itertools.py
+-rw-rw-rw-   0        0        0     7248 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/tools/threading.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.782296 pywikibot-9.1.2/pywikibot/userinterfaces/
+-rw-rw-rw-   0        0        0      910 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/__init__.py
+-rw-rw-rw-   0        0        0     1885 2024-04-28 12:23:49.000000 pywikibot-9.1.2/pywikibot/userinterfaces/_interface_base.py
+-rw-rw-rw-   0        0        0     2713 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/buffer_interface.py
+-rw-rw-rw-   0        0        0    22357 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/gui.py
+-rw-rw-rw-   0        0        0      495 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/terminal_interface.py
+-rw-rw-rw-   0        0        0    25232 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/terminal_interface_base.py
+-rw-rw-rw-   0        0        0     2152 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/terminal_interface_unix.py
+-rw-rw-rw-   0        0        0     2048 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/terminal_interface_win32.py
+-rw-rw-rw-   0        0        0    90667 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/userinterfaces/transliteration.py
+-rw-rw-rw-   0        0        0    15031 2024-05-03 04:36:59.000000 pywikibot-9.1.2/pywikibot/version.py
+-rw-rw-rw-   0        0        0    11113 2024-04-20 14:45:29.000000 pywikibot-9.1.2/pywikibot/xmlreader.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.787212 pywikibot-9.1.2/pywikibot.egg-info/
+-rw-rw-rw-   0        0        0    17474 2024-05-03 06:01:54.000000 pywikibot-9.1.2/pywikibot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10561 2024-05-03 06:01:54.000000 pywikibot-9.1.2/pywikibot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 06:01:54.000000 pywikibot-9.1.2/pywikibot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-03 06:01:54.000000 pywikibot-9.1.2/pywikibot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      982 2024-05-03 06:01:54.000000 pywikibot-9.1.2/pywikibot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-03 06:01:54.000000 pywikibot-9.1.2/pywikibot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 06:01:55.801658 pywikibot-9.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     8130 2024-04-28 12:23:49.000000 pywikibot-9.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 06:01:55.785244 pywikibot-9.1.2/tests/
+-rw-rw-rw-   0        0        0     2832 2024-04-20 14:45:29.000000 pywikibot-9.1.2/tests/tests_tests.py
```

### Comparing `pywikibot-9.1.1/AUTHORS.rst` & `pywikibot-9.1.2/AUTHORS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Ævar Arnfjörð Bjarmason
     akashagarwal
     AkshitKumar
     Alangi Derick
     Alex Shih-Han Lin
     Alexander Jones
     Alexander Shtyrov
+    Alexander Vorwerk
     Alfio
     Allen Guo
     Amir Sarabadani
     Ananth subray
     André Costa
     Andre Engels
     André Malafaya Baptista
```

### Comparing `pywikibot-9.1.1/LICENSE` & `pywikibot-9.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/PKG-INFO` & `pywikibot-9.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 9.1.1
+Version: 9.1.2
 Summary: Python MediaWiki Bot Framework
 Author-email: xqt <info@gno.de>
 Maintainer-email: The Pywikibot team <pywikibot@lists.wikimedia.org>
 License: MIT License
 Project-URL: Homepage, https://www.mediawiki.org/wiki/Manual:Pywikibot
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
 Project-URL: Repository, https://gerrit.wikimedia.org/r/plugins/gitiles/pywikibot/core/
@@ -295,16 +295,16 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* Add support for new wikis
-  (T363272, T363265T363258T363251T363245T360312T360305)
+* Remove line endings in version.getversion_nightly(T363943)
+* Provide ``-nouser`` option with pywikibot.scripts.version
 * i18n updates
 
 Deprecations
 ------------
 
 * 9.0.0: The *content* parameter of proofreadpage.IndexPage.page_genis deprecated and will be ignored
   (T358635)
```

### Comparing `pywikibot-9.1.1/README.rst` & `pywikibot-9.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/ROADMAP.rst` & `pywikibot-9.1.2/ROADMAP.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Current release
 ---------------
 
-* Add support for new wikis
-  (:phab:`T363272`, :phab:`T363265`:phab:`T363258`:phab:`T363251`:phab:`T363245`:phab:`T360312`:phab:`T360305`)
+* Remove line endings in :func:`version.getversion_nightly` (:phab:`T363943`)
+* Provide ``-nouser`` option with :mod:`pywikibot.scripts.version`
 * i18n updates
 
 Deprecations
 ------------
 
 * 9.0.0: The *content* parameter of :meth:`proofreadpage.IndexPage.page_gen` is deprecated and will be ignored
   (:phab:`T358635`)
```

### Comparing `pywikibot-9.1.1/pyproject.toml` & `pywikibot-9.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/__init__.py` & `pywikibot-9.1.2/pywikibot/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/_wbtypes.py` & `pywikibot-9.1.2/pywikibot/_wbtypes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/backports.py` & `pywikibot-9.1.2/pywikibot/backports.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/bot.py` & `pywikibot-9.1.2/pywikibot/bot.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/bot_choice.py` & `pywikibot-9.1.2/pywikibot/bot_choice.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/comms/eventstreams.py` & `pywikibot-9.1.2/pywikibot/comms/eventstreams.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/comms/http.py` & `pywikibot-9.1.2/pywikibot/comms/http.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/config.py` & `pywikibot-9.1.2/pywikibot/config.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/cosmetic_changes.py` & `pywikibot-9.1.2/pywikibot/cosmetic_changes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/daemonize.py` & `pywikibot-9.1.2/pywikibot/daemonize.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/data/__init__.py` & `pywikibot-9.1.2/pywikibot/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/data/api/__init__.py` & `pywikibot-9.1.2/pywikibot/data/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/data/api/_generators.py` & `pywikibot-9.1.2/pywikibot/data/api/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/data/api/_optionset.py` & `pywikibot-9.1.2/pywikibot/data/api/_optionset.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/data/api/_paraminfo.py` & `pywikibot-9.1.2/pywikibot/data/api/_paraminfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/data/api/_requests.py` & `pywikibot-9.1.2/pywikibot/data/api/_requests.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/data/memento.py` & `pywikibot-9.1.2/pywikibot/data/memento.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/data/mysql.py` & `pywikibot-9.1.2/pywikibot/data/mysql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/data/sparql.py` & `pywikibot-9.1.2/pywikibot/data/sparql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/data/wikistats.py` & `pywikibot-9.1.2/pywikibot/data/wikistats.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/date.py` & `pywikibot-9.1.2/pywikibot/date.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/diff.py` & `pywikibot-9.1.2/pywikibot/diff.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/echo.py` & `pywikibot-9.1.2/pywikibot/echo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/editor.py` & `pywikibot-9.1.2/pywikibot/editor.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/exceptions.py` & `pywikibot-9.1.2/pywikibot/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,19 +73,19 @@
   - CaptchaError: Captcha is asked and config.solve_captcha == False
   - ClientError: A problem with the client request
   - AutoblockUserError: requested action on a virtual autoblock user not valid
   - InvalidTitleError: Invalid page title
   - NoUsernameError: Username is not in user config file, or it is invalid.
   - PageInUseError: Page cannot be reserved due to a lock
   - SectionError: The section specified by # does not exist
-  - TranslationError: no language translation found
+  - TranslationError: no language translation found, i18n/l10n message
+    not available
   - UnknownExtensionError: Extension is not defined for this site
   - UserRightsError: insufficient rights for requested action
   - VersionParseError: failed to parse version information
-  - i18n.TranslationError: i18n/l10n message not available
 
 APIError: wiki API returned an error
 
   - APIMWError: MediaWiki internal exception
   - UploadError: upload failed
 
 SiteDefinitionError: Site loading problem
```

### Comparing `pywikibot-9.1.1/pywikibot/families/commons_family.py` & `pywikibot-9.1.2/pywikibot/families/commons_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/lingualibre_family.py` & `pywikibot-9.1.2/pywikibot/families/lingualibre_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/meta_family.py` & `pywikibot-9.1.2/pywikibot/families/meta_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/osm_family.py` & `pywikibot-9.1.2/pywikibot/families/osm_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/vikidia_family.py` & `pywikibot-9.1.2/pywikibot/families/vikidia_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/wikibooks_family.py` & `pywikibot-9.1.2/pywikibot/families/wikibooks_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/wikidata_family.py` & `pywikibot-9.1.2/pywikibot/families/wikidata_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/wikihow_family.py` & `pywikibot-9.1.2/pywikibot/families/wikihow_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/wikimania_family.py` & `pywikibot-9.1.2/pywikibot/families/wikimania_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/wikimediachapter_family.py` & `pywikibot-9.1.2/pywikibot/families/wikimediachapter_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/wikinews_family.py` & `pywikibot-9.1.2/pywikibot/families/wikinews_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/wikipedia_family.py` & `pywikibot-9.1.2/pywikibot/families/wikipedia_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/wikiquote_family.py` & `pywikibot-9.1.2/pywikibot/families/wikiquote_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/wikisource_family.py` & `pywikibot-9.1.2/pywikibot/families/wikisource_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/wikiversity_family.py` & `pywikibot-9.1.2/pywikibot/families/wikiversity_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/wikivoyage_family.py` & `pywikibot-9.1.2/pywikibot/families/wikivoyage_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/wiktionary_family.py` & `pywikibot-9.1.2/pywikibot/families/wiktionary_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/families/wowwiki_family.py` & `pywikibot-9.1.2/pywikibot/families/wowwiki_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/family.py` & `pywikibot-9.1.2/pywikibot/family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/fixes.py` & `pywikibot-9.1.2/pywikibot/fixes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/flow.py` & `pywikibot-9.1.2/pywikibot/flow.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/i18n.py` & `pywikibot-9.1.2/pywikibot/i18n.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/interwiki_graph.py` & `pywikibot-9.1.2/pywikibot/interwiki_graph.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/logentries.py` & `pywikibot-9.1.2/pywikibot/logentries.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/logging.py` & `pywikibot-9.1.2/pywikibot/logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/login.py` & `pywikibot-9.1.2/pywikibot/login.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/page/__init__.py` & `pywikibot-9.1.2/pywikibot/page/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/page/_basepage.py` & `pywikibot-9.1.2/pywikibot/page/_basepage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/page/_category.py` & `pywikibot-9.1.2/pywikibot/page/_category.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/page/_collections.py` & `pywikibot-9.1.2/pywikibot/page/_collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/page/_decorators.py` & `pywikibot-9.1.2/pywikibot/page/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/page/_filepage.py` & `pywikibot-9.1.2/pywikibot/page/_filepage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/page/_links.py` & `pywikibot-9.1.2/pywikibot/page/_links.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/page/_page.py` & `pywikibot-9.1.2/pywikibot/page/_page.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/page/_revision.py` & `pywikibot-9.1.2/pywikibot/page/_revision.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/page/_toolforge.py` & `pywikibot-9.1.2/pywikibot/page/_toolforge.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/page/_user.py` & `pywikibot-9.1.2/pywikibot/page/_user.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/page/_wikibase.py` & `pywikibot-9.1.2/pywikibot/page/_wikibase.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/pagegenerators/__init__.py` & `pywikibot-9.1.2/pywikibot/pagegenerators/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/pagegenerators/_factory.py` & `pywikibot-9.1.2/pywikibot/pagegenerators/_factory.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/pagegenerators/_filters.py` & `pywikibot-9.1.2/pywikibot/pagegenerators/_filters.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/pagegenerators/_generators.py` & `pywikibot-9.1.2/pywikibot/pagegenerators/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/plural.py` & `pywikibot-9.1.2/pywikibot/plural.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/proofreadpage.py` & `pywikibot-9.1.2/pywikibot/proofreadpage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/__init__.py` & `pywikibot-9.1.2/pywikibot/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/generate_family_file.py` & `pywikibot-9.1.2/pywikibot/scripts/generate_family_file.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/generate_user_files.py` & `pywikibot-9.1.2/pywikibot/scripts/generate_user_files.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ar.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ar.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ast.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ast.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/az.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/az.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/azb.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/azb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ba.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ba.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/bcc.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bcc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/be-tarask.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/be-tarask.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/be.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/be.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/bg.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/bn.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/br.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/bs.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/bs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ca.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ca.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ce.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ce.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ckb.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ckb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/cs.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/cs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/csb.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/csb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/cy.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/cy.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/da.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/da.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/de.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/de.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/diq.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/diq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/el.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/el.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/en.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/en.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/eo.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/eo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/es.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/es.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/eu.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/eu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/fa.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fa.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/fi.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/fo.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/fr.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/fr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/frr.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/frr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/gl.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/gl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/gsw.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/gsw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/hak.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hak.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/haw.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/haw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/he.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/he.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/hi.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/hsb.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hsb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/hu.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/hu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ia.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ia.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/id.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/id.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/io.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/io.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/is.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/is.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/it.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/it.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ja.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ja.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/kab.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/kab.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/kk.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/kk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/km.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/km.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/kn.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/kn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ko.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ko.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/krc.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/krc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ksh.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ksh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ku.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ku.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/lb.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/lb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/lt.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/lt.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/lv.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/lv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/map-bms.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/map-bms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/mg.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/mg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/min.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/min.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/mk.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/mk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ml.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ml.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ms.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/my.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/my.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/nan.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nan.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/nb.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/nds-nl.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nds-nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ne.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ne.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/new.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/new.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/nl.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/nqo.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/nqo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/pl.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/pms.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/pt-br.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pt-br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/pt.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/pt.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/qqq.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/qqq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ro.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ro.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ru.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ru.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sco.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sco.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sh.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/si.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/si.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sk.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sl.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/so.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/so.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sr.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sv.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/sw.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/sw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ta.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ta.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/te.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/te.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/th.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/th.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/tly.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tly.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/tr.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/tr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/uk.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/uk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/ur.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/ur.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/vi.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/vi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/yue.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/yue.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/i18n/pywikibot/zh.json` & `pywikibot-9.1.2/pywikibot/scripts/i18n/pywikibot/zh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/login.py` & `pywikibot-9.1.2/pywikibot/scripts/login.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/preload_sites.py` & `pywikibot-9.1.2/pywikibot/scripts/preload_sites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/shell.py` & `pywikibot-9.1.2/pywikibot/scripts/shell.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/scripts/version.py` & `pywikibot-9.1.2/pywikibot/scripts/version.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 #!/usr/bin/env python3
 """Script to determine the Pywikibot version (tag, revision and date).
 
+The following option is supported:
+
+-usernames  print usernames for each registered family
+
 .. versionchanged:: 7.0
    version script was moved to the framework scripts folder
+.. versionadded:: 9.1.2
+   the *-nouser* option.
 """
 #
 # (C) Pywikibot team, 2007-2024
 #
 # Distributed under the terms of the MIT license.
 #
 from __future__ import annotations
@@ -47,15 +53,19 @@
     requests = DummyModule()
 
 
 WMF_CACERT = 'MIIDxTCCAq2gAwIBAgIQAqxcJmoLQJuPC3nyrkYldzANBgkqhkiG9w0BAQUFADBs'
 
 
 def main(*args: str) -> None:
-    """Print pywikibot version and important settings."""
+    """Print pywikibot version and important settings.
+
+    .. versionchanged:: 9.1.2
+       usernames are not printed with ``-nouser`` option.
+    """
     pywikibot.info('Pywikibot: ' + getversion())
     pywikibot.info('Release version: ' + pywikibot.__version__)
     pywikibot.info('packaging version: ' + packaging.__version__)
     pywikibot.info('mwparserfromhell version: ' + mwparserfromhell.__version__)
     pywikibot.info('wikitextparser version: ' + wikitextparser.__version__)
     pywikibot.info('requests version: ' + requests.__version__)
 
@@ -86,15 +96,20 @@
                      'PYWIKIBOT_NO_USER_CONFIG'])
     for environ_name in sorted(settings):
         pywikibot.info(
             '{}: {}'.format(environ_name,
                             os.environ.get(environ_name, 'Not set') or "''"))
 
     pywikibot.info('Config base dir: ' + pywikibot.config.base_dir)
-    for family, usernames in pywikibot.config.usernames.items():
+
+    if '-nouser' in sys.argv:
+        usernames_items = {}
+    else:
+        usernames_items = pywikibot.config.usernames.items()
+    for family, usernames in usernames_items:
         if not usernames:
             continue
         pywikibot.info(f"Usernames for family '{family}':")
         for lang, username in usernames.items():
             pywikibot.info(f'\t{lang}: {username}')
```

### Comparing `pywikibot-9.1.1/pywikibot/scripts/wrapper.py` & `pywikibot-9.1.2/pywikibot/scripts/wrapper.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/site/__init__.py` & `pywikibot-9.1.2/pywikibot/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/site/_apisite.py` & `pywikibot-9.1.2/pywikibot/site/_apisite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/site/_basesite.py` & `pywikibot-9.1.2/pywikibot/site/_basesite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/site/_datasite.py` & `pywikibot-9.1.2/pywikibot/site/_datasite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/site/_decorators.py` & `pywikibot-9.1.2/pywikibot/site/_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                     rights = ' but:\n' + fill(
                         str(sorted(self.userinfo['rights'])),
                         width=76, break_on_hyphens=False)
                 else:
                     rights = '.'
                 raise UserRightsError(
                     f'User "{self.user()}" does not have required user right '
-                    f'"{right}"{rights}')
+                    f'"{right}" on site {self}{rights}')
             return fn(self, *args, **kwargs)
 
         manage_wrapping(callee, fn)
         return callee
 
     return decorator
```

### Comparing `pywikibot-9.1.1/pywikibot/site/_extensions.py` & `pywikibot-9.1.2/pywikibot/site/_extensions.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/site/_generators.py` & `pywikibot-9.1.2/pywikibot/site/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/site/_interwikimap.py` & `pywikibot-9.1.2/pywikibot/site/_interwikimap.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/site/_namespace.py` & `pywikibot-9.1.2/pywikibot/site/_namespace.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/site/_obsoletesites.py` & `pywikibot-9.1.2/pywikibot/site/_obsoletesites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/site/_siteinfo.py` & `pywikibot-9.1.2/pywikibot/site/_siteinfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/site/_tokenwallet.py` & `pywikibot-9.1.2/pywikibot/site/_tokenwallet.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/site/_upload.py` & `pywikibot-9.1.2/pywikibot/site/_upload.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/site_detect.py` & `pywikibot-9.1.2/pywikibot/site_detect.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/specialbots/_unlink.py` & `pywikibot-9.1.2/pywikibot/specialbots/_unlink.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/specialbots/_upload.py` & `pywikibot-9.1.2/pywikibot/specialbots/_upload.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/textlib.py` & `pywikibot-9.1.2/pywikibot/textlib.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/throttle.py` & `pywikibot-9.1.2/pywikibot/throttle.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/time.py` & `pywikibot-9.1.2/pywikibot/time.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/titletranslate.py` & `pywikibot-9.1.2/pywikibot/titletranslate.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/tools/__init__.py` & `pywikibot-9.1.2/pywikibot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/tools/_deprecate.py` & `pywikibot-9.1.2/pywikibot/tools/_deprecate.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,15 +309,15 @@
 
     Usage:
 
         @deprecate_arg('foo', 'bar')
         def my_function(bar='baz'): pass
         # replaces 'foo' keyword by 'bar' used by my_function
 
-        @deprecare_arg('foo', None)
+        @deprecate_arg('foo', None)
         def my_function(): pass
         # ignores 'foo' keyword no longer used by my_function
 
     :func:`deprecated_args` decorator should be used in favour of this
     ``deprecate_arg`` decorator but it is held to deprecate args which
     become a reserved word in future Python releases and to prevent
     syntax errors.
```

### Comparing `pywikibot-9.1.1/pywikibot/tools/_logging.py` & `pywikibot-9.1.2/pywikibot/tools/_logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/tools/_unidata.py` & `pywikibot-9.1.2/pywikibot/tools/_unidata.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/tools/chars.py` & `pywikibot-9.1.2/pywikibot/tools/chars.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/tools/collections.py` & `pywikibot-9.1.2/pywikibot/tools/collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/tools/djvu.py` & `pywikibot-9.1.2/pywikibot/tools/djvu.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/tools/formatter.py` & `pywikibot-9.1.2/pywikibot/tools/formatter.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/tools/itertools.py` & `pywikibot-9.1.2/pywikibot/tools/itertools.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/tools/threading.py` & `pywikibot-9.1.2/pywikibot/tools/threading.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/userinterfaces/__init__.py` & `pywikibot-9.1.2/pywikibot/userinterfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/userinterfaces/_interface_base.py` & `pywikibot-9.1.2/pywikibot/userinterfaces/_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/userinterfaces/buffer_interface.py` & `pywikibot-9.1.2/pywikibot/userinterfaces/buffer_interface.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/userinterfaces/gui.py` & `pywikibot-9.1.2/pywikibot/userinterfaces/gui.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/userinterfaces/terminal_interface_base.py` & `pywikibot-9.1.2/pywikibot/userinterfaces/terminal_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/userinterfaces/terminal_interface_unix.py` & `pywikibot-9.1.2/pywikibot/userinterfaces/terminal_interface_unix.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/userinterfaces/terminal_interface_win32.py` & `pywikibot-9.1.2/pywikibot/userinterfaces/terminal_interface_win32.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/userinterfaces/transliteration.py` & `pywikibot-9.1.2/pywikibot/userinterfaces/transliteration.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot/version.py` & `pywikibot-9.1.2/pywikibot/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,33 +237,36 @@
     rev = f'g{len(rev.splitlines())}'
     hsh = info[3]  # also stored in '.git/refs/heads/master'
     if (not date or not tag or not rev) and not path:
         raise VersionParseError
     return (tag, rev, date, hsh)
 
 
-def getversion_nightly(path: str | Path | None = None):  # pragma: no cover
+def getversion_nightly(path: str | Path | None = None):
     """Get version info for a nightly release.
 
     .. hint::
        the version informations of the nightly dump is stored in the
        ``version`` file within the ``pywikibot`` folder.
 
     :param path: directory of the uncompressed nightly.
     :return:
         - tag (name for the repository),
         - rev (current revision identifier),
         - date (date of current revision),
         - hash (git hash for the current revision)
     :rtype: ``tuple`` of three ``str`` and a ``time.struct_time``
     """
-    file = Path(path or _get_program_dir()) / 'pywikibot' / 'version'
+    file = Path(path or _get_program_dir())
+    if not path:
+        file /= 'pywikibot'
+    file /= 'version'
 
     with file.open() as data:
-        (tag, rev, date, hsh) = data.readlines()
+        (tag, rev, date, hsh) = data.read().splitlines()
 
     date = time.strptime(date[:19], '%Y-%m-%dT%H:%M:%S')
 
     if not date or not tag or not rev:
         raise VersionParseError
     return (tag, rev, date, hsh)
 
@@ -283,15 +286,15 @@
 
     tag = 'pywikibot/__init__.py'
     rev = '-1 (unknown)'
 
     return (tag, rev, date, hsh)
 
 
-def getversion_onlinerepo(path: str = 'branches/master'):
+def getversion_onlinerepo(path: str = 'branches/master') -> str:
     """Retrieve current framework git hash from Gerrit."""
     # Gerrit API responses include )]}' at the beginning,
     # make sure to strip it out
     buf = fetch(
         'https://gerrit.wikimedia.org/r/projects/pywikibot%2Fcore/' + path,
         headers={'user-agent': '{pwb}'}).text[4:]
     try:
```

### Comparing `pywikibot-9.1.1/pywikibot/xmlreader.py` & `pywikibot-9.1.2/pywikibot/xmlreader.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot.egg-info/PKG-INFO` & `pywikibot-9.1.2/pywikibot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 9.1.1
+Version: 9.1.2
 Summary: Python MediaWiki Bot Framework
 Author-email: xqt <info@gno.de>
 Maintainer-email: The Pywikibot team <pywikibot@lists.wikimedia.org>
 License: MIT License
 Project-URL: Homepage, https://www.mediawiki.org/wiki/Manual:Pywikibot
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
 Project-URL: Repository, https://gerrit.wikimedia.org/r/plugins/gitiles/pywikibot/core/
@@ -295,16 +295,16 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* Add support for new wikis
-  (T363272, T363265T363258T363251T363245T360312T360305)
+* Remove line endings in version.getversion_nightly(T363943)
+* Provide ``-nouser`` option with pywikibot.scripts.version
 * i18n updates
 
 Deprecations
 ------------
 
 * 9.0.0: The *content* parameter of proofreadpage.IndexPage.page_genis deprecated and will be ignored
   (T358635)
```

### Comparing `pywikibot-9.1.1/pywikibot.egg-info/SOURCES.txt` & `pywikibot-9.1.2/pywikibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/pywikibot.egg-info/requires.txt` & `pywikibot-9.1.2/pywikibot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/setup.py` & `pywikibot-9.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.1.1/tests/tests_tests.py` & `pywikibot-9.1.2/tests/tests_tests.py`

 * *Files identical despite different names*

