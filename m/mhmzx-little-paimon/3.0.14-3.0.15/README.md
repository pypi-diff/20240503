# Comparing `tmp/mhmzx_little_paimon-3.0.14.tar.gz` & `tmp/mhmzx_little_paimon-3.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mhmzx_little_paimon-3.0.14.tar", max compression
+gzip compressed data, was "mhmzx_little_paimon-3.0.15.tar", max compression
```

## Comparing `mhmzx_little_paimon-3.0.14.tar` & `mhmzx_little_paimon-3.0.15.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0    34523 2023-10-03 11:58:12.363188 mhmzx_little_paimon-3.0.14/LICENSE
--rw-r--r--   0        0        0     3118 2023-10-04 07:14:41.385648 mhmzx_little_paimon-3.0.14/LittlePaimon/__init__.py
--rw-r--r--   0        0        0      186 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.14/LittlePaimon/config/__init__.py
--rw-r--r--   0        0        0     1665 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.14/LittlePaimon/config/command/__init__.py
--rw-r--r--   0        0        0     1752 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.14/LittlePaimon/config/config/manage.py
--rw-r--r--   0        0        0     3423 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/config/model.py
--rw-r--r--   0        0        0    36975 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/alias.json
--rw-r--r--   0        0        0    35003 2024-01-05 08:01:44.338265 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/artifact.json
--rw-r--r--   0        0        0    25724 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/ban_word.txt
--rw-r--r--   0        0        0    57661 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/genshin_info.json
--rw-r--r--   0        0        0     1508 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/prop.json
--rw-r--r--   0        0        0    43602 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/role_skill.json
--rw-r--r--   0        0        0    33754 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/role_talent.json
--rw-r--r--   0        0        0  1377251 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/roles_data.json
--rw-r--r--   0        0        0    25277 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/score.json
--rw-r--r--   0        0        0      949 2023-10-03 14:13:02.126748 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/upheaval.json
--rw-r--r--   0        0        0    22269 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/weapon.json
--rw-r--r--   0        0        0     7720 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/类型.json
--rw-r--r--   0        0        0     8927 2023-12-07 12:32:23.023892 mhmzx_little_paimon-3.0.14/LittlePaimon/config/plugin/manage.py
--rw-r--r--   0        0        0      795 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/config/plugin/model.py
--rw-r--r--   0        0        0     4161 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/__init__.py
--rw-r--r--   0        0        0      308 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/__init__.py
--rw-r--r--   0        0        0    11634 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/abyss_info.py
--rw-r--r--   0        0        0    20220 2023-12-07 15:12:48.876317 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/character.py
--rw-r--r--   0        0        0     2602 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/cookie.py
--rw-r--r--   0        0        0     1234 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/genshin_voice.py
--rw-r--r--   0        0        0     2733 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/manage.py
--rw-r--r--   0        0        0      451 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/memory_db.py
--rw-r--r--   0        0        0      782 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/other.py
--rw-r--r--   0        0        0    12879 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/player_info.py
--rw-r--r--   0        0        0     3546 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/subscription.py
--rw-r--r--   0        0        0     4573 2023-12-07 12:32:23.023892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/__init__.py
--rw-r--r--   0        0        0     6849 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/event.py
--rw-r--r--   0        0        0     2540 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/generate.py
--rw-r--r--   0        0        0     2466 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/calendar.html
--rw-r--r--   0        0        0     6882 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/index.css
--rw-r--r--   0        0        0   315626 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/iview.css
--rw-r--r--   0        0        0     6346 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/normalize.css
--rw-r--r--   0        0        0   158333 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/sy.jpg
--rw-r--r--   0        0        0     4436 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/__init__.py
--rw-r--r--   0        0        0     2535 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/draw.py
--rw-r--r--   0        0        0     5816 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/handler.py
--rw-r--r--   0        0        0     3565 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/resources.py
--rw-r--r--   0        0        0     3382 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/__init__.py
--rw-r--r--   0        0        0     3046 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/config.py
--rw-r--r--   0        0        0     6587 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/genshin_word.txt
--rw-r--r--   0        0        0    30915 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/handler.py
--rw-r--r--   0        0        0     3970 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/models.py
--rw-r--r--   0        0        0     9972 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/web_api.py
--rw-r--r--   0        0        0    23060 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/web_page.py
--rw-r--r--   0        0        0     1306 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Mihoyo_bbs/__init__.py
--rw-r--r--   0        0        0    10040 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/NoticeAndRequest/__init__.py
--rw-r--r--   0        0        0     1235 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/NoticeAndRequest/config.py
--rw-r--r--   0        0        0     3343 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/__init__.py
--rw-r--r--   0        0        0    16481 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/abyss_statistics.py
--rw-r--r--   0        0        0    13495 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/draw_abyss.py
--rw-r--r--   0        0        0       28 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/youchuang/__init__.py
--rw-r--r--   0        0        0     1727 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/youchuang/api.py
--rw-r--r--   0        0        0     3552 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/youchuang/draw.py
--rw-r--r--   0        0        0      991 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/youchuang/models.py
--rw-r--r--   0        0        0     8135 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/__init__.py
--rw-r--r--   0        0        0    14974 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/coin_handle.py
--rw-r--r--   0        0        0     2733 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/draw.py
--rw-r--r--   0        0        0     8833 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/sign_handle.py
--rw-r--r--   0        0        0    20499 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Bind/__init__.py
--rw-r--r--   0        0        0    11054 2023-12-07 13:48:58.774988 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Bind/get_cookie.py
--rw-r--r--   0        0        0     4387 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_CloudGenshin/__init__.py
--rw-r--r--   0        0        0     1768 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_CloudGenshin/api.py
--rw-r--r--   0        0        0     3894 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_CloudGenshin/handler.py
--rw-r--r--   0        0        0     3147 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_DailyNote/__init__.py
--rw-r--r--   0        0        0     9780 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_DailyNote/draw.py
--rw-r--r--   0        0        0     7660 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_DailyNote/handler.py
--rw-r--r--   0        0        0    10565 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/__init__.py
--rw-r--r--   0        0        0     1341 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/data_handle.py
--rw-r--r--   0        0        0     7925 2023-11-29 06:20:17.596561 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/data_source.py
--rw-r--r--   0        0        0     4364 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/draw.py
--rw-r--r--   0        0        0     8177 2023-12-07 13:49:08.459066 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/__init__.py
--rw-r--r--   0        0        0    10500 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/data_source.py
--rw-r--r--   0        0        0    13429 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/draw.py
--rw-r--r--   0        0        0     3852 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/models.py
--rw-r--r--   0        0        0    15959 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/__init__.py
--rw-r--r--   0        0        0    11703 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/damage_cal.py
--rw-r--r--   0        0        0    65408 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/damage_model.py
--rw-r--r--   0        0        0    10845 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_character_bag.py
--rw-r--r--   0        0        0     7799 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_character_card.py
--rw-r--r--   0        0        0    14100 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_character_detail.py
--rw-r--r--   0        0        0     9721 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_player_card.py
--rw-r--r--   0        0        0     1502 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_MonthInfo/__init__.py
--rw-r--r--   0        0        0     3990 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_MonthInfo/draw.py
--rw-r--r--   0        0        0     1431 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_MonthInfo/handler.py
--rw-r--r--   0        0        0      123 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/Atlas/__init__.py
--rw-r--r--   0        0        0     2029 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/Atlas/api.py
--rw-r--r--   0        0        0       37 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/__init__.py
--rw-r--r--   0        0        0     3357 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/api.py
--rw-r--r--   0        0        0     5089 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/draw.py
--rw-r--r--   0        0        0      209 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/models.py
--rw-r--r--   0        0        0    22279 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/__init__.py
--rw-r--r--   0        0        0     7572 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/draw_daily_material.py
--rw-r--r--   0        0        0     8754 2023-11-29 04:10:49.880595 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/draw_map.py
--rw-r--r--   0        0        0      888 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/__init__.py
--rw-r--r--   0        0        0      446 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/exc.py
--rw-r--r--   0        0        0     2600 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/img.py
--rw-r--r--   0        0        0     3573 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/models.py
--rw-r--r--   0        0        0     4320 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/request.py
--rw-r--r--   0        0        0     2902 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/utils.py
--rw-r--r--   0        0        0     1231 2023-11-02 02:35:17.358460 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/wiki_api.py
--rw-r--r--   0        0        0     7228 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/bot_manager/__init__.py
--rw-r--r--   0        0        0     4615 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/news60s/__init__.py
--rw-r--r--   0        0        0     8537 2023-12-07 12:31:51.791454 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/plugin_manager/__init__.py
--rw-r--r--   0        0        0     5192 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/plugin_manager/draw_help.py
--rw-r--r--   0        0        0     1443 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/tools/__init__.py
--rw-r--r--   0        0        0      607 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/__init__.py
--rw-r--r--   0        0        0     6214 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/alias.py
--rw-r--r--   0        0        0    18691 2023-12-07 15:12:48.876317 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/api.py
--rw-r--r--   0        0        0     3844 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/browser.py
--rw-r--r--   0        0        0     2695 2024-01-20 15:42:35.073417 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/files.py
--rw-r--r--   0        0        0     2420 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/filter.py
--rw-r--r--   0        0        0    19469 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/genshin.py
--rw-r--r--   0        0        0    22406 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/image.py
--rw-r--r--   0        0        0     1380 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/logger.py
--rw-r--r--   0        0        0    14786 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/message.py
--rw-r--r--   0        0        0     2380 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/path.py
--rw-r--r--   0        0        0     9531 2023-11-29 04:13:41.406015 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/requests.py
--rw-r--r--   0        0        0     1254 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/scheduler.py
--rw-r--r--   0        0        0     1600 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/status.py
--rw-r--r--   0        0        0     5838 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/tool.py
--rw-r--r--   0        0        0     3829 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/typing.py
--rw-r--r--   0        0        0     4568 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/utils/update.py
--rw-r--r--   0        0        0     2576 2024-01-20 15:42:35.073417 mhmzx_little_paimon-3.0.14/LittlePaimon/web/__init__.py
--rw-r--r--   0        0        0      655 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/__init__.py
--rw-r--r--   0        0        0     4853 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/bot_info.py
--rw-r--r--   0        0        0     1807 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/command_alias.py
--rw-r--r--   0        0        0    15631 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/cookie.py
--rw-r--r--   0        0        0      791 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/login.py
--rw-r--r--   0        0        0     6463 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/plugin.py
--rw-r--r--   0        0        0     1974 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/status.py
--rw-r--r--   0        0        0     1081 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/utils.py
--rw-r--r--   0        0        0      112 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/__init__.py
--rw-r--r--   0        0        0     1651 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/bind_cookie.py
--rw-r--r--   0        0        0     3525 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/command_alias.py
--rw-r--r--   0        0        0    16990 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/config_manage.py
--rw-r--r--   0        0        0      347 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/constants.py
--rw-r--r--   0        0        0     5482 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/home_page.py
--rw-r--r--   0        0        0     1903 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/login.py
--rw-r--r--   0        0        0     1816 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/main.py
--rw-r--r--   0        0        0     8089 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/plugin_manage.py
--rw-r--r--   0        0        0     6613 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/private_cookie.py
--rw-r--r--   0        0        0     3067 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/public_cookie.py
--rw-r--r--   0        0        0     1251 2024-04-06 04:32:46.440414 mhmzx_little_paimon-3.0.14/pyproject.toml
--rw-r--r--   0        0        0     1730 1970-01-01 00:00:00.000000 mhmzx_little_paimon-3.0.14/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-10-03 11:58:12.363188 mhmzx_little_paimon-3.0.15/LICENSE
+-rw-r--r--   0        0        0     3118 2023-10-04 07:14:41.385648 mhmzx_little_paimon-3.0.15/LittlePaimon/__init__.py
+-rw-r--r--   0        0        0      186 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.15/LittlePaimon/config/__init__.py
+-rw-r--r--   0        0        0     1665 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.15/LittlePaimon/config/command/__init__.py
+-rw-r--r--   0        0        0     1752 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.15/LittlePaimon/config/config/manage.py
+-rw-r--r--   0        0        0     3423 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/config/config/model.py
+-rw-r--r--   0        0        0    37053 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/alias.json
+-rw-r--r--   0        0        0    35968 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/artifact.json
+-rw-r--r--   0        0        0    25724 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/ban_word.txt
+-rw-r--r--   0        0        0    57930 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/genshin_info.json
+-rw-r--r--   0        0        0     1508 2023-10-03 14:13:02.118748 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/prop.json
+-rw-r--r--   0        0        0    44920 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/role_skill.json
+-rw-r--r--   0        0        0    34331 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/role_talent.json
+-rw-r--r--   0        0        0  1377336 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/roles_data.json
+-rw-r--r--   0        0        0    25343 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/score.json
+-rw-r--r--   0        0        0      949 2023-10-03 14:13:02.126748 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/upheaval.json
+-rw-r--r--   0        0        0    22390 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/weapon.json
+-rw-r--r--   0        0        0     7744 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/类型.json
+-rw-r--r--   0        0        0     8927 2023-12-07 12:32:23.023892 mhmzx_little_paimon-3.0.15/LittlePaimon/config/plugin/manage.py
+-rw-r--r--   0        0        0      795 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/config/plugin/model.py
+-rw-r--r--   0        0        0     4161 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/__init__.py
+-rw-r--r--   0        0        0      308 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/__init__.py
+-rw-r--r--   0        0        0    11634 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/abyss_info.py
+-rw-r--r--   0        0        0    20220 2023-12-07 15:12:48.876317 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/character.py
+-rw-r--r--   0        0        0     2602 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/cookie.py
+-rw-r--r--   0        0        0     1234 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/genshin_voice.py
+-rw-r--r--   0        0        0     2733 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/manage.py
+-rw-r--r--   0        0        0      451 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/memory_db.py
+-rw-r--r--   0        0        0      782 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/other.py
+-rw-r--r--   0        0        0    12879 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/player_info.py
+-rw-r--r--   0        0        0     3546 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/subscription.py
+-rw-r--r--   0        0        0     4573 2023-12-07 12:32:23.023892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/__init__.py
+-rw-r--r--   0        0        0     6849 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/event.py
+-rw-r--r--   0        0        0     2540 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/generate.py
+-rw-r--r--   0        0        0     2466 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/calendar.html
+-rw-r--r--   0        0        0     6882 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/index.css
+-rw-r--r--   0        0        0   315626 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/iview.css
+-rw-r--r--   0        0        0     6346 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/normalize.css
+-rw-r--r--   0        0        0   158333 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/sy.jpg
+-rw-r--r--   0        0        0     4436 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/__init__.py
+-rw-r--r--   0        0        0     2535 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/draw.py
+-rw-r--r--   0        0        0     5816 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/handler.py
+-rw-r--r--   0        0        0     3565 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/resources.py
+-rw-r--r--   0        0        0     3382 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/__init__.py
+-rw-r--r--   0        0        0     3046 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/config.py
+-rw-r--r--   0        0        0     6587 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/genshin_word.txt
+-rw-r--r--   0        0        0    30915 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/handler.py
+-rw-r--r--   0        0        0     3970 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/models.py
+-rw-r--r--   0        0        0     9972 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/web_api.py
+-rw-r--r--   0        0        0    23060 2023-10-03 14:13:02.130748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/web_page.py
+-rw-r--r--   0        0        0     1306 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Mihoyo_bbs/__init__.py
+-rw-r--r--   0        0        0    10040 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/NoticeAndRequest/__init__.py
+-rw-r--r--   0        0        0     1235 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/NoticeAndRequest/config.py
+-rw-r--r--   0        0        0     3343 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/__init__.py
+-rw-r--r--   0        0        0    16481 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/abyss_statistics.py
+-rw-r--r--   0        0        0    13495 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/draw_abyss.py
+-rw-r--r--   0        0        0       28 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/youchuang/__init__.py
+-rw-r--r--   0        0        0     1727 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/youchuang/api.py
+-rw-r--r--   0        0        0     3552 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/youchuang/draw.py
+-rw-r--r--   0        0        0      991 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/youchuang/models.py
+-rw-r--r--   0        0        0     8135 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/__init__.py
+-rw-r--r--   0        0        0    14974 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/coin_handle.py
+-rw-r--r--   0        0        0     2733 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/draw.py
+-rw-r--r--   0        0        0     8833 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/sign_handle.py
+-rw-r--r--   0        0        0    20499 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Bind/__init__.py
+-rw-r--r--   0        0        0    11054 2023-12-07 13:48:58.774988 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Bind/get_cookie.py
+-rw-r--r--   0        0        0     4387 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_CloudGenshin/__init__.py
+-rw-r--r--   0        0        0     1768 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_CloudGenshin/api.py
+-rw-r--r--   0        0        0     3894 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_CloudGenshin/handler.py
+-rw-r--r--   0        0        0     3147 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_DailyNote/__init__.py
+-rw-r--r--   0        0        0     9780 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_DailyNote/draw.py
+-rw-r--r--   0        0        0     7660 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_DailyNote/handler.py
+-rw-r--r--   0        0        0    10565 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/__init__.py
+-rw-r--r--   0        0        0     1341 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/data_handle.py
+-rw-r--r--   0        0        0     7925 2023-11-29 06:20:17.596561 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/data_source.py
+-rw-r--r--   0        0        0     4364 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/draw.py
+-rw-r--r--   0        0        0     8158 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/__init__.py
+-rw-r--r--   0        0        0    10507 2024-05-03 13:27:48.010549 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/data_source.py
+-rw-r--r--   0        0        0    13429 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/draw.py
+-rw-r--r--   0        0        0     3852 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/models.py
+-rw-r--r--   0        0        0    15959 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/__init__.py
+-rw-r--r--   0        0        0    11703 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/damage_cal.py
+-rw-r--r--   0        0        0    65408 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/damage_model.py
+-rw-r--r--   0        0        0    10845 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_character_bag.py
+-rw-r--r--   0        0        0     7799 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_character_card.py
+-rw-r--r--   0        0        0    14100 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_character_detail.py
+-rw-r--r--   0        0        0     9721 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_player_card.py
+-rw-r--r--   0        0        0     1502 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_MonthInfo/__init__.py
+-rw-r--r--   0        0        0     3990 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_MonthInfo/draw.py
+-rw-r--r--   0        0        0     1431 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_MonthInfo/handler.py
+-rw-r--r--   0        0        0      123 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/Atlas/__init__.py
+-rw-r--r--   0        0        0     2029 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/Atlas/api.py
+-rw-r--r--   0        0        0       37 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/__init__.py
+-rw-r--r--   0        0        0     3357 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/api.py
+-rw-r--r--   0        0        0     5089 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/draw.py
+-rw-r--r--   0        0        0      209 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/models.py
+-rw-r--r--   0        0        0    22279 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/__init__.py
+-rw-r--r--   0        0        0     7572 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/draw_daily_material.py
+-rw-r--r--   0        0        0     8754 2023-11-29 04:10:49.880595 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/draw_map.py
+-rw-r--r--   0        0        0      888 2023-10-03 14:13:02.134748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/__init__.py
+-rw-r--r--   0        0        0      446 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/exc.py
+-rw-r--r--   0        0        0     2600 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/img.py
+-rw-r--r--   0        0        0     3573 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/models.py
+-rw-r--r--   0        0        0     4320 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/request.py
+-rw-r--r--   0        0        0     2902 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/utils.py
+-rw-r--r--   0        0        0     1231 2023-11-02 02:35:17.358460 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/wiki_api.py
+-rw-r--r--   0        0        0     7228 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/bot_manager/__init__.py
+-rw-r--r--   0        0        0     4615 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/news60s/__init__.py
+-rw-r--r--   0        0        0     8537 2023-12-07 12:31:51.791454 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/plugin_manager/__init__.py
+-rw-r--r--   0        0        0     5192 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/plugin_manager/draw_help.py
+-rw-r--r--   0        0        0     1443 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/tools/__init__.py
+-rw-r--r--   0        0        0      607 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/__init__.py
+-rw-r--r--   0        0        0     6214 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/alias.py
+-rw-r--r--   0        0        0    18691 2024-05-03 13:28:19.726888 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/api.py
+-rw-r--r--   0        0        0     3844 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/browser.py
+-rw-r--r--   0        0        0     2695 2024-01-20 15:42:35.073417 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/files.py
+-rw-r--r--   0        0        0     2420 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/filter.py
+-rw-r--r--   0        0        0    19469 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/genshin.py
+-rw-r--r--   0        0        0    22406 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/image.py
+-rw-r--r--   0        0        0     1380 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/logger.py
+-rw-r--r--   0        0        0    14786 2023-12-07 12:32:23.027892 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/message.py
+-rw-r--r--   0        0        0     2380 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/path.py
+-rw-r--r--   0        0        0     9531 2023-11-29 04:13:41.406015 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/requests.py
+-rw-r--r--   0        0        0     1254 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/scheduler.py
+-rw-r--r--   0        0        0     1600 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/status.py
+-rw-r--r--   0        0        0     5838 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/tool.py
+-rw-r--r--   0        0        0     3829 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/typing.py
+-rw-r--r--   0        0        0     4568 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/utils/update.py
+-rw-r--r--   0        0        0     2576 2024-01-20 15:42:35.073417 mhmzx_little_paimon-3.0.15/LittlePaimon/web/__init__.py
+-rw-r--r--   0        0        0      655 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/__init__.py
+-rw-r--r--   0        0        0     4853 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/bot_info.py
+-rw-r--r--   0        0        0     1807 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/command_alias.py
+-rw-r--r--   0        0        0    15631 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/cookie.py
+-rw-r--r--   0        0        0      791 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/login.py
+-rw-r--r--   0        0        0     6463 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/plugin.py
+-rw-r--r--   0        0        0     1974 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/status.py
+-rw-r--r--   0        0        0     1081 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/utils.py
+-rw-r--r--   0        0        0      112 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/__init__.py
+-rw-r--r--   0        0        0     1651 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/bind_cookie.py
+-rw-r--r--   0        0        0     3525 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/command_alias.py
+-rw-r--r--   0        0        0    16990 2024-04-06 04:38:28.975420 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/config_manage.py
+-rw-r--r--   0        0        0      347 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/constants.py
+-rw-r--r--   0        0        0     5482 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/home_page.py
+-rw-r--r--   0        0        0     1903 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/login.py
+-rw-r--r--   0        0        0     1816 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/main.py
+-rw-r--r--   0        0        0     8089 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/plugin_manage.py
+-rw-r--r--   0        0        0     6613 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/private_cookie.py
+-rw-r--r--   0        0        0     3067 2023-10-03 14:13:02.138748 mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/public_cookie.py
+-rw-r--r--   0        0        0     1251 2024-05-03 13:29:30.667635 mhmzx_little_paimon-3.0.15/pyproject.toml
+-rw-r--r--   0        0        0     1730 1970-01-01 00:00:00.000000 mhmzx_little_paimon-3.0.15/PKG-INFO
```

### Comparing `mhmzx_little_paimon-3.0.14/LICENSE` & `mhmzx_little_paimon-3.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/command/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/command/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/config/manage.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/config/manage.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/config/model.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/config/model.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/alias.json` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/alias.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984756097560976%*

 * *Differences: {"'角色'": "{'10000096': ['阿蕾奇诺', '仆人', '父亲']}"}*

```diff
@@ -2064,10 +2064,15 @@
             "\u5609\u660e"
         ],
         "10000093": [
             "\u95f2\u4e91"
         ],
         "10000094": [
             "\u5343\u7ec7"
+        ],
+        "10000096": [
+            "\u963f\u857e\u5947\u8bfa",
+            "\u4ec6\u4eba",
+            "\u7236\u4eb2"
         ]
     }
 }
