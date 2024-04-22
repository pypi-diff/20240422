# Comparing `tmp/pywikibot-9.0.0.tar.gz` & `tmp/pywikibot-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywikibot-9.0.0.tar", last modified: Fri Mar  8 09:41:55 2024, max compression
+gzip compressed data, was "pywikibot-9.1.0.tar", last modified: Mon Apr 22 08:24:36 2024, max compression
```

## Comparing `pywikibot-9.0.0.tar` & `pywikibot-9.1.0.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:55.369630 pywikibot-9.0.0/
--rw-rw-rw-   0        0        0     4169 2024-03-08 06:19:06.000000 pywikibot-9.0.0/AUTHORS.rst
--rw-rw-rw-   0        0        0      177 2024-02-19 10:51:11.000000 pywikibot-9.0.0/CODE_OF_CONDUCT.rst
--rw-rw-rw-   0        0        0     1086 2024-03-08 06:19:06.000000 pywikibot-9.0.0/LICENSE
--rw-rw-rw-   0        0        0       90 2024-02-19 10:51:11.000000 pywikibot-9.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    22127 2024-03-08 09:41:55.368633 pywikibot-9.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5484 2024-03-08 06:19:06.000000 pywikibot-9.0.0/README.rst
--rw-rw-rw-   0        0        0    11766 2024-03-08 08:53:18.000000 pywikibot-9.0.0/ROADMAP.rst
--rw-rw-rw-   0        0        0     4617 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:54.603671 pywikibot-9.0.0/pywikibot/
--rw-rw-rw-   0        0        0    14027 2024-03-08 08:53:18.000000 pywikibot-9.0.0/pywikibot/__init__.py
--rw-rw-rw-   0        0        0      367 2024-03-08 08:53:18.000000 pywikibot-9.0.0/pywikibot/__metadata__.py
--rw-rw-rw-   0        0        0    43975 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/_wbtypes.py
--rw-rw-rw-   0        0        0     6653 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/backports.py
--rw-rw-rw-   0        0        0    86641 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/bot.py
--rw-rw-rw-   0        0        0    27855 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/bot_choice.py
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:54.627609 pywikibot-9.0.0/pywikibot/comms/
--rw-rw-rw-   0        0        0      121 2024-02-19 10:51:11.000000 pywikibot-9.0.0/pywikibot/comms/__init__.py
--rw-rw-rw-   0        0        0    15778 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/comms/eventstreams.py
--rw-rw-rw-   0        0        0    20032 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/comms/http.py
--rw-rw-rw-   0        0        0    45908 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/config.py
--rw-rw-rw-   0        0        0    46627 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/cosmetic_changes.py
--rw-rw-rw-   0        0        0     2096 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/daemonize.py
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:54.633592 pywikibot-9.0.0/pywikibot/data/
--rw-rw-rw-   0        0        0     1990 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:54.637578 pywikibot-9.0.0/pywikibot/data/api/
--rw-rw-rw-   0        0        0     3212 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/data/api/__init__.py
--rw-rw-rw-   0        0        0    41853 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/data/api/_generators.py
--rw-rw-rw-   0        0        0     7556 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/data/api/_optionset.py
--rw-rw-rw-   0        0        0    16895 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/data/api/_paraminfo.py
--rw-rw-rw-   0        0        0    53136 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/data/api/_requests.py
--rw-rw-rw-   0        0        0    14075 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/data/memento.py
--rw-rw-rw-   0        0        0     2599 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/data/mysql.py
--rw-rw-rw-   0        0        0     9737 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/data/sparql.py
--rw-rw-rw-   0        0        0     4104 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/data/wikistats.py
--rw-rw-rw-   0        0        0    97086 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/date.py
--rw-rw-rw-   0        0        0    24621 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/diff.py
--rw-rw-rw-   0        0        0     1937 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/echo.py
--rw-rw-rw-   0        0        0     8033 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/editor.py
--rw-rw-rw-   0        0        0    20754 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:54.665505 pywikibot-9.0.0/pywikibot/families/
--rw-rw-rw-   0        0        0      118 2024-02-19 10:51:11.000000 pywikibot-9.0.0/pywikibot/families/__init__.py
--rw-rw-rw-   0        0        0     1792 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/commons_family.py
--rw-rw-rw-   0        0        0      481 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/foundation_family.py
--rw-rw-rw-   0        0        0      376 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/i18n_family.py
--rw-rw-rw-   0        0        0      393 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/incubator_family.py
--rw-rw-rw-   0        0        0      621 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/lingualibre_family.py
--rw-rw-rw-   0        0        0      439 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/mediawiki_family.py
--rw-rw-rw-   0        0        0      629 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/meta_family.py
--rw-rw-rw-   0        0        0     1243 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/osm_family.py
--rw-rw-rw-   0        0        0      407 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/outreach_family.py
--rw-rw-rw-   0        0        0      399 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/species_family.py
--rw-rw-rw-   0        0        0     1169 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/vikidia_family.py
--rw-rw-rw-   0        0        0     2444 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wikibooks_family.py
--rw-rw-rw-   0        0        0      996 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wikidata_family.py
--rw-rw-rw-   0        0        0      403 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wikifunctions_family.py
--rw-rw-rw-   0        0        0     1669 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wikihow_family.py
--rw-rw-rw-   0        0        0     1047 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wikimania_family.py
--rw-rw-rw-   0        0        0      813 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wikimediachapter_family.py
--rw-rw-rw-   0        0        0     1856 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wikinews_family.py
--rw-rw-rw-   0        0        0    11103 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wikipedia_family.py
--rw-rw-rw-   0        0        0     2919 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wikiquote_family.py
--rw-rw-rw-   0        0        0     5355 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wikisource_family.py
--rw-rw-rw-   0        0        0      469 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wikispore_family.py
--rw-rw-rw-   0        0        0      463 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wikitech_family.py
--rw-rw-rw-   0        0        0     1176 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wikiversity_family.py
--rw-rw-rw-   0        0        0     1053 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wikivoyage_family.py
--rw-rw-rw-   0        0        0     4159 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wiktionary_family.py
--rw-rw-rw-   0        0        0     2452 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/families/wowwiki_family.py
--rw-rw-rw-   0        0        0    43417 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/family.py
--rw-rw-rw-   0        0        0    33229 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/fixes.py
--rw-rw-rw-   0        0        0    20614 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/flow.py
--rw-rw-rw-   0        0        0    29937 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/i18n.py
--rw-rw-rw-   0        0        0     7896 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/interwiki_graph.py
--rw-rw-rw-   0        0        0    13048 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/logentries.py
--rw-rw-rw-   0        0        0    12576 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/logging.py
--rw-rw-rw-   0        0        0    22774 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/login.py
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:54.677472 pywikibot-9.0.0/pywikibot/page/
--rw-rw-rw-   0        0        0     1289 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/page/__init__.py
--rw-rw-rw-   0        0        0    87492 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/page/_basepage.py
--rw-rw-rw-   0        0        0    14617 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/page/_category.py
--rw-rw-rw-   0        0        0    19031 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/page/_collections.py
--rw-rw-rw-   0        0        0     2175 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/page/_decorators.py
--rw-rw-rw-   0        0        0    19949 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/page/_filepage.py
--rw-rw-rw-   0        0        0    29468 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/page/_links.py
--rw-rw-rw-   0        0        0     8551 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/page/_page.py
--rw-rw-rw-   0        0        0     3035 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/page/_revision.py
--rw-rw-rw-   0        0        0     4055 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/page/_toolforge.py
--rw-rw-rw-   0        0        0    16532 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/page/_user.py
--rw-rw-rw-   0        0        0    90696 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/page/_wikibase.py
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:54.683458 pywikibot-9.0.0/pywikibot/pagegenerators/
--rw-rw-rw-   0        0        0    29759 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/pagegenerators/__init__.py
--rw-rw-rw-   0        0        0    41066 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/pagegenerators/_factory.py
--rw-rw-rw-   0        0        0    18463 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/pagegenerators/_filters.py
--rw-rw-rw-   0        0        0    46417 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/pagegenerators/_generators.py
--rw-rw-rw-   0        0        0     3955 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/plural.py
--rw-rw-rw-   0        0        0    49322 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/proofreadpage.py
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:54.691437 pywikibot-9.0.0/pywikibot/scripts/
--rw-rw-rw-   0        0        0      921 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/scripts/__init__.py
--rw-rw-rw-   0        0        0    12328 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/scripts/generate_family_file.py
--rw-rw-rw-   0        0        0    20040 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/scripts/generate_user_files.py
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:54.691437 pywikibot-9.0.0/pywikibot/scripts/i18n/
--rw-rw-rw-   0        0        0      349 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:55.312782 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/
--rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ab.json
--rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/af.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/an.json
--rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ar.json
--rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/arc.json
--rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ast.json
--rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/av.json
--rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/awa.json
--rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/az.json
--rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/azb.json
--rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ba.json
--rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/bar.json
--rw-rw-rw-   0        0        0      991 2023-10-07 15:32:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/bcc.json
--rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/be-tarask.json
--rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/be.json
--rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/bg.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/bjn.json
--rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/bn.json
--rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/bo.json
--rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/br.json
--rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/bs.json
--rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ca.json
--rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ce.json
--rw-rw-rw-   0        0        0      865 2023-10-07 15:32:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ckb.json
--rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/cs.json
--rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/csb.json
--rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/cy.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/da.json
--rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/de.json
--rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/diq.json
--rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/el.json
--rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/en.json
--rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/eo.json
--rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/es.json
--rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/et.json
--rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/eu.json
--rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/fa.json
--rw-rw-rw-   0        0        0      713 2023-07-21 09:20:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/fi.json
--rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/fo.json
--rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/fr.json
--rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/frp.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/frr.json
--rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/fy.json
--rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ga.json
--rw-rw-rw-   0        0        0     1083 2023-07-21 09:20:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/gl.json
--rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/gsw.json
--rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/hak.json
--rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/haw.json
--rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/he.json
--rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/hi.json
--rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/hr.json
--rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/hsb.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/hu.json
--rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/hy.json
--rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ia.json
--rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/id.json
--rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ie.json
--rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ig.json
--rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ilo.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/io.json
--rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/is.json
--rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/it.json
--rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ja.json
--rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/jv.json
--rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/kab.json
--rw-rw-rw-   0        0        0     1079 2023-07-21 09:20:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/kk.json
--rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/km.json
--rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/kn.json
--rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ko.json
--rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/krc.json
--rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ksh.json
--rw-rw-rw-   0        0        0      652 2024-01-30 13:30:45.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ku.json
--rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ky.json
--rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/la.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/lb.json
--rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/li.json
--rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/lki.json
--rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/lt.json
--rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/lv.json
--rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/map-bms.json
--rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/mg.json
--rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/min.json
--rw-rw-rw-   0        0        0     1360 2023-07-21 09:20:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/mk.json
--rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ml.json
--rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/mni.json
--rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/mr.json
--rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ms.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/mt.json
--rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/my.json
--rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/nan.json
--rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/nb.json
--rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/nds-nl.json
--rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/nds.json
--rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ne.json
--rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/new.json
--rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/nl.json
--rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/nn.json
--rw-rw-rw-   0        0        0     1443 2023-07-21 09:20:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/nqo.json
--rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/nyn.json
--rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/oc.json
--rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/olo.json
--rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/or.json
--rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/pa.json
--rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/pdc.json
--rw-rw-rw-   0        0        0      150 2023-07-21 09:20:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/pfl.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/pl.json
--rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/pms.json
--rw-rw-rw-   0        0        0     1092 2023-10-07 15:32:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/pt-br.json
--rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/pt.json
--rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/qqq.json
--rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ro.json
--rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ru.json
--rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/scn.json
--rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sco.json
--rw-rw-rw-   0        0        0      369 2023-07-21 09:20:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sd.json
--rw-rw-rw-   0        0        0      101 2023-10-07 15:32:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sdh.json
--rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sh.json
--rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/si.json
--rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sk.json
--rw-rw-rw-   0        0        0      193 2023-10-07 15:32:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/skr.json
--rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sl.json
--rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sms.json
--rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/so.json
--rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sq.json
--rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sr.json
--rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/su.json
--rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sv.json
--rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sw.json
--rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/szl.json
--rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ta.json
--rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/te.json
--rw-rw-rw-   0        0        0      116 2023-07-21 09:20:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/tg.json
--rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/th.json
--rw-rw-rw-   0        0        0      170 2023-07-21 09:20:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/tk.json
--rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/tl.json
--rw-rw-rw-   0        0        0     1126 2023-07-21 09:20:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/tly.json
--rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/tr.json
--rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/tt.json
--rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/uk.json
--rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ur.json
--rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/uz.json
--rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/vec.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/vep.json
--rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/vi.json
--rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/vo.json
--rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/war.json
--rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/yi.json
--rw-rw-rw-   0        0        0      832 2023-10-07 15:32:07.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/yue.json
--rw-rw-rw-   0        0        0     1094 2023-12-04 18:41:20.000000 pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/zh.json
--rw-rw-rw-   0        0        0     6095 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/scripts/login.py
--rw-rw-rw-   0        0        0     3449 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/scripts/preload_sites.py
--rw-rw-rw-   0        0        0     2045 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/scripts/shell.py
--rw-rw-rw-   0        0        0     3139 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/scripts/version.py
--rw-rw-rw-   0        0        0    18640 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/scripts/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:55.327742 pywikibot-9.0.0/pywikibot/site/
--rw-rw-rw-   0        0        0      862 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/site/__init__.py
--rw-rw-rw-   0        0        0   116975 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/site/_apisite.py
--rw-rw-rw-   0        0        0    16617 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/site/_basesite.py
--rw-rw-rw-   0        0        0    38399 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/site/_datasite.py
--rw-rw-rw-   0        0        0     4047 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/site/_decorators.py
--rw-rw-rw-   0        0        0    29727 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/site/_extensions.py
--rw-rw-rw-   0        0        0    96330 2024-03-08 08:53:18.000000 pywikibot-9.0.0/pywikibot/site/_generators.py
--rw-rw-rw-   0        0        0     3004 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/site/_interwikimap.py
--rw-rw-rw-   0        0        0    15079 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/site/_namespace.py
--rw-rw-rw-   0        0        0     1586 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/site/_obsoletesites.py
--rw-rw-rw-   0        0        0    12928 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/site/_siteinfo.py
--rw-rw-rw-   0        0        0     4844 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/site/_tokenwallet.py
--rw-rw-rw-   0        0        0    25238 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/site/_upload.py
--rw-rw-rw-   0        0        0    11158 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/site_detect.py
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:55.330736 pywikibot-9.0.0/pywikibot/specialbots/
--rw-rw-rw-   0        0        0      409 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/specialbots/__init__.py
--rw-rw-rw-   0        0        0     3142 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/specialbots/_unlink.py
--rw-rw-rw-   0        0        0    19880 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/specialbots/_upload.py
--rw-rw-rw-   0        0        0    87673 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/textlib.py
--rw-rw-rw-   0        0        0    12246 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/throttle.py
--rw-rw-rw-   0        0        0    20620 2024-03-08 08:53:18.000000 pywikibot-9.0.0/pywikibot/time.py
--rw-rw-rw-   0        0        0     3259 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/titletranslate.py
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:55.342702 pywikibot-9.0.0/pywikibot/tools/
--rw-rw-rw-   0        0        0    27110 2024-03-08 08:53:18.000000 pywikibot-9.0.0/pywikibot/tools/__init__.py
--rw-rw-rw-   0        0        0    25676 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/tools/_deprecate.py
--rw-rw-rw-   0        0        0     1243 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/tools/_logging.py
--rw-rw-rw-   0        0        0    22245 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/tools/_unidata.py
--rw-rw-rw-   0        0        0     4456 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/tools/chars.py
--rw-rw-rw-   0        0        0    10286 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/tools/collections.py
--rw-rw-rw-   0        0        0    10984 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/tools/djvu.py
--rw-rw-rw-   0        0        0     4060 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/tools/formatter.py
--rw-rw-rw-   0        0        0     8988 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/tools/itertools.py
--rw-rw-rw-   0        0        0     7248 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/tools/threading.py
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:55.358660 pywikibot-9.0.0/pywikibot/userinterfaces/
--rw-rw-rw-   0        0        0      910 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/userinterfaces/__init__.py
--rw-rw-rw-   0        0        0     1885 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/userinterfaces/_interface_base.py
--rw-rw-rw-   0        0        0     2713 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/userinterfaces/buffer_interface.py
--rw-rw-rw-   0        0        0    22357 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/userinterfaces/gui.py
--rw-rw-rw-   0        0        0      495 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/userinterfaces/terminal_interface.py
--rw-rw-rw-   0        0        0    25232 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/userinterfaces/terminal_interface_base.py
--rw-rw-rw-   0        0        0     2152 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/userinterfaces/terminal_interface_unix.py
--rw-rw-rw-   0        0        0     2048 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/userinterfaces/terminal_interface_win32.py
--rw-rw-rw-   0        0        0    90667 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/userinterfaces/transliteration.py
--rw-rw-rw-   0        0        0    16723 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/version.py
--rw-rw-rw-   0        0        0    11113 2024-03-08 06:19:06.000000 pywikibot-9.0.0/pywikibot/xmlreader.py
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:55.360654 pywikibot-9.0.0/pywikibot.egg-info/
--rw-rw-rw-   0        0        0    22127 2024-03-08 09:41:54.000000 pywikibot-9.0.0/pywikibot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10561 2024-03-08 09:41:54.000000 pywikibot-9.0.0/pywikibot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-08 09:41:54.000000 pywikibot-9.0.0/pywikibot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-03-08 09:41:54.000000 pywikibot-9.0.0/pywikibot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      982 2024-03-08 09:41:54.000000 pywikibot-9.0.0/pywikibot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-08 09:41:54.000000 pywikibot-9.0.0/pywikibot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-08 09:41:55.369630 pywikibot-9.0.0/setup.cfg
--rw-rw-rw-   0        0        0     8130 2024-03-08 08:53:18.000000 pywikibot-9.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-08 09:41:55.359658 pywikibot-9.0.0/tests/
--rw-rw-rw-   0        0        0     2832 2024-03-08 06:19:06.000000 pywikibot-9.0.0/tests/tests_tests.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:36.142940 pywikibot-9.1.0/
+-rw-rw-rw-   0        0        0     4184 2024-04-20 14:45:29.000000 pywikibot-9.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0      177 2024-04-20 14:45:29.000000 pywikibot-9.1.0/CODE_OF_CONDUCT.rst
+-rw-rw-rw-   0        0        0     1086 2024-04-20 14:45:29.000000 pywikibot-9.1.0/LICENSE
+-rw-rw-rw-   0        0        0       90 2024-04-20 14:45:29.000000 pywikibot-9.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    18233 2024-04-22 08:24:36.140942 pywikibot-9.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5484 2024-04-20 14:45:29.000000 pywikibot-9.1.0/README.rst
+-rw-rw-rw-   0        0        0     7046 2024-04-21 11:23:51.000000 pywikibot-9.1.0/ROADMAP.rst
+-rw-rw-rw-   0        0        0     4617 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:34.879101 pywikibot-9.1.0/pywikibot/
+-rw-rw-rw-   0        0        0    14027 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/__init__.py
+-rw-rw-rw-   0        0        0      367 2024-04-22 08:22:18.000000 pywikibot-9.1.0/pywikibot/__metadata__.py
+-rw-rw-rw-   0        0        0    43977 2024-04-22 07:17:40.000000 pywikibot-9.1.0/pywikibot/_wbtypes.py
+-rw-rw-rw-   0        0        0     6897 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/backports.py
+-rw-rw-rw-   0        0        0    87385 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/bot.py
+-rw-rw-rw-   0        0        0    27855 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/bot_choice.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:34.922986 pywikibot-9.1.0/pywikibot/comms/
+-rw-rw-rw-   0        0        0      121 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/comms/__init__.py
+-rw-rw-rw-   0        0        0    15778 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/comms/eventstreams.py
+-rw-rw-rw-   0        0        0    20032 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/comms/http.py
+-rw-rw-rw-   0        0        0    45908 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/config.py
+-rw-rw-rw-   0        0        0    46627 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/cosmetic_changes.py
+-rw-rw-rw-   0        0        0     2096 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/daemonize.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:34.951862 pywikibot-9.1.0/pywikibot/data/
+-rw-rw-rw-   0        0        0     1990 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:34.997777 pywikibot-9.1.0/pywikibot/data/api/
+-rw-rw-rw-   0        0        0     3212 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/data/api/__init__.py
+-rw-rw-rw-   0        0        0    41998 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/data/api/_generators.py
+-rw-rw-rw-   0        0        0     7556 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/data/api/_optionset.py
+-rw-rw-rw-   0        0        0    16895 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/data/api/_paraminfo.py
+-rw-rw-rw-   0        0        0    53137 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/data/api/_requests.py
+-rw-rw-rw-   0        0        0    14075 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/data/memento.py
+-rw-rw-rw-   0        0        0     2599 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/data/mysql.py
+-rw-rw-rw-   0        0        0     9737 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/data/sparql.py
+-rw-rw-rw-   0        0        0     4104 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/data/wikistats.py
+-rw-rw-rw-   0        0        0    97086 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/date.py
+-rw-rw-rw-   0        0        0    24621 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/diff.py
+-rw-rw-rw-   0        0        0     1937 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/echo.py
+-rw-rw-rw-   0        0        0     8033 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/editor.py
+-rw-rw-rw-   0        0        0    20754 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:35.233350 pywikibot-9.1.0/pywikibot/families/
+-rw-rw-rw-   0        0        0      118 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/__init__.py
+-rw-rw-rw-   0        0        0     1792 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/commons_family.py
+-rw-rw-rw-   0        0        0      481 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/foundation_family.py
+-rw-rw-rw-   0        0        0      376 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/i18n_family.py
+-rw-rw-rw-   0        0        0      393 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/incubator_family.py
+-rw-rw-rw-   0        0        0      621 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/lingualibre_family.py
+-rw-rw-rw-   0        0        0      439 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/mediawiki_family.py
+-rw-rw-rw-   0        0        0      629 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/meta_family.py
+-rw-rw-rw-   0        0        0     1243 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/osm_family.py
+-rw-rw-rw-   0        0        0      407 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/outreach_family.py
+-rw-rw-rw-   0        0        0      399 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/species_family.py
+-rw-rw-rw-   0        0        0     1169 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/vikidia_family.py
+-rw-rw-rw-   0        0        0     2444 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wikibooks_family.py
+-rw-rw-rw-   0        0        0      996 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wikidata_family.py
+-rw-rw-rw-   0        0        0      403 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wikifunctions_family.py
+-rw-rw-rw-   0        0        0     1669 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wikihow_family.py
+-rw-rw-rw-   0        0        0     1047 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wikimania_family.py
+-rw-rw-rw-   0        0        0      813 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wikimediachapter_family.py
+-rw-rw-rw-   0        0        0     1856 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wikinews_family.py
+-rw-rw-rw-   0        0        0    11103 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wikipedia_family.py
+-rw-rw-rw-   0        0        0     2919 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wikiquote_family.py
+-rw-rw-rw-   0        0        0     5355 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wikisource_family.py
+-rw-rw-rw-   0        0        0      469 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wikispore_family.py
+-rw-rw-rw-   0        0        0      463 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wikitech_family.py
+-rw-rw-rw-   0        0        0     1176 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wikiversity_family.py
+-rw-rw-rw-   0        0        0     1053 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wikivoyage_family.py
+-rw-rw-rw-   0        0        0     4159 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wiktionary_family.py
+-rw-rw-rw-   0        0        0     2452 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/families/wowwiki_family.py
+-rw-rw-rw-   0        0        0    43417 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/family.py
+-rw-rw-rw-   0        0        0    33229 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/fixes.py
+-rw-rw-rw-   0        0        0    20614 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/flow.py
+-rw-rw-rw-   0        0        0    29937 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/i18n.py
+-rw-rw-rw-   0        0        0     7896 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/interwiki_graph.py
+-rw-rw-rw-   0        0        0    13048 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/logentries.py
+-rw-rw-rw-   0        0        0    12576 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/logging.py
+-rw-rw-rw-   0        0        0    22774 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/login.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:35.251304 pywikibot-9.1.0/pywikibot/page/
+-rw-rw-rw-   0        0        0     1289 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/page/__init__.py
+-rw-rw-rw-   0        0        0    88531 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/page/_basepage.py
+-rw-rw-rw-   0        0        0    14617 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/page/_category.py
+-rw-rw-rw-   0        0        0    19031 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/page/_collections.py
+-rw-rw-rw-   0        0        0     2175 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/page/_decorators.py
+-rw-rw-rw-   0        0        0    19962 2024-04-22 07:17:40.000000 pywikibot-9.1.0/pywikibot/page/_filepage.py
+-rw-rw-rw-   0        0        0    29468 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/page/_links.py
+-rw-rw-rw-   0        0        0     8551 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/page/_page.py
+-rw-rw-rw-   0        0        0     3035 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/page/_revision.py
+-rw-rw-rw-   0        0        0     4055 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/page/_toolforge.py
+-rw-rw-rw-   0        0        0    16532 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/page/_user.py
+-rw-rw-rw-   0        0        0    90813 2024-04-22 07:17:40.000000 pywikibot-9.1.0/pywikibot/page/_wikibase.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:35.258286 pywikibot-9.1.0/pywikibot/pagegenerators/
+-rw-rw-rw-   0        0        0    29759 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/pagegenerators/__init__.py
+-rw-rw-rw-   0        0        0    41066 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/pagegenerators/_factory.py
+-rw-rw-rw-   0        0        0    18463 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/pagegenerators/_filters.py
+-rw-rw-rw-   0        0        0    46417 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/pagegenerators/_generators.py
+-rw-rw-rw-   0        0        0     3955 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/plural.py
+-rw-rw-rw-   0        0        0    49322 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/proofreadpage.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:35.347049 pywikibot-9.1.0/pywikibot/scripts/
+-rw-rw-rw-   0        0        0      921 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/scripts/__init__.py
+-rw-rw-rw-   0        0        0    12328 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/scripts/generate_family_file.py
+-rw-rw-rw-   0        0        0    20040 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/scripts/generate_user_files.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:35.358021 pywikibot-9.1.0/pywikibot/scripts/i18n/
+-rw-rw-rw-   0        0        0      349 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:35.982363 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/
+-rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ab.json
+-rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/af.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/an.json
+-rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ar.json
+-rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/arc.json
+-rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ast.json
+-rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/av.json
+-rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/awa.json
+-rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/az.json
+-rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/azb.json
+-rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ba.json
+-rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/bar.json
+-rw-rw-rw-   0        0        0      991 2023-10-07 15:32:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/bcc.json
+-rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/be-tarask.json
+-rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/be.json
+-rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/bg.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/bjn.json
+-rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/bn.json
+-rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/bo.json
+-rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/br.json
+-rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/bs.json
+-rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ca.json
+-rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ce.json
+-rw-rw-rw-   0        0        0      865 2023-10-07 15:32:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ckb.json
+-rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/cs.json
+-rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/csb.json
+-rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/cy.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/da.json
+-rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/de.json
+-rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/diq.json
+-rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/el.json
+-rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/en.json
+-rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/eo.json
+-rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/es.json
+-rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/et.json
+-rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/eu.json
+-rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/fa.json
+-rw-rw-rw-   0        0        0      713 2023-07-21 09:20:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/fi.json
+-rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/fo.json
+-rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/fr.json
+-rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/frp.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/frr.json
+-rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/fy.json
+-rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ga.json
+-rw-rw-rw-   0        0        0     1083 2023-07-21 09:20:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/gl.json
+-rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/gsw.json
+-rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/hak.json
+-rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/haw.json
+-rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/he.json
+-rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/hi.json
+-rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/hr.json
+-rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/hsb.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/hu.json
+-rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/hy.json
+-rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ia.json
+-rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/id.json
+-rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ie.json
+-rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ig.json
+-rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ilo.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/io.json
+-rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/is.json
+-rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/it.json
+-rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ja.json
+-rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/jv.json
+-rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/kab.json
+-rw-rw-rw-   0        0        0     1079 2023-07-21 09:20:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/kk.json
+-rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/km.json
+-rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/kn.json
+-rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ko.json
+-rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/krc.json
+-rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ksh.json
+-rw-rw-rw-   0        0        0      652 2024-01-30 13:30:45.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ku.json
+-rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ky.json
+-rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/la.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/lb.json
+-rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/li.json
+-rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/lki.json
+-rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/lt.json
+-rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/lv.json
+-rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/map-bms.json
+-rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/mg.json
+-rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/min.json
+-rw-rw-rw-   0        0        0     1360 2023-07-21 09:20:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/mk.json
+-rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ml.json
+-rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/mni.json
+-rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/mr.json
+-rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ms.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/mt.json
+-rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/my.json
+-rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/nan.json
+-rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/nb.json
+-rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/nds-nl.json
+-rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/nds.json
+-rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ne.json
+-rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/new.json
+-rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/nl.json
+-rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/nn.json
+-rw-rw-rw-   0        0        0     1443 2023-07-21 09:20:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/nqo.json
+-rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/nyn.json
+-rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/oc.json
+-rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/olo.json
+-rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/or.json
+-rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/pa.json
+-rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/pdc.json
+-rw-rw-rw-   0        0        0      150 2023-07-21 09:20:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/pfl.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/pl.json
+-rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/pms.json
+-rw-rw-rw-   0        0        0     1092 2023-10-07 15:32:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/pt-br.json
+-rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/pt.json
+-rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/qqq.json
+-rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ro.json
+-rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ru.json
+-rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/scn.json
+-rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sco.json
+-rw-rw-rw-   0        0        0      369 2023-07-21 09:20:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sd.json
+-rw-rw-rw-   0        0        0      101 2023-10-07 15:32:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sdh.json
+-rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sh.json
+-rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/si.json
+-rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sk.json
+-rw-rw-rw-   0        0        0      193 2023-10-07 15:32:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/skr.json
+-rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sl.json
+-rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sms.json
+-rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/so.json
+-rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sq.json
+-rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sr.json
+-rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/su.json
+-rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sv.json
+-rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sw.json
+-rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/szl.json
+-rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ta.json
+-rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/te.json
+-rw-rw-rw-   0        0        0      116 2023-07-21 09:20:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/tg.json
+-rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/th.json
+-rw-rw-rw-   0        0        0      170 2023-07-21 09:20:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/tk.json
+-rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/tl.json
+-rw-rw-rw-   0        0        0     1126 2023-07-21 09:20:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/tly.json
+-rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/tr.json
+-rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/tt.json
+-rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/uk.json
+-rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ur.json
+-rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/uz.json
+-rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/vec.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/vep.json
+-rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/vi.json
+-rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/vo.json
+-rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/war.json
+-rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/yi.json
+-rw-rw-rw-   0        0        0      832 2023-10-07 15:32:07.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/yue.json
+-rw-rw-rw-   0        0        0     1094 2023-12-04 18:41:20.000000 pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/zh.json
+-rw-rw-rw-   0        0        0     6095 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/scripts/login.py
+-rw-rw-rw-   0        0        0     3449 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/scripts/preload_sites.py
+-rw-rw-rw-   0        0        0     2045 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/scripts/shell.py
+-rw-rw-rw-   0        0        0     3507 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/scripts/version.py
+-rw-rw-rw-   0        0        0    18718 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/scripts/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:36.005303 pywikibot-9.1.0/pywikibot/site/
+-rw-rw-rw-   0        0        0     1051 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/site/__init__.py
+-rw-rw-rw-   0        0        0   116994 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/site/_apisite.py
+-rw-rw-rw-   0        0        0    16617 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/site/_basesite.py
+-rw-rw-rw-   0        0        0    38399 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/site/_datasite.py
+-rw-rw-rw-   0        0        0     4047 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/site/_decorators.py
+-rw-rw-rw-   0        0        0    29727 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/site/_extensions.py
+-rw-rw-rw-   0        0        0    98105 2024-04-22 07:17:40.000000 pywikibot-9.1.0/pywikibot/site/_generators.py
+-rw-rw-rw-   0        0        0     3004 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/site/_interwikimap.py
+-rw-rw-rw-   0        0        0    15079 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/site/_namespace.py
+-rw-rw-rw-   0        0        0     1586 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/site/_obsoletesites.py
+-rw-rw-rw-   0        0        0    12928 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/site/_siteinfo.py
+-rw-rw-rw-   0        0        0     4844 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/site/_tokenwallet.py
+-rw-rw-rw-   0        0        0    25238 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/site/_upload.py
+-rw-rw-rw-   0        0        0    11158 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/site_detect.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:36.042205 pywikibot-9.1.0/pywikibot/specialbots/
+-rw-rw-rw-   0        0        0      409 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/specialbots/__init__.py
+-rw-rw-rw-   0        0        0     3142 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/specialbots/_unlink.py
+-rw-rw-rw-   0        0        0    20865 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/specialbots/_upload.py
+-rw-rw-rw-   0        0        0    87673 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/textlib.py
+-rw-rw-rw-   0        0        0    12246 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/throttle.py
+-rw-rw-rw-   0        0        0    20620 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/time.py
+-rw-rw-rw-   0        0        0     3259 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/titletranslate.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:36.079107 pywikibot-9.1.0/pywikibot/tools/
+-rw-rw-rw-   0        0        0    27110 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/tools/__init__.py
+-rw-rw-rw-   0        0        0    25676 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/tools/_deprecate.py
+-rw-rw-rw-   0        0        0     1243 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/tools/_logging.py
+-rw-rw-rw-   0        0        0    22245 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/tools/_unidata.py
+-rw-rw-rw-   0        0        0     4456 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/tools/chars.py
+-rw-rw-rw-   0        0        0    10286 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/tools/collections.py
+-rw-rw-rw-   0        0        0    10984 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/tools/djvu.py
+-rw-rw-rw-   0        0        0     4060 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/tools/formatter.py
+-rw-rw-rw-   0        0        0     8988 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/tools/itertools.py
+-rw-rw-rw-   0        0        0     7248 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/tools/threading.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:36.119004 pywikibot-9.1.0/pywikibot/userinterfaces/
+-rw-rw-rw-   0        0        0      910 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/userinterfaces/__init__.py
+-rw-rw-rw-   0        0        0     1885 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/userinterfaces/_interface_base.py
+-rw-rw-rw-   0        0        0     2713 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/userinterfaces/buffer_interface.py
+-rw-rw-rw-   0        0        0    22357 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/userinterfaces/gui.py
+-rw-rw-rw-   0        0        0      495 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/userinterfaces/terminal_interface.py
+-rw-rw-rw-   0        0        0    25232 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/userinterfaces/terminal_interface_base.py
+-rw-rw-rw-   0        0        0     2152 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/userinterfaces/terminal_interface_unix.py
+-rw-rw-rw-   0        0        0     2048 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/userinterfaces/terminal_interface_win32.py
+-rw-rw-rw-   0        0        0    90667 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/userinterfaces/transliteration.py
+-rw-rw-rw-   0        0        0    14992 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/version.py
+-rw-rw-rw-   0        0        0    11113 2024-04-20 14:45:29.000000 pywikibot-9.1.0/pywikibot/xmlreader.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:36.132964 pywikibot-9.1.0/pywikibot.egg-info/
+-rw-rw-rw-   0        0        0    18233 2024-04-22 08:24:34.000000 pywikibot-9.1.0/pywikibot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10561 2024-04-22 08:24:34.000000 pywikibot-9.1.0/pywikibot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 08:24:34.000000 pywikibot-9.1.0/pywikibot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-22 08:24:34.000000 pywikibot-9.1.0/pywikibot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      982 2024-04-22 08:24:34.000000 pywikibot-9.1.0/pywikibot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-22 08:24:34.000000 pywikibot-9.1.0/pywikibot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 08:24:36.142940 pywikibot-9.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     8130 2024-04-20 14:45:29.000000 pywikibot-9.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:24:36.131969 pywikibot-9.1.0/tests/
+-rw-rw-rw-   0        0        0     2832 2024-04-20 14:45:29.000000 pywikibot-9.1.0/tests/tests_tests.py
```

### Comparing `pywikibot-9.0.0/AUTHORS.rst` & `pywikibot-9.1.0/AUTHORS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 
 ::
 
     Ebrahim Byagowi
     Egon
     Enag2000
     Eranroz
