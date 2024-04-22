# Comparing `tmp/arts-2024.4.19.1.tar.gz` & `tmp/arts-2024.4.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arts-2024.4.19.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "arts-2024.4.22.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `arts-2024.4.19.1.tar` & `arts-2024.4.22.tar`

### file list

```diff
@@ -1,239 +1,239 @@
--rw-r--r--   0        0        0     2175 2023-12-20 10:09:43.709218 arts-2024.4.19.1/.gitignore
--rw-r--r--   0        0        0       46 2024-03-10 10:13:06.948005 arts-2024.4.19.1/README.md
--rw-r--r--   0        0        0      317 2024-02-22 12:02:36.224046 arts-2024.4.19.1/arts/CoolMemory-English/Copyright
--rw-r--r--   0        0        0    10492 2024-04-12 03:24:43.904296 arts-2024.4.19.1/arts/CoolMemory-English/README.md
--rw-r--r--   0        0        0      110 2024-03-06 00:07:28.301653 arts-2024.4.19.1/arts/CoolMemory-English/art.json
--rw-r--r--   0        0        0      393 2023-12-10 08:00:44.000000 arts-2024.4.19.1/arts/CoolMemory-English/licenses/README.md
--rw-r--r--   0        0        0     1586 2023-12-10 08:00:44.000000 arts-2024.4.19.1/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE
--rw-r--r--   0        0        0    11550 2023-12-10 08:00:44.000000 arts-2024.4.19.1/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE
--rw-r--r--   0        0        0    32825 2023-12-10 08:00:44.000000 arts-2024.4.19.1/arts/CoolMemory-English/licenses/licenses/Python/LICENSE
--rw-r--r--   0        0        0     2987 2023-12-10 08:00:44.000000 arts-2024.4.19.1/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE
--rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.19.1/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE
--rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.19.1/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE
--rw-r--r--   0        0        0      106 2024-03-31 10:18:29.252509 arts-2024.4.19.1/arts/WeChat-Art-Museum/art.json
--rw-r--r--   0        0        0    53616 2024-04-13 08:11:29.182384 arts-2024.4.19.1/arts/WeChat-Art-Museum/index.html
--rw-r--r--   0        0        0        0 2024-02-22 15:47:26.927352 arts-2024.4.19.1/arts/__init__.py
--rw-r--r--   0        0        0     3088 2023-09-24 08:08:30.000000 arts-2024.4.19.1/arts/articles/010-赚钱宝典/010-财富的本质/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:01:11.532367 arts-2024.4.19.1/arts/articles/010-赚钱宝典/010-财富的本质/art.json
--rw-r--r--   0        0        0     1681 2023-12-20 10:09:07.827303 arts-2024.4.19.1/arts/articles/010-赚钱宝典/020-商业价值/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:01:11.533332 arts-2024.4.19.1/arts/articles/010-赚钱宝典/020-商业价值/art.json
--rw-r--r--   0        0        0     3552 2023-12-22 07:27:54.636897 arts-2024.4.19.1/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md
--rw-r--r--   0        0        0       44 2023-12-22 07:26:00.584312 arts-2024.4.19.1/arts/articles/010-赚钱宝典/030-财富稳定型社会/art.json
--rw-r--r--   0        0        0     1812 2024-01-02 20:05:02.520382 arts-2024.4.19.1/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md
--rw-r--r--   0        0        0       44 2024-01-02 20:46:41.567445 arts-2024.4.19.1/arts/articles/075-追英赶美/300-产业升级与失业潮/art.json
--rw-r--r--   0        0        0     1253 2024-01-18 01:49:14.297346 arts-2024.4.19.1/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md
--rw-r--r--   0        0        0       44 2024-01-02 20:47:04.916014 arts-2024.4.19.1/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/art.json
--rw-r--r--   0        0        0     1559 2023-11-15 13:45:10.000000 arts-2024.4.19.1/arts/articles/150-小民参政/300-广义的民主/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:02:18.547561 arts-2024.4.19.1/arts/articles/150-小民参政/300-广义的民主/art.json
--rw-r--r--   0        0        0     3056 2024-04-15 06:41:13.052262 arts-2024.4.19.1/arts/articles/150-小民参政/450-我们处于史上最好的时代/README.md
--rw-r--r--   0        0        0       44 2024-04-14 07:59:47.314020 arts-2024.4.19.1/arts/articles/150-小民参政/450-我们处于史上最好的时代/art.json
--rw-r--r--   0        0        0     1499 2023-10-24 11:49:00.000000 arts-2024.4.19.1/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:02:18.545561 arts-2024.4.19.1/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/art.json
--rw-r--r--   0        0        0     1450 2023-11-05 04:22:04.000000 arts-2024.4.19.1/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.648073 arts-2024.4.19.1/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/art.json
--rw-r--r--   0        0        0     3278 2024-02-25 10:11:51.363950 arts-2024.4.19.1/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.644190 arts-2024.4.19.1/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/art.json
--rw-r--r--   0        0        0     1265 2024-03-28 16:30:38.111960 arts-2024.4.19.1/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.645220 arts-2024.4.19.1/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/art.json
--rw-r--r--   0        0        0     1135 2024-03-04 05:13:36.283230 arts-2024.4.19.1/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:03:07.647184 arts-2024.4.19.1/arts/articles/300-批判那些伪文艺/800-务实与务虚/art.json
--rw-r--r--   0        0        0     2095 2024-01-18 01:48:33.751985 arts-2024.4.19.1/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.900873 arts-2024.4.19.1/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/art.json
--rw-r--r--   0        0        0     1668 2023-11-05 03:35:50.000000 arts-2024.4.19.1/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.909872 arts-2024.4.19.1/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/art.json
--rw-r--r--   0        0        0     1669 2023-11-15 13:41:24.000000 arts-2024.4.19.1/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.903896 arts-2024.4.19.1/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/art.json
--rw-r--r--   0        0        0     1906 2023-12-27 20:37:35.730568 arts-2024.4.19.1/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.899872 arts-2024.4.19.1/arts/articles/450-万象思考/200-人工智能会不会统治人类？/art.json
--rw-r--r--   0        0        0     1154 2023-11-05 02:49:06.000000 arts-2024.4.19.1/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.907909 arts-2024.4.19.1/arts/articles/450-万象思考/250-忒修斯之船悖论/art.json
--rw-r--r--   0        0        0     3155 2023-12-27 20:37:10.901781 arts-2024.4.19.1/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md
--rw-r--r--   0        0        0       44 2024-01-05 13:23:02.578368 arts-2024.4.19.1/arts/articles/450-万象思考/300-有无相生，难易相成的启发/art.json
--rw-r--r--   0        0        0     1354 2023-11-05 03:42:52.000000 arts-2024.4.19.1/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md
--rw-r--r--   0        0        0       44 2024-01-05 13:30:30.884939 arts-2024.4.19.1/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/art.json
--rw-r--r--   0        0        0     1123 2023-09-10 18:11:18.000000 arts-2024.4.19.1/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.906885 arts-2024.4.19.1/arts/articles/450-万象思考/500-人们为什么希望拥有后代/art.json
--rw-r--r--   0        0        0      708 2023-12-27 20:36:45.425482 arts-2024.4.19.1/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.904897 arts-2024.4.19.1/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/art.json
--rw-r--r--   0        0        0     5024 2024-04-19 10:28:44.045083 arts-2024.4.19.1/arts/articles/450-万象思考/700-堕胎自由权/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.901873 arts-2024.4.19.1/arts/articles/450-万象思考/700-堕胎自由权/art.json
--rw-r--r--   0        0        0     3701 2023-11-15 13:30:02.000000 arts-2024.4.19.1/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:00.910899 arts-2024.4.19.1/arts/articles/450-万象思考/800-人人平等是个伪概念/art.json
--rw-r--r--   0        0        0     3385 2023-12-27 20:36:19.402593 arts-2024.4.19.1/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.414383 arts-2024.4.19.1/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/art.json
--rw-r--r--   0        0        0     2466 2024-02-25 10:07:00.576902 arts-2024.4.19.1/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.399805 arts-2024.4.19.1/arts/articles/600-时空猜想/400-我们可能处在人造世界/art.json
--rw-r--r--   0        0        0     3007 2023-11-04 19:08:36.000000 arts-2024.4.19.1/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.412423 arts-2024.4.19.1/arts/articles/600-时空猜想/600-占卜真的存在吗？/art.json
--rw-r--r--   0        0        0     2630 2023-11-04 19:15:30.000000 arts-2024.4.19.1/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:21.411378 arts-2024.4.19.1/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/art.json
--rw-r--r--   0        0        0     2038 2023-12-28 02:10:43.748193 arts-2024.4.19.1/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md
--rw-r--r--   0        0        0       44 2023-12-28 02:02:17.049897 arts-2024.4.19.1/arts/articles/700-论时事/300-那些年，我们经历过的历史/art.json
--rw-r--r--   0        0        0     1742 2024-01-13 20:46:22.292355 arts-2024.4.19.1/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:04:35.958057 arts-2024.4.19.1/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/art.json
--rw-r--r--   0        0        0     7343 2023-06-23 06:29:18.000000 arts-2024.4.19.1/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:05:12.312457 arts-2024.4.19.1/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/art.json
--rw-r--r--   0        0        0     1652 2023-06-23 06:48:36.000000 arts-2024.4.19.1/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:05:34.053435 arts-2024.4.19.1/arts/articles/800-小说/600-一念天堂/050-被绑架/art.json
--rw-r--r--   0        0        0    11275 2024-04-13 03:33:01.837811 arts-2024.4.19.1/arts/base95/LICENSE
--rw-r--r--   0        0        0     2677 2024-04-19 10:45:27.323930 arts-2024.4.19.1/arts/base95/README.md
--rw-r--r--   0        0        0       63 2024-04-19 09:19:32.694427 arts-2024.4.19.1/arts/base95/__init__.py
--rw-r--r--   0        0        0     3568 2024-04-19 11:05:40.541843 arts-2024.4.19.1/arts/base95/_core.py
--rw-r--r--   0        0        0       98 2024-04-13 08:02:33.643534 arts-2024.4.19.1/arts/base95/art.json
--rw-r--r--   0        0        0       74 2024-04-19 09:19:40.646468 arts-2024.4.19.1/arts/base95/base95.py
--rw-r--r--   0        0        0      672 2024-04-19 09:47:07.876329 arts-2024.4.19.1/arts/base95/pyproject.toml
--rw-r--r--   0        0        0    11283 2024-02-22 12:02:36.224046 arts-2024.4.19.1/arts/cooltypes/LICENSE
--rw-r--r--   0        0        0      293 2024-03-22 15:18:30.564599 arts-2024.4.19.1/arts/cooltypes/__init__.py
--rw-r--r--   0        0        0     1542 2024-03-31 09:40:29.228723 arts-2024.4.19.1/arts/cooltypes/envname/README.md
--rw-r--r--   0        0        0       62 2024-02-23 04:28:30.402332 arts-2024.4.19.1/arts/cooltypes/envname/__init__.py
--rw-r--r--   0        0        0      447 2024-04-08 07:02:42.471320 arts-2024.4.19.1/arts/cooltypes/envname/_core.py
--rw-r--r--   0        0        0      548 2024-04-08 07:01:42.600503 arts-2024.4.19.1/arts/cooltypes/moduledb/README.md
--rw-r--r--   0        0        0       32 2024-02-23 04:03:44.487797 arts-2024.4.19.1/arts/cooltypes/moduledb/__init__.py
--rw-r--r--   0        0        0     3515 2024-04-08 06:57:45.544745 arts-2024.4.19.1/arts/cooltypes/moduledb/_core.py
--rw-r--r--   0        0        0        0 2024-03-11 20:20:36.445694 arts-2024.4.19.1/arts/cooltypes/modules/coolstr/__init__.py
--rw-r--r--   0        0        0     2181 2024-03-22 15:28:12.579126 arts-2024.4.19.1/arts/cooltypes/modules/coolstr/_core.py
--rw-r--r--   0        0        0     3316 2024-03-31 09:40:29.228723 arts-2024.4.19.1/arts/cooltypes/modules/cooltime/README.md
--rw-r--r--   0        0        0        0 2024-03-11 20:20:55.541076 arts-2024.4.19.1/arts/cooltypes/modules/cooltime/__init__.py
--rw-r--r--   0        0        0       44 2024-02-22 10:39:05.460423 arts-2024.4.19.1/arts/cooltypes/modules/cooltime/_art.json
--rw-r--r--   0        0        0     3665 2024-03-22 15:09:31.411034 arts-2024.4.19.1/arts/cooltypes/modules/cooltime/_core.py
--rw-r--r--   0        0        0     5793 2024-03-22 15:12:37.868753 arts-2024.4.19.1/arts/cooltypes/modules/rslice/README.md
--rw-r--r--   0        0        0        0 2024-03-11 20:26:19.316480 arts-2024.4.19.1/arts/cooltypes/modules/rslice/__init__.py
--rw-r--r--   0        0        0     2764 2024-04-15 07:46:47.281317 arts-2024.4.19.1/arts/cooltypes/modules/rslice/_core.py
--rw-r--r--   0        0        0        0 2024-03-11 20:22:01.981114 arts-2024.4.19.1/arts/cooltypes/modules/vtype/__init__.py
--rw-r--r--   0        0        0    10012 2024-04-13 01:46:07.477663 arts-2024.4.19.1/arts/cooltypes/modules/vtype/_core.py
--rw-r--r--   0        0        0      238 2024-03-22 14:31:42.101320 arts-2024.4.19.1/arts/cooltypes/设计.md
--rw-r--r--   0        0        0    61654 2024-04-19 10:10:18.218640 arts-2024.4.19.1/arts/index.html
--rw-r--r--   0        0        0       44 2024-01-16 13:04:45.523107 arts-2024.4.19.1/arts/life/2018/莆田学院·毕业生留影/art.json
--rw-r--r--   0        0        0      830 2024-02-12 15:02:22.123647 arts-2024.4.19.1/arts/life/2018/莆田学院·毕业生留影/index.html
--rw-r--r--   0        0        0       44 2024-01-17 04:28:07.076300 arts-2024.4.19.1/arts/life/2019/苏州市虎丘山/art.json
--rw-r--r--   0        0        0     1233 2024-03-24 16:39:19.059155 arts-2024.4.19.1/arts/life/2019/苏州市虎丘山/index.html
--rw-r--r--   0        0        0       44 2024-01-17 03:40:13.294365 arts-2024.4.19.1/arts/life/2022/泉州市丰泽区·雨后街道/art.json
--rw-r--r--   0        0        0      969 2024-03-24 16:39:36.018072 arts-2024.4.19.1/arts/life/2022/泉州市丰泽区·雨后街道/index.html
--rw-r--r--   0        0        0       44 2024-01-30 05:00:40.402244 arts-2024.4.19.1/arts/life/2023/更换微信账号了/art.json
--rw-r--r--   0        0        0      898 2024-04-03 03:17:39.386427 arts-2024.4.19.1/arts/life/2023/更换微信账号了/index.html
--rw-r--r--   0        0        0       44 2024-03-24 16:41:15.708702 arts-2024.4.19.1/arts/life/2024/泉州市承天禅寺/art.json
--rw-r--r--   0        0        0     1133 2024-03-25 03:52:07.749983 arts-2024.4.19.1/arts/life/2024/泉州市承天禅寺/index.html
--rw-r--r--   0        0        0    11276 2024-02-22 12:02:36.224046 arts-2024.4.19.1/arts/miumapp/LICENSE
--rw-r--r--   0        0        0     5762 2024-03-31 09:40:29.228723 arts-2024.4.19.1/arts/miumapp/README.md
--rw-r--r--   0        0        0       36 2024-02-12 15:08:38.569224 arts-2024.4.19.1/arts/miumapp/__init__.py
--rw-r--r--   0        0        0     7645 2024-04-12 04:07:11.111023 arts-2024.4.19.1/arts/miumapp/_core.py
--rw-r--r--   0        0        0      111 2024-03-05 23:26:53.659150 arts-2024.4.19.1/arts/miumapp/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.19.1/arts/miumapp/licenses/README.md
--rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.19.1/arts/miumapp/licenses/pyppeteer/LICENSE
--rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.19.1/arts/miumapp/licenses/tornado/LICENSE
--rw-r--r--   0        0        0       48 2024-02-12 15:15:42.556195 arts-2024.4.19.1/arts/miumapp/miumapp/__init__.py
--rw-r--r--   0        0        0     4657 2024-02-22 17:30:50.375647 arts-2024.4.19.1/arts/miumapp/miumapp/demo.html
--rw-r--r--   0        0        0     1241 2024-03-25 04:09:36.827762 arts-2024.4.19.1/arts/miumapp/miumapp/demo.py
--rw-r--r--   0        0        0      644 2024-04-13 08:19:45.878790 arts-2024.4.19.1/arts/miumapp/pyproject.toml
--rw-r--r--   0        0        0    11273 2024-03-02 20:20:55.781363 arts-2024.4.19.1/arts/oodb/LICENSE
--rw-r--r--   0        0        0    22563 2024-03-31 09:40:29.216952 arts-2024.4.19.1/arts/oodb/README.md
--rw-r--r--   0        0        0       44 2024-03-06 00:36:04.879589 arts-2024.4.19.1/arts/oodb/__init__.py
--rw-r--r--   0        0        0    19029 2024-04-19 10:29:59.567475 arts-2024.4.19.1/arts/oodb/_core.py
--rw-r--r--   0        0        0       99 2024-03-06 01:01:05.433633 arts-2024.4.19.1/arts/oodb/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.19.1/arts/oodb/licenses/README.md
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.19.1/arts/oodb/licenses/pymongo/LICENSE
--rw-r--r--   0        0        0       53 2024-03-06 00:36:04.879589 arts-2024.4.19.1/arts/oodb/oodb.py
--rw-r--r--   0        0        0      627 2024-04-13 08:20:16.552792 arts-2024.4.19.1/arts/oodb/pyproject.toml
--rw-r--r--   0        0        0    11281 2024-03-03 07:09:08.518004 arts-2024.4.19.1/arts/oomongo/LICENSE
--rw-r--r--   0        0        0    17439 2024-03-31 09:40:29.227707 arts-2024.4.19.1/arts/oomongo/README.md
--rw-r--r--   0        0        0       49 2024-03-05 08:01:41.054010 arts-2024.4.19.1/arts/oomongo/__init__.py
--rw-r--r--   0        0        0    27613 2024-04-15 07:46:47.281317 arts-2024.4.19.1/arts/oomongo/_core.py
--rw-r--r--   0        0        0       92 2024-03-06 00:50:10.273786 arts-2024.4.19.1/arts/oomongo/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.19.1/arts/oomongo/licenses/README.md
--rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 arts-2024.4.19.1/arts/oomongo/licenses/motor/LICENSE
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.19.1/arts/oomongo/licenses/pymongo/LICENSE
--rw-r--r--   0        0        0       61 2024-03-05 08:01:41.059008 arts-2024.4.19.1/arts/oomongo/oomongo.py
--rw-r--r--   0        0        0      564 2024-04-13 08:20:16.553795 arts-2024.4.19.1/arts/oomongo/pyproject.toml
--rw-r--r--   0        0        0    11281 2024-03-03 07:10:17.933453 arts-2024.4.19.1/arts/oomysql/LICENSE
--rw-r--r--   0        0        0    17139 2024-03-31 09:40:29.228723 arts-2024.4.19.1/arts/oomysql/README.md
--rw-r--r--   0        0        0       45 2024-03-05 08:02:05.322948 arts-2024.4.19.1/arts/oomysql/__init__.py
--rw-r--r--   0        0        0    35301 2024-04-15 07:46:47.271326 arts-2024.4.19.1/arts/oomysql/_core.py
--rw-r--r--   0        0        0       90 2024-03-06 00:10:16.490984 arts-2024.4.19.1/arts/oomysql/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.19.1/arts/oomysql/licenses/README.md
--rw-r--r--   0        0        0     1070 2022-05-08 19:03:56.000000 arts-2024.4.19.1/arts/oomysql/licenses/aiomysql/LICENSE
--rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 arts-2024.4.19.1/arts/oomysql/licenses/pymysql/LICENSE
--rw-r--r--   0        0        0       57 2024-03-05 08:02:05.335929 arts-2024.4.19.1/arts/oomysql/oomysql.py
--rw-r--r--   0        0        0      642 2024-04-13 08:20:16.553795 arts-2024.4.19.1/arts/oomysql/pyproject.toml
--rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 arts-2024.4.19.1/arts/openai2/LICENSE
--rw-r--r--   0        0        0    13991 2024-04-07 02:46:07.779093 arts-2024.4.19.1/arts/openai2/README.md
--rw-r--r--   0        0        0      168 2024-04-07 02:56:58.773363 arts-2024.4.19.1/arts/openai2/__init__.py
--rw-r--r--   0        0        0     9858 2024-04-07 03:08:27.254965 arts-2024.4.19.1/arts/openai2/_core/chat.py
--rw-r--r--   0        0        0     2286 2024-04-08 06:59:43.786636 arts-2024.4.19.1/arts/openai2/_core/chat_in_cmd.py
--rw-r--r--   0        0        0     6925 2024-04-07 02:46:07.780076 arts-2024.4.19.1/arts/openai2/_core/group_chat.py
--rw-r--r--   0        0        0       99 2024-03-05 23:28:04.263728 arts-2024.4.19.1/arts/openai2/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.19.1/arts/openai2/licenses/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 arts-2024.4.19.1/arts/openai2/licenses/openai/LICENSE
--rw-r--r--   0        0        0      204 2024-04-07 03:59:45.705745 arts-2024.4.19.1/arts/openai2/openai2.py
--rw-r--r--   0        0        0      804 2024-04-13 08:15:29.737274 arts-2024.4.19.1/arts/openai2/pyproject.toml
--rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.19.1/arts/skybox/Copyright
--rw-r--r--   0        0        0      735 2024-02-25 06:24:00.741491 arts-2024.4.19.1/arts/skybox/README.md
--rw-r--r--   0        0        0      321 2024-04-13 08:32:12.081508 arts-2024.4.19.1/arts/skybox/pyproject.toml
--rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.19.1/arts/skybox/skybox/Copyright
--rw-r--r--   0        0        0      156 2024-02-25 06:24:00.741491 arts-2024.4.19.1/arts/skybox/skybox/__init__.py
--rw-r--r--   0        0        0    12359 2024-04-13 09:08:11.529449 arts-2024.4.19.1/arts/skybox/skybox/files_hashes
--rw-r--r--   0        0        0       44 2023-12-19 10:10:36.391618 arts-2024.4.19.1/arts/thoughts/2022/现代工人的螺丝钉处境/art.json
--rw-r--r--   0        0        0     1374 2024-01-16 22:36:30.326371 arts-2024.4.19.1/arts/thoughts/2022/现代工人的螺丝钉处境/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.542208 arts-2024.4.19.1/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/art.json
--rw-r--r--   0        0        0     1346 2024-01-30 04:04:01.359662 arts-2024.4.19.1/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.562268 arts-2024.4.19.1/arts/thoughts/2023/专利是个公平的赛道/art.json
--rw-r--r--   0        0        0     1340 2024-03-27 02:41:37.370555 arts-2024.4.19.1/arts/thoughts/2023/专利是个公平的赛道/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.547209 arts-2024.4.19.1/arts/thoughts/2023/事情的真实性是由度的/art.json
--rw-r--r--   0        0        0     1001 2024-01-16 22:36:30.329386 arts-2024.4.19.1/arts/thoughts/2023/事情的真实性是由度的/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.556244 arts-2024.4.19.1/arts/thoughts/2023/人无法摆脱兽性/art.json
--rw-r--r--   0        0        0     1659 2024-01-16 22:36:30.330406 arts-2024.4.19.1/arts/thoughts/2023/人无法摆脱兽性/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.551211 arts-2024.4.19.1/arts/thoughts/2023/什么是极端？/art.json
--rw-r--r--   0        0        0      884 2024-01-16 22:36:30.330406 arts-2024.4.19.1/arts/thoughts/2023/什么是极端？/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.541243 arts-2024.4.19.1/arts/thoughts/2023/保护好人/art.json
--rw-r--r--   0        0        0      802 2024-01-16 22:36:30.331373 arts-2024.4.19.1/arts/thoughts/2023/保护好人/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.554209 arts-2024.4.19.1/arts/thoughts/2023/只筛选，不教化/art.json
--rw-r--r--   0        0        0      853 2024-01-16 22:36:30.331373 arts-2024.4.19.1/arts/thoughts/2023/只筛选，不教化/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.549209 arts-2024.4.19.1/arts/thoughts/2023/喊高考加油是刷存在感/art.json
--rw-r--r--   0        0        0     1047 2024-01-16 22:36:30.332406 arts-2024.4.19.1/arts/thoughts/2023/喊高考加油是刷存在感/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.552210 arts-2024.4.19.1/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/art.json
--rw-r--r--   0        0        0     1630 2024-01-16 22:36:30.333372 arts-2024.4.19.1/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.553243 arts-2024.4.19.1/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/art.json
--rw-r--r--   0        0        0     2475 2024-01-30 04:03:34.796607 arts-2024.4.19.1/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.561243 arts-2024.4.19.1/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/art.json
--rw-r--r--   0        0        0      833 2024-01-18 01:51:26.994040 arts-2024.4.19.1/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.545246 arts-2024.4.19.1/arts/thoughts/2023/想去国外了解自己/art.json
--rw-r--r--   0        0        0      966 2024-01-16 22:36:30.335371 arts-2024.4.19.1/arts/thoughts/2023/想去国外了解自己/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.548245 arts-2024.4.19.1/arts/thoughts/2023/现代化的分工合作机制/art.json
--rw-r--r--   0        0        0     1668 2024-01-16 22:36:30.335371 arts-2024.4.19.1/arts/thoughts/2023/现代化的分工合作机制/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.544210 arts-2024.4.19.1/arts/thoughts/2023/用理性处理简单的事情/art.json
--rw-r--r--   0        0        0     1587 2024-01-16 22:36:30.336371 arts-2024.4.19.1/arts/thoughts/2023/用理性处理简单的事情/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.557226 arts-2024.4.19.1/arts/thoughts/2023/真正的问题无法通过花招解决/art.json
--rw-r--r--   0        0        0      977 2024-01-16 22:36:30.336371 arts-2024.4.19.1/arts/thoughts/2023/真正的问题无法通过花招解决/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.560208 arts-2024.4.19.1/arts/thoughts/2023/艺术本天成，媒介偶显之/art.json
--rw-r--r--   0        0        0      629 2024-01-16 22:36:30.337410 arts-2024.4.19.1/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html
--rw-r--r--   0        0        0       44 2023-12-19 10:11:02.558244 arts-2024.4.19.1/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/art.json
--rw-r--r--   0        0        0     1168 2024-01-16 22:36:30.338372 arts-2024.4.19.1/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html
--rw-r--r--   0        0        0       44 2024-01-13 21:13:40.122707 arts-2024.4.19.1/arts/thoughts/2024/不要害怕犯错/art.json
--rw-r--r--   0        0        0      698 2024-01-16 22:36:30.339373 arts-2024.4.19.1/arts/thoughts/2024/不要害怕犯错/index.html
--rw-r--r--   0        0        0       44 2024-01-01 14:23:12.130009 arts-2024.4.19.1/arts/thoughts/2024/新年题诗/art.json
--rw-r--r--   0        0        0     1152 2024-01-18 06:19:08.705581 arts-2024.4.19.1/arts/thoughts/2024/新年题诗/index.html
--rw-r--r--   0        0        0       44 2024-01-03 04:10:15.709103 arts-2024.4.19.1/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/art.json
--rw-r--r--   0        0        0     1270 2024-01-16 22:36:30.341372 arts-2024.4.19.1/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html
--rw-r--r--   0        0        0       44 2024-03-24 15:35:39.622105 arts-2024.4.19.1/arts/thoughts/2024/编程语言的进化/art.json
--rw-r--r--   0        0        0     1022 2024-03-24 16:22:12.389078 arts-2024.4.19.1/arts/thoughts/2024/编程语言的进化/example.html
--rw-r--r--   0        0        0     1520 2024-03-25 03:53:51.266590 arts-2024.4.19.1/arts/thoughts/2024/编程语言的进化/index.html
--rw-r--r--   0        0        0       44 2024-01-30 04:08:51.850343 arts-2024.4.19.1/arts/thoughts/2024/萝莉岛事件引发的信任危机/art.json
--rw-r--r--   0        0        0     1077 2024-01-30 04:15:45.681734 arts-2024.4.19.1/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html
--rw-r--r--   0        0        0       44 2024-01-18 06:20:18.873404 arts-2024.4.19.1/arts/thoughts/2024/霍金去萝莉岛干嘛了/art.json
--rw-r--r--   0        0        0     1174 2024-01-18 06:24:05.339876 arts-2024.4.19.1/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html
--rw-r--r--   0        0        0      103 2024-03-03 07:12:46.987154 arts-2024.4.19.1/arts/tutorials/150-操作MySQL/art.json
--rw-r--r--   0        0        0      103 2024-03-06 00:50:30.486267 arts-2024.4.19.1/arts/tutorials/225-操作MongoDB/art.json
--rw-r--r--   0        0        0      146 2024-02-25 14:11:14.480558 arts-2024.4.19.1/arts/tutorials/300-开发桌面GUI应用/art.json
--rw-r--r--   0        0        0      102 2024-04-13 07:55:06.222216 arts-2024.4.19.1/arts/tutorials/375-Base95编码/art.json
--rw-r--r--   0        0        0      103 2024-02-18 14:43:25.042841 arts-2024.4.19.1/arts/tutorials/450-对接ChatGPT/art.json
--rw-r--r--   0        0        0      122 2024-03-22 15:10:08.573597 arts-2024.4.19.1/arts/tutorials/525-时间模块/art.json
--rw-r--r--   0        0        0      100 2024-03-06 01:01:25.689741 arts-2024.4.19.1/arts/tutorials/562-面向对象数据库/art.json
--rw-r--r--   0        0        0     3415 2023-12-20 10:09:07.822297 arts-2024.4.19.1/arts/tutorials/600-用37行代码实现AI五子棋/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:14:03.255370 arts-2024.4.19.1/arts/tutorials/600-用37行代码实现AI五子棋/art.json
--rw-r--r--   0        0        0     8070 2024-02-25 05:45:21.624081 arts-2024.4.19.1/arts/tutorials/750-正则表达式/README.md
--rw-r--r--   0        0        0       44 2023-12-19 10:13:55.412792 arts-2024.4.19.1/arts/tutorials/750-正则表达式/art.json
--rw-r--r--   0        0        0       44 2024-01-30 03:46:52.790397 arts-2024.4.19.1/arts/videos/200-秦时明月[项羽]·谪居/art.json
--rw-r--r--   0        0        0       44 2023-12-19 10:07:05.944886 arts-2024.4.19.1/arts/videos/400-李连杰[霍元甲]·兰亭序/art.json
--rw-r--r--   0        0        0       44 2023-12-19 10:07:05.933448 arts-2024.4.19.1/arts/videos/600-楚门的世界·五月雨/art.json
--rw-r--r--   0        0        0       44 2024-01-05 13:31:13.729378 arts-2024.4.19.1/arts/videos/800-AI是这样画包拯的/art.json
--rw-r--r--   0        0        0      527 2024-04-19 11:09:12.547666 arts-2024.4.19.1/pyproject.toml
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 arts-2024.4.19.1/PKG-INFO
+-rw-r--r--   0        0        0     2175 2023-12-20 10:09:43.709218 arts-2024.4.22/.gitignore
+-rw-r--r--   0        0        0       46 2024-03-10 10:13:06.948005 arts-2024.4.22/README.md
+-rw-r--r--   0        0        0      317 2024-02-22 12:02:36.224046 arts-2024.4.22/arts/CoolMemory-English/Copyright
+-rw-r--r--   0        0        0    10492 2024-04-12 03:24:43.904296 arts-2024.4.22/arts/CoolMemory-English/README.md
+-rw-r--r--   0        0        0      110 2024-03-06 00:07:28.301653 arts-2024.4.22/arts/CoolMemory-English/art.json
+-rw-r--r--   0        0        0      393 2023-12-10 08:00:44.000000 arts-2024.4.22/arts/CoolMemory-English/licenses/README.md
+-rw-r--r--   0        0        0     1586 2023-12-10 08:00:44.000000 arts-2024.4.22/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE
+-rw-r--r--   0        0        0    11550 2023-12-10 08:00:44.000000 arts-2024.4.22/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE
+-rw-r--r--   0        0        0    32825 2023-12-10 08:00:44.000000 arts-2024.4.22/arts/CoolMemory-English/licenses/licenses/Python/LICENSE
+-rw-r--r--   0        0        0     2987 2023-12-10 08:00:44.000000 arts-2024.4.22/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE
+-rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.22/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE
+-rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.22/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE
+-rw-r--r--   0        0        0      106 2024-03-31 10:18:29.252509 arts-2024.4.22/arts/WeChat-Art-Museum/art.json
+-rw-r--r--   0        0        0    53616 2024-04-13 08:11:29.182384 arts-2024.4.22/arts/WeChat-Art-Museum/index.html
+-rw-r--r--   0        0        0        0 2024-02-22 15:47:26.927352 arts-2024.4.22/arts/__init__.py
+-rw-r--r--   0        0        0     3088 2023-09-24 08:08:30.000000 arts-2024.4.22/arts/articles/010-赚钱宝典/010-财富的本质/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:01:11.532367 arts-2024.4.22/arts/articles/010-赚钱宝典/010-财富的本质/art.json
+-rw-r--r--   0        0        0     1681 2023-12-20 10:09:07.827303 arts-2024.4.22/arts/articles/010-赚钱宝典/020-商业价值/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:01:11.533332 arts-2024.4.22/arts/articles/010-赚钱宝典/020-商业价值/art.json
+-rw-r--r--   0        0        0     3552 2023-12-22 07:27:54.636897 arts-2024.4.22/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md
+-rw-r--r--   0        0        0       44 2023-12-22 07:26:00.584312 arts-2024.4.22/arts/articles/010-赚钱宝典/030-财富稳定型社会/art.json
+-rw-r--r--   0        0        0     1812 2024-01-02 20:05:02.520382 arts-2024.4.22/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md
+-rw-r--r--   0        0        0       44 2024-01-02 20:46:41.567445 arts-2024.4.22/arts/articles/075-追英赶美/300-产业升级与失业潮/art.json
+-rw-r--r--   0        0        0     1253 2024-01-18 01:49:14.297346 arts-2024.4.22/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md
+-rw-r--r--   0        0        0       44 2024-01-02 20:47:04.916014 arts-2024.4.22/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/art.json
+-rw-r--r--   0        0        0     1559 2023-11-15 13:45:10.000000 arts-2024.4.22/arts/articles/150-小民参政/300-广义的民主/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:02:18.547561 arts-2024.4.22/arts/articles/150-小民参政/300-广义的民主/art.json
+-rw-r--r--   0        0        0     3056 2024-04-15 06:41:13.052262 arts-2024.4.22/arts/articles/150-小民参政/450-我们处于史上最好的时代/README.md
+-rw-r--r--   0        0        0       44 2024-04-14 07:59:47.314020 arts-2024.4.22/arts/articles/150-小民参政/450-我们处于史上最好的时代/art.json
+-rw-r--r--   0        0        0     1499 2023-10-24 11:49:00.000000 arts-2024.4.22/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:02:18.545561 arts-2024.4.22/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/art.json
+-rw-r--r--   0        0        0     1450 2023-11-05 04:22:04.000000 arts-2024.4.22/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.648073 arts-2024.4.22/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/art.json
+-rw-r--r--   0        0        0     3278 2024-02-25 10:11:51.363950 arts-2024.4.22/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.644190 arts-2024.4.22/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/art.json
+-rw-r--r--   0        0        0     1265 2024-03-28 16:30:38.111960 arts-2024.4.22/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.645220 arts-2024.4.22/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/art.json
+-rw-r--r--   0        0        0     1135 2024-03-04 05:13:36.283230 arts-2024.4.22/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:03:07.647184 arts-2024.4.22/arts/articles/300-批判那些伪文艺/800-务实与务虚/art.json
+-rw-r--r--   0        0        0     2095 2024-01-18 01:48:33.751985 arts-2024.4.22/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.900873 arts-2024.4.22/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/art.json
+-rw-r--r--   0        0        0     1668 2023-11-05 03:35:50.000000 arts-2024.4.22/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.909872 arts-2024.4.22/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/art.json
+-rw-r--r--   0        0        0     1669 2023-11-15 13:41:24.000000 arts-2024.4.22/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.903896 arts-2024.4.22/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/art.json
+-rw-r--r--   0        0        0     1906 2023-12-27 20:37:35.730568 arts-2024.4.22/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.899872 arts-2024.4.22/arts/articles/450-万象思考/200-人工智能会不会统治人类？/art.json
+-rw-r--r--   0        0        0     1154 2023-11-05 02:49:06.000000 arts-2024.4.22/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.907909 arts-2024.4.22/arts/articles/450-万象思考/250-忒修斯之船悖论/art.json
+-rw-r--r--   0        0        0     3155 2023-12-27 20:37:10.901781 arts-2024.4.22/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md
+-rw-r--r--   0        0        0       44 2024-01-05 13:23:02.578368 arts-2024.4.22/arts/articles/450-万象思考/300-有无相生，难易相成的启发/art.json
+-rw-r--r--   0        0        0     1354 2023-11-05 03:42:52.000000 arts-2024.4.22/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md
+-rw-r--r--   0        0        0       44 2024-01-05 13:30:30.884939 arts-2024.4.22/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/art.json
+-rw-r--r--   0        0        0     1123 2023-09-10 18:11:18.000000 arts-2024.4.22/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.906885 arts-2024.4.22/arts/articles/450-万象思考/500-人们为什么希望拥有后代/art.json
+-rw-r--r--   0        0        0      708 2023-12-27 20:36:45.425482 arts-2024.4.22/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.904897 arts-2024.4.22/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/art.json
+-rw-r--r--   0        0        0     5024 2024-04-19 10:28:44.045083 arts-2024.4.22/arts/articles/450-万象思考/700-堕胎自由权/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.901873 arts-2024.4.22/arts/articles/450-万象思考/700-堕胎自由权/art.json
+-rw-r--r--   0        0        0     3701 2023-11-15 13:30:02.000000 arts-2024.4.22/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:00.910899 arts-2024.4.22/arts/articles/450-万象思考/800-人人平等是个伪概念/art.json
+-rw-r--r--   0        0        0     3385 2023-12-27 20:36:19.402593 arts-2024.4.22/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.414383 arts-2024.4.22/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/art.json
+-rw-r--r--   0        0        0     2466 2024-02-25 10:07:00.576902 arts-2024.4.22/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.399805 arts-2024.4.22/arts/articles/600-时空猜想/400-我们可能处在人造世界/art.json
+-rw-r--r--   0        0        0     3007 2023-11-04 19:08:36.000000 arts-2024.4.22/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.412423 arts-2024.4.22/arts/articles/600-时空猜想/600-占卜真的存在吗？/art.json
+-rw-r--r--   0        0        0     2630 2023-11-04 19:15:30.000000 arts-2024.4.22/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:21.411378 arts-2024.4.22/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/art.json
+-rw-r--r--   0        0        0     2038 2023-12-28 02:10:43.748193 arts-2024.4.22/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md
+-rw-r--r--   0        0        0       44 2023-12-28 02:02:17.049897 arts-2024.4.22/arts/articles/700-论时事/300-那些年，我们经历过的历史/art.json
+-rw-r--r--   0        0        0     1742 2024-01-13 20:46:22.292355 arts-2024.4.22/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:04:35.958057 arts-2024.4.22/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/art.json
+-rw-r--r--   0        0        0     7343 2023-06-23 06:29:18.000000 arts-2024.4.22/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:05:12.312457 arts-2024.4.22/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/art.json
+-rw-r--r--   0        0        0     1652 2023-06-23 06:48:36.000000 arts-2024.4.22/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:05:34.053435 arts-2024.4.22/arts/articles/800-小说/600-一念天堂/050-被绑架/art.json
+-rw-r--r--   0        0        0    11275 2024-04-13 03:33:01.837811 arts-2024.4.22/arts/base95/LICENSE
+-rw-r--r--   0        0        0     2677 2024-04-19 10:45:27.323930 arts-2024.4.22/arts/base95/README.md
+-rw-r--r--   0        0        0       63 2024-04-19 09:19:32.694427 arts-2024.4.22/arts/base95/__init__.py
+-rw-r--r--   0        0        0     3568 2024-04-19 11:05:40.541843 arts-2024.4.22/arts/base95/_core.py
+-rw-r--r--   0        0        0       98 2024-04-13 08:02:33.643534 arts-2024.4.22/arts/base95/art.json
+-rw-r--r--   0        0        0       74 2024-04-19 09:19:40.646468 arts-2024.4.22/arts/base95/base95.py
+-rw-r--r--   0        0        0      672 2024-04-21 08:12:26.278708 arts-2024.4.22/arts/base95/pyproject.toml
+-rw-r--r--   0        0        0    11283 2024-02-22 12:02:36.224046 arts-2024.4.22/arts/cooltypes/LICENSE
+-rw-r--r--   0        0        0      293 2024-03-22 15:18:30.564599 arts-2024.4.22/arts/cooltypes/__init__.py
+-rw-r--r--   0        0        0     1542 2024-03-31 09:40:29.228723 arts-2024.4.22/arts/cooltypes/envname/README.md
+-rw-r--r--   0        0        0       62 2024-02-23 04:28:30.402332 arts-2024.4.22/arts/cooltypes/envname/__init__.py
+-rw-r--r--   0        0        0      447 2024-04-08 07:02:42.471320 arts-2024.4.22/arts/cooltypes/envname/_core.py
+-rw-r--r--   0        0        0      548 2024-04-08 07:01:42.600503 arts-2024.4.22/arts/cooltypes/moduledb/README.md
+-rw-r--r--   0        0        0       32 2024-02-23 04:03:44.487797 arts-2024.4.22/arts/cooltypes/moduledb/__init__.py
+-rw-r--r--   0        0        0     3515 2024-04-08 06:57:45.544745 arts-2024.4.22/arts/cooltypes/moduledb/_core.py
+-rw-r--r--   0        0        0        0 2024-03-11 20:20:36.445694 arts-2024.4.22/arts/cooltypes/modules/coolstr/__init__.py
+-rw-r--r--   0        0        0     2181 2024-03-22 15:28:12.579126 arts-2024.4.22/arts/cooltypes/modules/coolstr/_core.py
+-rw-r--r--   0        0        0     3316 2024-03-31 09:40:29.228723 arts-2024.4.22/arts/cooltypes/modules/cooltime/README.md
+-rw-r--r--   0        0        0        0 2024-03-11 20:20:55.541076 arts-2024.4.22/arts/cooltypes/modules/cooltime/__init__.py
+-rw-r--r--   0        0        0       44 2024-02-22 10:39:05.460423 arts-2024.4.22/arts/cooltypes/modules/cooltime/_art.json
+-rw-r--r--   0        0        0     3665 2024-03-22 15:09:31.411034 arts-2024.4.22/arts/cooltypes/modules/cooltime/_core.py
+-rw-r--r--   0        0        0     5793 2024-03-22 15:12:37.868753 arts-2024.4.22/arts/cooltypes/modules/rslice/README.md
+-rw-r--r--   0        0        0        0 2024-03-11 20:26:19.316480 arts-2024.4.22/arts/cooltypes/modules/rslice/__init__.py
+-rw-r--r--   0        0        0     2764 2024-04-15 07:46:47.281317 arts-2024.4.22/arts/cooltypes/modules/rslice/_core.py
+-rw-r--r--   0        0        0        0 2024-03-11 20:22:01.981114 arts-2024.4.22/arts/cooltypes/modules/vtype/__init__.py
+-rw-r--r--   0        0        0    10012 2024-04-13 01:46:07.477663 arts-2024.4.22/arts/cooltypes/modules/vtype/_core.py
+-rw-r--r--   0        0        0      238 2024-03-22 14:31:42.101320 arts-2024.4.22/arts/cooltypes/设计.md
+-rw-r--r--   0        0        0    62883 2024-04-22 02:33:42.282104 arts-2024.4.22/arts/index.html
+-rw-r--r--   0        0        0       44 2024-01-16 13:04:45.523107 arts-2024.4.22/arts/life/2018/莆田学院·毕业生留影/art.json
+-rw-r--r--   0        0        0      830 2024-02-12 15:02:22.123647 arts-2024.4.22/arts/life/2018/莆田学院·毕业生留影/index.html
+-rw-r--r--   0        0        0       44 2024-01-17 04:28:07.076300 arts-2024.4.22/arts/life/2019/苏州市虎丘山/art.json
+-rw-r--r--   0        0        0     1233 2024-03-24 16:39:19.059155 arts-2024.4.22/arts/life/2019/苏州市虎丘山/index.html
+-rw-r--r--   0        0        0       44 2024-01-17 03:40:13.294365 arts-2024.4.22/arts/life/2022/泉州市丰泽区·雨后街道/art.json
+-rw-r--r--   0        0        0      969 2024-03-24 16:39:36.018072 arts-2024.4.22/arts/life/2022/泉州市丰泽区·雨后街道/index.html
+-rw-r--r--   0        0        0       44 2024-01-30 05:00:40.402244 arts-2024.4.22/arts/life/2023/更换微信账号了/art.json
+-rw-r--r--   0        0        0      898 2024-04-03 03:17:39.386427 arts-2024.4.22/arts/life/2023/更换微信账号了/index.html
+-rw-r--r--   0        0        0       44 2024-03-24 16:41:15.708702 arts-2024.4.22/arts/life/2024/泉州市承天禅寺/art.json
+-rw-r--r--   0        0        0     1133 2024-03-25 03:52:07.749983 arts-2024.4.22/arts/life/2024/泉州市承天禅寺/index.html
+-rw-r--r--   0        0        0    11276 2024-02-22 12:02:36.224046 arts-2024.4.22/arts/miumapp/LICENSE
+-rw-r--r--   0        0        0     5762 2024-03-31 09:40:29.228723 arts-2024.4.22/arts/miumapp/README.md
+-rw-r--r--   0        0        0       36 2024-02-12 15:08:38.569224 arts-2024.4.22/arts/miumapp/__init__.py
+-rw-r--r--   0        0        0     7645 2024-04-12 04:07:11.111023 arts-2024.4.22/arts/miumapp/_core.py
+-rw-r--r--   0        0        0      111 2024-03-05 23:26:53.659150 arts-2024.4.22/arts/miumapp/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.22/arts/miumapp/licenses/README.md
+-rw-r--r--   0        0        0     1166 2023-12-10 08:00:44.000000 arts-2024.4.22/arts/miumapp/licenses/pyppeteer/LICENSE
+-rw-r--r--   0        0        0    11560 2023-12-10 08:00:44.000000 arts-2024.4.22/arts/miumapp/licenses/tornado/LICENSE
+-rw-r--r--   0        0        0       48 2024-02-12 15:15:42.556195 arts-2024.4.22/arts/miumapp/miumapp/__init__.py
+-rw-r--r--   0        0        0     4657 2024-02-22 17:30:50.375647 arts-2024.4.22/arts/miumapp/miumapp/demo.html
+-rw-r--r--   0        0        0     1241 2024-03-25 04:09:36.827762 arts-2024.4.22/arts/miumapp/miumapp/demo.py
+-rw-r--r--   0        0        0      644 2024-04-13 08:19:45.878790 arts-2024.4.22/arts/miumapp/pyproject.toml
+-rw-r--r--   0        0        0    11273 2024-03-02 20:20:55.781363 arts-2024.4.22/arts/oodb/LICENSE
+-rw-r--r--   0        0        0    22563 2024-03-31 09:40:29.216952 arts-2024.4.22/arts/oodb/README.md
+-rw-r--r--   0        0        0       44 2024-03-06 00:36:04.879589 arts-2024.4.22/arts/oodb/__init__.py
+-rw-r--r--   0        0        0    19029 2024-04-19 10:29:59.567475 arts-2024.4.22/arts/oodb/_core.py
+-rw-r--r--   0        0        0       99 2024-03-06 01:01:05.433633 arts-2024.4.22/arts/oodb/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.22/arts/oodb/licenses/README.md
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.22/arts/oodb/licenses/pymongo/LICENSE
+-rw-r--r--   0        0        0       53 2024-03-06 00:36:04.879589 arts-2024.4.22/arts/oodb/oodb.py
+-rw-r--r--   0        0        0      627 2024-04-13 08:20:16.552792 arts-2024.4.22/arts/oodb/pyproject.toml
+-rw-r--r--   0        0        0    11281 2024-03-03 07:09:08.518004 arts-2024.4.22/arts/oomongo/LICENSE
+-rw-r--r--   0        0        0    17439 2024-03-31 09:40:29.227707 arts-2024.4.22/arts/oomongo/README.md
+-rw-r--r--   0        0        0       49 2024-03-05 08:01:41.054010 arts-2024.4.22/arts/oomongo/__init__.py
+-rw-r--r--   0        0        0    27613 2024-04-15 07:46:47.281317 arts-2024.4.22/arts/oomongo/_core.py
+-rw-r--r--   0        0        0       92 2024-03-06 00:50:10.273786 arts-2024.4.22/arts/oomongo/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.22/arts/oomongo/licenses/README.md
+-rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 arts-2024.4.22/arts/oomongo/licenses/motor/LICENSE
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:26.000000 arts-2024.4.22/arts/oomongo/licenses/pymongo/LICENSE
+-rw-r--r--   0        0        0       61 2024-03-05 08:01:41.059008 arts-2024.4.22/arts/oomongo/oomongo.py
+-rw-r--r--   0        0        0      564 2024-04-13 08:20:16.553795 arts-2024.4.22/arts/oomongo/pyproject.toml
+-rw-r--r--   0        0        0    11281 2024-03-03 07:10:17.933453 arts-2024.4.22/arts/oomysql/LICENSE
+-rw-r--r--   0        0        0    17139 2024-03-31 09:40:29.228723 arts-2024.4.22/arts/oomysql/README.md
+-rw-r--r--   0        0        0       45 2024-03-05 08:02:05.322948 arts-2024.4.22/arts/oomysql/__init__.py
+-rw-r--r--   0        0        0    35301 2024-04-15 07:46:47.271326 arts-2024.4.22/arts/oomysql/_core.py
+-rw-r--r--   0        0        0       90 2024-03-06 00:10:16.490984 arts-2024.4.22/arts/oomysql/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.22/arts/oomysql/licenses/README.md
+-rw-r--r--   0        0        0     1070 2022-05-08 19:03:56.000000 arts-2024.4.22/arts/oomysql/licenses/aiomysql/LICENSE
+-rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 arts-2024.4.22/arts/oomysql/licenses/pymysql/LICENSE
+-rw-r--r--   0        0        0       57 2024-03-05 08:02:05.335929 arts-2024.4.22/arts/oomysql/oomysql.py
+-rw-r--r--   0        0        0      642 2024-04-13 08:20:16.553795 arts-2024.4.22/arts/oomysql/pyproject.toml
+-rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 arts-2024.4.22/arts/openai2/LICENSE
+-rw-r--r--   0        0        0    13991 2024-04-07 02:46:07.779093 arts-2024.4.22/arts/openai2/README.md
+-rw-r--r--   0        0        0      168 2024-04-07 02:56:58.773363 arts-2024.4.22/arts/openai2/__init__.py
+-rw-r--r--   0        0        0     9858 2024-04-07 03:08:27.254965 arts-2024.4.22/arts/openai2/_core/chat.py
+-rw-r--r--   0        0        0     2286 2024-04-08 06:59:43.786636 arts-2024.4.22/arts/openai2/_core/chat_in_cmd.py
+-rw-r--r--   0        0        0     6925 2024-04-07 02:46:07.780076 arts-2024.4.22/arts/openai2/_core/group_chat.py
+-rw-r--r--   0        0        0       99 2024-03-05 23:28:04.263728 arts-2024.4.22/arts/openai2/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 arts-2024.4.22/arts/openai2/licenses/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 arts-2024.4.22/arts/openai2/licenses/openai/LICENSE
+-rw-r--r--   0        0        0      204 2024-04-07 03:59:45.705745 arts-2024.4.22/arts/openai2/openai2.py
+-rw-r--r--   0        0        0      804 2024-04-13 08:15:29.737274 arts-2024.4.22/arts/openai2/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.22/arts/skybox/Copyright
+-rw-r--r--   0        0        0      735 2024-02-25 06:24:00.741491 arts-2024.4.22/arts/skybox/README.md
+-rw-r--r--   0        0        0      321 2024-04-13 08:32:12.081508 arts-2024.4.22/arts/skybox/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 arts-2024.4.22/arts/skybox/skybox/Copyright
+-rw-r--r--   0        0        0      156 2024-02-25 06:24:00.741491 arts-2024.4.22/arts/skybox/skybox/__init__.py
+-rw-r--r--   0        0        0    12359 2024-04-13 09:08:11.529449 arts-2024.4.22/arts/skybox/skybox/files_hashes
+-rw-r--r--   0        0        0       44 2023-12-19 10:10:36.391618 arts-2024.4.22/arts/thoughts/2022/现代工人的螺丝钉处境/art.json
+-rw-r--r--   0        0        0     1374 2024-01-16 22:36:30.326371 arts-2024.4.22/arts/thoughts/2022/现代工人的螺丝钉处境/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.542208 arts-2024.4.22/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/art.json
+-rw-r--r--   0        0        0     1346 2024-01-30 04:04:01.359662 arts-2024.4.22/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.562268 arts-2024.4.22/arts/thoughts/2023/专利是个公平的赛道/art.json
+-rw-r--r--   0        0        0     1340 2024-03-27 02:41:37.370555 arts-2024.4.22/arts/thoughts/2023/专利是个公平的赛道/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.547209 arts-2024.4.22/arts/thoughts/2023/事情的真实性是由度的/art.json
+-rw-r--r--   0        0        0     1001 2024-01-16 22:36:30.329386 arts-2024.4.22/arts/thoughts/2023/事情的真实性是由度的/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.556244 arts-2024.4.22/arts/thoughts/2023/人无法摆脱兽性/art.json
+-rw-r--r--   0        0        0     1659 2024-01-16 22:36:30.330406 arts-2024.4.22/arts/thoughts/2023/人无法摆脱兽性/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.551211 arts-2024.4.22/arts/thoughts/2023/什么是极端？/art.json
+-rw-r--r--   0        0        0      884 2024-01-16 22:36:30.330406 arts-2024.4.22/arts/thoughts/2023/什么是极端？/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.541243 arts-2024.4.22/arts/thoughts/2023/保护好人/art.json
+-rw-r--r--   0        0        0      802 2024-01-16 22:36:30.331373 arts-2024.4.22/arts/thoughts/2023/保护好人/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.554209 arts-2024.4.22/arts/thoughts/2023/只筛选，不教化/art.json
+-rw-r--r--   0        0        0      853 2024-01-16 22:36:30.331373 arts-2024.4.22/arts/thoughts/2023/只筛选，不教化/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.549209 arts-2024.4.22/arts/thoughts/2023/喊高考加油是刷存在感/art.json
+-rw-r--r--   0        0        0     1047 2024-01-16 22:36:30.332406 arts-2024.4.22/arts/thoughts/2023/喊高考加油是刷存在感/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.552210 arts-2024.4.22/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/art.json
+-rw-r--r--   0        0        0     1630 2024-01-16 22:36:30.333372 arts-2024.4.22/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.553243 arts-2024.4.22/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/art.json
+-rw-r--r--   0        0        0     2475 2024-01-30 04:03:34.796607 arts-2024.4.22/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.561243 arts-2024.4.22/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/art.json
+-rw-r--r--   0        0        0      833 2024-01-18 01:51:26.994040 arts-2024.4.22/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.545246 arts-2024.4.22/arts/thoughts/2023/想去国外了解自己/art.json
+-rw-r--r--   0        0        0      966 2024-01-16 22:36:30.335371 arts-2024.4.22/arts/thoughts/2023/想去国外了解自己/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.548245 arts-2024.4.22/arts/thoughts/2023/现代化的分工合作机制/art.json
+-rw-r--r--   0        0        0     1668 2024-01-16 22:36:30.335371 arts-2024.4.22/arts/thoughts/2023/现代化的分工合作机制/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.544210 arts-2024.4.22/arts/thoughts/2023/用理性处理简单的事情/art.json
+-rw-r--r--   0        0        0     1587 2024-01-16 22:36:30.336371 arts-2024.4.22/arts/thoughts/2023/用理性处理简单的事情/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.557226 arts-2024.4.22/arts/thoughts/2023/真正的问题无法通过花招解决/art.json
+-rw-r--r--   0        0        0      977 2024-01-16 22:36:30.336371 arts-2024.4.22/arts/thoughts/2023/真正的问题无法通过花招解决/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.560208 arts-2024.4.22/arts/thoughts/2023/艺术本天成，媒介偶显之/art.json
+-rw-r--r--   0        0        0      629 2024-01-16 22:36:30.337410 arts-2024.4.22/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html
+-rw-r--r--   0        0        0       44 2023-12-19 10:11:02.558244 arts-2024.4.22/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/art.json
+-rw-r--r--   0        0        0     1168 2024-01-16 22:36:30.338372 arts-2024.4.22/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html
+-rw-r--r--   0        0        0       44 2024-01-13 21:13:40.122707 arts-2024.4.22/arts/thoughts/2024/不要害怕犯错/art.json
+-rw-r--r--   0        0        0      698 2024-01-16 22:36:30.339373 arts-2024.4.22/arts/thoughts/2024/不要害怕犯错/index.html
+-rw-r--r--   0        0        0       44 2024-01-01 14:23:12.130009 arts-2024.4.22/arts/thoughts/2024/新年题诗/art.json
+-rw-r--r--   0        0        0     1152 2024-01-18 06:19:08.705581 arts-2024.4.22/arts/thoughts/2024/新年题诗/index.html
+-rw-r--r--   0        0        0       44 2024-01-03 04:10:15.709103 arts-2024.4.22/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/art.json
+-rw-r--r--   0        0        0     1270 2024-01-16 22:36:30.341372 arts-2024.4.22/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html
+-rw-r--r--   0        0        0       44 2024-03-24 15:35:39.622105 arts-2024.4.22/arts/thoughts/2024/编程语言的进化/art.json
+-rw-r--r--   0        0        0     1022 2024-03-24 16:22:12.389078 arts-2024.4.22/arts/thoughts/2024/编程语言的进化/example.html
+-rw-r--r--   0        0        0     1520 2024-03-25 03:53:51.266590 arts-2024.4.22/arts/thoughts/2024/编程语言的进化/index.html
+-rw-r--r--   0        0        0       44 2024-01-30 04:08:51.850343 arts-2024.4.22/arts/thoughts/2024/萝莉岛事件引发的信任危机/art.json
+-rw-r--r--   0        0        0     1077 2024-01-30 04:15:45.681734 arts-2024.4.22/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html
+-rw-r--r--   0        0        0       44 2024-01-18 06:20:18.873404 arts-2024.4.22/arts/thoughts/2024/霍金去萝莉岛干嘛了/art.json
+-rw-r--r--   0        0        0     1174 2024-01-18 06:24:05.339876 arts-2024.4.22/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html
+-rw-r--r--   0        0        0      103 2024-03-03 07:12:46.987154 arts-2024.4.22/arts/tutorials/150-操作MySQL/art.json
+-rw-r--r--   0        0        0      103 2024-03-06 00:50:30.486267 arts-2024.4.22/arts/tutorials/225-操作MongoDB/art.json
+-rw-r--r--   0        0        0      146 2024-02-25 14:11:14.480558 arts-2024.4.22/arts/tutorials/300-开发桌面GUI应用/art.json
+-rw-r--r--   0        0        0      102 2024-04-13 07:55:06.222216 arts-2024.4.22/arts/tutorials/375-Base95编码/art.json
+-rw-r--r--   0        0        0      103 2024-02-18 14:43:25.042841 arts-2024.4.22/arts/tutorials/450-对接ChatGPT/art.json
+-rw-r--r--   0        0        0      122 2024-03-22 15:10:08.573597 arts-2024.4.22/arts/tutorials/525-时间模块/art.json
+-rw-r--r--   0        0        0      100 2024-03-06 01:01:25.689741 arts-2024.4.22/arts/tutorials/562-面向对象数据库/art.json
+-rw-r--r--   0        0        0     3415 2023-12-20 10:09:07.822297 arts-2024.4.22/arts/tutorials/600-用37行代码实现AI五子棋/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:14:03.255370 arts-2024.4.22/arts/tutorials/600-用37行代码实现AI五子棋/art.json
+-rw-r--r--   0        0        0     8070 2024-02-25 05:45:21.624081 arts-2024.4.22/arts/tutorials/750-正则表达式/README.md
+-rw-r--r--   0        0        0       44 2023-12-19 10:13:55.412792 arts-2024.4.22/arts/tutorials/750-正则表达式/art.json
+-rw-r--r--   0        0        0       44 2024-01-30 03:46:52.790397 arts-2024.4.22/arts/videos/200-秦时明月[项羽]·谪居/art.json
+-rw-r--r--   0        0        0       44 2023-12-19 10:07:05.944886 arts-2024.4.22/arts/videos/400-李连杰[霍元甲]·兰亭序/art.json
+-rw-r--r--   0        0        0       44 2023-12-19 10:07:05.933448 arts-2024.4.22/arts/videos/600-楚门的世界·五月雨/art.json
+-rw-r--r--   0        0        0       44 2024-01-05 13:31:13.729378 arts-2024.4.22/arts/videos/800-AI是这样画包拯的/art.json
+-rw-r--r--   0        0        0      525 2024-04-22 02:52:46.157202 arts-2024.4.22/pyproject.toml
+-rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 arts-2024.4.22/PKG-INFO
```