```

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/artifact.json` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/artifact.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9894416099773242%*

 * *Differences: {"'Mapping'": "{'灵露倾洒的狂诗': '谐律异想断章', '古海玄幽的夜想': '谐律异想断章', '异想零落的圆舞': '谐律异想断章', '谐律交响的前奏': "*

 * *              "'谐律异想断章', '命途轮转的谐谑': '谐律异想断章', '筹谋的共樽': '未竟的遐思', '褪光的翠尾': '未竟的遐思', '失冕的宝冠': "*

 * *              "'未竟的遐思', '暗结的明花': '未竟的遐思', '举业的识刻': '未竟的遐思'}",*

 * * "'Name'": "{'UI_RelicIcon_15031_3': '老兵的容颜', 'UI_RelicIcon_15031_5': '裁判的时刻', "*

 * *           "'UI_RelicIcon_15035_1': '灵露倾洒的狂诗', 'UI_RelicIcon_15035_2': '古海玄幽的夜想', "*

 * *           "'UI_RelicIcon_15035_3': '异想零落的圆舞', 'UI_RelicIcon_15035_4': '谐律交响的前奏', "*

 * *           "'UI_ […]*

```diff
@@ -442,14 +442,15 @@
                 "2": "\u62a4\u76fe\u5f3a\u6548\u63d0\u9ad835%\u3002",
                 "4": "\u5904\u4e8e\u62a4\u76fe\u5e87\u62a4\u4e0b\u65f6\uff0c\u989d\u5916\u83b7\u5f9740%\u666e\u901a\u653b\u51fb\u548c\u91cd\u51fb\u4f24\u5bb3\u52a0\u6210\u3002"
             }
         }
     },
     "Mapping": {
         "\u4e0d\u52a8\u7384\u77f3\u4e4b\u76f8": "\u60a0\u53e4\u7684\u78d0\u5ca9",
+        "\u4e3e\u4e1a\u7684\u8bc6\u523b": "\u672a\u7adf\u7684\u9050\u601d",
         "\u4e45\u8fdc\u82b1\u843d\u4e4b\u65f6": "\u82b1\u6d77\u7518\u9732\u4e4b\u5149",
         "\u4e50\u56e2\u7684\u6668\u5149": "\u6d41\u6d6a\u5927\u5730\u7684\u4e50\u56e2",
         "\u4f17\u738b\u4e4b\u90fd\u7684\u5f00\u7aef": "\u6c99\u4e0a\u697c\u9601\u53f2\u8bdd",
         "\u4f17\u751f\u4e4b\u8c23": "\u534e\u9986\u68a6\u9192\u5f62\u9ab8\u8bb0",
         "\u505c\u6446\u4e4b\u523b": "\u82cd\u767d\u4e4b\u706b",
         "\u5192\u9669\u5bb6\u4e4b\u82b1": "\u5192\u9669\u5bb6",
         "\u5192\u9669\u5bb6\u5934\u5e26": "\u5192\u9669\u5bb6",
@@ -469,25 +470,28 @@
         "\u52c7\u58eb\u7684\u671f\u8bb8": "\u52c7\u58eb\u4e4b\u5fc3",
         "\u52c7\u8005\u4eec\u7684\u8336\u4f1a": "\u6c34\u4ed9\u4e4b\u68a6",
         "\u52cb\u7ee9\u4e4b\u82b1": "\u5343\u5ca9\u7262\u56fa",
         "\u5317\u98ce\u4e4b\u76cf": "\u51b0\u4e4b\u5ddd\u4e0e\u96ea\u4e4b\u7802",
         "\u534e\u9970\u4e4b\u515c": "\u7edd\u7f18\u4e4b\u65d7\u5370",
         "\u534e\u9986\u4e4b\u7fbd": "\u534e\u9986\u68a6\u9192\u5f62\u9ab8\u8bb0",
         "\u5386\u7ecf\u98ce\u96ea\u7684\u601d\u5ff5": "\u51b0\u98ce\u8ff7\u9014\u7684\u52c7\u58eb",
+        "\u53e4\u6d77\u7384\u5e7d\u7684\u591c\u60f3": "\u8c10\u5f8b\u5f02\u60f3\u65ad\u7ae0",
         "\u541f\u6e38\u8005\u4e4b\u58f6": "\u6d41\u6d6a\u5927\u5730\u7684\u4e50\u56e2",
+        "\u547d\u9014\u8f6e\u8f6c\u7684\u8c10\u8c11": "\u8c10\u5f8b\u5f02\u60f3\u65ad\u7ae0",
         "\u5524\u96f7\u7684\u5934\u51a0": "\u5982\u96f7\u7684\u76db\u6012",
         "\u55e4\u7b11\u4e4b\u9762": "\u82cd\u767d\u4e4b\u706b",
         "\u574f\u5deb\u5e08\u7684\u7fbd\u6756": "\u6c34\u4ed9\u4e4b\u68a6",
         "\u575a\u94dc\u7f57\u76d8": "\u6c89\u6ca6\u4e4b\u5fc3",
         "\u5782\u7389\u4e4b\u53f6": "\u6765\u6b46\u4f59\u54cd",
         "\u590f\u796d\u4e4b\u523b": "\u9006\u98de\u7684\u6d41\u661f",
         "\u590f\u796d\u4e4b\u82b1": "\u9006\u98de\u7684\u6d41\u661f",
         "\u590f\u796d\u4e4b\u9762": "\u9006\u98de\u7684\u6d41\u661f",
         "\u590f\u796d\u6c34\u7389": "\u9006\u98de\u7684\u6d41\u661f",
         "\u590f\u796d\u7ec8\u672b": "\u9006\u98de\u7684\u6d41\u661f",
+        "\u5931\u5195\u7684\u5b9d\u51a0": "\u672a\u7adf\u7684\u9050\u601d",
         "\u5931\u843d\u8ff7\u9014\u7684\u673a\u82af": "\u6c99\u4e0a\u697c\u9601\u53f2\u8bdd",
         "\u5947\u8ff9\u4e4b\u676f": "\u5947\u8ff9",
         "\u5947\u8ff9\u4e4b\u6c99": "\u5947\u8ff9",
         "\u5947\u8ff9\u4e4b\u7fbd": "\u5947\u8ff9",
         "\u5947\u8ff9\u4e4b\u82b1": "\u5947\u8ff9",
         "\u5947\u8ff9\u8033\u5760": "\u5947\u8ff9",
         "\u5982\u871c\u7684\u7ec8\u5bb4": "\u9970\u91d1\u4e4b\u68a6",
@@ -521,14 +525,15 @@
         "\u5e73\u96f7\u4e4b\u7fbd": "\u5e73\u606f\u9e23\u96f7\u7684\u5c0a\u8005",
         "\u5e78\u8fd0\u513f\u4e4b\u676f": "\u5e78\u8fd0\u513f",
         "\u5e78\u8fd0\u513f\u6c99\u6f0f": "\u5e78\u8fd0\u513f",
         "\u5e78\u8fd0\u513f\u7eff\u82b1": "\u5e78\u8fd0\u513f",
         "\u5e78\u8fd0\u513f\u94f6\u51a0": "\u5e78\u8fd0\u513f",
         "\u5e78\u8fd0\u513f\u9e70\u7fbd": "\u5e78\u8fd0\u513f",
         "\u5f02\u56fd\u4e4b\u76cf": "\u884c\u8005\u4e4b\u5fc3",
+        "\u5f02\u60f3\u96f6\u843d\u7684\u5706\u821e": "\u8c10\u5f8b\u5f02\u60f3\u65ad\u7ae0",
         "\u5f52\u4e61\u4e4b\u7fbd": "\u884c\u8005\u4e4b\u5fc3",
         "\u5f62\u9ab8\u4e4b\u7b20": "\u534e\u9986\u68a6\u9192\u5f62\u9ab8\u8bb0",
         "\u5fe0\u5b9e\u7684\u7802\u65f6\u8ba1": "\u56de\u58f0\u4e4b\u6797\u591c\u8bdd",
         "\u601d\u5fc6\u4e4b\u77e2": "\u8ffd\u5fc6\u4e4b\u6ce8\u8fde",
         "\u6076\u9f99\u7684\u5355\u7247\u955c": "\u6c34\u4ed9\u4e4b\u68a6",
         "\u611f\u522b\u4e4b\u51a0": "\u884c\u8005\u4e4b\u5fc3",
         "\u6148\u7231\u7684\u6dd1\u5973\u5e3d": "\u56de\u58f0\u4e4b\u6797\u591c\u8bdd",
@@ -555,14 +560,15 @@
         "\u6614\u65f6\u4f20\u594f\u4e4b\u8bd7": "\u6614\u65f6\u4e4b\u6b4c",
         "\u6614\u65f6\u56de\u6620\u4e4b\u97f3": "\u6614\u65f6\u4e4b\u6b4c",
         "\u6614\u65f6\u5e94\u8bb8\u4e4b\u68a6": "\u6614\u65f6\u4e4b\u6b4c",
         "\u6614\u65f6\u6d6e\u60f3\u4e4b\u601d": "\u6614\u65f6\u4e4b\u6b4c",
         "\u6614\u65f6\u9057\u843d\u4e4b\u8a93": "\u6614\u65f6\u4e4b\u6b4c",
         "\u661f\u7f57\u572d\u74a7\u4e4b\u6677": "\u60a0\u53e4\u7684\u78d0\u5ca9",
         "\u662d\u6b66\u7fce\u7fbd": "\u5343\u5ca9\u7262\u56fa",
+        "\u6697\u7ed3\u7684\u660e\u82b1": "\u672a\u7adf\u7684\u9050\u601d",
         "\u6708\u5973\u7684\u534e\u5f69": "\u4e50\u56ed\u9057\u843d\u4e4b\u82b1",
         "\u6708\u6842\u7684\u5b9d\u51a0": "\u6df1\u6797\u7684\u8bb0\u5fc6",
         "\u671d\u9732\u4e4b\u65f6": "\u8ffd\u5fc6\u4e4b\u6ce8\u8fde",
         "\u6770\u4f5c\u7684\u5e8f\u66f2": "\u9010\u5f71\u730e\u4eba",
         "\u67d3\u8840\u7684\u94c1\u4e4b\u5fc3": "\u67d3\u8840\u7684\u9a91\u58eb\u9053",
         "\u67d3\u8840\u7684\u94c1\u5047\u9762": "\u67d3\u8840\u7684\u9a91\u58eb\u9053",
         "\u67d3\u8840\u7684\u9ed1\u4e4b\u7fbd": "\u67d3\u8840\u7684\u9a91\u58eb\u9053",
@@ -598,14 +604,15 @@
         "\u6e38\u533b\u7684\u65b9\u5dfe": "\u6e38\u533b",
         "\u6e38\u533b\u7684\u67ad\u7fbd": "\u6e38\u533b",
         "\u6e38\u533b\u7684\u836f\u58f6": "\u6e38\u533b",
         "\u6e38\u533b\u7684\u94f6\u83b2": "\u6e38\u533b",
         "\u6f5c\u5149\u7247\u7fbd": "\u8fb0\u7802\u5f80\u751f\u5f55",
         "\u7075\u5149\u660e\u70c1\u4e4b\u5fc3": "\u82b1\u6d77\u7518\u9732\u4e4b\u5149",
         "\u7075\u5149\u6e90\u8d77\u4e4b\u854a": "\u82b1\u6d77\u7518\u9732\u4e4b\u5149",
+        "\u7075\u9732\u503e\u6d12\u7684\u72c2\u8bd7": "\u8c10\u5f8b\u5f02\u60f3\u65ad\u7ae0",
         "\u7126\u707c\u7684\u9b54\u5973\u5e3d": "\u70bd\u70c8\u7684\u708e\u4e4b\u9b54\u5973",
         "\u730e\u4eba\u7684\u80f8\u82b1": "\u9010\u5f71\u730e\u4eba",
         "\u730e\u4eba\u9752\u7fe0\u7684\u7bad\u7fbd": "\u7fe0\u7eff\u4e4b\u5f71",
         "\u7426\u8272\u7075\u5f69\u4e4b\u7fbd": "\u82b1\u6d77\u7518\u9732\u4e4b\u5149",
         "\u7434\u5e08\u7684\u7bad\u7fbd": "\u6d41\u6d6a\u5927\u5730\u7684\u4e50\u56e2",
         "\u751f\u7075\u4e4b\u534e": "\u8fb0\u7802\u5f80\u751f\u5f55",
         "\u76df\u8a93\u91d1\u7235": "\u5343\u5ca9\u7262\u56fa",
@@ -616,34 +623,37 @@
         "\u795d\u7940\u4e4b\u51ed": "\u6765\u6b46\u4f59\u54cd",
         "\u796d\u51b0\u793c\u51a0": "\u796d\u51b0\u4e4b\u4eba",
         "\u796d\u6c34\u793c\u51a0": "\u796d\u6c34\u4e4b\u4eba",
         "\u796d\u706b\u793c\u51a0": "\u796d\u706b\u4e4b\u4eba",
         "\u796d\u96f7\u793c\u51a0": "\u796d\u96f7\u4e4b\u4eba",
         "\u796d\u98ce\u793c\u51a0": "\u796d\u98ce\u4e4b\u4eba",
         "\u79bb\u522b\u4e4b\u8d1d": "\u6d77\u67d3\u7817\u78f2",
+        "\u7b79\u8c0b\u7684\u5171\u6a3d": "\u672a\u7adf\u7684\u9050\u601d",
         "\u7d2b\u6676\u7684\u82b1\u51a0": "\u4e50\u56ed\u9057\u843d\u4e4b\u82b1",
         "\u7ec8\u5e55\u7684\u65f6\u8ba1": "\u6d41\u6d6a\u5927\u5730\u7684\u4e50\u56e2",
         "\u7ed3\u5951\u4e4b\u523b": "\u8fb0\u7802\u5f80\u751f\u5f55",
         "\u7eef\u82b1\u4e4b\u58f6": "\u7edd\u7f18\u4e4b\u65d7\u5370",
         "\u7f81\u7f20\u4e4b\u82b1": "\u8ffd\u5fc6\u4e4b\u6ce8\u8fde",
         "\u7fe0\u7eff\u730e\u4eba\u7684\u5bb9\u5668": "\u7fe0\u7eff\u4e4b\u5f71",
         "\u7fe0\u7eff\u730e\u4eba\u7684\u7b03\u5b9a": "\u7fe0\u7eff\u4e4b\u5f71",
         "\u7fe0\u7eff\u7684\u730e\u4eba\u4e4b\u51a0": "\u7fe0\u7eff\u4e4b\u5f71",
         "\u7fe0\u8513\u7684\u667a\u8005": "\u6df1\u6797\u7684\u8bb0\u5fc6",
         "\u8001\u5175\u7684\u5bb9\u989c": "\u9010\u5f71\u730e\u4eba",
         "\u8363\u82b1\u4e4b\u671f": "\u534e\u9986\u68a6\u9192\u5f62\u9ab8\u8bb0",
         "\u867a\u96f7\u4e4b\u59ff": "\u8fb0\u7802\u5f80\u751f\u5f55",
         "\u88c1\u5224\u7684\u65f6\u523b": "\u9010\u5f71\u730e\u4eba",
         "\u88c1\u65ad\u7684\u7fce\u7fbd": "\u9970\u91d1\u4e4b\u68a6",
+        "\u892a\u5149\u7684\u7fe0\u5c3e": "\u672a\u7adf\u7684\u9050\u601d",
         "\u89d2\u6597\u58eb\u7684\u51ef\u65cb": "\u89d2\u6597\u58eb\u7684\u7ec8\u5e55\u793c",
         "\u89d2\u6597\u58eb\u7684\u5e0c\u5180": "\u89d2\u6597\u58eb\u7684\u7ec8\u5e55\u793c",
         "\u89d2\u6597\u58eb\u7684\u5f52\u5bbf": "\u89d2\u6597\u58eb\u7684\u7ec8\u5e55\u793c",
         "\u89d2\u6597\u58eb\u7684\u7559\u604b": "\u89d2\u6597\u58eb\u7684\u7ec8\u5e55\u793c",
         "\u89d2\u6597\u58eb\u7684\u9163\u9189": "\u89d2\u6597\u58eb\u7684\u7ec8\u5e55\u793c",
         "\u8bda\u6073\u7684\u8638\u6c34\u7b14": "\u56de\u58f0\u4e4b\u6797\u591c\u8bdd",
+        "\u8c10\u5f8b\u4ea4\u54cd\u7684\u524d\u594f": "\u8c10\u5f8b\u5f02\u60f3\u65ad\u7ae0",
         "\u8c22\u843d\u7684\u7b75\u5e2d": "\u4e50\u56ed\u9057\u843d\u4e4b\u82b1",
         "\u8d24\u533b\u4e4b\u7fbd": "\u82cd\u767d\u4e4b\u706b",
         "\u8d24\u667a\u7684\u5b9a\u671f": "\u6df1\u6797\u7684\u8bb0\u5fc6",
         "\u8d4c\u5f92\u7684\u6000\u8868": "\u8d4c\u5f92",
         "\u8d4c\u5f92\u7684\u7fbd\u9970": "\u8d4c\u5f92",
         "\u8d4c\u5f92\u7684\u8033\u73af": "\u8d4c\u5f92",
         "\u8d4c\u5f92\u7684\u80f8\u82b1": "\u8d4c\u5f92",
@@ -902,32 +912,42 @@
         "UI_RelicIcon_15030_1": "\u65e0\u8fb9\u9163\u4e50\u4e4b\u7b75",
         "UI_RelicIcon_15030_2": "\u7426\u8272\u7075\u5f69\u4e4b\u7fbd",
         "UI_RelicIcon_15030_3": "\u7075\u5149\u660e\u70c1\u4e4b\u5fc3",
         "UI_RelicIcon_15030_4": "\u7075\u5149\u6e90\u8d77\u4e4b\u854a",
         "UI_RelicIcon_15030_5": "\u4e45\u8fdc\u82b1\u843d\u4e4b\u65f6",
         "UI_RelicIcon_15031_1": "\u9057\u5fd8\u7684\u5bb9\u5668",
         "UI_RelicIcon_15031_2": "\u6770\u4f5c\u7684\u5e8f\u66f2",
-        "UI_RelicIcon_15031_3": "\u88c1\u5224\u7684\u65f6\u523b",
+        "UI_RelicIcon_15031_3": "\u8001\u5175\u7684\u5bb9\u989c",
         "UI_RelicIcon_15031_4": "\u730e\u4eba\u7684\u80f8\u82b1",
-        "UI_RelicIcon_15031_5": "\u8001\u5175\u7684\u5bb9\u989c",
+        "UI_RelicIcon_15031_5": "\u88c1\u5224\u7684\u65f6\u523b",
         "UI_RelicIcon_15032_1": "\u9ec4\u91d1\u4e4b\u591c\u7684\u55a7\u56a3",
         "UI_RelicIcon_15032_2": "\u9ec4\u91d1\u98de\u9e1f\u7684\u843d\u7fbd",
         "UI_RelicIcon_15032_3": "\u9ec4\u91d1\u5267\u56e2\u7684\u5956\u8d4f",
         "UI_RelicIcon_15032_4": "\u9ec4\u91d1\u4e50\u66f2\u7684\u53d8\u594f",
         "UI_RelicIcon_15032_5": "\u9ec4\u91d1\u65f6\u4ee3\u7684\u5148\u58f0",
         "UI_RelicIcon_15033_1": "\u6614\u65f6\u5e94\u8bb8\u4e4b\u68a6",
         "UI_RelicIcon_15033_2": "\u6614\u65f6\u6d6e\u60f3\u4e4b\u601d",
         "UI_RelicIcon_15033_3": "\u6614\u65f6\u4f20\u594f\u4e4b\u8bd7",
         "UI_RelicIcon_15033_4": "\u6614\u65f6\u9057\u843d\u4e4b\u8a93",
         "UI_RelicIcon_15033_5": "\u6614\u65f6\u56de\u6620\u4e4b\u97f3",
         "UI_RelicIcon_15034_1": "\u6177\u6168\u7684\u58a8\u6c34\u74f6",
         "UI_RelicIcon_15034_2": "\u8bda\u6073\u7684\u8638\u6c34\u7b14",
         "UI_RelicIcon_15034_3": "\u6148\u7231\u7684\u6dd1\u5973\u5e3d",
         "UI_RelicIcon_15034_4": "\u65e0\u79c1\u7684\u5986\u9970\u82b1",
-        "UI_RelicIcon_15034_5": "\u5fe0\u5b9e\u7684\u7802\u65f6\u8ba1"
+        "UI_RelicIcon_15034_5": "\u5fe0\u5b9e\u7684\u7802\u65f6\u8ba1",
+        "UI_RelicIcon_15035_1": "\u7075\u9732\u503e\u6d12\u7684\u72c2\u8bd7",
+        "UI_RelicIcon_15035_2": "\u53e4\u6d77\u7384\u5e7d\u7684\u591c\u60f3",
+        "UI_RelicIcon_15035_3": "\u5f02\u60f3\u96f6\u843d\u7684\u5706\u821e",
+        "UI_RelicIcon_15035_4": "\u8c10\u5f8b\u4ea4\u54cd\u7684\u524d\u594f",
+        "UI_RelicIcon_15035_5": "\u547d\u9014\u8f6e\u8f6c\u7684\u8c10\u8c11",
+        "UI_RelicIcon_15036_1": "\u7b79\u8c0b\u7684\u5171\u6a3d",
+        "UI_RelicIcon_15036_2": "\u892a\u5149\u7684\u7fe0\u5c3e",
+        "UI_RelicIcon_15036_3": "\u5931\u5195\u7684\u5b9d\u51a0",
+        "UI_RelicIcon_15036_4": "\u6697\u7ed3\u7684\u660e\u82b1",
+        "UI_RelicIcon_15036_5": "\u4e3e\u4e1a\u7684\u8bc6\u523b"
     },
     "Piece": {
         "1": [
             "goblet",
             "\u7a7a\u4e4b\u676f"
         ],
         "2": [
```

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/ban_word.txt` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/ban_word.txt`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/genshin_info.json` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/genshin_info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9897959183673469%*

 * *Differences: {"'10000096'": "OrderedDict([('SkillOrder', [10941, 10942, 10945]), ('Skills', "*

 * *               "OrderedDict([('10941', 'Skill_A_03'), ('10942', 'Skill_S_Arlecchino_01'), "*

 * *               "('10945', 'Skill_E_Arlecchino_01')])), ('SideIconName', "*

 * *               "'UI_AvatarIcon_Side_Arlecchino')])"}*

```diff
@@ -2549,9 +2549,22 @@
             10945
         ],
         "Skills": {
             "10941": "Skill_A_01",
             "10942": "Skill_S_Chiori_01",
             "10945": "Skill_E_Chiori_01"
         }