+    Eric Pien
     Erwin
     Evrifaessa
 
 F
 -
 
 ::
```

### Comparing `pywikibot-9.0.0/LICENSE` & `pywikibot-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/PKG-INFO` & `pywikibot-9.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 9.0.0
+Version: 9.1.0
 Summary: Python MediaWiki Bot Framework
 Author-email: xqt <info@gno.de>
 Maintainer-email: The Pywikibot team <pywikibot@lists.wikimedia.org>
 License: MIT License
 Project-URL: Homepage, https://www.mediawiki.org/wiki/Manual:Pywikibot
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
 Project-URL: Repository, https://gerrit.wikimedia.org/r/plugins/gitiles/pywikibot/core/
@@ -295,101 +295,30 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-Improvements
-^^^^^^^^^^^^
-
-* Python 3.13 is supported
-* Update tools._unidata._category_cf from Unicodedata version 15.1.0
-* Timestamp.nowutc()and
-  Timestamp.utcnow()were added (T337748)
-* Remove content parameter of proofreadpage.IndexPage.page_genmethod. (T358635)
-* Backport ``itertools.batched`` from Python 3.13 to backports.batched
-* A copy button was added to the sphinx documentation.
-* Make languages_by_sizedynamic (T78396). The property is
-  only available for family.WikimediaFamilyfamilies. The ``wikimedia_sites.py`` maintenance script was
-  removed.
-* Add config.base_dirto scripts search path with pwbwrapper (T324287)
-* pywikibot.WbTime.equal_instantwas added (T325248)
-* ``revisions`` parameter of xmlreader.XmlDumpwas introduced to specify parsing method
-  (T340804)
-* Pass global -nolog argument into bot script from wrapper (T328900)
-* Add site.APISite.ratelimit()method
-  and tools.collections.RateLimitNamedTuple (T304808)
-* L10N and i18n updates
-* Add pagegenerators.PagePilePageGenerator(T353086)
-
-Bugfixes
-^^^^^^^^
-
-* Timestamp.now()and
-  Timestamp.fromtimestamp()also returns a
-  Timestampobject with Python 3.7
-* Populate pywikibot.MediaInfo._content with expected attributes when loaded (T357608)
-* Raise exceptions.APIErrorif the same error comes twice within data.api.Request.submitloop
-  (T357870)
-* Only delegate sitemethods to public family.Familymethods which have *code* as first parameter.
-* Use ``str`` instead of ``repr`` for several messages with family.Familyobjects (T356782)
-* Add ``hy`` to special languages in textlib.TimeStripper(T356175)
-* Pass login token when using ``action=login`` (T309898)
-* Detect range blocks with pywikibot.User.is_blocked(T301282)
-* Use only ``end`` tags in ElementTree.iterparse in xmlreadermodule (T354095)
-* Suppress error in cosmetic_changes.CosmeticChangesToolkit.cleanUpLinks(T337045)
-* pywikibot.input_choicevalidates *default* parameter (T353097)
-* Remove typing imports from user-config.py file (T352965)
-
-Breaking changes and code cleanups
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-* Cache directory was renamed from ``apicache-py3`` to ``apicache`` due to timestamp changes. (T337748)
-  **Warning:** Do not use Pywikibot 9+ together with Pywikibot 3.0.20181203 and below.
-* Raise ``TypeError`` instead of ``AttributeError`` in Site.randompages()
-  if *redirects* parameter is invalid.
-* A RuntimeError will be raised if a family.Familysubclass has an ``__init__`` initializer method.
-  family.Family.__post_init__classmethod can be used instead.
-* InteractiveReplacewas moved from botto bot_choicemodule
-* ``userinterfaces.transliteration.transliterator`` was renamed to Transliterator
-  
-* ``pywikibot.BaseSite`` and ``pywikibotAPISite`` were dropped. pywikibot.Sitehas to be used to create a
-  siteobject.
-* ``next`` parameter of userinterfaces.transliteration.Transliterator.transliteratewas renamed to ``succ``
-* ``type`` parameter of site.APISite.protectedpages()
-  was renamed to ``protect_type``
-* ``all`` parameter of site.APISite.namespace()was renamed to
-  ``all_ns``
-* ``filter`` parameter of date.dhwas renamed to ``filter_func``
-* ``dict`` parameter of data.api.OptionSetwas renamed to ``data``
-* ``setuptools`` package is no longer mandatory but required for tests
-  (T340640, T347052, T354515)
-* ``root`` attribute of xmlreader.XmlDumpwas removed
-* ``tools.Version`` class was removed; use classes from ``packaging.version`` instead (T340640)
-* ``packaging`` package is mandatory; ``importlib_metadata`` package is required for Python 3.7 (T340640)
-* ``SelfCallMixin``, ``SelfCallDict`` and ``SelfCallString`` of toolsmodule were removed
-* Calling site.BaseSite.sitenameas a function
-  is no longer supported
-* ``config.register_family_file()`` function was removed
-* require ``PyMySQL >= 1.0.0`` if necessary
-* ``keys()`` and ``items()`` methods of data.api.Requestgives a view instead a list (T310953)
-* ``SequenceOutputter.format_list()`` was removed in favour of tools.formatter.SequenceOutputter.outproperty
-* *output* parameter of bot_choice.OutputProxyOption(i.e. ``OutputOption`` instance) without *out* property is
-  no longer supported
-* ``OutputOption.output()`` method was removed
-* ``ContextOption.output_range()`` and ``HighlightContextOption.output_range()`` methods were removed
-* ``page.url2unicode()`` function was removed in favour of tools.chars.url2string
-* *iterables* of tools.itertools.intersect_generatorsmust not be given as a single list or tuple;
-  either consecutive iterables must be used or '*' to unpack
-* *allow_duplicates* parameter of tools.itertools.intersect_generatorsmust be given as keyword argument
-* Infinite rotating file handler with ``config.logfilesize`` of -1 is no longer supported
-* ``Throttle.multiplydelay`` attribute was removed
-* Python 3.6 support was dropped (T347026)
-
+* ``-usernames`` option was added to versionscript
+* Circumvent problems with *unique* and *prefix* parameters in Site.alllinks()
+  (T359427)
+* Detect nighly version file with version.getversion_nightly(T362492)
+* version.github_svn_rev2hash() was removed; it was no longer functional (T362484)
+* SVN support has been dropped; ``.svnprops`` property settings was removed (T362484)
+* Skip process that requires login to logout (T326614)
+* File title of specialbots.UploadRobotmust have a valid file extension (T345786)
+* Add a post_processorattribute to specialbots.UploadRobot
+  which can be called after each upload (T359766)
+* Avoid using pywikibot.handle_argsin private scripts;
+  use pwbwrapper instead (T359766)
+* Show upload count with specialbots.UploadRobot
+* Use the same ``iiprop`` properties in data.api.PageGeneratoras in
+  APISite.loadimageinfo(T360093)
+* i18n updates
 
 Deprecations
 ------------
 
 * 9.0.0: The *content* parameter of proofreadpage.IndexPage.page_genis deprecated and will be ignored
   (T358635)
 * 9.0.0: ``userinterfaces.transliteration.transliterator`` was renamed to Transliterator