### Comparing `arts-2024.4.19.1/.gitignore` & `arts-2024.4.22/.gitignore`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/CoolMemory-English/README.md` & `arts-2024.4.22/arts/CoolMemory-English/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE` & `arts-2024.4.22/arts/CoolMemory-English/licenses/licenses/Chromium/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE` & `arts-2024.4.22/arts/CoolMemory-English/licenses/licenses/Nuitka/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/CoolMemory-English/licenses/licenses/Python/LICENSE` & `arts-2024.4.22/arts/CoolMemory-English/licenses/licenses/Python/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE` & `arts-2024.4.22/arts/CoolMemory-English/licenses/licenses/pycryptodome/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE` & `arts-2024.4.22/arts/CoolMemory-English/licenses/licenses/pyppeteer/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE` & `arts-2024.4.22/arts/CoolMemory-English/licenses/licenses/tornado/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/WeChat-Art-Museum/index.html` & `arts-2024.4.22/arts/WeChat-Art-Museum/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/010-赚钱宝典/010-财富的本质/README.md` & `arts-2024.4.22/arts/articles/010-赚钱宝典/010-财富的本质/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/010-赚钱宝典/020-商业价值/README.md` & `arts-2024.4.22/arts/articles/010-赚钱宝典/020-商业价值/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md` & `arts-2024.4.22/arts/articles/010-赚钱宝典/030-财富稳定型社会/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md` & `arts-2024.4.22/arts/articles/075-追英赶美/300-产业升级与失业潮/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md` & `arts-2024.4.22/arts/articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/150-小民参政/300-广义的民主/README.md` & `arts-2024.4.22/arts/articles/150-小民参政/300-广义的民主/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/150-小民参政/450-我们处于史上最好的时代/README.md` & `arts-2024.4.22/arts/articles/150-小民参政/450-我们处于史上最好的时代/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md` & `arts-2024.4.22/arts/articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md` & `arts-2024.4.22/arts/articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md` & `arts-2024.4.22/arts/articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md` & `arts-2024.4.22/arts/articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md` & `arts-2024.4.22/arts/articles/300-批判那些伪文艺/800-务实与务虚/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md` & `arts-2024.4.22/arts/articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md` & `arts-2024.4.22/arts/articles/450-万象思考/100-怎么理解「迷信科学」？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md` & `arts-2024.4.22/arts/articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md` & `arts-2024.4.22/arts/articles/450-万象思考/200-人工智能会不会统治人类？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md` & `arts-2024.4.22/arts/articles/450-万象思考/250-忒修斯之船悖论/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md` & `arts-2024.4.22/arts/articles/450-万象思考/300-有无相生，难易相成的启发/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md` & `arts-2024.4.22/arts/articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md` & `arts-2024.4.22/arts/articles/450-万象思考/500-人们为什么希望拥有后代/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md` & `arts-2024.4.22/arts/articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/450-万象思考/700-堕胎自由权/README.md` & `arts-2024.4.22/arts/articles/450-万象思考/700-堕胎自由权/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md` & `arts-2024.4.22/arts/articles/450-万象思考/800-人人平等是个伪概念/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md` & `arts-2024.4.22/arts/articles/600-时空猜想/200-轮回转世真的存在吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md` & `arts-2024.4.22/arts/articles/600-时空猜想/400-我们可能处在人造世界/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md` & `arts-2024.4.22/arts/articles/600-时空猜想/600-占卜真的存在吗？/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md` & `arts-2024.4.22/arts/articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md` & `arts-2024.4.22/arts/articles/700-论时事/300-那些年，我们经历过的历史/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md` & `arts-2024.4.22/arts/articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md` & `arts-2024.4.22/arts/articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md` & `arts-2024.4.22/arts/articles/800-小说/600-一念天堂/050-被绑架/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/base95/LICENSE` & `arts-2024.4.22/arts/base95/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/base95/README.md` & `arts-2024.4.22/arts/base95/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/base95/_core.py` & `arts-2024.4.22/arts/base95/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/base95/pyproject.toml` & `arts-2024.4.22/arts/base95/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/cooltypes/LICENSE` & `arts-2024.4.22/arts/cooltypes/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/cooltypes/envname/README.md` & `arts-2024.4.22/arts/cooltypes/envname/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/cooltypes/moduledb/README.md` & `arts-2024.4.22/arts/cooltypes/moduledb/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/cooltypes/moduledb/_core.py` & `arts-2024.4.22/arts/cooltypes/moduledb/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/cooltypes/modules/coolstr/_core.py` & `arts-2024.4.22/arts/cooltypes/modules/coolstr/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/cooltypes/modules/cooltime/README.md` & `arts-2024.4.22/arts/cooltypes/modules/cooltime/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/cooltypes/modules/cooltime/_core.py` & `arts-2024.4.22/arts/cooltypes/modules/cooltime/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/cooltypes/modules/rslice/README.md` & `arts-2024.4.22/arts/cooltypes/modules/rslice/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/cooltypes/modules/rslice/_core.py` & `arts-2024.4.22/arts/cooltypes/modules/rslice/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/cooltypes/modules/vtype/_core.py` & `arts-2024.4.22/arts/cooltypes/modules/vtype/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/index.html` & `arts-2024.4.22/arts/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -5,42 +5,42 @@
     * {vertical-align:middle; text-decoration:none; position:relative; padding:0; overflow:auto; outline:none; margin:0; font-family:'Chinese Quote', 'Segoe UI', Roboto, RobotoNum, 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', 'Helvetica Neue', Helvetica, Arial, sans-serif; box-sizing:border-box; border-width:0; border-style:solid;}
     .ch_157 {width:100vw; height:100vh; display:block; background-color:white;}
     .ch_186 {display:inline-block; align-self:end;}
     .ch_187 {display:inline-block; align-self:start;}
     .ch_159 {width:100%; padding:0.5rem 0 0 0; height:100%; grid-auto-rows:3rem 1fr; display:inline-grid; background-color:white;}
     .ch_170 {z-index:100; width:100%; min-height:calc(100vh - 3rem - 3.1rem); display:inline-grid; align-content:start;}
     .ch_171 {padding:0 1.25rem; margin:0.5rem 0; justify-content:flex-start; font-weight:500; font-size:1.5rem; display:inline-grid; color:rgb(225, 172, 12);}
-    .ch_174 {width:15rem; text-decoration:none; height:9.27rem; grid-template-rows:1fr auto; display:inline-grid; color:black; background-size:cover; background-color:rgb(255, 237, 195);}
+    .ch_175 {width:15rem; text-decoration:none; height:9.27rem; grid-template-rows:1fr auto; display:inline-grid; color:black; background-size:cover; background-color:rgb(255, 237, 195);}
     .ch_176 {width:100%; text-align:center; line-height:1.5; letter-spacing:0.075em; height:100%; font-size:1.1rem; display:inline-grid; align-items:center;}
     .ch_177 {padding:0 0.25rem 0.25rem 0.25rem; justify-items:end; display:inline-grid; color:green; align-items:end;}
     .ch_178 {width:100%; display:inline-grid;}
     .ch_180 {width:100%; text-shadow:black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em, black 0px -0.1em 0.2em, black 0.1em 0px 0.2em, black 0px 0.1em 0.2em, black -0.1em 0px 0.2em; text-align:center; line-height:1.5; letter-spacing:0.075em; height:100%; font-weight:600; font-size:1.2rem; display:inline-grid; color:white; align-items:center; -webkit-font-smoothing:antialiased;}
     .ch_181 {display:inline-grid;}
-    .ch_184 {row-gap:0.5rem; justify-items:center; justify-content:center; grid-template-rows:auto auto; grid-auto-flow:column; font-weight:500; font-size:1.1rem; display:inline-grid; column-gap:4rem; align-content:center;}
-    body[is_x_screen='False'] .ch_183 {grid-auto-flow:row; display:inline-grid;}
+    .ch_183 {row-gap:0.5rem; justify-items:center; justify-content:center; grid-template-rows:auto auto; grid-auto-flow:column; font-weight:500; font-size:1.1rem; display:inline-grid; column-gap:4rem; align-content:center;}
+    body[is_x_screen='False'] .ch_184 {grid-auto-flow:row; display:inline-grid;}
     body[is_x_screen='False'] .ch_185 {padding:1.5em 0 0 0; display:inline-grid; color:rgb(225, 172, 12);}
-    .ch_161 {z-index:200; white-space:nowrap; scrollbar-width:none; overflow:auto; max-width:100%; margin:0 1.25rem; justify-content:space-between; display:inline-block; background-color:white; -ms-overflow-style:none;}
-    .ch_160::-webkit-scrollbar {display:none;}
+    .ch_160 {z-index:200; white-space:nowrap; scrollbar-width:none; overflow:auto; max-width:100%; margin:0 1.25rem; justify-content:space-between; display:inline-block; background-color:white; -ms-overflow-style:none;}
+    .ch_161::-webkit-scrollbar {display:none;}
     .ch_172 {row-gap:1.5rem; justify-content:center; grid-template-columns:repeat(auto-fill, 15rem); display:inline-grid; column-gap:1.5rem;}
     .ch_163 {padding:0.618em 1em 0.618em 1em; font-size:1rem; border-radius:3em; background-color:transparent;}
     body[is_x_screen='True'] .ch_164:not([is_current_nav="True"]):hover {background-color:rgba(247, 215, 114, 0.45);}
     .ch_162[is_current_nav="True"] {background-color:rgba(247, 215, 114, 1);}
     .ch_168 {white-space:nowrap; scrollbar-width:none; overflow-x:auto; display:inline-block; -ms-overflow-style:none;}
     .ch_166:not(.ch_exec_goto_scrollLeft) {scroll-snap-type:x mandatory;}
     .ch_165::-webkit-scrollbar {display:none;}
     .ch_167 > * {white-space:normal;}
     .ch_169 {width:100%; scroll-snap-align:start; padding:0; overflow:auto; margin:0; height:100%; flex-wrap:wrap; display:inline-flex;}
     .ch_191 {vertical-align:middle;}
-    .ch_190 {vertical-align:baseline; display:inline-block; color:rgba(0, 89, 255, 0.758);}
-    .ch_189:hover {color:rgb(0, 55, 255);}
-    .ch_188:visited {color:rgba(0, 89, 255, 0.758);}
+    .ch_188 {vertical-align:baseline; display:inline-block; color:rgba(0, 89, 255, 0.758);}
+    .ch_190:hover {color:rgb(0, 55, 255);}
+    .ch_189:visited {color:rgba(0, 89, 255, 0.758);}
     .ch_179 {border-width:0.02rem; border-color:rgb(205, 205, 205);}
     .ch_182 {margin:1em 0; justify-self:center; font-weight:500; font-size:1.5rem; color:rgb(225, 172, 12);}
-    .ch_173:hover::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.3);}
-    .ch_175:active::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.5);}
+    .ch_174:hover::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.3);}
+    .ch_173:active::before {width:100%; position:absolute; height:100%; content:''; background-color:rgba(0, 0, 0, 0.5);}
 </style></head>
 <body class='ch_159'>
 <script>
 "use strict";
 
                     if (1 + 1 === 2) {
                         window.ch = new Proxy(
@@ -49,15 +49,15 @@
                         )
                     }
                     else {
                         window.ch = {}
                         console.log('type(ch) is not Map !')
                     }
                 