+    },
+    "10000096": {
+        "SideIconName": "UI_AvatarIcon_Side_Arlecchino",
+        "SkillOrder": [
+            10941,
+            10942,
+            10945
+        ],
+        "Skills": {
+            "10941": "Skill_A_03",
+            "10942": "Skill_S_Arlecchino_01",
+            "10945": "Skill_E_Arlecchino_01"
+        }
     }
 }
```

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/prop.json` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/prop.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/role_skill.json` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/role_skill.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9852941176470589%*

 * *Differences: {"'Icon'": "{'10961': 'Skill_A_03', '10962': 'Skill_S_Arlecchino_01', '10963': "*

 * *           "'Skill_S_Arlecchino_01', '10965': 'Skill_E_Arlecchino_01', '10966': 'Skill_A_03', "*

 * *           "'10967': 'Skill_A_03', '20076': '', '20081': 'Skill_Music', '20086': 'Skill_Music', "*

 * *           "'20346': 'Btn_Whale_Interrupt', '20532': 'Btn_HideAndSeekV4_Seeker_A_03', '20533': "*

 * *           "'Btn_HideAndSeekV4_Seeker_E_03', '20534': 'Btn_HideAndSeekV4_Hider_S', '20535': "*

 * *           "'Btn_HideAndSeekV4_Hider_S', '2053 […]*

```diff
@@ -390,14 +390,20 @@
         "10935": "Skill_E_Liuyun_01",
         "10936": "Skill_S_Liuyun_03",
         "10937": "Skill_S_Liuyun_05",
         "10941": "Skill_A_01",
         "10942": "Skill_S_Chiori_01",
         "10944": "Skill_S_Chiori_03",
         "10945": "Skill_E_Chiori_01",