@@ -435,14 +364,16 @@
 * 8.0.0: Page.editTime()method is deprecated and should be replaced by
   Page.latest_revision.timestamp
 
 
 Will be removed in Pywikibot 10
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
+* 9.1.0: version.svn_rev_infoand version.getversion_svnwill be removed. SVN is no longer supported.
+  (T362484)
 * 7.7.0: tools.threadingclasses should no longer imported from tools
 * 7.6.0: tools.itertoolsdatatypes should no longer imported from tools
 * 7.6.0: tools.collectionsdatatypes should no longer imported from tools
 * 7.5.0: textlib.tzoneFixedOffset class will be removed in favour of time.TZoneFixedOffset
 * 7.4.0: ``FilePage.usingPages()`` was renamed to using_pages()
 * 7.3.0: Old color escape sequences like ``\03{color}`` is deprecated in favour of new color format like <<color>>
 * 7.3.0: ``linkitrail`` method of family.Familyis deprecated; use APISite.linktrail()
```

### Comparing `pywikibot-9.0.0/README.rst` & `pywikibot-9.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pyproject.toml` & `pywikibot-9.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/__init__.py` & `pywikibot-9.1.0/pywikibot/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/_wbtypes.py` & `pywikibot-9.1.0/pywikibot/_wbtypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -694,15 +694,15 @@
         .. seealso:: :meth:`fromTimestr` for differences between output
            with and without *force_iso* parameter.
 
         .. versionchanged:: 8.0
            *normalize* parameter was added.
         .. versionchanged:: 8.2
            *normalize* parameter was removed due to :phab:`T340495` and