-</script><div class='ch_160 ch_161' id=ch_127><button class='ch_162 ch_163 ch_164 is_nav' is_current_nav='True'>动态</button><button class='ch_162 ch_163 ch_164 is_nav'>视频</button><button class='ch_162 ch_163 ch_164 is_nav'>文章</button><button class='ch_162 ch_163 ch_164 is_nav'>想法</button><button class='ch_162 ch_163 ch_164 is_nav'>软件</button><button class='ch_162 ch_163 ch_164 is_nav'>Python教程</button><button class='ch_162 ch_163 ch_164 is_nav'>生活</button><button class='ch_162 ch_163 ch_164 is_nav'>自述</button></div><div class='ch_165 ch_166 ch_167 ch_168' id=ch_142><div class='ch_169'><div class='ch_170'><div class='ch_171'>2024-04-14</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/450-我们处于史上最好的时代/README.md' target='_blank'><div class='ch_176'>我们处于史上最好的时代</div><div class='ch_177'>2024-04-14</div></a></div><div class='ch_171'>2024-04-13</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='base95/README.md' target='_blank'><div class='ch_176'>base95<br/>（字节编码方法）</div><div class='ch_177'>2024-04-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/base95' target='_blank'><div class='ch_176'>Base95编码</div><div class='ch_177'>2024-04-13</div></a></div><div class='ch_171'>2024-03-31</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='WeChat-Art-Museum/index.html' target='_blank'><div class='ch_176'>WeChat Art Museum<br/>（微信艺术馆）</div><div class='ch_177'>2024-03-31</div></a></div><div class='ch_171'>2024-03-18</div><iframe class='ch_178' src='life/2024/泉州市承天禅寺/index.html' loading='lazy' id=ch_109></iframe><hr class='ch_179' style="width:100%;"><iframe class='ch_178' src='thoughts/2024/编程语言的进化/index.html' loading='lazy' id=ch_13></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-03-06</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='oodb/README.md' target='_blank'><div class='ch_176'>oodb<br/>（面向对象数据库）</div><div class='ch_177'>2024-03-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oodb' target='_blank'><div class='ch_176'>面向对象数据库</div><div class='ch_177'>2024-03-06</div></a></div><div class='ch_171'>2024-02-13</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='miumapp/README.md' target='_blank'><div class='ch_176'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_177'>2024-02-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/miumapp' target='_blank'><div class='ch_176'>开发跨平台GUI应用</div><div class='ch_177'>2024-02-13</div></a></div><div class='ch_171'>2024-01-30</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/200-秦时明月[项羽]·谪居/README.mp4' target='_blank' style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_180'>秦时明月[项羽]·谪居</div><div class='ch_177'>2024-01-30</div></a></div><div class='ch_171'>2024-01-25</div><iframe class='ch_178' src='thoughts/2024/萝莉岛事件引发的信任危机/index.html' loading='lazy' id=ch_17></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-13</div><iframe class='ch_178' src='thoughts/2024/不要害怕犯错/index.html' loading='lazy' id=ch_21></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-09</div><iframe class='ch_178' src='thoughts/2024/霍金去萝莉岛干嘛了/index.html' loading='lazy' id=ch_25></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-03</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/300-产业升级与失业潮/README.md' target='_blank' style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_180'>产业升级与失业潮</div><div class='ch_177'>2024-01-03</div></a><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md' target='_blank'><div class='ch_176'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_177'>2024-01-03</div></a></div><iframe class='ch_178' src='thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html' loading='lazy' id=ch_29></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-01</div><iframe class='ch_178' src='thoughts/2024/新年题诗/index.html' loading='lazy' id=ch_33></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-12-28</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/300-那些年，我们经历过的历史/README.md' target='_blank'><div class='ch_176'>那些年，我们经历过的历史</div><div class='ch_177'>2023-12-28</div></a></div><div class='ch_171'>2023-12-22</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/030-财富稳定型社会/README.md' target='_blank'><div class='ch_176'>财富稳定型社会</div><div class='ch_177'>2023-12-22</div></a></div><div class='ch_171'>2023-12-11</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='CoolMemory-English/README.md' target='_blank'><div class='ch_176'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_177'>2023-12-11</div></a></div><div class='ch_171'>2023-11-12</div><iframe class='ch_178' src='thoughts/2023/只筛选，不教化/index.html' loading='lazy' id=ch_37></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-11-02</div><iframe class='ch_178' src='thoughts/2023/现代化的分工合作机制/index.html' loading='lazy' id=ch_41></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-10-24</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md' target='_blank'><div class='ch_176'>年轻人不结婚是文明的进步</div><div class='ch_177'>2023-10-24</div></a></div><div class='ch_171'>2023-10-09</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md' target='_blank'><div class='ch_176'>未经他人苦，莫劝他人善？</div><div class='ch_177'>2023-10-09</div></a></div><div class='ch_171'>2023-10-06</div><iframe class='ch_178' src='life/2023/更换微信账号了/index.html' loading='lazy' id=ch_113></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-22</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/020-商业价值/README.md' target='_blank'><div class='ch_176'>商业价值</div><div class='ch_177'>2023-09-22</div></a></div><div class='ch_171'>2023-09-20</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/010-财富的本质/README.md' target='_blank'><div class='ch_176'>财富的本质</div><div class='ch_177'>2023-09-20</div></a></div><div class='ch_171'>2023-09-15</div><iframe class='ch_178' src='thoughts/2023/宣扬出来的宽容是恶的代名词/index.html' loading='lazy' id=ch_45></iframe><hr class='ch_179' style="width:100%;"><iframe class='ch_178' src='thoughts/2023/什么是极端？/index.html' loading='lazy' id=ch_49></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-08</div><iframe class='ch_178' src='thoughts/2023/专利是个公平的赛道/index.html' loading='lazy' id=ch_53></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-18</div><iframe class='ch_178' src='thoughts/2023/真正的问题无法通过花招解决/index.html' loading='lazy' id=ch_57></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-17</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/500-人们为什么希望拥有后代/README.md' target='_blank'><div class='ch_176'>人们为什么希望拥有后代</div><div class='ch_177'>2023-08-17</div></a></div><div class='ch_171'>2023-08-06</div><iframe class='ch_178' src='thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html' loading='lazy' id=ch_61></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-30</div><iframe class='ch_178' src='thoughts/2023/艺术本天成，媒介偶显之/index.html' loading='lazy' id=ch_65></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-20</div><iframe class='ch_178' src='thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html' loading='lazy' id=ch_69></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-19</div><iframe class='ch_178' src='thoughts/2023/ChatGPT动了学阀的蛋糕/index.html' loading='lazy' id=ch_73></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-11</div><iframe class='ch_178' src='thoughts/2023/想去国外了解自己/index.html' loading='lazy' id=ch_77></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-10</div><iframe class='ch_178' src='thoughts/2023/人无法摆脱兽性/index.html' loading='lazy' id=ch_81></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-09</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md' target='_blank'><div class='ch_176'>一元官司有意义吗？</div><div class='ch_177'>2023-07-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md' target='_blank'><div class='ch_176'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_177'>2023-07-09</div></a></div><div class='ch_171'>2023-07-06</div><iframe class='ch_178' src='thoughts/2023/保护好人/index.html' loading='lazy' id=ch_85></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-04</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md' target='_blank'><div class='ch_176'>心理学中个案研究有意义吗？</div><div class='ch_177'>2023-07-04</div></a></div><div class='ch_171'>2023-07-01</div><iframe class='ch_178' src='thoughts/2023/用理性处理简单的事情/index.html' loading='lazy' id=ch_89></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-25</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/cooltypes/modules/cooltime' target='_blank'><div class='ch_176'>时间模块</div><div class='ch_177'>2023-06-25</div></a></div><div class='ch_171'>2023-06-19</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='tutorials/750-正则表达式/README.md' target='_blank'><div class='ch_176'>正则表达式</div><div class='ch_177'>2023-06-19</div></a></div><div class='ch_171'>2023-06-18</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md' target='_blank' style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_180'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_177'>2023-06-18</div></a></div><div class='ch_171'>2023-06-09</div><iframe class='ch_178' src='thoughts/2023/事情的真实性是由度的/index.html' loading='lazy' id=ch_93></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-07</div><iframe class='ch_178' src='thoughts/2023/喊高考加油是刷存在感/index.html' loading='lazy' id=ch_97></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-05-26</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md' target='_blank'><div class='ch_176'>万物为什么会遵循着物理定律？</div><div class='ch_177'>2023-05-26</div></a></div><div class='ch_171'>2023-05-13</div><iframe class='ch_178' src='thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html' loading='lazy' id=ch_101></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-03-07</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='openai2/README.md' target='_blank'><div class='ch_176'>openai2<br/>（openai接口封装）</div><div class='ch_177'>2023-03-07</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/openai2' target='_blank'><div class='ch_176'>对接ChatGPT</div><div class='ch_177'>2023-03-07</div></a></div><div class='ch_171'>2023-03-06</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md' target='_blank'><div class='ch_176'>ChatGPT已经有自我意识了</div><div class='ch_177'>2023-03-06</div></a></div><div class='ch_171'>2022-12-31</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/800-务实与务虚/README.md' target='_blank'><div class='ch_176'>务实与务虚</div><div class='ch_177'>2022-12-31</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/800-人人平等是个伪概念/README.md' target='_blank'><div class='ch_176'>人人平等是个伪概念</div><div class='ch_177'>2022-12-31</div></a></div><div class='ch_171'>2022-12-25</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/200-人工智能会不会统治人类？/README.md' target='_blank' style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_180'>人工智能会不会统治人类？</div><div class='ch_177'>2022-12-25</div></a></div><div class='ch_171'>2022-12-16</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/300-广义的民主/README.md' target='_blank' style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_180'>广义的民主</div><div class='ch_177'>2022-12-16</div></a></div><div class='ch_171'>2022-11-25</div><iframe class='ch_178' src='life/2022/泉州市丰泽区·雨后街道/index.html' loading='lazy' id=ch_117></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2022-09-27</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/400-李连杰[霍元甲]·兰亭序/README.mp4' target='_blank' style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_180'>李连杰[霍元甲]·兰亭序</div><div class='ch_177'>2022-09-27</div></a></div><div class='ch_171'>2022-09-21</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/700-堕胎自由权/README.md' target='_blank'><div class='ch_176'>堕胎自由权</div><div class='ch_177'>2022-09-21</div></a></div><div class='ch_171'>2022-09-08</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/600-楚门的世界·五月雨/README.mp4' target='_blank' style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_180'>楚门的世界·五月雨</div><div class='ch_177'>2022-09-08</div></a></div><div class='ch_171'>2022-08-12</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/600-一念天堂/050-被绑架/README.md' target='_blank'><div class='ch_176'>被绑架</div><div class='ch_177'>2022-08-12</div></a></div><div class='ch_171'>2022-08-01</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/100-怎么理解「迷信科学」？/README.md' target='_blank'><div class='ch_176'>怎么理解「迷信科学」？</div><div class='ch_177'>2022-08-01</div></a></div><div class='ch_171'>2022-06-15</div><iframe class='ch_178' src='thoughts/2022/现代工人的螺丝钉处境/index.html' loading='lazy' id=ch_105></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2021-07-28</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/800-AI是这样画包拯的/README.mp4' target='_blank' style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_180'>AI是这样画包拯的</div><div class='ch_177'>2021-07-28</div></a></div><div class='ch_171'>2021-06-11</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md' target='_blank'><div class='ch_176'>“自由意志”其实是“随机意志”</div><div class='ch_177'>2021-06-11</div></a></div><div class='ch_171'>2021-06-10</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/300-有无相生，难易相成的启发/README.md' target='_blank'><div class='ch_176'>有无相生，难易相成的启发</div><div class='ch_177'>2021-06-10</div></a></div><div class='ch_171'>2021-06-09</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/600-占卜真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_180'>占卜真的存在吗？</div><div class='ch_177'>2021-06-09</div></a></div><div class='ch_171'>2021-06-07</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/400-我们可能处在人造世界/README.md' target='_blank'><div class='ch_176'>我们可能处在人造世界</div><div class='ch_177'>2021-06-07</div></a></div><div class='ch_171'>2021-06-06</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='oomongo/README.md' target='_blank'><div class='ch_176'>oomongo<br/>（MongoDB ODM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomongo' target='_blank'><div class='ch_176'>操作MongoDB</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='oomysql/README.md' target='_blank'><div class='ch_176'>oomysql<br/>（MySQL ORM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomysql' target='_blank'><div class='ch_176'>操作MySQL</div><div class='ch_177'>2021-06-06</div></a></div><div class='ch_171'>2021-06-05</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/200-轮回转世真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_180'>轮回转世真的存在吗？</div><div class='ch_177'>2021-06-05</div></a></div><div class='ch_171'>2021-06-03</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md' target='_blank' style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_180'>唯有变化是不变的？</div><div class='ch_177'>2021-06-03</div></a></div><div class='ch_171'>2021-06-01</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/250-忒修斯之船悖论/README.md' target='_blank'><div class='ch_176'>忒修斯之船悖论</div><div class='ch_177'>2021-06-01</div></a></div><div class='ch_171'>2020-12-31</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md' target='_blank'><div class='ch_176'>燕山宝藏 第1章</div><div class='ch_177'>2020-12-31</div></a></div><div class='ch_171'>2019-08-05</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='tutorials/600-用37行代码实现AI五子棋/README.md' target='_blank'><div class='ch_176'>用37行代码实现AI五子棋</div><div class='ch_177'>2019-08-05</div></a></div><div class='ch_171'>2019-05-01</div><iframe class='ch_178' src='life/2019/苏州市虎丘山/index.html' loading='lazy' id=ch_121></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2018-05-28</div><iframe class='ch_178' src='life/2018/莆田学院·毕业生留影/index.html' loading='lazy' id=ch_125></iframe><hr class='ch_179' style="width:100%;"></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>videos</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/200-秦时明月[项羽]·谪居/README.mp4' target='_blank' style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_180'>秦时明月[项羽]·谪居</div><div class='ch_177'>2024-01-30</div></a><a class='ch_173 ch_174 ch_175' href='videos/400-李连杰[霍元甲]·兰亭序/README.mp4' target='_blank' style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_180'>李连杰[霍元甲]·兰亭序</div><div class='ch_177'>2022-09-27</div></a><a class='ch_173 ch_174 ch_175' href='videos/600-楚门的世界·五月雨/README.mp4' target='_blank' style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_180'>楚门的世界·五月雨</div><div class='ch_177'>2022-09-08</div></a><a class='ch_173 ch_174 ch_175' href='videos/800-AI是这样画包拯的/README.mp4' target='_blank' style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_180'>AI是这样画包拯的</div><div class='ch_177'>2021-07-28</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>赚钱宝典</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/010-财富的本质/README.md' target='_blank'><div class='ch_176'>财富的本质</div><div class='ch_177'>2023-09-20</div></a><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/020-商业价值/README.md' target='_blank'><div class='ch_176'>商业价值</div><div class='ch_177'>2023-09-22</div></a><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/030-财富稳定型社会/README.md' target='_blank'><div class='ch_176'>财富稳定型社会</div><div class='ch_177'>2023-12-22</div></a></div><h3 class='ch_182'>追英赶美</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/300-产业升级与失业潮/README.md' target='_blank' style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_180'>产业升级与失业潮</div><div class='ch_177'>2024-01-03</div></a><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md' target='_blank'><div class='ch_176'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_177'>2024-01-03</div></a></div><h3 class='ch_182'>小民参政</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/300-广义的民主/README.md' target='_blank' style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_180'>广义的民主</div><div class='ch_177'>2022-12-16</div></a><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/450-我们处于史上最好的时代/README.md' target='_blank'><div class='ch_176'>我们处于史上最好的时代</div><div class='ch_177'>2024-04-14</div></a><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md' target='_blank'><div class='ch_176'>年轻人不结婚是文明的进步</div><div class='ch_177'>2023-10-24</div></a></div><h3 class='ch_182'>批判那些伪文艺</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md' target='_blank'><div class='ch_176'>一元官司有意义吗？</div><div class='ch_177'>2023-07-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md' target='_blank' style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_180'>唯有变化是不变的？</div><div class='ch_177'>2021-06-03</div></a><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md' target='_blank'><div class='ch_176'>未经他人苦，莫劝他人善？</div><div class='ch_177'>2023-10-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/800-务实与务虚/README.md' target='_blank'><div class='ch_176'>务实与务虚</div><div class='ch_177'>2022-12-31</div></a></div><h3 class='ch_182'>万象思考</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md' target='_blank'><div class='ch_176'>ChatGPT已经有自我意识了</div><div class='ch_177'>2023-03-06</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/100-怎么理解「迷信科学」？/README.md' target='_blank'><div class='ch_176'>怎么理解「迷信科学」？</div><div class='ch_177'>2022-08-01</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md' target='_blank'><div class='ch_176'>心理学中个案研究有意义吗？</div><div class='ch_177'>2023-07-04</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/200-人工智能会不会统治人类？/README.md' target='_blank' style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_180'>人工智能会不会统治人类？</div><div class='ch_177'>2022-12-25</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/250-忒修斯之船悖论/README.md' target='_blank'><div class='ch_176'>忒修斯之船悖论</div><div class='ch_177'>2021-06-01</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/300-有无相生，难易相成的启发/README.md' target='_blank'><div class='ch_176'>有无相生，难易相成的启发</div><div class='ch_177'>2021-06-10</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md' target='_blank'><div class='ch_176'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_177'>2023-07-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/500-人们为什么希望拥有后代/README.md' target='_blank'><div class='ch_176'>人们为什么希望拥有后代</div><div class='ch_177'>2023-08-17</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md' target='_blank'><div class='ch_176'>万物为什么会遵循着物理定律？</div><div class='ch_177'>2023-05-26</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/700-堕胎自由权/README.md' target='_blank'><div class='ch_176'>堕胎自由权</div><div class='ch_177'>2022-09-21</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/800-人人平等是个伪概念/README.md' target='_blank'><div class='ch_176'>人人平等是个伪概念</div><div class='ch_177'>2022-12-31</div></a></div><h3 class='ch_182'>时空猜想</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/200-轮回转世真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_180'>轮回转世真的存在吗？</div><div class='ch_177'>2021-06-05</div></a><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/400-我们可能处在人造世界/README.md' target='_blank'><div class='ch_176'>我们可能处在人造世界</div><div class='ch_177'>2021-06-07</div></a><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/600-占卜真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_180'>占卜真的存在吗？</div><div class='ch_177'>2021-06-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md' target='_blank'><div class='ch_176'>“自由意志”其实是“随机意志”</div><div class='ch_177'>2021-06-11</div></a></div><h3 class='ch_182'>论时事</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/300-那些年，我们经历过的历史/README.md' target='_blank'><div class='ch_176'>那些年，我们经历过的历史</div><div class='ch_177'>2023-12-28</div></a><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md' target='_blank' style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_180'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_177'>2023-06-18</div></a></div><h3 class='ch_182'>小说 / 陆小凤新传</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md' target='_blank'><div class='ch_176'>燕山宝藏 第1章</div><div class='ch_177'>2020-12-31</div></a></div><h3 class='ch_182'>小说 / 一念天堂</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/600-一念天堂/050-被绑架/README.md' target='_blank'><div class='ch_176'>被绑架</div><div class='ch_177'>2022-08-12</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><div class='ch_171'>2024-03-18</div><iframe class='ch_178' src='thoughts/2024/编程语言的进化/index.html' loading='lazy' id=ch_10></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-25</div><iframe class='ch_178' src='thoughts/2024/萝莉岛事件引发的信任危机/index.html' loading='lazy' id=ch_15></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-13</div><iframe class='ch_178' src='thoughts/2024/不要害怕犯错/index.html' loading='lazy' id=ch_19></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-09</div><iframe class='ch_178' src='thoughts/2024/霍金去萝莉岛干嘛了/index.html' loading='lazy' id=ch_23></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-03</div><iframe class='ch_178' src='thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html' loading='lazy' id=ch_27></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-01</div><iframe class='ch_178' src='thoughts/2024/新年题诗/index.html' loading='lazy' id=ch_31></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-11-12</div><iframe class='ch_178' src='thoughts/2023/只筛选，不教化/index.html' loading='lazy' id=ch_35></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-11-02</div><iframe class='ch_178' src='thoughts/2023/现代化的分工合作机制/index.html' loading='lazy' id=ch_39></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-15</div><iframe class='ch_178' src='thoughts/2023/宣扬出来的宽容是恶的代名词/index.html' loading='lazy' id=ch_43></iframe><hr class='ch_179' style="width:100%;"><iframe class='ch_178' src='thoughts/2023/什么是极端？/index.html' loading='lazy' id=ch_47></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-08</div><iframe class='ch_178' src='thoughts/2023/专利是个公平的赛道/index.html' loading='lazy' id=ch_51></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-18</div><iframe class='ch_178' src='thoughts/2023/真正的问题无法通过花招解决/index.html' loading='lazy' id=ch_55></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-06</div><iframe class='ch_178' src='thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html' loading='lazy' id=ch_59></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-30</div><iframe class='ch_178' src='thoughts/2023/艺术本天成，媒介偶显之/index.html' loading='lazy' id=ch_63></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-20</div><iframe class='ch_178' src='thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html' loading='lazy' id=ch_67></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-19</div><iframe class='ch_178' src='thoughts/2023/ChatGPT动了学阀的蛋糕/index.html' loading='lazy' id=ch_71></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-11</div><iframe class='ch_178' src='thoughts/2023/想去国外了解自己/index.html' loading='lazy' id=ch_75></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-10</div><iframe class='ch_178' src='thoughts/2023/人无法摆脱兽性/index.html' loading='lazy' id=ch_79></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-06</div><iframe class='ch_178' src='thoughts/2023/保护好人/index.html' loading='lazy' id=ch_83></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-01</div><iframe class='ch_178' src='thoughts/2023/用理性处理简单的事情/index.html' loading='lazy' id=ch_87></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-09</div><iframe class='ch_178' src='thoughts/2023/事情的真实性是由度的/index.html' loading='lazy' id=ch_91></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-07</div><iframe class='ch_178' src='thoughts/2023/喊高考加油是刷存在感/index.html' loading='lazy' id=ch_95></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-05-13</div><iframe class='ch_178' src='thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html' loading='lazy' id=ch_99></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2022-06-15</div><iframe class='ch_178' src='thoughts/2022/现代工人的螺丝钉处境/index.html' loading='lazy' id=ch_103></iframe><hr class='ch_179' style="width:100%;"></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>software</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='base95/README.md' target='_blank'><div class='ch_176'>base95<br/>（字节编码方法）</div><div class='ch_177'>2024-04-13</div></a><a class='ch_173 ch_174 ch_175' href='CoolMemory-English/README.md' target='_blank'><div class='ch_176'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_177'>2023-12-11</div></a><a class='ch_173 ch_174 ch_175' href='miumapp/README.md' target='_blank'><div class='ch_176'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_177'>2024-02-13</div></a><a class='ch_173 ch_174 ch_175' href='oodb/README.md' target='_blank'><div class='ch_176'>oodb<br/>（面向对象数据库）</div><div class='ch_177'>2024-03-06</div></a><a class='ch_173 ch_174 ch_175' href='oomongo/README.md' target='_blank'><div class='ch_176'>oomongo<br/>（MongoDB ODM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='oomysql/README.md' target='_blank'><div class='ch_176'>oomysql<br/>（MySQL ORM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='openai2/README.md' target='_blank'><div class='ch_176'>openai2<br/>（openai接口封装）</div><div class='ch_177'>2023-03-07</div></a><a class='ch_173 ch_174 ch_175' href='WeChat-Art-Museum/index.html' target='_blank'><div class='ch_176'>WeChat Art Museum<br/>（微信艺术馆）</div><div class='ch_177'>2024-03-31</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>tutorials</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomysql' target='_blank'><div class='ch_176'>操作MySQL</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomongo' target='_blank'><div class='ch_176'>操作MongoDB</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/miumapp' target='_blank'><div class='ch_176'>开发跨平台GUI应用</div><div class='ch_177'>2024-02-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/base95' target='_blank'><div class='ch_176'>Base95编码</div><div class='ch_177'>2024-04-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/openai2' target='_blank'><div class='ch_176'>对接ChatGPT</div><div class='ch_177'>2023-03-07</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/cooltypes/modules/cooltime' target='_blank'><div class='ch_176'>时间模块</div><div class='ch_177'>2023-06-25</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oodb' target='_blank'><div class='ch_176'>面向对象数据库</div><div class='ch_177'>2024-03-06</div></a><a class='ch_173 ch_174 ch_175' href='tutorials/600-用37行代码实现AI五子棋/README.md' target='_blank'><div class='ch_176'>用37行代码实现AI五子棋</div><div class='ch_177'>2019-08-05</div></a><a class='ch_173 ch_174 ch_175' href='tutorials/750-正则表达式/README.md' target='_blank'><div class='ch_176'>正则表达式</div><div class='ch_177'>2023-06-19</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><div class='ch_171'>2024-03-18</div><iframe class='ch_178' src='life/2024/泉州市承天禅寺/index.html' loading='lazy' id=ch_107></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-10-06</div><iframe class='ch_178' src='life/2023/更换微信账号了/index.html' loading='lazy' id=ch_111></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2022-11-25</div><iframe class='ch_178' src='life/2022/泉州市丰泽区·雨后街道/index.html' loading='lazy' id=ch_115></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2019-05-01</div><iframe class='ch_178' src='life/2019/苏州市虎丘山/index.html' loading='lazy' id=ch_119></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2018-05-28</div><iframe class='ch_178' src='life/2018/莆田学院·毕业生留影/index.html' loading='lazy' id=ch_123></iframe><hr class='ch_179' style="width:100%;"></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170' style="align-content:stretch;"><div class='ch_183 ch_184'><div class='ch_185 ch_186'>邮箱</div><div class='ch_187'><a class='ch_188 ch_189 ch_190' href='mailto:lcctoor@outlook.com'>lcctoor@outlook.com</a></div><div class='ch_185 ch_186'>微信</div><div class='ch_187'><img class='ch_191' src='./ip_static/WeChatQRC.jpg' style="max-width:15rem; height:auto;"></div><div class='ch_185 ch_186'>捐赠</div><div class='ch_187'><img class='ch_191' src='./ip_static/DonationQRC-0rmb.jpg' style="max-width:15rem; height:auto;"></div></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div></div>
+</script><div class='ch_160 ch_161' id=ch_127><button class='is_nav ch_162 ch_163 ch_164' is_current_nav='True'>动态</button><button class='is_nav ch_162 ch_163 ch_164'>视频</button><button class='is_nav ch_162 ch_163 ch_164'>文章</button><button class='is_nav ch_162 ch_163 ch_164'>想法</button><button class='is_nav ch_162 ch_163 ch_164'>软件</button><button class='is_nav ch_162 ch_163 ch_164'>Python教程</button><button class='is_nav ch_162 ch_163 ch_164'>生活</button><button class='is_nav ch_162 ch_163 ch_164'>自述</button></div><div class='ch_165 ch_166 ch_167 ch_168' id=ch_142><div class='ch_169'><div class='ch_170'><div class='ch_171'>2024-04-14</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/450-我们处于史上最好的时代/README.md' target='_blank'><div class='ch_176'>我们处于史上最好的时代</div><div class='ch_177'>2024-04-14</div></a></div><div class='ch_171'>2024-04-13</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='base95/README.md' target='_blank'><div class='ch_176'>base95<br/>（字节编码方法）</div><div class='ch_177'>2024-04-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/base95' target='_blank'><div class='ch_176'>Base95编码</div><div class='ch_177'>2024-04-13</div></a></div><div class='ch_171'>2024-03-31</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='WeChat-Art-Museum/index.html' target='_blank'><div class='ch_176'>WeChat Art Museum<br/>（微信艺术馆）</div><div class='ch_177'>2024-03-31</div></a></div><div class='ch_171'>2024-03-18</div><iframe class='ch_178' src='life/2024/泉州市承天禅寺/index.html' loading='lazy' id=ch_109></iframe><hr class='ch_179' style="width:100%;"><iframe class='ch_178' src='thoughts/2024/编程语言的进化/index.html' loading='lazy' id=ch_13></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-03-06</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='oodb/README.md' target='_blank'><div class='ch_176'>oodb<br/>（面向对象数据库）</div><div class='ch_177'>2024-03-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oodb' target='_blank'><div class='ch_176'>面向对象数据库</div><div class='ch_177'>2024-03-06</div></a></div><div class='ch_171'>2024-02-13</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='miumapp/README.md' target='_blank'><div class='ch_176'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_177'>2024-02-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/miumapp' target='_blank'><div class='ch_176'>开发跨平台GUI应用</div><div class='ch_177'>2024-02-13</div></a></div><div class='ch_171'>2024-01-30</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/200-秦时明月[项羽]·谪居/README.mp4' target='_blank' style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_180'>秦时明月[项羽]·谪居</div><div class='ch_177'>2024-01-30</div></a></div><div class='ch_171'>2024-01-25</div><iframe class='ch_178' src='thoughts/2024/萝莉岛事件引发的信任危机/index.html' loading='lazy' id=ch_17></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-13</div><iframe class='ch_178' src='thoughts/2024/不要害怕犯错/index.html' loading='lazy' id=ch_21></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-09</div><iframe class='ch_178' src='thoughts/2024/霍金去萝莉岛干嘛了/index.html' loading='lazy' id=ch_25></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-03</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/300-产业升级与失业潮/README.md' target='_blank' style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_180'>产业升级与失业潮</div><div class='ch_177'>2024-01-03</div></a><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md' target='_blank'><div class='ch_176'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_177'>2024-01-03</div></a></div><iframe class='ch_178' src='thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html' loading='lazy' id=ch_29></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-01</div><iframe class='ch_178' src='thoughts/2024/新年题诗/index.html' loading='lazy' id=ch_33></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-12-28</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/300-那些年，我们经历过的历史/README.md' target='_blank'><div class='ch_176'>那些年，我们经历过的历史</div><div class='ch_177'>2023-12-28</div></a></div><div class='ch_171'>2023-12-22</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/030-财富稳定型社会/README.md' target='_blank'><div class='ch_176'>财富稳定型社会</div><div class='ch_177'>2023-12-22</div></a></div><div class='ch_171'>2023-12-11</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='CoolMemory-English/README.md' target='_blank'><div class='ch_176'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_177'>2023-12-11</div></a></div><div class='ch_171'>2023-11-12</div><iframe class='ch_178' src='thoughts/2023/只筛选，不教化/index.html' loading='lazy' id=ch_37></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-11-02</div><iframe class='ch_178' src='thoughts/2023/现代化的分工合作机制/index.html' loading='lazy' id=ch_41></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-10-24</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md' target='_blank'><div class='ch_176'>年轻人不结婚是文明的进步</div><div class='ch_177'>2023-10-24</div></a></div><div class='ch_171'>2023-10-09</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md' target='_blank'><div class='ch_176'>未经他人苦，莫劝他人善？</div><div class='ch_177'>2023-10-09</div></a></div><div class='ch_171'>2023-10-06</div><iframe class='ch_178' src='life/2023/更换微信账号了/index.html' loading='lazy' id=ch_113></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-22</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/020-商业价值/README.md' target='_blank'><div class='ch_176'>商业价值</div><div class='ch_177'>2023-09-22</div></a></div><div class='ch_171'>2023-09-20</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/010-财富的本质/README.md' target='_blank'><div class='ch_176'>财富的本质</div><div class='ch_177'>2023-09-20</div></a></div><div class='ch_171'>2023-09-15</div><iframe class='ch_178' src='thoughts/2023/宣扬出来的宽容是恶的代名词/index.html' loading='lazy' id=ch_45></iframe><hr class='ch_179' style="width:100%;"><iframe class='ch_178' src='thoughts/2023/什么是极端？/index.html' loading='lazy' id=ch_49></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-08</div><iframe class='ch_178' src='thoughts/2023/专利是个公平的赛道/index.html' loading='lazy' id=ch_53></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-18</div><iframe class='ch_178' src='thoughts/2023/真正的问题无法通过花招解决/index.html' loading='lazy' id=ch_57></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-17</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/500-人们为什么希望拥有后代/README.md' target='_blank'><div class='ch_176'>人们为什么希望拥有后代</div><div class='ch_177'>2023-08-17</div></a></div><div class='ch_171'>2023-08-06</div><iframe class='ch_178' src='thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html' loading='lazy' id=ch_61></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-30</div><iframe class='ch_178' src='thoughts/2023/艺术本天成，媒介偶显之/index.html' loading='lazy' id=ch_65></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-20</div><iframe class='ch_178' src='thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html' loading='lazy' id=ch_69></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-19</div><iframe class='ch_178' src='thoughts/2023/ChatGPT动了学阀的蛋糕/index.html' loading='lazy' id=ch_73></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-11</div><iframe class='ch_178' src='thoughts/2023/想去国外了解自己/index.html' loading='lazy' id=ch_77></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-10</div><iframe class='ch_178' src='thoughts/2023/人无法摆脱兽性/index.html' loading='lazy' id=ch_81></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-09</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md' target='_blank'><div class='ch_176'>一元官司有意义吗？</div><div class='ch_177'>2023-07-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md' target='_blank'><div class='ch_176'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_177'>2023-07-09</div></a></div><div class='ch_171'>2023-07-06</div><iframe class='ch_178' src='thoughts/2023/保护好人/index.html' loading='lazy' id=ch_85></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-04</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md' target='_blank'><div class='ch_176'>心理学中个案研究有意义吗？</div><div class='ch_177'>2023-07-04</div></a></div><div class='ch_171'>2023-07-01</div><iframe class='ch_178' src='thoughts/2023/用理性处理简单的事情/index.html' loading='lazy' id=ch_89></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-25</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/cooltypes/modules/cooltime' target='_blank'><div class='ch_176'>时间模块</div><div class='ch_177'>2023-06-25</div></a></div><div class='ch_171'>2023-06-19</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='tutorials/750-正则表达式/README.md' target='_blank'><div class='ch_176'>正则表达式</div><div class='ch_177'>2023-06-19</div></a></div><div class='ch_171'>2023-06-18</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md' target='_blank' style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_180'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_177'>2023-06-18</div></a></div><div class='ch_171'>2023-06-09</div><iframe class='ch_178' src='thoughts/2023/事情的真实性是由度的/index.html' loading='lazy' id=ch_93></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-07</div><iframe class='ch_178' src='thoughts/2023/喊高考加油是刷存在感/index.html' loading='lazy' id=ch_97></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-05-26</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md' target='_blank'><div class='ch_176'>万物为什么会遵循着物理定律？</div><div class='ch_177'>2023-05-26</div></a></div><div class='ch_171'>2023-05-13</div><iframe class='ch_178' src='thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html' loading='lazy' id=ch_101></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-03-07</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='openai2/README.md' target='_blank'><div class='ch_176'>openai2<br/>（openai接口封装）</div><div class='ch_177'>2023-03-07</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/openai2' target='_blank'><div class='ch_176'>对接ChatGPT</div><div class='ch_177'>2023-03-07</div></a></div><div class='ch_171'>2023-03-06</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md' target='_blank'><div class='ch_176'>ChatGPT已经有自我意识了</div><div class='ch_177'>2023-03-06</div></a></div><div class='ch_171'>2022-12-31</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/800-务实与务虚/README.md' target='_blank'><div class='ch_176'>务实与务虚</div><div class='ch_177'>2022-12-31</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/800-人人平等是个伪概念/README.md' target='_blank'><div class='ch_176'>人人平等是个伪概念</div><div class='ch_177'>2022-12-31</div></a></div><div class='ch_171'>2022-12-25</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/200-人工智能会不会统治人类？/README.md' target='_blank' style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_180'>人工智能会不会统治人类？</div><div class='ch_177'>2022-12-25</div></a></div><div class='ch_171'>2022-12-16</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/300-广义的民主/README.md' target='_blank' style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_180'>广义的民主</div><div class='ch_177'>2022-12-16</div></a></div><div class='ch_171'>2022-11-25</div><iframe class='ch_178' src='life/2022/泉州市丰泽区·雨后街道/index.html' loading='lazy' id=ch_117></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2022-09-27</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/400-李连杰[霍元甲]·兰亭序/README.mp4' target='_blank' style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_180'>李连杰[霍元甲]·兰亭序</div><div class='ch_177'>2022-09-27</div></a></div><div class='ch_171'>2022-09-21</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/700-堕胎自由权/README.md' target='_blank'><div class='ch_176'>堕胎自由权</div><div class='ch_177'>2022-09-21</div></a></div><div class='ch_171'>2022-09-08</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/600-楚门的世界·五月雨/README.mp4' target='_blank' style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_180'>楚门的世界·五月雨</div><div class='ch_177'>2022-09-08</div></a></div><div class='ch_171'>2022-08-12</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/600-一念天堂/050-被绑架/README.md' target='_blank'><div class='ch_176'>被绑架</div><div class='ch_177'>2022-08-12</div></a></div><div class='ch_171'>2022-08-01</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/100-怎么理解「迷信科学」？/README.md' target='_blank'><div class='ch_176'>怎么理解「迷信科学」？</div><div class='ch_177'>2022-08-01</div></a></div><div class='ch_171'>2022-06-15</div><iframe class='ch_178' src='thoughts/2022/现代工人的螺丝钉处境/index.html' loading='lazy' id=ch_105></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2021-07-28</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/800-AI是这样画包拯的/README.mp4' target='_blank' style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_180'>AI是这样画包拯的</div><div class='ch_177'>2021-07-28</div></a></div><div class='ch_171'>2021-06-11</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md' target='_blank'><div class='ch_176'>“自由意志”其实是“随机意志”</div><div class='ch_177'>2021-06-11</div></a></div><div class='ch_171'>2021-06-10</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/300-有无相生，难易相成的启发/README.md' target='_blank'><div class='ch_176'>有无相生，难易相成的启发</div><div class='ch_177'>2021-06-10</div></a></div><div class='ch_171'>2021-06-09</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/600-占卜真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_180'>占卜真的存在吗？</div><div class='ch_177'>2021-06-09</div></a></div><div class='ch_171'>2021-06-07</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/400-我们可能处在人造世界/README.md' target='_blank'><div class='ch_176'>我们可能处在人造世界</div><div class='ch_177'>2021-06-07</div></a></div><div class='ch_171'>2021-06-06</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='oomongo/README.md' target='_blank'><div class='ch_176'>oomongo<br/>（MongoDB ODM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomongo' target='_blank'><div class='ch_176'>操作MongoDB</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='oomysql/README.md' target='_blank'><div class='ch_176'>oomysql<br/>（MySQL ORM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomysql' target='_blank'><div class='ch_176'>操作MySQL</div><div class='ch_177'>2021-06-06</div></a></div><div class='ch_171'>2021-06-05</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/200-轮回转世真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_180'>轮回转世真的存在吗？</div><div class='ch_177'>2021-06-05</div></a></div><div class='ch_171'>2021-06-03</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md' target='_blank' style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_180'>唯有变化是不变的？</div><div class='ch_177'>2021-06-03</div></a></div><div class='ch_171'>2021-06-01</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/250-忒修斯之船悖论/README.md' target='_blank'><div class='ch_176'>忒修斯之船悖论</div><div class='ch_177'>2021-06-01</div></a></div><div class='ch_171'>2020-12-31</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md' target='_blank'><div class='ch_176'>燕山宝藏 第1章</div><div class='ch_177'>2020-12-31</div></a></div><div class='ch_171'>2019-08-05</div><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='tutorials/600-用37行代码实现AI五子棋/README.md' target='_blank'><div class='ch_176'>用37行代码实现AI五子棋</div><div class='ch_177'>2019-08-05</div></a></div><div class='ch_171'>2019-05-01</div><iframe class='ch_178' src='life/2019/苏州市虎丘山/index.html' loading='lazy' id=ch_121></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2018-05-28</div><iframe class='ch_178' src='life/2018/莆田学院·毕业生留影/index.html' loading='lazy' id=ch_125></iframe><hr class='ch_179' style="width:100%;"></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>videos</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='videos/200-秦时明月[项羽]·谪居/README.mp4' target='_blank' style="background-image:url('videos/200-秦时明月[项羽]·谪居/ip_static/cover.jpg');"><div class='ch_180'>秦时明月[项羽]·谪居</div><div class='ch_177'>2024-01-30</div></a><a class='ch_173 ch_174 ch_175' href='videos/400-李连杰[霍元甲]·兰亭序/README.mp4' target='_blank' style="background-image:url('videos/400-李连杰[霍元甲]·兰亭序/ip_static/cover.jpg');"><div class='ch_180'>李连杰[霍元甲]·兰亭序</div><div class='ch_177'>2022-09-27</div></a><a class='ch_173 ch_174 ch_175' href='videos/600-楚门的世界·五月雨/README.mp4' target='_blank' style="background-image:url('videos/600-楚门的世界·五月雨/ip_static/cover.jpeg');"><div class='ch_180'>楚门的世界·五月雨</div><div class='ch_177'>2022-09-08</div></a><a class='ch_173 ch_174 ch_175' href='videos/800-AI是这样画包拯的/README.mp4' target='_blank' style="background-image:url('videos/800-AI是这样画包拯的/ip_static/cover.jpg');"><div class='ch_180'>AI是这样画包拯的</div><div class='ch_177'>2021-07-28</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>赚钱宝典</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/010-财富的本质/README.md' target='_blank'><div class='ch_176'>财富的本质</div><div class='ch_177'>2023-09-20</div></a><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/020-商业价值/README.md' target='_blank'><div class='ch_176'>商业价值</div><div class='ch_177'>2023-09-22</div></a><a class='ch_173 ch_174 ch_175' href='articles/010-赚钱宝典/030-财富稳定型社会/README.md' target='_blank'><div class='ch_176'>财富稳定型社会</div><div class='ch_177'>2023-12-22</div></a></div><h3 class='ch_182'>追英赶美</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/300-产业升级与失业潮/README.md' target='_blank' style="background-image:url('articles/075-追英赶美/300-产业升级与失业潮/ip_static/cover.png');"><div class='ch_180'>产业升级与失业潮</div><div class='ch_177'>2024-01-03</div></a><a class='ch_173 ch_174 ch_175' href='articles/075-追英赶美/600-在ChatGPT冲击下，打造国家级公共知识库迫在眉睫/README.md' target='_blank'><div class='ch_176'>在ChatGPT冲击下，打造国家级公共知识库迫在眉睫</div><div class='ch_177'>2024-01-03</div></a></div><h3 class='ch_182'>小民参政</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/300-广义的民主/README.md' target='_blank' style="background-image:url('articles/150-小民参政/300-广义的民主/ip_static/cover.png');"><div class='ch_180'>广义的民主</div><div class='ch_177'>2022-12-16</div></a><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/450-我们处于史上最好的时代/README.md' target='_blank'><div class='ch_176'>我们处于史上最好的时代</div><div class='ch_177'>2024-04-14</div></a><a class='ch_173 ch_174 ch_175' href='articles/150-小民参政/600-年轻人不结婚是文明的进步/README.md' target='_blank'><div class='ch_176'>年轻人不结婚是文明的进步</div><div class='ch_177'>2023-10-24</div></a></div><h3 class='ch_182'>批判那些伪文艺</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/200-一元官司有意义吗？/README.md' target='_blank'><div class='ch_176'>一元官司有意义吗？</div><div class='ch_177'>2023-07-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/400-唯有变化是不变的？/README.md' target='_blank' style="background-image:url('articles/300-批判那些伪文艺/400-唯有变化是不变的？/ip_static/cover.png');"><div class='ch_180'>唯有变化是不变的？</div><div class='ch_177'>2021-06-03</div></a><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/600-未经他人苦，莫劝他人善？/README.md' target='_blank'><div class='ch_176'>未经他人苦，莫劝他人善？</div><div class='ch_177'>2023-10-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/300-批判那些伪文艺/800-务实与务虚/README.md' target='_blank'><div class='ch_176'>务实与务虚</div><div class='ch_177'>2022-12-31</div></a></div><h3 class='ch_182'>万象思考</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/050-ChatGPT已经有自我意识了/README.md' target='_blank'><div class='ch_176'>ChatGPT已经有自我意识了</div><div class='ch_177'>2023-03-06</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/100-怎么理解「迷信科学」？/README.md' target='_blank'><div class='ch_176'>怎么理解「迷信科学」？</div><div class='ch_177'>2022-08-01</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/150-心理学中个案研究有意义吗？/README.md' target='_blank'><div class='ch_176'>心理学中个案研究有意义吗？</div><div class='ch_177'>2023-07-04</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/200-人工智能会不会统治人类？/README.md' target='_blank' style="background-image:url('articles/450-万象思考/200-人工智能会不会统治人类？/ip_static/cover.png');"><div class='ch_180'>人工智能会不会统治人类？</div><div class='ch_177'>2022-12-25</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/250-忒修斯之船悖论/README.md' target='_blank'><div class='ch_176'>忒修斯之船悖论</div><div class='ch_177'>2021-06-01</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/300-有无相生，难易相成的启发/README.md' target='_blank'><div class='ch_176'>有无相生，难易相成的启发</div><div class='ch_177'>2021-06-10</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/400-熵增都是坏的，熵减都是好的吗？/README.md' target='_blank'><div class='ch_176'>熵增都是坏的，熵减都是好的吗？</div><div class='ch_177'>2023-07-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/500-人们为什么希望拥有后代/README.md' target='_blank'><div class='ch_176'>人们为什么希望拥有后代</div><div class='ch_177'>2023-08-17</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/600-万物为什么会遵循着物理定律？/README.md' target='_blank'><div class='ch_176'>万物为什么会遵循着物理定律？</div><div class='ch_177'>2023-05-26</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/700-堕胎自由权/README.md' target='_blank'><div class='ch_176'>堕胎自由权</div><div class='ch_177'>2022-09-21</div></a><a class='ch_173 ch_174 ch_175' href='articles/450-万象思考/800-人人平等是个伪概念/README.md' target='_blank'><div class='ch_176'>人人平等是个伪概念</div><div class='ch_177'>2022-12-31</div></a></div><h3 class='ch_182'>时空猜想</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/200-轮回转世真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/200-轮回转世真的存在吗？/ip_static/cover.jpg');"><div class='ch_180'>轮回转世真的存在吗？</div><div class='ch_177'>2021-06-05</div></a><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/400-我们可能处在人造世界/README.md' target='_blank'><div class='ch_176'>我们可能处在人造世界</div><div class='ch_177'>2021-06-07</div></a><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/600-占卜真的存在吗？/README.md' target='_blank' style="background-image:url('articles/600-时空猜想/600-占卜真的存在吗？/ip_static/cover.png');"><div class='ch_180'>占卜真的存在吗？</div><div class='ch_177'>2021-06-09</div></a><a class='ch_173 ch_174 ch_175' href='articles/600-时空猜想/800-“自由意志”其实是“随机意志”/README.md' target='_blank'><div class='ch_176'>“自由意志”其实是“随机意志”</div><div class='ch_177'>2021-06-11</div></a></div><h3 class='ch_182'>论时事</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/300-那些年，我们经历过的历史/README.md' target='_blank'><div class='ch_176'>那些年，我们经历过的历史</div><div class='ch_177'>2023-12-28</div></a><a class='ch_173 ch_174 ch_175' href='articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/README.md' target='_blank' style="background-image:url('articles/700-论时事/600-评价在北京工体冲进场的梅西粉丝/ip_static/cover.jpg');"><div class='ch_180'>评价在北京工体冲进场的梅西粉丝</div><div class='ch_177'>2023-06-18</div></a></div><h3 class='ch_182'>小说 / 陆小凤新传</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/300-陆小凤新传/050-燕山宝藏 第1章/README.md' target='_blank'><div class='ch_176'>燕山宝藏 第1章</div><div class='ch_177'>2020-12-31</div></a></div><h3 class='ch_182'>小说 / 一念天堂</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='articles/800-小说/600-一念天堂/050-被绑架/README.md' target='_blank'><div class='ch_176'>被绑架</div><div class='ch_177'>2022-08-12</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><div class='ch_171'>2024-03-18</div><iframe class='ch_178' src='thoughts/2024/编程语言的进化/index.html' loading='lazy' id=ch_10></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-25</div><iframe class='ch_178' src='thoughts/2024/萝莉岛事件引发的信任危机/index.html' loading='lazy' id=ch_15></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-13</div><iframe class='ch_178' src='thoughts/2024/不要害怕犯错/index.html' loading='lazy' id=ch_19></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-09</div><iframe class='ch_178' src='thoughts/2024/霍金去萝莉岛干嘛了/index.html' loading='lazy' id=ch_23></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-03</div><iframe class='ch_178' src='thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html' loading='lazy' id=ch_27></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2024-01-01</div><iframe class='ch_178' src='thoughts/2024/新年题诗/index.html' loading='lazy' id=ch_31></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-11-12</div><iframe class='ch_178' src='thoughts/2023/只筛选，不教化/index.html' loading='lazy' id=ch_35></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-11-02</div><iframe class='ch_178' src='thoughts/2023/现代化的分工合作机制/index.html' loading='lazy' id=ch_39></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-15</div><iframe class='ch_178' src='thoughts/2023/宣扬出来的宽容是恶的代名词/index.html' loading='lazy' id=ch_43></iframe><hr class='ch_179' style="width:100%;"><iframe class='ch_178' src='thoughts/2023/什么是极端？/index.html' loading='lazy' id=ch_47></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-09-08</div><iframe class='ch_178' src='thoughts/2023/专利是个公平的赛道/index.html' loading='lazy' id=ch_51></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-18</div><iframe class='ch_178' src='thoughts/2023/真正的问题无法通过花招解决/index.html' loading='lazy' id=ch_55></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-08-06</div><iframe class='ch_178' src='thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html' loading='lazy' id=ch_59></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-30</div><iframe class='ch_178' src='thoughts/2023/艺术本天成，媒介偶显之/index.html' loading='lazy' id=ch_63></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-20</div><iframe class='ch_178' src='thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html' loading='lazy' id=ch_67></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-19</div><iframe class='ch_178' src='thoughts/2023/ChatGPT动了学阀的蛋糕/index.html' loading='lazy' id=ch_71></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-11</div><iframe class='ch_178' src='thoughts/2023/想去国外了解自己/index.html' loading='lazy' id=ch_75></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-10</div><iframe class='ch_178' src='thoughts/2023/人无法摆脱兽性/index.html' loading='lazy' id=ch_79></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-06</div><iframe class='ch_178' src='thoughts/2023/保护好人/index.html' loading='lazy' id=ch_83></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-07-01</div><iframe class='ch_178' src='thoughts/2023/用理性处理简单的事情/index.html' loading='lazy' id=ch_87></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-09</div><iframe class='ch_178' src='thoughts/2023/事情的真实性是由度的/index.html' loading='lazy' id=ch_91></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-06-07</div><iframe class='ch_178' src='thoughts/2023/喊高考加油是刷存在感/index.html' loading='lazy' id=ch_95></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-05-13</div><iframe class='ch_178' src='thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html' loading='lazy' id=ch_99></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2022-06-15</div><iframe class='ch_178' src='thoughts/2022/现代工人的螺丝钉处境/index.html' loading='lazy' id=ch_103></iframe><hr class='ch_179' style="width:100%;"></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>software</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='base95/README.md' target='_blank'><div class='ch_176'>base95<br/>（字节编码方法）</div><div class='ch_177'>2024-04-13</div></a><a class='ch_173 ch_174 ch_175' href='CoolMemory-English/README.md' target='_blank'><div class='ch_176'>CoolMemory-English<br/>（单词记忆软件）</div><div class='ch_177'>2023-12-11</div></a><a class='ch_173 ch_174 ch_175' href='miumapp/README.md' target='_blank'><div class='ch_176'>miumapp<br/>（跨平台GUI应用开发工具）</div><div class='ch_177'>2024-02-13</div></a><a class='ch_173 ch_174 ch_175' href='oodb/README.md' target='_blank'><div class='ch_176'>oodb<br/>（面向对象数据库）</div><div class='ch_177'>2024-03-06</div></a><a class='ch_173 ch_174 ch_175' href='oomongo/README.md' target='_blank'><div class='ch_176'>oomongo<br/>（MongoDB ODM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='oomysql/README.md' target='_blank'><div class='ch_176'>oomysql<br/>（MySQL ORM）</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='openai2/README.md' target='_blank'><div class='ch_176'>openai2<br/>（openai接口封装）</div><div class='ch_177'>2023-03-07</div></a><a class='ch_173 ch_174 ch_175' href='WeChat-Art-Museum/index.html' target='_blank'><div class='ch_176'>WeChat Art Museum<br/>（微信艺术馆）</div><div class='ch_177'>2024-03-31</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><h3 class='ch_182'>tutorials</h3><div class='ch_172'><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomysql' target='_blank'><div class='ch_176'>操作MySQL</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oomongo' target='_blank'><div class='ch_176'>操作MongoDB</div><div class='ch_177'>2021-06-06</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/miumapp' target='_blank'><div class='ch_176'>开发跨平台GUI应用</div><div class='ch_177'>2024-02-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/base95' target='_blank'><div class='ch_176'>Base95编码</div><div class='ch_177'>2024-04-13</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/openai2' target='_blank'><div class='ch_176'>对接ChatGPT</div><div class='ch_177'>2023-03-07</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/cooltypes/modules/cooltime' target='_blank'><div class='ch_176'>时间模块</div><div class='ch_177'>2023-06-25</div></a><a class='ch_173 ch_174 ch_175' href='https://lcctoor.github.io/arts/arts/oodb' target='_blank'><div class='ch_176'>面向对象数据库</div><div class='ch_177'>2024-03-06</div></a><a class='ch_173 ch_174 ch_175' href='tutorials/600-用37行代码实现AI五子棋/README.md' target='_blank'><div class='ch_176'>用37行代码实现AI五子棋</div><div class='ch_177'>2019-08-05</div></a><a class='ch_173 ch_174 ch_175' href='tutorials/750-正则表达式/README.md' target='_blank'><div class='ch_176'>正则表达式</div><div class='ch_177'>2023-06-19</div></a></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170'><div class='ch_171'>2024-03-18</div><iframe class='ch_178' src='life/2024/泉州市承天禅寺/index.html' loading='lazy' id=ch_107></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2023-10-06</div><iframe class='ch_178' src='life/2023/更换微信账号了/index.html' loading='lazy' id=ch_111></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2022-11-25</div><iframe class='ch_178' src='life/2022/泉州市丰泽区·雨后街道/index.html' loading='lazy' id=ch_115></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2019-05-01</div><iframe class='ch_178' src='life/2019/苏州市虎丘山/index.html' loading='lazy' id=ch_119></iframe><hr class='ch_179' style="width:100%;"><div class='ch_171'>2018-05-28</div><iframe class='ch_178' src='life/2018/莆田学院·毕业生留影/index.html' loading='lazy' id=ch_123></iframe><hr class='ch_179' style="width:100%;"></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div><div class='ch_169'><div class='ch_170' style="align-content:stretch;"><div class='ch_183 ch_184'><div class='ch_185 ch_186'>邮箱</div><div class='ch_187'><a class='ch_188 ch_189 ch_190' href='mailto:lcctoor@outlook.com'>lcctoor@outlook.com</a></div><div class='ch_185 ch_186'>微信</div><div class='ch_187'><img class='ch_191' src='./ip_static/WeChatQRC.jpg' style="max-width:15rem; height:auto;"></div><div class='ch_185 ch_186'>捐赠</div><div class='ch_187'><img class='ch_191' src='./ip_static/DonationQRC-0rmb.jpg' style="max-width:15rem; height:auto;"></div></div></div><div class='ch_181' style="text-align:center; width:100%; padding:0.618em 1em 0.618em 1em; color:grey;">Copyright 2018-2024 lcctoor@outlook.com</div></div></div>
 <script>
 "use strict";
 
 ch.ch_2 = () => window.innerWidth > window.innerHeight
 ch.ch_3 = (ele, name, value) => {
             try {ele.setAttribute(name, value)} catch (e) {}
             try {ele[name] = value} catch (e) {}
@@ -68,14 +68,20 @@
             if (value)
                 { ch.ch_3(ch.ch_4, 'is_x_screen', 'True') }
             else
                 { ch.ch_3(ch.ch_4, 'is_x_screen', 'False') }
             return value
         }
 ch.ch_130()