+        "10961": "Skill_A_03",
+        "10962": "Skill_S_Arlecchino_01",
+        "10963": "Skill_S_Arlecchino_01",
+        "10965": "Skill_E_Arlecchino_01",
+        "10966": "Skill_A_03",
+        "10967": "Skill_A_03",
         "11301": "Skill_A_02",
         "11302": "Skill_S_Ambor_01",
         "11305": "Skill_E_Beidou_01",
         "11371": "Skill_A_02",
         "11372": "Skill_S_Razor_01",
         "11373": "Skill_E_Razor_01",
         "11374": "Skill_A_02",
@@ -450,19 +456,22 @@
         "20062": "Skill_Diving_Echo",
         "20063": "Skill_Diving_Octopus",
         "20064": "Btn_HideAndSeek_Seeker_A_01",
         "20065": "Btn_CatchAnimal_Shoot",
         "20066": "Btn_HideAndSeek_Seeker_S_01",
         "20067": "Skill_Diving_Octopus",
         "20070": "QuesteventSkillIcon_01",
+        "20076": "",
         "20077": "Skill_LanV4PartyLion_01",
         "20080": "QuesteventSkillIcon_01",
+        "20081": "Skill_Music",
         "20082": "",
         "20083": "Skill_LanV4PartyLion_01",
         "20084": "Skill_LanV4PartyLion_01",