-           :phab:`57755`
+           :phab:`T57755`
 
         :param force_iso: whether the output should be forced to ISO 8601
         :return: Timestamp in a format resembling ISO 8601
         """
         if force_iso:
             return Timestamp._ISO8601Format_new.format(
                 self.year, max(1, self.month), max(1, self.day),
@@ -735,15 +735,15 @@
     def toWikibase(self) -> dict[str, Any]:
         """Convert the data to a JSON object for the Wikibase API.
 
         .. versionchanged:: 8.0
            *normalize* parameter was added.
         .. versionchanged:: 8.2
            *normalize* parameter was removed due to :phab:`T340495` and
-           :phab:`57755`
+           :phab:`T57755`
 
         :return: Wikibase JSON
         """
         json = {'time': self.toTimestr(),
                 'precision': self.precision,
                 'after': self.after,
                 'before': self.before,
```

### Comparing `pywikibot-9.0.0/pywikibot/backports.py` & `pywikibot-9.1.0/pywikibot/backports.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,17 +173,21 @@
         .. versionchanged:: 9.0
            Added *strict* option, backported from Python 3.13
 
         :param n: How many items of the iterable to get in one chunk
         :param strict: raise a ValueError if the final batch is shorter
             than *n*.
         :raise ValueError: batched(): incomplete batch
+        :raise TypeError: *n* cannot be interpreted as an integer
         """
         msg = 'batched(): incomplete batch'
         if PYTHON_VERSION < (3, 12):
+            if not isinstance(n, int):
+                raise TypeError(f'{type(n),__name__!r} object cannot be'
+                                ' interpreted as an integer')
             group = []
             for item in iterable:
                 group.append(item)
                 if len(group) == n:
                     yield tuple(group)
                     group.clear()
             if group:
```

### Comparing `pywikibot-9.0.0/pywikibot/bot.py` & `pywikibot-9.1.0/pywikibot/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -668,14 +668,34 @@
     >>> local_args  # doctest: +SKIP
     []
     >>> local_args = pywikibot.handle_args(['-simulate', '-myoption'])
     >>> local_args  # global optons are handled, show the remaining
     ['-myoption']
     >>> for arg in local_args: pass  # do whatever is wanted with local_args
 
+    .. caution::
+       Global options might be introduced without warning period. It is
+       up to developers to verify that global options do not interfere
+       with local script options of private scripts.
+
+    .. tip::
+       Avoid using this method in your private scripts and use the
+       :mod:`pwb<pywikibot.scripts.wrapper>` wrapper instead. In
+       directory mode::
+
+           python pwb.py <global options> <name_of_script> <local options>
+
+       With installed site package::
+
+           pwb <global options> <name_of_script> <local options>
+
+       .. note:: the :mod:`pwb<pywikibot.scripts.wrapper>` wrapper can
+          be used even if the `handle_args` method is used within the
+          script.
+
     .. versionchanged:: 5.2
        *-site* global option was added
     .. versionchanged:: 7.1
        *-cosmetic_changes* and *-cc* may be set directly instead of
        toggling the value. Refer :func:`tools.strtobool` for valid values.
     .. versionchanged:: 7.7
        *-config* global option was added.
```

### Comparing `pywikibot-9.0.0/pywikibot/bot_choice.py` & `pywikibot-9.1.0/pywikibot/bot_choice.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/comms/eventstreams.py` & `pywikibot-9.1.0/pywikibot/comms/eventstreams.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/comms/http.py` & `pywikibot-9.1.0/pywikibot/comms/http.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/config.py` & `pywikibot-9.1.0/pywikibot/config.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/cosmetic_changes.py` & `pywikibot-9.1.0/pywikibot/cosmetic_changes.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     cosmetic_changes_mylang_only = False
 
 if you're running a bot on multiple sites and want to do cosmetic changes on
 all of them, but be careful if you do.
 
 You may disable cosmetic changes by adding the all unwanted languages to
 the `dictionary cosmetic_changes_disable` in your user config file
-(`user_config.py`). It should contain a tuple of languages for each site
+(`user-config.py`). It should contain a tuple of languages for each site
 where you wish to disable cosmetic changes. You may use it with
 `cosmetic_changes_mylang_only` is False, but you can also disable your
 own language. This also overrides the settings in the dictionary
 `cosmetic_changes_enable`. Please set this dictionary by adding such
 lines to your user config file::
 
     cosmetic_changes_disable['wikipedia'] = ('de', 'en', 'fr')
@@ -47,15 +47,15 @@
 
 or by adding a list to the given one::
 
     cosmetic_changes_deny_script += ['your_script_name_1',
                                      'your_script_name_2']
 """
 #
-# (C) Pywikibot team, 2006-2023
+# (C) Pywikibot team, 2006-2024
 #
 # Distributed under the terms of the MIT license.
 #
 from __future__ import annotations
 
 import re
 from contextlib import suppress
```

### Comparing `pywikibot-9.0.0/pywikibot/daemonize.py` & `pywikibot-9.1.0/pywikibot/daemonize.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/data/__init__.py` & `pywikibot-9.1.0/pywikibot/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/data/api/__init__.py` & `pywikibot-9.1.0/pywikibot/data/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/data/api/_generators.py` & `pywikibot-9.1.0/pywikibot/data/api/_generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 .. versionchanged:: 7.6
    All Objects were changed from Iterable object to a Generator object.
    They are subclassed from
    :class:`tools.collections.GeneratorWrapper`
 """
 #
-# (C) Pywikibot team, 2008-2023
+# (C) Pywikibot team, 2008-2024
 #
 # Distributed under the terms of the MIT license.
 #
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from contextlib import suppress
 from typing import Any
 from warnings import warn
 
 import pywikibot
 from pywikibot import config