+document.addEventListener("DOMContentLoaded", function() {
+                let urlParams = new URLSearchParams(window.location.search)
+                if (urlParams.has('nav')) {
+                    ch.ch_151.firstChild.textContent = decodeURIComponent(urlParams.get('nav'))
+                }
+            })
 ch.ch_128 = document.getElementById("ch_127")
 ch.ch_134 = Array.from(ch.ch_128.querySelectorAll('.is_nav'))
 ch.ch_131 = (items, last_value=null) =>
             (outward_dict=null) =>
                 value => {
                     if (outward_dict && outward_dict.has(value)) {value = outward_dict.get(value)}
                     if (last_value !== value) {
@@ -175,15 +181,15 @@
 ch.ch_151 = document.getElementById("ch_150")
 ch.ch_154 = (value) => { ch.ch_151.firstChild.textContent = value }
 ch.ch_155 = new Map([["1", "动态"], ["2", "视频"], ["3", "文章"], ["4", "想法"], ["5", "软件"], ["6", "Python教程"], ["7", "生活"], ["8", "自述"]])
 ch.ch_156 = [ch.ch_154, ch.ch_155]
 ch.ch_132 = [ch.ch_140, ch.ch_149, ch.ch_156]
 ch.ch_135 = new Map([])
 ch.ch_145 = new Map([])
-ch.ch_152 = new Map([])
+ch.ch_152 = new Map([["动态", "1"], ["视频", "2"], ["文章", "3"], ["想法", "4"], ["软件", "5"], ["Python教程", "6"], ["生活", "7"], ["自述", "8"]])
 ch.ch_136 = ch.ch_131(ch.ch_132, null)
 ch.ch_137 = (navigation, navs, sync_value) => {
             navigation.addEventListener('click',
                 () => {
                     let nav = event.target
                     if (nav.classList.contains('is_nav'))
                         {sync_value(String( navs.indexOf(nav)+1 ))}
@@ -201,14 +207,32 @@
                             sync_value( String(index) )
                         }
                     }
                 }
             )
         }
 ch.ch_146(ch.ch_143, ch.ch_144, ch.ch_136(ch.ch_145))