+        "20086": "Skill_Music",
         "20093": "Btn_SlimeCannon_Fire_01",
         "20094": "Btn_SlimeCannon_Fire_04",
         "20100": "Btn_HideAndSeek_Seeker_A_01",
         "20101": "Btn_HideAndSeek_Seeker_A_01",
         "20110": "Btn_HideAndSeek_Seeker_S_01",
         "20111": "Btn_HideAndSeek_Seeker_S_02",
         "20120": "Btn_HideAndSeek_Seeker_E_01",
@@ -492,14 +501,15 @@
         "20323": "Btn_Blocking_Burst03",
         "20330": "Btn_Arana_Shoot",
         "20331": "Btn_Arana_Exchange",
         "20340": "Btn_BrickBreaker_Launch",
         "20341": "Skill_LanV3_Icon05",
         "20342": "Skill_LanV3_Icon05",
         "20345": "Btn_PacMan",
+        "20346": "Btn_Whale_Interrupt",
         "20350": "Skill_E_Klee_01",
         "20351": "Skill_E_Klee_01",
         "20352": "Btn_Fishing_Bait",
         "20361": "Skill_E_Klee_01",
         "20362": "Skill_PoetryFestival_PitchPot_Icon01",
         "20363": "Skill_E_Klee_01",
         "20364": "Skill_E_BubbleGun_01",
@@ -526,14 +536,22 @@
         "20525": "Btn_HideAndSeek_Hider_A_01",
         "20526": "Btn_HideAndSeek_Hider_A_03",
         "20527": "Skill_CarpJump_02",
         "20528": "Skill_C_FairyGadgetSet",
         "20529": "Btn_Fishing_Exit",
         "20530": "Skill_CarpJump_01",
         "20531": "Btn_Fishing_Exit",
+        "20532": "Btn_HideAndSeekV4_Seeker_A_03",
+        "20533": "Btn_HideAndSeekV4_Seeker_E_03",
+        "20534": "Btn_HideAndSeekV4_Hider_S",
+        "20535": "Btn_HideAndSeekV4_Hider_S",
+        "20538": "Btn_HideAndSeekV4_Seeker_E_01",
+        "20539": "Btn_HideAndSeekV4_Seeker_S",
+        "20540": "Btn_HideAndSeekV4_Seeker_S",
+        "20541": "Btn_HideAndSeekV4_Seeker_A_01",
         "20561": "",
         "20562": "",
         "5002010": "Skill_A_01",
         "5003010": "Skill_A_01",
         "5005010": "Skill_A_01",
         "5005020": "Skill_A_01",
         "5005030": "Skill_A_01",