-from pywikibot.backports import Callable
+from pywikibot.backports import Callable, Iterable
 from pywikibot.exceptions import Error, InvalidTitleError, UnsupportedPageError
 from pywikibot.site import Namespace
 from pywikibot.tools import deprecated
 from pywikibot.tools.collections import GeneratorWrapper
 
 
 __all__ = (
@@ -671,45 +671,49 @@
 
     def __init__(
         self,
         generator: str,
         g_content: bool = False,
         **kwargs
     ) -> None:
-        """
-        Initializer.
+        """Initializer.
 
-        Required and optional parameters are as for ``Request``, except that
-        action=query is assumed and generator is required.
+        Required and optional parameters are as for ``Request``, except
+        that ``action=query`` is assumed and generator is required.
+
+        .. versionchanged:: 9.1
+           retrieve the same imageinfo properties as in
+           :meth:`APISite.loadimageinfo()
+           <pywikibot.site._apisite.APISite.loadimageinfo>` with default
+           parameters.
 
         :param generator: the "generator=" type from api.php
         :param g_content: if True, retrieve the contents of the current
             version of each Page (default False)
-
         """
-        # If possible, use self.request after __init__ instead of appendParams
+        # If possible, use self.request after __init__ instead of append_params
         def append_params(params, key, value) -> None:
             if key in params:
                 params[key] += '|' + value
             else:
                 params[key] = value
+
         kwargs = self._clean_kwargs(kwargs)
         parameters = kwargs['parameters']
         # get some basic information about every page generated
         append_params(parameters, 'prop', 'info|imageinfo|categoryinfo')
         if g_content:
             # retrieve the current revision
             append_params(parameters, 'prop', 'revisions')
             append_params(parameters, 'rvprop',
                           'ids|timestamp|flags|comment|user|content')
         if not ('inprop' in parameters
                 and 'protection' in parameters['inprop']):
             append_params(parameters, 'inprop', 'protection')
-        append_params(parameters, 'iiprop',
-                      'timestamp|user|comment|url|size|sha1')
+        append_params(parameters, 'iiprop', pywikibot.site._IIPROP)
         append_params(parameters, 'iilimit', 'max')  # T194233
         parameters['generator'] = generator
         super().__init__(**kwargs)
         self.resultkey = 'pages'  # element to look for in result
         self.props = self.request['prop']
 
     def result(self, pagedata: dict[str, Any]) -> pywikibot.Page:
@@ -955,75 +959,71 @@
                                      globe=co['globe'],  # See [[gerrit:67886]]
                                      primary='primary' in co
                                      )
         coords.append(coord)
     page._coords = coords
 
 
-def update_page(page, pagedict: dict, props=None):
-    """Update attributes of Page object page, based on query data in pagedict.
+def update_page(page: pywikibot.Page,
+                pagedict: dict[str, Any],
+                props: Iterable[str] | None = None) -> None:
+    """
+    Update attributes of Page object *page*, based on query data in *pagedict*.
 
     :param page: object to be updated
-    :type page: pywikibot.page.Page
-    :param pagedict: the contents of a "page" element of a query response
-    :param props: the property names which resulted in pagedict. If a missing
-        value in pagedict can indicate both 'false' and 'not present' the
-        property which would make the value present must be in the props
-        parameter.
-    :type props: iterable of string
-    :raises pywikibot.exceptions.InvalidTitleError: Page title is invalid
-    :raises pywikibot.exceptions.UnsupportedPageError: Page with namespace < 0
-        is not supported yet
+    :param pagedict: the contents of a *page* element of a query
+        response
+    :param props: the property names which resulted in *pagedict*. If a
+        missing value in *pagedict* can indicate both 'false' and
+        'not present' the property which would make the value present
+        must be in the *props* parameter.
+    :raises InvalidTitleError: Page title is invalid
+    :raises UnsupportedPageError: Page with namespace < 0 is not
+        supported yet
     """
     _update_pageid(page, pagedict)
     _update_contentmodel(page, pagedict)
 
     props = props or []
+
+    # test for pagedict content only and call updater function
+    for element in ('coordinates', 'revisions'):
+        if element in pagedict:
+            updater = globals()['_update_' + element]
+            updater(page, pagedict[element])
+
+    # test for pagedict and props contents, call updater or set attribute
+    for element in ('categories', 'langlinks', 'templates'):
+        if element in pagedict:
+            updater = globals()['_update_' + element]
+            updater(page, pagedict[element])
+        elif element in props:
+            setattr(page, '_' + element, set())
+
     if 'info' in props:
         page._isredir = 'redirect' in pagedict
 
     if 'touched' in pagedict:
         page._timestamp = pagedict['touched']
 
     if 'protection' in pagedict:
         _update_protection(page, pagedict)
 
-    if 'revisions' in pagedict:
-        _update_revisions(page, pagedict['revisions'])
-
     if 'lastrevid' in pagedict:
         page.latest_revision_id = pagedict['lastrevid']
 
     if 'imageinfo' in pagedict:
         if not isinstance(page, pywikibot.FilePage):
             raise RuntimeError(
                 f'"imageinfo" found but {page} is not a FilePage object')
         page._load_file_revisions(pagedict['imageinfo'])
 
     if 'categoryinfo' in pagedict:
         page._catinfo = pagedict['categoryinfo']
 
-    if 'templates' in pagedict:
-        _update_templates(page, pagedict['templates'])
-    elif 'templates' in props:
-        page._templates = set()
-
-    if 'categories' in pagedict:
-        _update_categories(page, pagedict['categories'])
-    elif 'categories' in props:
-        page._categories = set()
-
-    if 'langlinks' in pagedict:
-        _update_langlinks(page, pagedict['langlinks'])
-    elif 'langlinks' in props:
-        page._langlinks = set()
-
-    if 'coordinates' in pagedict:
-        _update_coordinates(page, pagedict['coordinates'])
-
     if 'pageimage' in pagedict:
         page._pageimage = pywikibot.FilePage(page.site, pagedict['pageimage'])
 
     if 'pageprops' in pagedict:
         page._pageprops = pagedict['pageprops']
     elif 'pageprops' in props:
         page._pageprops = {}
```

### Comparing `pywikibot-9.0.0/pywikibot/data/api/_optionset.py` & `pywikibot-9.1.0/pywikibot/data/api/_optionset.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/data/api/_paraminfo.py` & `pywikibot-9.1.0/pywikibot/data/api/_paraminfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/data/api/_requests.py` & `pywikibot-9.1.0/pywikibot/data/api/_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -946,15 +946,15 @@
         return True
 
     def wait(self, delay: int | None = None) -> None:
         """Determine how long to wait after a failed request.
 
         Also reset last API error with wait cycles.
 
-        .. versionadded: 9.0
+        .. versionadded:: 9.0
 
         :param delay: Minimum time in seconds to wait. Overwrites
             ``retry_wait`` variable if given. The delay doubles each
             retry until ``retry_max`` seconds is reached.
         """
         self.last_error = dict.fromkeys(['code', 'info'])
         super().wait(delay)
```

### Comparing `pywikibot-9.0.0/pywikibot/data/memento.py` & `pywikibot-9.1.0/pywikibot/data/memento.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/data/mysql.py` & `pywikibot-9.1.0/pywikibot/data/mysql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/data/sparql.py` & `pywikibot-9.1.0/pywikibot/data/sparql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/data/wikistats.py` & `pywikibot-9.1.0/pywikibot/data/wikistats.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/date.py` & `pywikibot-9.1.0/pywikibot/date.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/diff.py` & `pywikibot-9.1.0/pywikibot/diff.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/echo.py` & `pywikibot-9.1.0/pywikibot/echo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/editor.py` & `pywikibot-9.1.0/pywikibot/editor.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/exceptions.py` & `pywikibot-9.1.0/pywikibot/exceptions.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/commons_family.py` & `pywikibot-9.1.0/pywikibot/families/commons_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/lingualibre_family.py` & `pywikibot-9.1.0/pywikibot/families/lingualibre_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/meta_family.py` & `pywikibot-9.1.0/pywikibot/families/meta_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/osm_family.py` & `pywikibot-9.1.0/pywikibot/families/osm_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/vikidia_family.py` & `pywikibot-9.1.0/pywikibot/families/vikidia_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/wikibooks_family.py` & `pywikibot-9.1.0/pywikibot/families/wikibooks_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/wikidata_family.py` & `pywikibot-9.1.0/pywikibot/families/wikidata_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/wikihow_family.py` & `pywikibot-9.1.0/pywikibot/families/wikihow_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/wikimania_family.py` & `pywikibot-9.1.0/pywikibot/families/wikimania_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/wikimediachapter_family.py` & `pywikibot-9.1.0/pywikibot/families/wikimediachapter_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/wikinews_family.py` & `pywikibot-9.1.0/pywikibot/families/wikinews_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/wikipedia_family.py` & `pywikibot-9.1.0/pywikibot/families/wikipedia_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/wikiquote_family.py` & `pywikibot-9.1.0/pywikibot/families/wikiquote_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/wikisource_family.py` & `pywikibot-9.1.0/pywikibot/families/wikisource_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/wikiversity_family.py` & `pywikibot-9.1.0/pywikibot/families/wikiversity_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/wikivoyage_family.py` & `pywikibot-9.1.0/pywikibot/families/wikivoyage_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/wiktionary_family.py` & `pywikibot-9.1.0/pywikibot/families/wiktionary_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/families/wowwiki_family.py` & `pywikibot-9.1.0/pywikibot/families/wowwiki_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/family.py` & `pywikibot-9.1.0/pywikibot/family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/fixes.py` & `pywikibot-9.1.0/pywikibot/fixes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/flow.py` & `pywikibot-9.1.0/pywikibot/flow.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/i18n.py` & `pywikibot-9.1.0/pywikibot/i18n.py`

 * *Files 0% similar despite different names*

```diff
@@ -909,15 +909,15 @@
 
     >>> from pywikibot import i18n
     >>> i18n.known_languages()[:10]
     ['ab', 'aeb', 'af', 'am', 'an', 'ang', 'anp', 'ar', 'arc', 'ary']
     >>> i18n.known_languages()[-10:]
     ['vo', 'vro', 'wa', 'war', 'xal', 'xmf', 'yi', 'yo', 'yue', 'zh']
     >>> len(i18n.known_languages())
-    254
+    255
 
     The implementation is roughly equivalent to:
 
     .. code-block:: Python
 
        langs = set()
        for dirpath in bundles():
```

### Comparing `pywikibot-9.0.0/pywikibot/interwiki_graph.py` & `pywikibot-9.1.0/pywikibot/interwiki_graph.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/logentries.py` & `pywikibot-9.1.0/pywikibot/logentries.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/logging.py` & `pywikibot-9.1.0/pywikibot/logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/login.py` & `pywikibot-9.1.0/pywikibot/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Library to log the bot in to a wiki account."""
 #
-# (C) Pywikibot team, 2003-2023
+# (C) Pywikibot team, 2003-2024
 #
 # Distributed under the terms of the MIT license.
 #
 from __future__ import annotations
 
 import codecs
 import datetime
@@ -101,15 +101,15 @@
             try:
                 user = code_to_usr.get(site.code) or code_to_usr['*']
             except KeyError:
                 raise NoUsernameError(
                     'ERROR: '
                     'username for {site.family.name}:{site.code} is undefined.'
                     '\nIf you have a username for that site, please add a '
-                    'line to user config file (user_config.py) as follows:\n'
+                    'line to user config file (user-config.py) as follows:\n'
                     "usernames['{site.family.name}']['{site.code}'] = "
                     "'myUsername'".format(site=site))
         self.password = password
         self.login_name = self.username = user
         if getattr(config, 'password_file', ''):
             self.readPassword()
```

### Comparing `pywikibot-9.0.0/pywikibot/page/__init__.py` & `pywikibot-9.1.0/pywikibot/page/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/page/_basepage.py` & `pywikibot-9.1.0/pywikibot/page/_basepage.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,27 +354,39 @@
         """Return True if title of this Page is in the autoFormat dict."""
         return self.autoFormat()[0] is not None
 
     def get(self, force: bool = False, get_redirect: bool = False) -> str:
         """Return the wiki-text of the page.
 
         This will retrieve the page from the server if it has not been
-        retrieved yet, or if force is True. This can raise the following
-        exceptions that should be caught by the calling code:
+        retrieved yet, or if force is True. Exceptions should be caught
+        by the calling code.
 
-        :exception pywikibot.exceptions.NoPageError: The page does not exist
-        :exception pywikibot.exceptions.IsRedirectPageError: The page is a
-            redirect. The argument of the exception is the title of the page
-            it redirects to.
-        :exception pywikibot.exceptions.SectionError: The section does not
-            exist on a page with a # link
-
-        :param force:           reload all page attributes, including errors.
-        :param get_redirect:    return the redirect text, do not follow the
-                                redirect, do not raise an exception.
+        **Example:**
+
+        >>> import pywikibot
+        >>> site = pywikibot.Site('mediawiki')
+        >>> page = pywikibot.Page(site, 'Pywikibot')
+        >>> page.get(get_redirect=True)
+        '#REDIRECT[[Manual:Pywikibot]]'
+        >>> page.get()
+        Traceback (most recent call last):
+         ...
+        pywikibot.exceptions.IsRedirectPageError: ... is a redirect page.
+
+        .. seealso:: :attr:`text` property
+
+        :param force: reload all page attributes, including errors.
+        :param get_redirect: return the redirect text, do not follow the
+            redirect, do not raise an exception.
+
+        :raises NoPageError: The page does not exist.
+        :raises IsRedirectPageError: The page is a redirect.
+        :raises SectionError: The section does not exist on a page with
+            a # link.
         """
         if force:
             del self.latest_revision_id
             if hasattr(self, '_bot_may_edit'):
                 del self._bot_may_edit
         try:
             self._getInternals()
@@ -515,30 +527,51 @@
 
         with suppress(StopIteration):
             return next(self.revisions(content=True, total=1))
         raise InvalidPageError(self)
 
     @property
     def text(self) -> str:
-        """
-        Return the current (edited) wikitext, loading it if necessary.
+        """Return the current (edited) wikitext, loading it if necessary.
+
+        This property should be prefered over :meth:`get`. If the page
+        does not exist, an empty string will be returned. For a redirect
+        it returns the redirect page content and does not raise an
+        :exc:`exceptions.IsRedirectPageError` exception.
+
+        **Example:**
+
+        >>> import pywikibot
+        >>> site = pywikibot.Site('mediawiki')
+        >>> page = pywikibot.Page(site, 'Pywikibot')
+        >>> page.text
+        '#REDIRECT[[Manual:Pywikibot]]'
+        >>> page.text = 'PWB Framework'
+        >>> page.text
+        'PWB Framework'
+        >>> page.text = None  # reload from wiki
+        >>> page.text
+        '#REDIRECT[[Manual:Pywikibot]]'
+        >>> del page.text  # other way to reload from wiki
+
+        To save the modified text :meth:`save` is one possible method.
 
         :return: text of the page
         """
         if hasattr(self, '_text') and self._text is not None:
             return self._text
 
         try:
             return self.get(get_redirect=True)
         except NoPageError:
             # TODO: what other exceptions might be returned?
             return ''
 
     @text.setter
-    def text(self, value: str | None):
+    def text(self, value: str | None) -> None:
         """Update the current (edited) wikitext.
 
         :param value: New value or None
         """
         try:
             self.botMayEdit()  # T262136, T267770
         except Exception as e:
```

### Comparing `pywikibot-9.0.0/pywikibot/page/_category.py` & `pywikibot-9.1.0/pywikibot/page/_category.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/page/_collections.py` & `pywikibot-9.1.0/pywikibot/page/_collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/page/_decorators.py` & `pywikibot-9.1.0/pywikibot/page/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/page/_filepage.py` & `pywikibot-9.1.0/pywikibot/page/_filepage.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,17 +429,17 @@
         """
         return self.site.globalusage(self, total=total)
 
     def data_item(self):
         """
         Convenience function to get the associated Wikibase item of the file.
 
-        If WikibaseMediaInfo extension is available (e.g. on Commons),
+        If WikibaseMediaInfo extension is available (e.g., on Commons),
         the method returns the associated mediainfo entity. Otherwise,
-        it falls back to behavior of BasePage.data_item.
+        it falls back to the behavior of :meth:`BasePage.data_item`.
 
         .. versionadded:: 6.5
 
         :rtype: pywikibot.page.WikibaseEntity
         """
         if self.site.has_extension('WikibaseMediaInfo'):
             if not hasattr(self, '_item'):
```

### Comparing `pywikibot-9.0.0/pywikibot/page/_links.py` & `pywikibot-9.1.0/pywikibot/page/_links.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/page/_page.py` & `pywikibot-9.1.0/pywikibot/page/_page.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/page/_revision.py` & `pywikibot-9.1.0/pywikibot/page/_revision.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/page/_toolforge.py` & `pywikibot-9.1.0/pywikibot/page/_toolforge.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/page/_user.py` & `pywikibot-9.1.0/pywikibot/page/_user.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/page/_wikibase.py` & `pywikibot-9.1.0/pywikibot/page/_wikibase.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,17 +80,18 @@
 
     """
     The base interface for Wikibase entities.
 
     Each entity is identified by a data repository it belongs to
     and an identifier.
 
-    :cvar DATA_ATTRIBUTES: dictionary which maps data attributes (eg. 'labels',
-        'claims') to appropriate collection classes (eg. LanguageDict,
-        ClaimsCollection)
+    :cvar DATA_ATTRIBUTES: dictionary which maps data attributes
+        (e.g., 'labels', 'claims') to appropriate collection classes
+        (e.g., :class:`LanguageDict<pywikibot.page._collections.LanguageDict>`,
+        :class:`ClaimCollection<pywikibot.page._collections.ClaimCollection>`)
 
     :cvar entity_type: entity type identifier
     :type entity_type: str
 
     :cvar title_pattern: regular expression which matches all possible
         entity ids for this entity type
     :type title_pattern: str
```

### Comparing `pywikibot-9.0.0/pywikibot/pagegenerators/__init__.py` & `pywikibot-9.1.0/pywikibot/pagegenerators/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/pagegenerators/_factory.py` & `pywikibot-9.1.0/pywikibot/pagegenerators/_factory.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/pagegenerators/_filters.py` & `pywikibot-9.1.0/pywikibot/pagegenerators/_filters.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/pagegenerators/_generators.py` & `pywikibot-9.1.0/pywikibot/pagegenerators/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/plural.py` & `pywikibot-9.1.0/pywikibot/plural.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/proofreadpage.py` & `pywikibot-9.1.0/pywikibot/proofreadpage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/__init__.py` & `pywikibot-9.1.0/pywikibot/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/generate_family_file.py` & `pywikibot-9.1.0/pywikibot/scripts/generate_family_file.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/generate_user_files.py` & `pywikibot-9.1.0/pywikibot/scripts/generate_user_files.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ar.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ar.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ast.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ast.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/az.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/az.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/azb.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/azb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ba.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ba.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/bcc.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/bcc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/be-tarask.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/be-tarask.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/be.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/be.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/bg.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/bg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/bn.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/bn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/br.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/bs.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/bs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ca.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ca.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ce.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ce.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ckb.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ckb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/cs.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/cs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/csb.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/csb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/cy.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/cy.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/da.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/da.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/de.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/de.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/diq.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/diq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/el.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/el.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/en.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/en.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/eo.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/eo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/es.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/es.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/eu.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/eu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/fa.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/fa.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/fi.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/fi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/fo.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/fo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/fr.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/fr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/frr.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/frr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/gl.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/gl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/gsw.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/gsw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/hak.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/hak.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/haw.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/haw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/he.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/he.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/hi.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/hi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/hsb.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/hsb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/hu.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/hu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ia.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ia.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/id.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/id.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/io.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/io.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/is.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/is.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/it.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/it.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ja.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ja.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/kab.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/kab.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/kk.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/kk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/km.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/km.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/kn.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/kn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ko.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ko.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/krc.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/krc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ksh.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ksh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ku.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ku.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/lb.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/lb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/lt.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/lt.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/lv.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/lv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/map-bms.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/map-bms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/mg.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/mg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/min.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/min.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/mk.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/mk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ml.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ml.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ms.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/my.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/my.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/nan.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/nan.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/nb.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/nb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/nds-nl.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/nds-nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ne.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ne.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/new.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/new.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/nl.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/nqo.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/nqo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/pl.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/pl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/pms.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/pms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/pt-br.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/pt-br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/pt.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/pt.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/qqq.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/qqq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ro.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ro.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ru.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ru.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sco.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sco.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sh.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/si.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/si.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sk.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sl.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/so.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/so.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sr.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sv.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/sw.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/sw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ta.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ta.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/te.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/te.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/th.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/th.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/tly.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/tly.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/tr.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/tr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/uk.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/uk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/ur.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/ur.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/vi.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/vi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/yue.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/yue.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/i18n/pywikibot/zh.json` & `pywikibot-9.1.0/pywikibot/scripts/i18n/pywikibot/zh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/login.py` & `pywikibot-9.1.0/pywikibot/scripts/login.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/preload_sites.py` & `pywikibot-9.1.0/pywikibot/scripts/preload_sites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/shell.py` & `pywikibot-9.1.0/pywikibot/scripts/shell.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/scripts/version.py` & `pywikibot-9.1.0/pywikibot/scripts/version.py`

 * *Files 12% similar despite different names*

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
+.. versionadded:: 9.1
+   the *-usernames* option.
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
+    .. versionchanged:: 9.1
+       usernames are printed with ``-usernames`` option only.
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
+    if '-usernames' in sys.argv:
+        usernames_items = pywikibot.config.usernames.items()
+    else:
+        usernames_items = {}
+    for family, usernames in usernames_items:
         if not usernames:
             continue
         pywikibot.info(f"Usernames for family '{family}':")
         for lang, username in usernames.items():
             pywikibot.info(f'\t{lang}: {username}')
```

### Comparing `pywikibot-9.0.0/pywikibot/scripts/wrapper.py` & `pywikibot-9.1.0/pywikibot/scripts/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,22 @@
 will fix up search paths so the package does not need to be installed, etc.
 
 Currently, `<pwb options>` are :ref:`global options`. This can be used
 for tests to set the default site (see :phab:`T216825`)::
 
     python pwb.py -lang:de bot_tests -v
 
+.. seealso:: :mod:`pwb` entry point
 .. versionchanged:: 7.0
-   pwb wrapper was added to the Python site package lib
+   pwb wrapper was added to the Python site package lib.
 .. versionchanged:: 7.7
-   pwb wrapper is able to set ``PYWIKIBOT_TEST_...`` environment variables
+   pwb wrapper is able to set ``PYWIKIBOT_TEST_...`` environment variables,
+   see :ref:`Environment variables`.
 .. versionchanged:: 8.0
-   renamed to wrapper.py
+   renamed to wrapper.py.
 """
 #
 # (C) Pywikibot team, 2012-2024
 #
 # Distributed under the terms of the MIT license.
 #
 from __future__ import annotations
```

### Comparing `pywikibot-9.0.0/pywikibot/site/_apisite.py` & `pywikibot-9.1.0/pywikibot/site/_apisite.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,18 +467,20 @@
         .. seealso:: :api:`Logout`
 
         :raises APIError: Logout is not available when OAuth enabled.
         """
         if self.is_oauth_token_available():
             pywikibot.warning('Using OAuth suppresses logout function')
 
-        req_params = {'action': 'logout', 'token': self.tokens['csrf']}
-        uirequest = self.simple_request(**req_params)
-        uirequest.submit()
-        self._loginstatus = login.LoginStatus.NOT_LOGGED_IN
+        # check if already logged out to avoid requiring logging in
+        if not self._loginstatus == login.LoginStatus.NOT_LOGGED_IN:
+            req_params = {'action': 'logout', 'token': self.tokens['csrf']}
+            uirequest = self.simple_request(**req_params)
+            uirequest.submit()
+            self._loginstatus = login.LoginStatus.NOT_LOGGED_IN
 
         # Reset tokens and user properties
         del self.userinfo
         self.tokens.clear()
         self._paraminfo = api.ParamInfo(self)
 
         # Clear also cookies for site's second level domain (T224712)
@@ -1484,19 +1486,18 @@
         url_param: str | None = None,
         timestamp: pywikibot.Timestamp | None = None
     ) -> None:
         """Load image info from api and save in page attributes.
 
         The following properties are loaded: ``timestamp``, ``user``,
         ``comment``, ``url``, ``size``, ``sha1``, ``mime``, ``mediatype``,
-        ``archivename`` and ``bitdepth``.
-        ``metadata``is loaded only if history is False.
-        If *url_width*, *url_height* or *url_param* is given, additional
-        properties ``thumbwidth``, ``thumbheight``, ``thumburl`` and
-        ``responsiveUrls`` are given.
+        ``archivename`` and ``bitdepth``. ``metadata`` is loaded only if
+        *history* is False. If *url_width*, *url_height* or *url_param*
+        is given, additional properties ``thumbwidth``, ``thumbheight``,
+        ``thumburl`` and ``responsiveUrls`` are given.
 
         .. note:: Parameters validation and error handling left to the
            API call.
         .. versionchanged:: 8.2
            *mediatype* and *bitdepth* properties were added.
         .. versionchanged:: 8.6.
            Added *timestamp* parameter.
@@ -1504,30 +1505,27 @@
         .. seealso:: :api:`Imageinfo`
 
         :param history: if true, return the image's version history
         :param url_width: get info for a thumbnail with given width
         :param url_height: get info for a thumbnail with given height
         :param url_param:  get info for a thumbnail with given param
         :param timestamp: timestamp of the image's version to retrieve.
-            It has effect only if history is False.
+            It has effect only if *history* is False.
             If omitted, the latest version will be fetched.
         """
         args = {
             'titles': page.title(with_section=False),
             'iiurlwidth': url_width,
             'iiurlheight': url_height,
             'iiurlparam': url_param,
-            'iiprop': [
-                'timestamp', 'user', 'comment', 'url', 'size', 'sha1', 'mime',
-                'mediatype', 'archivename', 'bitdepth',
-            ]
+            'iiprop': pywikibot.site._IIPROP
         }
         if not history:
             args['total'] = 1