+ch.ch_9 = window.MutationObserver || window.WebKitMutationObserver || window.MozMutationObserver
+ch.ch_153 = (sync_value, ele) => {
+            let textNode = null
+            let firstSon = ele.firstChild
+            if (firstSon && firstSon.nodeName === '#text')
+                { textNode = firstSon }
+            else {
+                textNode = document.createTextNode('')
+                if (firstSon)
+                    { ele.insertBefore(textNode, firstSon) }
+                else
+                    { ele.appendChild(textNode) }
+            }
+            new ch.ch_9(
+                (records, _) => { sync_value(textNode.textContent) }
+            ).observe(textNode, {characterData: true})
+        }
+ch.ch_153(ch.ch_136(ch.ch_152), ch.ch_151)
 ch.ch_129 = (ele, px) => {
                     ele.scrollLeft += px
                     try {event.preventDefault()} catch (e) {}  // 阻止其它默认行为
                 }
 ch.ch_128.addEventListener('wheel', () => {ch.ch_129(ch.ch_128, event.deltaY)})
 ch.ch_11 = document.getElementById("ch_10")
 ch.ch_14 = document.getElementById("ch_13")
```

### Comparing `arts-2024.4.19.1/arts/life/2018/莆田学院·毕业生留影/index.html` & `arts-2024.4.22/arts/life/2018/莆田学院·毕业生留影/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/life/2019/苏州市虎丘山/index.html` & `arts-2024.4.22/arts/life/2019/苏州市虎丘山/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/life/2022/泉州市丰泽区·雨后街道/index.html` & `arts-2024.4.22/arts/life/2022/泉州市丰泽区·雨后街道/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/life/2023/更换微信账号了/index.html` & `arts-2024.4.22/arts/life/2023/更换微信账号了/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/life/2024/泉州市承天禅寺/index.html` & `arts-2024.4.22/arts/life/2024/泉州市承天禅寺/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/miumapp/LICENSE` & `arts-2024.4.22/arts/miumapp/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/miumapp/README.md` & `arts-2024.4.22/arts/miumapp/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/miumapp/_core.py` & `arts-2024.4.22/arts/miumapp/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/miumapp/licenses/pyppeteer/LICENSE` & `arts-2024.4.22/arts/miumapp/licenses/pyppeteer/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/miumapp/licenses/tornado/LICENSE` & `arts-2024.4.22/arts/miumapp/licenses/tornado/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/miumapp/miumapp/demo.html` & `arts-2024.4.22/arts/miumapp/miumapp/demo.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/miumapp/miumapp/demo.py` & `arts-2024.4.22/arts/miumapp/miumapp/demo.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/miumapp/pyproject.toml` & `arts-2024.4.22/arts/miumapp/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oodb/LICENSE` & `arts-2024.4.22/arts/oodb/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oodb/README.md` & `arts-2024.4.22/arts/oodb/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oodb/_core.py` & `arts-2024.4.22/arts/oodb/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oodb/licenses/pymongo/LICENSE` & `arts-2024.4.22/arts/oodb/licenses/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oodb/pyproject.toml` & `arts-2024.4.22/arts/oodb/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oomongo/LICENSE` & `arts-2024.4.22/arts/oomongo/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oomongo/README.md` & `arts-2024.4.22/arts/oomongo/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oomongo/_core.py` & `arts-2024.4.22/arts/oomongo/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oomongo/licenses/motor/LICENSE` & `arts-2024.4.22/arts/oomongo/licenses/motor/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oomongo/licenses/pymongo/LICENSE` & `arts-2024.4.22/arts/oomongo/licenses/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oomongo/pyproject.toml` & `arts-2024.4.22/arts/oomongo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oomysql/LICENSE` & `arts-2024.4.22/arts/oomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oomysql/README.md` & `arts-2024.4.22/arts/oomysql/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oomysql/_core.py` & `arts-2024.4.22/arts/oomysql/_core.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oomysql/licenses/aiomysql/LICENSE` & `arts-2024.4.22/arts/oomysql/licenses/aiomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oomysql/licenses/pymysql/LICENSE` & `arts-2024.4.22/arts/oomysql/licenses/pymysql/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/oomysql/pyproject.toml` & `arts-2024.4.22/arts/oomysql/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/openai2/LICENSE` & `arts-2024.4.22/arts/openai2/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/openai2/README.md` & `arts-2024.4.22/arts/openai2/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/openai2/_core/chat.py` & `arts-2024.4.22/arts/openai2/_core/chat.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/openai2/_core/chat_in_cmd.py` & `arts-2024.4.22/arts/openai2/_core/chat_in_cmd.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/openai2/_core/group_chat.py` & `arts-2024.4.22/arts/openai2/_core/group_chat.py`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/openai2/licenses/openai/LICENSE` & `arts-2024.4.22/arts/openai2/licenses/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/openai2/pyproject.toml` & `arts-2024.4.22/arts/openai2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/skybox/README.md` & `arts-2024.4.22/arts/skybox/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/skybox/skybox/files_hashes` & `arts-2024.4.22/arts/skybox/skybox/files_hashes`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2022/现代工人的螺丝钉处境/index.html` & `arts-2024.4.22/arts/thoughts/2022/现代工人的螺丝钉处境/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html` & `arts-2024.4.22/arts/thoughts/2023/ChatGPT动了学阀的蛋糕/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/专利是个公平的赛道/index.html` & `arts-2024.4.22/arts/thoughts/2023/专利是个公平的赛道/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/事情的真实性是由度的/index.html` & `arts-2024.4.22/arts/thoughts/2023/事情的真实性是由度的/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/人无法摆脱兽性/index.html` & `arts-2024.4.22/arts/thoughts/2023/人无法摆脱兽性/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/什么是极端？/index.html` & `arts-2024.4.22/arts/thoughts/2023/什么是极端？/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/保护好人/index.html` & `arts-2024.4.22/arts/thoughts/2023/保护好人/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/只筛选，不教化/index.html` & `arts-2024.4.22/arts/thoughts/2023/只筛选，不教化/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/喊高考加油是刷存在感/index.html` & `arts-2024.4.22/arts/thoughts/2023/喊高考加油是刷存在感/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html` & `arts-2024.4.22/arts/thoughts/2023/宣扬出来的宽容是恶的代名词/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html` & `arts-2024.4.22/arts/thoughts/2023/对ChatGPT将带来的变革感到不知所措/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html` & `arts-2024.4.22/arts/thoughts/2023/强人工智能真的出现了，那就是 ChatGPT-4/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/想去国外了解自己/index.html` & `arts-2024.4.22/arts/thoughts/2023/想去国外了解自己/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/现代化的分工合作机制/index.html` & `arts-2024.4.22/arts/thoughts/2023/现代化的分工合作机制/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/用理性处理简单的事情/index.html` & `arts-2024.4.22/arts/thoughts/2023/用理性处理简单的事情/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/真正的问题无法通过花招解决/index.html` & `arts-2024.4.22/arts/thoughts/2023/真正的问题无法通过花招解决/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html` & `arts-2024.4.22/arts/thoughts/2023/艺术本天成，媒介偶显之/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html` & `arts-2024.4.22/arts/thoughts/2023/阳光下的美好是以阴影中的丑陋为代价/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2024/不要害怕犯错/index.html` & `arts-2024.4.22/arts/thoughts/2024/不要害怕犯错/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2024/新年题诗/index.html` & `arts-2024.4.22/arts/thoughts/2024/新年题诗/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html` & `arts-2024.4.22/arts/thoughts/2024/比特币无法成为取缔实体货币的最终币种/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2024/编程语言的进化/example.html` & `arts-2024.4.22/arts/thoughts/2024/编程语言的进化/example.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2024/编程语言的进化/index.html` & `arts-2024.4.22/arts/thoughts/2024/编程语言的进化/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html` & `arts-2024.4.22/arts/thoughts/2024/萝莉岛事件引发的信任危机/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html` & `arts-2024.4.22/arts/thoughts/2024/霍金去萝莉岛干嘛了/index.html`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/tutorials/600-用37行代码实现AI五子棋/README.md` & `arts-2024.4.22/arts/tutorials/600-用37行代码实现AI五子棋/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/arts/tutorials/750-正则表达式/README.md` & `arts-2024.4.22/arts/tutorials/750-正则表达式/README.md`

 * *Files identical despite different names*

### Comparing `arts-2024.4.19.1/pyproject.toml` & `arts-2024.4.22/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "arts"
-version = "2024.4.19.1"
+version = "2024.4.22"
 description = "对 Python 开发中常用功能的封装"
 dependencies = ["openai>=1.2.4", "numpy", "pymysql", "aiomysql", "pymongo", "motor", "pyppeteer>=2.0.0", "tornado"]
 
 
 requires-python = ">=3.10"
 readme = "README.md"
 authors = [{name = "江南雨上", email = "lcctoor@outlook.com"}]
```

### Comparing `arts-2024.4.19.1/PKG-INFO` & `arts-2024.4.22/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arts
-Version: 2024.4.19.1
+Version: 2024.4.22
 Summary: 对 Python 开发中常用功能的封装
 Author-email: 江南雨上 <lcctoor@outlook.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.2.4
 Requires-Dist: numpy
 Requires-Dist: pymysql
```