@@ -622,15 +640,16 @@
         "5087010": "Skill_A_Catalyst_MD",
         "5088010": "Skill_A_Catalyst_MD",
         "5089010": "Skill_A_01",
         "5090010": "Skill_A_03",
         "5091010": "Skill_A_04",
         "5092010": "Skill_A_04",
         "5093010": "Skill_A_Catalyst_MD",
-        "5094010": "Skill_A_01"
+        "5094010": "Skill_A_01",
+        "5096010": "Skill_A_03"
     },
     "Name": {
         "10001": "\u5355\u624b\u5251\u91cd\u653b\u51fb",
         "10002": "\u957f\u67aa\u91cd\u653b\u51fb",
         "10003": "\u6cd5\u5668\u91cd\u51fb",
         "10004": "\u53cc\u624b\u5251\u5355\u6b21\u91cd\u51fb",
         "10006": "\u84c4\u529b\u6280\u80fd\u6559\u5b66\u89e6\u53d1\u5668",
@@ -1019,14 +1038,20 @@
         "10935": "\u66ae\u96c6\u7af9\u661f",
         "10936": "\u7559\u4e91\u5143\u7d20\u6218\u6280_\u7b2c\u4e09\u8df3",
         "10937": "\u7559\u4e91\u547d6_\u5730\u9762\u7b2c\u4e00\u8df3",
         "10941": "\u666e\u901a\u653b\u51fb\u00b7\u5fc3\u7ec7\u5200\u6d41",
         "10942": "\u7fbd\u8896\u4e00\u89e6",
         "10944": "\u5343\u7ec7\u4e8c\u6bb5E\u540e-\u6280\u80fd\u66ff\u6362",
         "10945": "\u4e8c\u5200\u4e4b\u5f62\u00b7\u6bd4\u7ffc",
+        "10961": "\u666e\u901a\u653b\u51fb\u00b7\u65a9\u9996\u4e4b\u9080",
+        "10962": "\u4e07\u76f8\u5316\u7070",
+        "10963": "\u5143\u7d20\u6218\u6280\u66ff\u6362\u6280\u80fd",
+        "10965": "\u5384\u6708\u5c06\u5347",
+        "10966": "\u963f\u857e\u5947\u8bfa\u91cd\u51fb\u8fdc\u8ddd\u79bb\u7d22\u654c",
+        "10967": "\u963f\u857e\u5947\u8bfa\u62b5\u6b7b\u56de\u8840",
         "11301": "\u83f2\u8c22\u5c14\u666e\u653b",
         "11302": "\u83f2\u8c22\u5c14\u5c0f\u6280\u80fd",
         "11305": "\u83f2\u8c22\u5c14\u5145\u80fd\u6280",
         "11371": "Rx\u767d\u76d2\u6d4b\u8bd5\u666e\u653b",
         "11372": "Rx\u767d\u76d2\u6d4b\u8bd5\u6280\u80fd1",
         "11373": "Rx\u767d\u76d2\u6d4b\u8bd5\u6280\u80fd2",
         "11374": "Rx\u767d\u76d2\u8fdb\u5165\u7784\u51c6",
@@ -1079,19 +1104,22 @@
         "20062": "4.0\u6c34\u4e0b\u5438\u6536-\u56de\u58f0",
         "20063": "4.2 \u6c34\u4e0b\u7ae0\u9c7c-\u55b7\u5c04",
         "20064": "\u63d0\u7ebf\u6728\u5076-\u653b\u51fb\u5de6\uff08\u767d\u76d2\uff09",
         "20065": "\u63d0\u7ebf\u6728\u5076-\u653b\u51fb\u53f3\uff08\u767d\u76d2\uff09",
         "20066": "\u63d0\u7ebf\u6728\u5076-\u5de6\u53f3\u8fde\u6253\uff08\u767d\u76d2\uff09",
         "20067": "4.2 \u9646\u5730\u7ae0\u9c7c-\u55b7\u5c04\u80fd\u529b",
         "20070": "\u63a2\u67e5\u6280\u80fd",
+        "20076": "4.6\u9cb8\u9c7c\u94a9\u722a",
         "20077": "4.4\u6d77\u706f\u8282-\u53d8\u8eab\u6280\u80fd-\u91d1\u5e01\u5173",
         "20080": "\u63a2\u67e5\u6280\u80fd",
+        "20081": "4.6\u97f3\u4e50\u673a\u5236",
         "20082": "4.2\u6c34\u4e0b\u5f39\u5c04",
         "20083": "4.4\u6d77\u706f\u8282-\u53d8\u8eab\u6280\u80fd-\u79ef\u5206\u5173",
         "20084": "4.4\u6d77\u706f\u8282-\u53d8\u8eab\u6280\u80fd-\u751f\u5b58\u5173",
+        "20086": "4.6\u97f3\u4e50\u673a\u5236\u6c34\u4e0b",
         "20093": "4.5\u53f2\u83b1\u59c6\u7403-\u5143\u7d20\u5f39",
         "20094": "4.5\u53f2\u83b1\u59c6\u7403-\u7269\u7406\u8fde\u5c04",
         "20100": "\u6355\u83b7\uff01",
         "20101": "\u6355\u83b7\uff01",
         "20110": "\u795e\u79d8\u9884\u611f",
         "20111": "\u611f\u5e94\u5149\u73af",
         "20120": "\u72e9\u730e\u76f4\u89c9",
@@ -1121,14 +1149,15 @@
         "20323": "\u683c\u6321\u73a9\u6cd5-\u5fc5\u6740\u62803",
         "20330": "\u5170\u90a3\u7f57\u5c0f\u9053\u5177-\u53d1\u5c04",
         "20331": "\u5170\u90a3\u7f57\u5c0f\u9053\u5177-\u5207\u6362",
         "20340": "\u6253\u7816\u5757\u53d1\u7403",
         "20341": "3.4\u8dd1\u9177\u51b2\u523a",
         "20342": "3.4\u8dd1\u9177\u51b2\u523a\u7a7a\u4e2d",
         "20345": "3.5\u5403\u8c46\u4eba",
+        "20346": "4.6\u9cb8\u9c7c\u94a9\u722a\u9000\u51fa",
         "20350": "3.8\u8fc7\u5c71\u8f66-\u5de6\u653b\u51fb",
         "20351": "3.8\u8fc7\u5c71\u8f66-\u53f3\u653b\u51fb",
         "20352": "3.8\u8fc7\u5c71\u8f66-\u8dc3\u8fc1",
         "20361": "4.0\u4eba\u95f4\u5927\u70ae-\u53d1\u5c04\u952e",
         "20362": "4.1\u6295\u58f6\u6280\u80fd \u957fCD",
         "20363": "4.1\u6295\u58f6\u6280\u80fd \u77edCD(\u8fd9\u884c\u540e\u9762\u5e9f\u5f03\u4e86",
         "20364": "4.1\u4e09\u5468\u5e74\u5e86-\u6ce1\u6ce1\u67aa",
@@ -1155,14 +1184,22 @@
         "20525": "\u4f2a\u88c5",
         "20526": "\u4f2a\u88c5",
         "20527": "\u9c7c\u8dc3",
         "20528": "\u666f\u89c2\u73a9\u6cd5",
         "20529": "\u9c7c\u8dc3\u5f39\u51fa",
         "20530": "\u87ad\u795e\u50cf\u53d1\u5b50\u5f39",
         "20531": "\u87ad\u795e\u50cf\u5f39\u51fa",
+        "20532": "\u6355\u5f71\u4fe1\u6807",
+        "20533": "\u65e0\u5f62\u8ffd\u8ff9",
+        "20534": "\u4f2a\u88c5",
+        "20535": "\u4f2a\u88c5",
+        "20538": "\u7981\u9522\u8bc5\u5492",
+        "20539": "\u6355\u83b7\uff01",
+        "20540": "\u6355\u83b7\uff01",
+        "20541": "\u795e\u79d8\u9884\u611f",
         "20561": "\u9c7c\u8dc3T\u5730\u9762",
         "20562": "\u9c7c\u8dc3T\u7a7a\u4e2d",
         "5002010": "\u795e\u91cc\u7eeb\u534e\u7a7a\u4e2d\u653b\u51fb",
         "5003010": "\u7434\u7a7a\u4e2d\u653b\u51fb",
         "5005010": "\u7537\u4e3b\u89d2\u7a7a\u4e2d\u653b\u51fb",
         "5005020": "\u7537\u4e3b\u89d2(\u706b)\u7a7a\u4e2d\u653b\u51fb",
         "5005030": "\u7537\u4e3b\u89d2(\u6c34)\u7a7a\u4e2d\u653b\u51fb",
@@ -1251,10 +1288,11 @@
         "5087010": "\u90a3\u7ef4\u83b1\u7279\u7a7a\u4e2d\u653b\u51fb",
         "5088010": "\u590f\u6d1b\u8482\u7a7a\u4e2d\u653b\u51fb",
         "5089010": "\u8299\u5b81\u5a1c\u7a7a\u4e2d\u653b\u51fb",
         "5090010": "\u590f\u6c83\u857e\u7a7a\u4e2d\u653b\u51fb",
         "5091010": "\u5a1c\u7ef4\u5a05\u7a7a\u4e2d\u653b\u51fb",
         "5092010": "\u5609\u660e\u7a7a\u4e2d\u653b\u51fb",
         "5093010": "\u95f2\u4e91\u7a7a\u4e2d\u653b\u51fb",
-        "5094010": "\u5343\u7ec7\u7a7a\u4e2d\u653b\u51fb"
+        "5094010": "\u5343\u7ec7\u7a7a\u4e2d\u653b\u51fb",
+        "5096010": "\u963f\u857e\u5947\u8bfa\u7a7a\u4e2d\u653b\u51fb"
     }
 }