-            args['iiprop'].append('metadata')
+            args['iiprop'] += ('metadata', )
             if timestamp:
                 args['iistart'] = args['iiend'] = timestamp.isoformat()
 
         query = self._generator(api.PropertyGenerator,
                                 type_arg='imageinfo',
                                 **args)
         self._update_page(page, query, verify_imageinfo=True)
```

### Comparing `pywikibot-9.0.0/pywikibot/site/_basesite.py` & `pywikibot-9.1.0/pywikibot/site/_basesite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/site/_datasite.py` & `pywikibot-9.1.0/pywikibot/site/_datasite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/site/_decorators.py` & `pywikibot-9.1.0/pywikibot/site/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/site/_extensions.py` & `pywikibot-9.1.0/pywikibot/site/_extensions.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/site/_generators.py` & `pywikibot-9.1.0/pywikibot/site/_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,15 +424,17 @@
         namespaces: NamespaceArgType = None,
         follow_redirects: bool = False,
         total: int | None = None,
         content: bool = False,
     ) -> Generator[pywikibot.Page, None, None]:
         """Yield internal wikilinks contained (or transcluded) on page.
 
-        .. seealso:: :api:`Links`
+        .. seealso::
+           - :api:`Links`
+           - :meth:`page.BasePage.linkedPages`
 
         :param namespaces: Only iterate pages in these namespaces
             (default: all)
         :param follow_redirects: if True, yields the target of any redirects,
             rather than the redirect page
         :param total: iterate no more than this number of pages in total
         :param content: if True, load the current content of each iterated page
@@ -971,52 +973,95 @@
                 apgen.request['gapprlevel'] = protect_level
         if reverse:
             apgen.request['gapdir'] = 'descending'
         return apgen
 
     def alllinks(
         self,
-        start: str = '!',
+        start: str = '',
         prefix: str = '',
         namespace: SingleNamespaceType = 0,
         unique: bool = False,
         fromids: bool = False,
         total: int | None = None,
     ) -> Generator[pywikibot.Page, None, None]:
         """Iterate all links to pages (which need not exist) in one namespace.
 
-        Note that, in practice, links that were found on pages that have
-        been deleted may not have been removed from the links table, so this
-        method can return false positives.
-
-        .. seealso:: :api:`Alllinks`
+        .. note:: In practice, links that were found on pages that have
+           been deleted may not have been removed from the links table,
+           so this method can return false positives.
+
+        .. caution:: *unique* parameter is no longer supported by
+           MediaWiki 1.43 or higher. Pywikibot uses
+           :func:`tools.itertools.filter_unique` in that case which
+           might be memory intensive. Use it with care.
+
+        .. important:: Using *namespace* option different from ``0``
+           needs a lot of time on Wikidata site. You have to increase
+           the **read** timeout part of ``socket_timeout`` in
+           :ref:`Http Settings` in your ``user-config.py`` file. Or
+           increase it patially within your code like:
+
+           .. code:: python
+
+              from pywikibot import config
+              save_timeout = config.socket_timeout  # save the timeout config
+              config.socket_timeout = save_timeout[0], 60
+              ... # your code here
+              config.socket_timeout = save_timeout  # restore timeout config
+
+           The minimum read timeout value should be 60 seconds in that
+           case.
+
+        .. seealso::
+           - :api:`Alllinks`
+           - :meth:`pagebacklinks`
+           - :meth:`pagelinks`
 
         :param start: Start at this title (page need not exist).
         :param prefix: Only yield pages starting with this string.
         :param namespace: Iterate pages from this (single) namespace
-        :param unique: If True, only iterate each link title once (default:
-            iterate once for each linking page)
-        :param fromids: if True, include the pageid of the page containing
-            each link (default: False) as the '_fromid' attribute of the Page;
-            cannot be combined with unique
-        :raises KeyError: the namespace identifier was not resolved
-        :raises TypeError: the namespace identifier has an inappropriate
-            type such as bool, or an iterable with more than one namespace
+        :param unique: If True, only iterate each link title once
+            (default: False)
+        :param fromids: if True, include the pageid of the page
+            containing each link (default: False) as the '_fromid'
+            attribute of the Page; cannot be combined with *unique*
+        :raises KeyError: the *namespace* identifier was not resolved
+        :raises TypeError: the *namespace* identifier has an
+            inappropriate type such as bool, or an iterable with more
+            than one namespace
         """
         if unique and fromids:
             raise Error('alllinks: unique and fromids cannot both be True.')
         algen = self._generator(api.ListGenerator, type_arg='alllinks',
-                                namespaces=namespace, alfrom=start,
-                                total=total, alunique=unique)
-        if prefix:
-            algen.request['alprefix'] = prefix
+                                namespaces=namespace, total=total)
         if fromids:
             algen.request['alprop'] = 'title|ids'
+
+        # circumvent problems with unique and prefix due to T359425 and T359427
+        if self.mw_version < '1.43':
+            if prefix:
+                algen.request['alprefix'] = prefix
+                prefix = ''  # don't break the loop later
+            if start:
+                algen.request['alfrom'] = start
+            algen.request['alunique'] = unique
+        else:
+            if prefix:
+                algen.request['alfrom'] = prefix
+            elif start:
+                algen.request['alfrom'] = start
+            if unique:
+                algen = filter_unique(
+                    algen, key=lambda link: (link['title'], link['ns']))
+
         for link in algen:
             p = pywikibot.Page(self, link['title'], link['ns'])
+            if prefix and p.title() > prefix:  # T359425, T359427
+                break
             if fromids:
                 p._fromid = link['fromid']  # type: ignore[attr-defined]
             yield p
 
     def allcategories(
         self,
         start: str = '!',
```

### Comparing `pywikibot-9.0.0/pywikibot/site/_interwikimap.py` & `pywikibot-9.1.0/pywikibot/site/_interwikimap.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/site/_namespace.py` & `pywikibot-9.1.0/pywikibot/site/_namespace.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/site/_obsoletesites.py` & `pywikibot-9.1.0/pywikibot/site/_obsoletesites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/site/_siteinfo.py` & `pywikibot-9.1.0/pywikibot/site/_siteinfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/site/_tokenwallet.py` & `pywikibot-9.1.0/pywikibot/site/_tokenwallet.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/site/_upload.py` & `pywikibot-9.1.0/pywikibot/site/_upload.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/site_detect.py` & `pywikibot-9.1.0/pywikibot/site_detect.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/specialbots/_unlink.py` & `pywikibot-9.1.0/pywikibot/specialbots/_unlink.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/specialbots/_upload.py` & `pywikibot-9.1.0/pywikibot/specialbots/_upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Special bot library containing UploadRobot.
 
 Do not import classes directly from here but from specialbots.
 """
 #
-# (C) Pywikibot team, 2003-2023
+# (C) Pywikibot team, 2003-2024
 #
 # Distributed under the terms of the MIT license.
 #
 from __future__ import annotations
 
 import os
 import tempfile
@@ -17,22 +17,44 @@
 from urllib.parse import urlparse
 
 import requests
 
 import pywikibot
 import pywikibot.comms.http as http
 from pywikibot import config
+from pywikibot.backports import Callable
 from pywikibot.bot import BaseBot, QuitKeyboardInterrupt
 from pywikibot.exceptions import APIError, FatalServerError, NoPageError
 
 
 class UploadRobot(BaseBot):
 
     """Upload bot."""
 