```

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/role_talent.json` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/role_talent.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9941176470588236%*

 * *Differences: {"'Icon'": "{'961': 'UI_Talent_S_Arlecchino_01', '962': 'UI_Talent_S_Arlecchino_02', '963': "*

 * *           "'UI_Talent_U_Arlecchino_01', '964': 'UI_Talent_S_Arlecchino_03', '965': "*

 * *           "'UI_Talent_U_Arlecchino_02', '966': 'UI_Talent_S_Arlecchino_04'}",*

 * * "'Name'": "{'961': '「所有的仇与债皆由我偿…」', '962': '「所有的赏与罚皆自我出…」', '963': '「你将成为我们新的家人…」', '964': "*

 * *           "'「此后，你们须相爱相护…」', '965': '「我们已孑然一身，与死无异…」', '966': '「自此以后，我们将共飨新生。」'}"}*

```diff
@@ -499,15 +499,21 @@
         "941": "UI_Talent_S_Chiori_01",
         "942": "UI_Talent_S_Chiori_03",
         "943": "UI_Talent_U_Chiori_01",
         "944": "UI_Talent_S_Chiori_02",
         "945": "UI_Talent_U_Chiori_02",
         "946": "UI_Talent_S_Chiori_04",
         "95": "UI_Talent_U_PlayerRock_01",
-        "96": "UI_Talent_S_PlayerRock_04"
+        "96": "UI_Talent_S_PlayerRock_04",
+        "961": "UI_Talent_S_Arlecchino_01",
+        "962": "UI_Talent_S_Arlecchino_02",
+        "963": "UI_Talent_U_Arlecchino_01",
+        "964": "UI_Talent_S_Arlecchino_03",
+        "965": "UI_Talent_U_Arlecchino_02",
+        "966": "UI_Talent_S_Arlecchino_04"
     },
     "Name": {
         "101": "\u4e30\u7a70\u7684\u6625\u96f7",
         "102": "\u9707\u6012\u7684\u82cd\u96f7",
         "103": "\u8fde\u5ef6\u7684\u8fdc\u96f7",
         "104": "\u96be\u6d4b\u7684\u4e91\u96f7",
         "105": "\u8352\u91ce\u7684\u9706\u96f7",
@@ -1005,10 +1011,16 @@
         "941": "\u6b63\u7ee2\u516d\u901a",
         "942": "\u843d\u67d3\u4e94\u8272",
         "943": "\u7f00\u9526\u56db\u5206",
         "944": "\u8863\u88c1\u4e09\u793c",
         "945": "\u7eeb\u7fbd\u4e8c\u91cd",
         "946": "\u4e07\u7406\u4e00\u7a7a",
         "95": "\u5929\u5760\u4e4b\u5ca9",
-        "96": "\u6c38\u4e16\u7684\u78d0\u5ca9"
+        "96": "\u6c38\u4e16\u7684\u78d0\u5ca9",
+        "961": "\u300c\u6240\u6709\u7684\u4ec7\u4e0e\u503a\u7686\u7531\u6211\u507f\u2026\u300d",
+        "962": "\u300c\u6240\u6709\u7684\u8d4f\u4e0e\u7f5a\u7686\u81ea\u6211\u51fa\u2026\u300d",
+        "963": "\u300c\u4f60\u5c06\u6210\u4e3a\u6211\u4eec\u65b0\u7684\u5bb6\u4eba\u2026\u300d",
+        "964": "\u300c\u6b64\u540e\uff0c\u4f60\u4eec\u987b\u76f8\u7231\u76f8\u62a4\u2026\u300d",
+        "965": "\u300c\u6211\u4eec\u5df2\u5b51\u7136\u4e00\u8eab\uff0c\u4e0e\u6b7b\u65e0\u5f02\u2026\u300d",
+        "966": "\u300c\u81ea\u6b64\u4ee5\u540e\uff0c\u6211\u4eec\u5c06\u5171\u98e8\u65b0\u751f\u3002\u300d"
     }
 }
```

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/roles_data.json` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/roles_data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9876543209876543%*

 * *Differences: {"'阿蕾奇诺'": "OrderedDict([('region', '枫丹'), ('star', 5), ('element', '火')])"}*

```diff
@@ -28908,14 +28908,19 @@
         "weapon": "\u957f\u67c4\u6b66\u5668"
     },
     "\u95f2\u4e91": {
         "element": "\u98ce",
         "region": "\u7483\u6708",
         "star": 5
     },