+    post_processor: Callable[[str, str | None], None] | None = None
+    """If this attribute is set to a callable, the :meth:`run` method
+    calls it after upload. The parameters passed to the callable is the
+    origin *file_url* passed to the :meth:`upload` method and the
+    *filename* returned from that method. It can be used like this:
+
+    .. code:: python
+
+       def summarize(old: str, new: str | None) -> None:
+           if new is None:
+               print(f'{old} was ignored')
+           else:
+               print(f'{old} was uploaded as {new}')
+
+       bot = UploadRobot('Myfile.bmp')
+       bot.post_processor = summarize
+       bot.run()
+
+    .. versionadded:: 9.1
+    """
+
     def __init__(self, url: list[str] | str, *,
                  url_encoding=None,
                  description: str = '',
                  use_filename=None,
                  keep_filename: bool = False,
                  verify_description: bool = True,
                  ignore_warning: bool | list = False,
@@ -44,53 +66,50 @@
                  filename_prefix: str | None = None,
                  force_if_shared: bool = False,
                  **kwargs) -> None:
         """Initializer.
 
         .. versionchanged:: 6.2
            asynchronous upload is used if *asynchronous* parameter is set
-
         .. versionchanged:: 6.4
            *force_if_shared* parameter was added
 
         :param url: path to url or local file, or list of urls or paths
             to local files.
         :param description: Description of file for its page. If multiple files
             are uploading the same description is used for every file.
-        :type description: str
         :param use_filename: Specify title of the file's page. If multiple
             files are uploading it asks to change the name for second, third,
             etc. files, otherwise the last file will overwrite the other.
         :param keep_filename: Set to True to keep original names of urls and
             files, otherwise it will ask to enter a name for each file.
         :param summary: Summary of the upload
         :param verify_description: Set to True to proofread the description.
         :param ignore_warning: Set this to True to upload even if another file
             would be overwritten or another mistake would be risked. Set it to
             an array of warning codes to selectively ignore specific warnings.
         :param target_site: Set the site to upload to. If target site is not
-            given it's taken from user config file (user_config.py).
+            given it's taken from user config file (user-config.py).
         :type target_site: object
         :param aborts: List of the warning types to abort upload on. Set to
             True to abort on any warning.
         :param chunk_size: Upload the file in chunks (more overhead, but
             restartable) specified in bytes. If no value is specified the file
             will be uploaded as whole.
         :param asynchronous: Make potentially large file operations
             asynchronous on the server side when possible.
         :param filename_prefix: Specify prefix for the title of every
             file's page.
         :param force_if_shared: Upload the file even if it's currently
             shared to the target site (e.g. when moving from Commons to another
             wiki)
-        :keyword always: Disables any input, requires that either
+        :keyword bool always: Disables any input, requires that either
             ignore_warning or aborts are set to True and that the
             description is also set. It overwrites verify_description to
             False and keep_filename to True.
-        :type always: bool
         """
         super().__init__(**kwargs)
         if self.opt.always:
             if ignore_warning is not True and aborts is not True:
                 raise ValueError(
                     'When always is set to True, '
                     'ignore_warning or aborts must be set to True.')
@@ -212,19 +231,21 @@
             if this_answer is None:
                 answer = None
         if answer is None:
             answer = pywikibot.input_yn('Do you want to ignore?',
                                         default=False, automatic_quit=False)
         return answer
 
-    def process_filename(self, file_url):
-        """Return base filename portion of file_url."""
+    def process_filename(self, file_url: str) -> str | None:
+        """Return base filename portion of *file_url*.
+
+        :param file_url: either a URL or a local file path
+        """
         # Isolate the pure name
         filename = file_url
-        # Filename may be either a URL or a local file path
         if '://' in filename:
             # extract the path portion of the URL
             filename = urlparse(filename).path
         filename = os.path.basename(filename)
         if self.use_filename:
             filename = self.use_filename
         if self.filename_prefix:
@@ -264,38 +285,38 @@
                     f'Invalid character(s): {c}. Please try again')
                 continue
 
             if allowed_formats and ext not in allowed_formats:
                 if self.opt.always:
                     pywikibot.info('File format is not one of [{}]'
                                    .format(' '.join(allowed_formats)))
-                    continue
 
-                if not pywikibot.input_yn(
-                        'File format is not one of [{}], but {!r}. Continue?'
-                        .format(' '.join(allowed_formats), ext),
-                        default=False):
-                    continue
+                elif pywikibot.input_yn(
+                        'File format is not one of [{}], but {!r}. Skip?'
+                        .format(' '.join(allowed_formats), ext)):
+                    return None
+
+                continue
 
             potential_file_page = pywikibot.FilePage(self.target_site,
                                                      filename)
             if potential_file_page.exists():
                 overwrite = self._handle_warning('exists')
                 if overwrite is False:
                     pywikibot.info(
                         'File exists and you asked to abort. Skipping.')
                     return None
 
                 if potential_file_page.has_permission():
                     if overwrite is None:
                         overwrite = not pywikibot.input_yn(
-                            'File with name {} already exists. '
-                            'Would you like to change the name? '
-                            '(Otherwise file will be overwritten.)'
-                            .format(filename), default=True,
+                            f'File with name {filename} already exists.'
+                            ' Would you like to change the name?'
+                            ' (Otherwise file will be overwritten.)',
+                            default=True,
                             automatic_quit=False)
                     if not overwrite:
                         continue
                     break
 
                 pywikibot.info(f'File with name {filename} already exists and '
                                f'cannot be overwritten.')
@@ -357,27 +378,29 @@
         """
         Determine if the warning message should be ignored.
 
         :param warn_code: The warning message
         """
         return self.ignore_warning is True or warn_code in self.ignore_warning
 
-    def upload_file(self, file_url):
+    def upload_file(self, file_url: str) -> str | None:
         """
         Upload the image at file_url to the target wiki.
 
         .. seealso:: :api:`Upload`
 
         Return the filename that was used to upload the image.
         If the upload fails, ask the user whether to try again or not.
         If the user chooses not to retry, return None.
 
         .. versionchanged:: 7.0
            If 'copyuploadbaddomain' API error occurred in first step,
            download the file and upload it afterwards
+
+        :param file_url: either a URL or a local file path
         """
         filename = self.process_filename(file_url)
         if not filename:
             return None
 
         site = self.target_site
         imagepage = pywikibot.FilePage(site, filename)  # normalizes filename
@@ -428,40 +451,47 @@
 
         return None
 
     def skip_run(self) -> bool:
         """Check whether processing is to be skipped."""
         # early check that upload is enabled
         if self.target_site.is_uploaddisabled():
-            pywikibot.error(
-                'Upload error: Local file uploads are disabled on {}.'
-                .format(self.target_site))
+            pywikibot.error(f'Upload error: Local file uploads are disabled '
+                            f'on {self.target_site}.')
             return True
 
         # early check that user has proper rights to upload
         self.target_site.login()
         if not self.target_site.has_right('upload'):
-            pywikibot.error(
-                "User '{}' does not have upload rights on site {}."
-                .format(self.target_site.user(), self.target_site))
+            pywikibot.error(f"User '{self.target_site.user()}' does not have "
+                            f'upload rights on site {self.target_site}.')
             return True
 
         return False
 
     def run(self):
-        """Run bot."""
+        """Run bot.
+
+        .. versionchanged:: 9.1
+           count uploads.
+        """
         if self.skip_run():
             return
+
         try:
             for file_url in self.url:
-                self.upload_file(file_url)
+                filename = self.upload_file(file_url)
                 self.counter['read'] += 1
+                if filename:
+                    self.counter['upload'] += 1
+                if callable(self.post_processor):
+                    self.post_processor(file_url, filename)
         except QuitKeyboardInterrupt:
-            pywikibot.info(f'\nUser quit {self.__class__.__name__} bot run...')
+            pywikibot.info(f'\nUser quit {type(self).__name__} bot run...')
         except KeyboardInterrupt:
             if config.verbose_output:
                 raise
 
-            pywikibot.info('\nKeyboardInterrupt during {} bot run...'
-                           .format(self.__class__.__name__))
+            pywikibot.info(
+                f'\nKeyboardInterrupt during {type(self).__name__} bot run...')
         finally:
             self.exit()
```

### Comparing `pywikibot-9.0.0/pywikibot/textlib.py` & `pywikibot-9.1.0/pywikibot/textlib.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/throttle.py` & `pywikibot-9.1.0/pywikibot/throttle.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/time.py` & `pywikibot-9.1.0/pywikibot/time.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/titletranslate.py` & `pywikibot-9.1.0/pywikibot/titletranslate.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/tools/__init__.py` & `pywikibot-9.1.0/pywikibot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/tools/_deprecate.py` & `pywikibot-9.1.0/pywikibot/tools/_deprecate.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/tools/_logging.py` & `pywikibot-9.1.0/pywikibot/tools/_logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/tools/_unidata.py` & `pywikibot-9.1.0/pywikibot/tools/_unidata.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/tools/chars.py` & `pywikibot-9.1.0/pywikibot/tools/chars.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/tools/collections.py` & `pywikibot-9.1.0/pywikibot/tools/collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/tools/djvu.py` & `pywikibot-9.1.0/pywikibot/tools/djvu.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/tools/formatter.py` & `pywikibot-9.1.0/pywikibot/tools/formatter.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/tools/itertools.py` & `pywikibot-9.1.0/pywikibot/tools/itertools.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/tools/threading.py` & `pywikibot-9.1.0/pywikibot/tools/threading.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/userinterfaces/__init__.py` & `pywikibot-9.1.0/pywikibot/userinterfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/userinterfaces/_interface_base.py` & `pywikibot-9.1.0/pywikibot/userinterfaces/_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/userinterfaces/buffer_interface.py` & `pywikibot-9.1.0/pywikibot/userinterfaces/buffer_interface.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/userinterfaces/gui.py` & `pywikibot-9.1.0/pywikibot/userinterfaces/gui.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/userinterfaces/terminal_interface_base.py` & `pywikibot-9.1.0/pywikibot/userinterfaces/terminal_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/userinterfaces/terminal_interface_unix.py` & `pywikibot-9.1.0/pywikibot/userinterfaces/terminal_interface_unix.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/userinterfaces/terminal_interface_win32.py` & `pywikibot-9.1.0/pywikibot/userinterfaces/terminal_interface_win32.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/userinterfaces/transliteration.py` & `pywikibot-9.1.0/pywikibot/userinterfaces/transliteration.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot/version.py` & `pywikibot-9.1.0/pywikibot/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """Module to determine the pywikibot version (tag, revision and date)."""
 #
-# (C) Pywikibot team, 2007-2022
+# (C) Pywikibot team, 2007-2024
 #
 # Distributed under the terms of the MIT license.
 #
 from __future__ import annotations
 
 import datetime
 import json
 import os
 import pathlib
 import socket
+import sqlite3
 import subprocess
 import sys
 import sysconfig
 import time
-import xml.dom.minidom
 from contextlib import closing, suppress
 from importlib import import_module
-from io import BytesIO
+from pathlib import Path
 from warnings import warn
 
 import pywikibot
 from pywikibot import config
 from pywikibot.backports import cache
 from pywikibot.comms.http import fetch
 from pywikibot.exceptions import VersionParseError
-from pywikibot.tools import deprecated
+from pywikibot.tools import deprecated, suppress_warnings
+from pywikibot.tools._deprecate import _NotImplementedWarning
 
 
 def _get_program_dir() -> str:
     return os.path.normpath(os.path.split(os.path.dirname(__file__))[0])
 
 
 @deprecated(since='9.0.0')
@@ -63,15 +64,15 @@
     hsh = {}
 
     if online:
         if not local_hsh:
             data['cmp_ver'] = 'UNKNOWN'
         else:
             for branch, path in branches.items():
-                with suppress(Exception):
+                with suppress(VersionParseError):
                     hsh[getversion_onlinerepo(path)] = branch
             if hsh:
                 data['cmp_ver'] = hsh.get(local_hsh, 'OUTDATED')
 
     data['hsh'] = local_hsh[:7]  # make short hash from full hash
     return '{tag} ({hsh}, {rev}, {date}, {cmp_ver})'.format_map(data)
 
@@ -90,27 +91,30 @@
     exceptions = {}
 
     for vcs_func in (getversion_git,
                      getversion_svn,
                      getversion_nightly,
                      getversion_package):
         try:
-            (tag, rev, date, hsh) = vcs_func(_program_dir)
+            with suppress_warnings(
+                f'.*({vcs_func.__name__}|svn_rev_info) is deprecated since '
+                    'release 9.1.', _NotImplementedWarning):
+                tag, rev, date, hsh = vcs_func(_program_dir)
         except Exception as e:
-            exceptions[vcs_func] = e
+            exceptions[vcs_func] = vcs_func.__name__, e
         else:
             break
     else:
         # nothing worked; version unknown (but suppress exceptions)
         # the value is most likely '$Id' + '$', it means that
         # pywikibot was imported without using version control at all.
         tag, rev, date, hsh = (
             '', '-1 (unknown)', '0 (unknown)', '(unknown)')
-        warn('Unable to detect version; exceptions raised:\n{!r}'
-             .format(exceptions), UserWarning)
+        warn(f'Unable to detect version; exceptions raised:\n{exceptions!r}',
+             UserWarning)
         exceptions = None
 
     # Git and SVN can silently fail, as it may be a nightly.
     if exceptions:
         pywikibot.debug(f'version algorithm exceptions:\n{exceptions!r}')
 
     if isinstance(date, str):
@@ -120,111 +124,70 @@
     else:
         warn('Unable to detect package date', UserWarning)
         datestring = '-2 (unknown)'
 
     return {'tag': tag, 'rev': rev, 'date': datestring, 'hsh': hsh}
 
 
-def svn_rev_info(path):  # pragma: no cover
+@deprecated(since='9.1')
+def svn_rev_info(path):
     """Fetch information about the current revision of a Subversion checkout.
 
+    .. deprecated:: 9.1
+       update to git repository.
+    .. versionchanged:: 9.1
+       drop support for svn 1.6 and older.
+
     :param path: directory of the Subversion checkout
     :return:
         - tag (name for the repository),
         - rev (current Subversion revision identifier),
         - date (date of current revision),
     :rtype: ``tuple`` of two ``str`` and a ``time.struct_time``
     """
     if not os.path.isdir(os.path.join(path, '.svn')):
         path = os.path.join(path, '..')
 
-    _program_dir = path
-    filename = os.path.join(_program_dir, '.svn/entries')
-    if os.path.isfile(filename):
-        with open(filename) as entries:
-            version = entries.readline().strip()
-            if version != '12':
-                for _ in range(3):
-                    entries.readline()
-                tag = entries.readline().strip()
-                t = tag.split('://', 1)
-                t[1] = t[1].replace('svn.wikimedia.org/svnroot/pywikipedia/',
-                                    '')
-                tag = '[{}] {}'.format(*t)
-                for _ in range(4):
-                    entries.readline()
-                date = time.strptime(entries.readline()[:19],
-                                     '%Y-%m-%dT%H:%M:%S')
-                rev = entries.readline()[:-1]
-                return tag, rev, date
-
-    # We haven't found the information in entries file.
-    # Use sqlite table for new entries format
-    from sqlite3 import dbapi2 as sqlite
     with closing(
-            sqlite.connect(os.path.join(_program_dir, '.svn/wc.db'))) as con:
+            sqlite3.connect(os.path.join(path, '.svn/wc.db'))) as con:
         cur = con.cursor()
         cur.execute("""select
 local_relpath, repos_path, revision, changed_date, checksum from nodes
 order by revision desc, changed_date desc""")
         _name, tag, rev, date, _checksum = cur.fetchone()
         cur.execute('select root from repository')
         tag, = cur.fetchone()
 
     tag = os.path.split(tag)[1]
     date = time.gmtime(date / 1_000_000)
     return tag, rev, date
 
 
-def github_svn_rev2hash(tag: str, rev):  # pragma: no cover
-    """Convert a Subversion revision to a Git hash using GitHub.
-
-    :param tag: name of the Subversion repo on GitHub
-    :param rev: Subversion revision identifier
-    :return: the git hash
-    """
-    uri = f'https://github.com/wikimedia/{tag}/!svn/vcc/default'
-    request = fetch(uri, method='PROPFIND',
-                    data="<?xml version='1.0' encoding='utf-8'?>"
-                         '<propfind xmlns=\"DAV:\"><allprop/></propfind>',
-                    headers={'label': str(rev),
-                             'user-agent': 'SVN/1.7.5 {pwb}'})
-    dom = xml.dom.minidom.parse(BytesIO(request.content))
-    hsh = dom.getElementsByTagName('C:git-commit')[0].firstChild.nodeValue
-    date = dom.getElementsByTagName('S:date')[0].firstChild.nodeValue
-    date = time.strptime(date[:19], '%Y-%m-%dT%H:%M:%S')
-    return hsh, date
-
-
-def getversion_svn(path=None):  # pragma: no cover
+@deprecated(since='9.1')
+def getversion_svn(path=None):
     """Get version info for a Subversion checkout.
 
+    .. deprecated:: 9.1
+       update to git repository.
+
     :param path: directory of the Subversion checkout
     :return:
         - tag (name for the repository),
         - rev (current Subversion revision identifier),
         - date (date of current revision),
-        - hash (git hash for the Subversion revision)
+        - hash '(unknown)'
     :rtype: ``tuple`` of three ``str`` and a ``time.struct_time``
     """
     _program_dir = path or _get_program_dir()
     tag, rev, date = svn_rev_info(_program_dir)
-    hsh, date2 = github_svn_rev2hash(tag, rev)
-    if date.tm_isdst >= 0 and date2.tm_isdst >= 0:
-        assert date == date2, 'Date of version is not consistent'
-    # date.tm_isdst is -1 means unknown state
-    # compare its contents except daylight saving time status
-    else:
-        for i in range(len(date) - 1):
-            assert date[i] == date2[i], 'Date of version is not consistent'
-
     rev = f's{rev}'
+
     if (not date or not tag or not rev) and not path:
         raise VersionParseError
-    return (tag, rev, date, hsh)
+    return (tag, rev, date, '(unknown)')
 
 
 def getversion_git(path=None):
     """Get version info for a Git clone.
 
     :param path: directory of the Git checkout
     :return:
@@ -274,29 +237,32 @@
     rev = f'g{len(rev.splitlines())}'
     hsh = info[3]  # also stored in '.git/refs/heads/master'
     if (not date or not tag or not rev) and not path:
         raise VersionParseError
     return (tag, rev, date, hsh)
 
 
-def getversion_nightly(path=None):  # pragma: no cover
+def getversion_nightly(path: str | Path | None = None):  # pragma: no cover
     """Get version info for a nightly release.
 
+    .. hint::
+       the version informations of the nightly dump is stored in the
+       ``version`` file within the ``pywikibot`` folder.
+
     :param path: directory of the uncompressed nightly.
     :return:
         - tag (name for the repository),
         - rev (current revision identifier),
         - date (date of current revision),
         - hash (git hash for the current revision)
     :rtype: ``tuple`` of three ``str`` and a ``time.struct_time``
     """
-    if not path:
-        path = _get_program_dir()
+    file = Path(path or _get_program_dir()) / 'pywikibot' / 'version'
 
-    with open(os.path.join(path, 'version')) as data:
+    with file.open() as data:
         (tag, rev, date, hsh) = data.readlines()
 
     date = time.strptime(date[:19], '%Y-%m-%dT%H:%M:%S')
 
     if not date or not tag or not rev:
         raise VersionParseError
     return (tag, rev, date, hsh)
@@ -348,15 +314,15 @@
     """
     if hasattr(module, '__file__'):
         filename = module.__file__
         if not filename or not os.path.exists(filename):
             return None
 
         program_dir = _get_program_dir()
-        if filename[:len(program_dir)] == program_dir:
+        if filename.startswith(program_dir):
             return filename
     return None
 
 
 def get_module_mtime(module):
     """
     Retrieve the modification time from an imported module.
```

### Comparing `pywikibot-9.0.0/pywikibot/xmlreader.py` & `pywikibot-9.1.0/pywikibot/xmlreader.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot.egg-info/PKG-INFO` & `pywikibot-9.1.0/pywikibot.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 9.0.0
+Version: 9.1.0
 Summary: Python MediaWiki Bot Framework
 Author-email: xqt <info@gno.de>
 Maintainer-email: The Pywikibot team <pywikibot@lists.wikimedia.org>
 License: MIT License
 Project-URL: Homepage, https://www.mediawiki.org/wiki/Manual:Pywikibot
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
 Project-URL: Repository, https://gerrit.wikimedia.org/r/plugins/gitiles/pywikibot/core/
@@ -295,101 +295,30 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-Improvements
-^^^^^^^^^^^^
-
-* Python 3.13 is supported
-* Update tools._unidata._category_cf from Unicodedata version 15.1.0
-* Timestamp.nowutc()and
-  Timestamp.utcnow()were added (T337748)
-* Remove content parameter of proofreadpage.IndexPage.page_genmethod. (T358635)
-* Backport ``itertools.batched`` from Python 3.13 to backports.batched
-* A copy button was added to the sphinx documentation.
-* Make languages_by_sizedynamic (T78396). The property is
-  only available for family.WikimediaFamilyfamilies. The ``wikimedia_sites.py`` maintenance script was
-  removed.
-* Add config.base_dirto scripts search path with pwbwrapper (T324287)
-* pywikibot.WbTime.equal_instantwas added (T325248)
-* ``revisions`` parameter of xmlreader.XmlDumpwas introduced to specify parsing method
-  (T340804)
-* Pass global -nolog argument into bot script from wrapper (T328900)
-* Add site.APISite.ratelimit()method
-  and tools.collections.RateLimitNamedTuple (T304808)
-* L10N and i18n updates
-* Add pagegenerators.PagePilePageGenerator(T353086)
-
-Bugfixes
-^^^^^^^^
-
-* Timestamp.now()and
-  Timestamp.fromtimestamp()also returns a
-  Timestampobject with Python 3.7
-* Populate pywikibot.MediaInfo._content with expected attributes when loaded (T357608)
-* Raise exceptions.APIErrorif the same error comes twice within data.api.Request.submitloop
-  (T357870)
-* Only delegate sitemethods to public family.Familymethods which have *code* as first parameter.
-* Use ``str`` instead of ``repr`` for several messages with family.Familyobjects (T356782)
-* Add ``hy`` to special languages in textlib.TimeStripper(T356175)
-* Pass login token when using ``action=login`` (T309898)
-* Detect range blocks with pywikibot.User.is_blocked(T301282)
-* Use only ``end`` tags in ElementTree.iterparse in xmlreadermodule (T354095)
-* Suppress error in cosmetic_changes.CosmeticChangesToolkit.cleanUpLinks(T337045)
-* pywikibot.input_choicevalidates *default* parameter (T353097)
-* Remove typing imports from user-config.py file (T352965)
-
-Breaking changes and code cleanups
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-* Cache directory was renamed from ``apicache-py3`` to ``apicache`` due to timestamp changes. (T337748)
-  **Warning:** Do not use Pywikibot 9+ together with Pywikibot 3.0.20181203 and below.
-* Raise ``TypeError`` instead of ``AttributeError`` in Site.randompages()
-  if *redirects* parameter is invalid.
-* A RuntimeError will be raised if a family.Familysubclass has an ``__init__`` initializer method.
-  family.Family.__post_init__classmethod can be used instead.
-* InteractiveReplacewas moved from botto bot_choicemodule
-* ``userinterfaces.transliteration.transliterator`` was renamed to Transliterator
-  
-* ``pywikibot.BaseSite`` and ``pywikibotAPISite`` were dropped. pywikibot.Sitehas to be used to create a
-  siteobject.
-* ``next`` parameter of userinterfaces.transliteration.Transliterator.transliteratewas renamed to ``succ``
-* ``type`` parameter of site.APISite.protectedpages()
-  was renamed to ``protect_type``
-* ``all`` parameter of site.APISite.namespace()was renamed to
-  ``all_ns``
-* ``filter`` parameter of date.dhwas renamed to ``filter_func``
-* ``dict`` parameter of data.api.OptionSetwas renamed to ``data``
-* ``setuptools`` package is no longer mandatory but required for tests
-  (T340640, T347052, T354515)
-* ``root`` attribute of xmlreader.XmlDumpwas removed
-* ``tools.Version`` class was removed; use classes from ``packaging.version`` instead (T340640)
-* ``packaging`` package is mandatory; ``importlib_metadata`` package is required for Python 3.7 (T340640)
-* ``SelfCallMixin``, ``SelfCallDict`` and ``SelfCallString`` of toolsmodule were removed
-* Calling site.BaseSite.sitenameas a function
-  is no longer supported
-* ``config.register_family_file()`` function was removed
-* require ``PyMySQL >= 1.0.0`` if necessary
-* ``keys()`` and ``items()`` methods of data.api.Requestgives a view instead a list (T310953)
-* ``SequenceOutputter.format_list()`` was removed in favour of tools.formatter.SequenceOutputter.outproperty
-* *output* parameter of bot_choice.OutputProxyOption(i.e. ``OutputOption`` instance) without *out* property is
-  no longer supported
-* ``OutputOption.output()`` method was removed
-* ``ContextOption.output_range()`` and ``HighlightContextOption.output_range()`` methods were removed
-* ``page.url2unicode()`` function was removed in favour of tools.chars.url2string
-* *iterables* of tools.itertools.intersect_generatorsmust not be given as a single list or tuple;
-  either consecutive iterables must be used or '*' to unpack
-* *allow_duplicates* parameter of tools.itertools.intersect_generatorsmust be given as keyword argument
-* Infinite rotating file handler with ``config.logfilesize`` of -1 is no longer supported
-* ``Throttle.multiplydelay`` attribute was removed
-* Python 3.6 support was dropped (T347026)
-
+* ``-usernames`` option was added to versionscript
+* Circumvent problems with *unique* and *prefix* parameters in Site.alllinks()
+  (T359427)
+* Detect nighly version file with version.getversion_nightly(T362492)
+* version.github_svn_rev2hash() was removed; it was no longer functional (T362484)
+* SVN support has been dropped; ``.svnprops`` property settings was removed (T362484)
+* Skip process that requires login to logout (T326614)
+* File title of specialbots.UploadRobotmust have a valid file extension (T345786)
+* Add a post_processorattribute to specialbots.UploadRobot
+  which can be called after each upload (T359766)
+* Avoid using pywikibot.handle_argsin private scripts;
+  use pwbwrapper instead (T359766)
+* Show upload count with specialbots.UploadRobot
+* Use the same ``iiprop`` properties in data.api.PageGeneratoras in
+  APISite.loadimageinfo(T360093)
+* i18n updates
 
 Deprecations
 ------------
 
 * 9.0.0: The *content* parameter of proofreadpage.IndexPage.page_genis deprecated and will be ignored
   (T358635)
 * 9.0.0: ``userinterfaces.transliteration.transliterator`` was renamed to Transliterator
@@ -435,14 +364,16 @@
 * 8.0.0: Page.editTime()method is deprecated and should be replaced by
   Page.latest_revision.timestamp
 
 
 Will be removed in Pywikibot 10
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
+* 9.1.0: version.svn_rev_infoand version.getversion_svnwill be removed. SVN is no longer supported.
+  (T362484)
 * 7.7.0: tools.threadingclasses should no longer imported from tools
 * 7.6.0: tools.itertoolsdatatypes should no longer imported from tools
 * 7.6.0: tools.collectionsdatatypes should no longer imported from tools
 * 7.5.0: textlib.tzoneFixedOffset class will be removed in favour of time.TZoneFixedOffset
 * 7.4.0: ``FilePage.usingPages()`` was renamed to using_pages()
 * 7.3.0: Old color escape sequences like ``\03{color}`` is deprecated in favour of new color format like <<color>>
 * 7.3.0: ``linkitrail`` method of family.Familyis deprecated; use APISite.linktrail()
```

### Comparing `pywikibot-9.0.0/pywikibot.egg-info/SOURCES.txt` & `pywikibot-9.1.0/pywikibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/pywikibot.egg-info/requires.txt` & `pywikibot-9.1.0/pywikibot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/setup.py` & `pywikibot-9.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pywikibot-9.0.0/tests/tests_tests.py` & `pywikibot-9.1.0/tests/tests_tests.py`

 * *Files identical despite different names*