+    "\u963f\u857e\u5947\u8bfa": {
+        "element": "\u706b",
+        "region": "\u67ab\u4e39",
+        "star": 5
+    },
     "\u963f\u8d1d\u591a": {
         "attribute": {
             "atk": {
                 "1": "20",
                 "20": "51",
                 "40": "101",
                 "50": "130",
```

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/score.json` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/score.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970588235294118%*

 * *Differences: {"'Talent'": "{'阿蕾奇诺': [0, 2]}"}*

```diff
@@ -1060,14 +1060,18 @@
             1,
             2
         ],
         "\u95f2\u4e91": [
             1,
             0
         ],
+        "\u963f\u857e\u5947\u8bfa": [
+            0,
+            2
+        ],
         "\u963f\u8d1d\u591a": [
             1,
             2
         ],
         "\u96f7\u4e3b": [
             1,
             0
```

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/upheaval.json` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/upheaval.json`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/weapon.json` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/weapon.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973903078810015%*

 * *Differences: {"'Icon'": "{'赤月之形': 'UI_EquipIcon_Pole_BloodMoon'}",*

 * * "'Name'": "{'2944936683': '赤月之形'}",*

 * * "'Type'": "{'赤月之形': '长柄武器'}"}*

```diff
@@ -144,14 +144,15 @@
         "\u8bd5\u4f5c\u53e4\u534e": "UI_EquipIcon_Claymore_Proto",
         "\u8bd5\u4f5c\u65a9\u5ca9": "UI_EquipIcon_Sword_Proto",
         "\u8bd5\u4f5c\u661f\u9570": "UI_EquipIcon_Pole_Proto",
         "\u8bd5\u4f5c\u6fb9\u6708": "UI_EquipIcon_Bow_Proto",
         "\u8bd5\u4f5c\u91d1\u73c0": "UI_EquipIcon_Catalyst_Proto",
         "\u8d2f\u6708\u77e2": "UI_EquipIcon_Pole_Arakalari",
         "\u8d2f\u8679\u4e4b\u69ca": "UI_EquipIcon_Pole_Kunwu",
+        "\u8d64\u6708\u4e4b\u5f62": "UI_EquipIcon_Pole_BloodMoon",
         "\u8d64\u6c99\u4e4b\u6756": "UI_EquipIcon_Pole_Deshret",
         "\u8d64\u89d2\u77f3\u6e83\u6775": "UI_EquipIcon_Claymore_Itadorimaru",
         "\u8fb0\u7802\u4e4b\u7eba\u9524": "UI_EquipIcon_Sword_Opus",
         "\u9057\u7940\u7389\u73d1": "UI_EquipIcon_Catalyst_Yue",
         "\u91d1\u6d41\u76d1\u7763": "UI_EquipIcon_Catalyst_Wheatley",
         "\u949f\u5251": "UI_EquipIcon_Claymore_Troupe",
         "\u94a2\u8f6e\u5f13": "UI_EquipIcon_Bow_Exotic",
@@ -275,14 +276,15 @@
         "2792766467": "\u65e0\u5de5\u4e4b\u5251",
         "2796697027": "\u65b0\u624b\u957f\u67aa",
         "2832648187": "\u5b97\u5ba4\u957f\u5f13",
         "2834063555": "\u82c7\u6d77\u4fe1\u6807",
         "2847771107": "\u6c99\u4e2d\u4f1f\u8d24\u7684\u5bf9\u7b54",
         "2918525947": "\u98de\u96f7\u4e4b\u5f26\u632f",
         "2935286715": "\u5b97\u5ba4\u730e\u67aa",
+        "2944936683": "\u8d64\u6708\u4e4b\u5f62",
         "2947140987": "\u6697\u5df7\u95ea\u5149",
         "2949448555": "\u82cd\u53e4\u81ea\u7531\u4e4b\u8a93",
         "2958179435": "\u70c8\u9633\u4e4b\u55e3",
         "2963220587": "\u7fe1\u7389\u6cd5\u7403",
         "2988480723": "\u6700\u521d\u7684\u5927\u9b54\u672f",
         "3016493955": "\u6c34\u4ed9\u5341\u5b57\u4e4b\u5251",
         "302691299": "\u7425\u73c0\u73a5",
@@ -532,14 +534,15 @@
         "\u8bd5\u4f5c\u53e4\u534e": "\u53cc\u624b\u5251",
         "\u8bd5\u4f5c\u65a9\u5ca9": "\u5355\u624b\u5251",
         "\u8bd5\u4f5c\u661f\u9570": "\u957f\u67c4\u6b66\u5668",
         "\u8bd5\u4f5c\u6fb9\u6708": "\u5f13",
         "\u8bd5\u4f5c\u91d1\u73c0": "\u6cd5\u5668",
         "\u8d2f\u6708\u77e2": "\u957f\u67c4\u6b66\u5668",
         "\u8d2f\u8679\u4e4b\u69ca": "\u957f\u67c4\u6b66\u5668",
+        "\u8d64\u6708\u4e4b\u5f62": "\u957f\u67c4\u6b66\u5668",
         "\u8d64\u6c99\u4e4b\u6756": "\u957f\u67c4\u6b66\u5668",
         "\u8d64\u89d2\u77f3\u6e83\u6775": "\u53cc\u624b\u5251",
         "\u8fb0\u7802\u4e4b\u7eba\u9524": "\u5355\u624b\u5251",
         "\u9057\u7940\u7389\u73d1": "\u6cd5\u5668",
         "\u91d1\u6d41\u76d1\u7763": "\u6cd5\u5668",
         "\u949f\u5251": "\u53cc\u624b\u5251",
         "\u94a2\u8f6e\u5f13": "\u5f13",
```

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/data/类型.json` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/data/类型.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995833333333333%*

 * *Differences: {"'角色'": "{'武器类型': {'长柄武器': {insert: [(14, '阿蕾奇诺')]}}}"}*

```diff
@@ -373,12 +373,13 @@
                 "\u96f7\u7535\u5c06\u519b",
                 "\u7533\u9e64",
                 "\u4e91\u5807",
                 "\u8d5b\u8bfa",
                 "\u574e\u8482\u4e1d",
                 "\u7476\u7476",
                 "\u7c73\u5361",
-                "\u590f\u6c83\u857e"
+                "\u590f\u6c83\u857e",
+                "\u963f\u857e\u5947\u8bfa"
             ]
         }
     }
 }
```

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/plugin/manage.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/plugin/manage.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/config/plugin/model.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/config/plugin/model.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/database/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/abyss_info.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/abyss_info.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/character.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/character.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/cookie.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/genshin_voice.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/genshin_voice.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/manage.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/manage.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/other.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/other.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/player_info.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/player_info.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/database/models/subscription.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/database/models/subscription.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/event.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/event.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/generate.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/generate.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/calendar.html` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/calendar.html`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/index.css` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/index.css`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/iview.css` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/iview.css`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/normalize.css` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/normalize.css`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Calendar/template/sy.jpg` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Calendar/template/sy.jpg`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/draw.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/handler.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/handler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Genshin_Voice/resources.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Genshin_Voice/resources.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/config.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/config.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/genshin_word.txt` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/genshin_word.txt`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/handler.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/handler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/models.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/models.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/web_api.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/web_api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Learning_Chat/web_page.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Learning_Chat/web_page.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Mihoyo_bbs/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Mihoyo_bbs/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/NoticeAndRequest/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/NoticeAndRequest/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/NoticeAndRequest/config.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/NoticeAndRequest/config.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/abyss_statistics.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/abyss_statistics.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/draw_abyss.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/draw_abyss.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/youchuang/api.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/youchuang/api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/youchuang/draw.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/youchuang/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Abyss/youchuang/models.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Abyss/youchuang/models.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/coin_handle.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/coin_handle.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/draw.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Autobbs/sign_handle.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Autobbs/sign_handle.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Bind/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Bind/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Bind/get_cookie.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Bind/get_cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_CloudGenshin/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_CloudGenshin/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_CloudGenshin/api.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_CloudGenshin/api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_CloudGenshin/handler.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_CloudGenshin/handler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_DailyNote/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_DailyNote/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_DailyNote/draw.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_DailyNote/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_DailyNote/handler.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_DailyNote/handler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/data_handle.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/data_handle.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/data_source.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/data_source.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha/draw.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from nonebot.plugin import PluginMetadata
 
 from LittlePaimon.utils import NICKNAME, logger
 from LittlePaimon.utils.api import get_authkey_by_stoken
 from LittlePaimon.utils.message import CommandPlayer, CommandUID
 
 from .data_source import (
+    GACHA_LOG_API,
     create_import_command,
     gacha_log_to_UIGF,
     get_gacha_log_data,
     get_gacha_log_img,
 )
 
 __plugin_meta__ = PluginMetadata(
@@ -178,24 +179,24 @@
 @gacha_url.handle()
 async def _(bot: Bot, event: MessageEvent, uid: str = CommandUID()):
     await gacha_url.send("正在获取抽卡记录链接")
     logger.info("获取抽卡记录链接", "开始执行")
     authkey, state, _ = await get_authkey_by_stoken(str(event.user_id), uid)
     if not state:
         return authkey
-    if authkey == {}:
+    if not authkey:
         await gacha_url.finish(authkey, at_sender=True)
     region = "cn_qd01" if uid[0] == "5" else "cn_gf01"
     url = (
-        f"https://hk4e-api.mihoyo.com/event/gacha_info/api/getGachaLog?"
+        f"{GACHA_LOG_API}?"
         f"authkey_ver=1&sign_type=2&auth_appid=webview_gacha&init_type=301&"
         f"gacha_id=fecafa7b6560db5f3182222395d88aaa6aaac1bc"
         f"&timestamp={int(time.time())}"
         f"&lang=zh-cn&device_type=mobile&plat_type=ios&region={region}"
-        f"&authkey={quote(authkey,'utf-8')}"
+        f"&authkey={quote(authkey,encoding='utf-8')}"
         f"&game_biz=hk4e_cn&gacha_type=301&page=1&size=5&end_id=0"
     )
     msgs = [
         {
             "type": "node",
             "data": {
                 "name": NICKNAME,
```

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/data_source.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from LittlePaimon.utils.requests import aiorequests
 from LittlePaimon.utils.api import get_authkey_by_stoken
 from LittlePaimon.utils.files import load_json, save_json
 from LittlePaimon.utils.path import GACHA_LOG
 from .draw import draw_gacha_log
 from .models import GachaItem, GachaLogInfo, GACHA_TYPE_LIST
 
-GACHA_LOG_API = 'https://hk4e-api.mihoyo.com/event/gacha_info/api/getGachaLog'
+GACHA_LOG_API = 'https://public-operation-hk4e.mihoyo.com/gacha_info/api/getGachaLog'
 HEADERS: Dict[str, str] = {
     'x-rpc-app_version': '2.11.1',
     'User-Agent':        'Mozilla/5.0 (iPhone; CPU iPhone OS 13_2_3 like Mac OS X) AppleWebKit/605.1.15 ('
                          'KHTML, like Gecko) miHoYoBBS/2.11.1',
     'x-rpc-client_type': '5',
     'Referer':           'https://webstatic.mihoyo.com/',
     'Origin':            'https://webstatic.mihoyo.com',
```

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/draw.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Gacha_Log/models.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Gacha_Log/models.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/damage_cal.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/damage_cal.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/damage_model.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/damage_model.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_character_bag.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_character_bag.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_character_card.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_character_card.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_character_detail.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_character_detail.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Info/draw_player_card.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Info/draw_player_card.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_MonthInfo/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_MonthInfo/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_MonthInfo/draw.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_MonthInfo/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_MonthInfo/handler.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_MonthInfo/handler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/Atlas/api.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/Atlas/api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/api.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/draw.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/SereniteaPot/draw.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/draw_daily_material.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/draw_daily_material.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/draw_map.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/draw_map.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/img.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/img.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/models.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/models.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/request.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/request.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/genshinmap/utils.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/genshinmap/utils.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/Paimon_Wiki/wiki_api.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/Paimon_Wiki/wiki_api.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/bot_manager/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/bot_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/news60s/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/news60s/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/plugin_manager/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/plugin_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/plugin_manager/draw_help.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/plugin_manager/draw_help.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/plugins/tools/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/plugins/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/alias.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/alias.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/api.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,17 +102,17 @@
 
 
 def get_old_version_ds(mhy_bbs: bool = False) -> str:
     """
     生成米游社旧版本headers的ds_token
     """
     if mhy_bbs:
-        s = 'N50pqm7FSy2AkFz2B3TqtuZMJ5TOl3Ep'
+        s = "1OJyMNCqFlstEQqqMOv0rKCIdTOoJhNt"
     else:
-        s = 'z8DRIUjNDT7IT5IZXvrUAxyupA1peND9'
+        s = "AcpNVhfh0oedCobdCyFV8EE1jMOVDy9q"
     t = str(int(time.time()))
     r = ''.join(random.sample(string.ascii_lowercase + string.digits, 6))
     c = md5(f"salt={s}&t={t}&r={r}")
     return f"{t},{r},{c}"
 
 
 def mihoyo_headers(cookie, q='', b=None) -> dict:
@@ -461,26 +461,26 @@
             + (f'或前往{config.CookieWeb_url}网页添加绑定' if config.CookieWeb_enable else ''),
             False,
             cookie_info,
         )
     if not cookie_info.stoken:
         return 'cookie中没有stoken字段，请重新绑定', False, cookie_info
     headers = {
-        'Cookie': cookie_info.stoken,
-        'DS': get_old_version_ds(True),
-        'User-Agent': 'okhttp/4.8.0',
-        'x-rpc-app_version': '2.35.2',
-        'x-rpc-sys_version': '12',
-        'x-rpc-client_type': '5',
-        'x-rpc-channel': 'mihoyo',
-        'x-rpc-device_id': random_hex(32),
-        'x-rpc-device_name': random_text(random.randint(1, 10)),
-        'x-rpc-device_model': 'Mi 10',
-        'Referer': 'https://app.mihoyo.com',
-        'Host': 'api-takumi.mihoyo.com',
+        "Cookie": cookie_info.stoken,
+        "DS": get_old_version_ds(True),
+        "User-Agent": "okhttp/4.8.0",
+        "x-rpc-app_version": "2.60.1",
+        "x-rpc-sys_version": "12",
+        "x-rpc-client_type": "5",
+        "x-rpc-channel": "mihoyo",
+        "x-rpc-device_id": random_hex(32),
+        "x-rpc-device_name": random_text(random.randint(1, 10)),
+        "x-rpc-device_model": "Mi 10",
+        "Referer": "https://app.mihoyo.com",
+        "Host": "api-takumi.mihoyo.com",
     }
     data = await aiorequests.post(
         url=AUTHKEY_API,
         headers=headers,
         json={
             'auth_appid': 'webview_gacha',
             'game_biz': 'hk4e_cn',
```

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/browser.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/browser.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/files.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/files.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/filter.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/filter.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/genshin.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/genshin.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/image.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/image.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/logger.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/logger.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/message.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/message.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/path.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/path.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/requests.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/requests.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/scheduler.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/status.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/status.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/tool.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/tool.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/typing.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/typing.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/utils/update.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/utils/update.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/__init__.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/__init__.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/bot_info.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/bot_info.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/command_alias.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/command_alias.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/cookie.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/login.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/login.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/plugin.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/plugin.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/status.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/status.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/api/utils.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/api/utils.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/bind_cookie.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/bind_cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/command_alias.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/command_alias.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/config_manage.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/config_manage.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/home_page.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/home_page.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/login.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/login.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/main.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/main.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/plugin_manage.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/plugin_manage.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/private_cookie.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/private_cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/LittlePaimon/web/pages/public_cookie.py` & `mhmzx_little_paimon-3.0.15/LittlePaimon/web/pages/public_cookie.py`

 * *Files identical despite different names*

### Comparing `mhmzx_little_paimon-3.0.14/pyproject.toml` & `mhmzx_little_paimon-3.0.15/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mhmzx-little-paimon"
-version = "3.0.14"
+version = "3.0.15"
 description = "（非官方）小派蒙！原神qq群机器人，基于NoneBot2的UID查询、抽卡导出分析、模拟抽卡、实时便签、札记等多功能小助手。"
 authors = ["Madray Haven <sgpublic2002@gmail.com>"]
 license = "AGPL"
 packages = [
     { include = "LittlePaimon" },
 ]
```

### Comparing `mhmzx_little_paimon-3.0.14/PKG-INFO` & `mhmzx_little_paimon-3.0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mhmzx-little-paimon
-Version: 3.0.14
+Version: 3.0.15
 Summary: （非官方）小派蒙！原神qq群机器人，基于NoneBot2的UID查询、抽卡导出分析、模拟抽卡、实时便签、札记等多功能小助手。
 License: AGPL
 Author: Madray Haven
 Author-email: sgpublic2002@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

